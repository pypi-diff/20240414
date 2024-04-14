# Comparing `tmp/huzzy_rabbit-0.1.1.tar.gz` & `tmp/huzzy_rabbit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huzzy_rabbit-0.1.1.tar", max compression
+gzip compressed data, was "huzzy_rabbit-0.1.2.tar", max compression
```

## Comparing `huzzy_rabbit-0.1.1.tar` & `huzzy_rabbit-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.1/huzzy_rabbit/__init__.py
--rw-r--r--   0        0        0     3340 2024-04-11 14:42:53.905731 huzzy_rabbit-0.1.1/huzzy_rabbit/rabbit_mq.py
--rw-r--r--   0        0        0      291 2024-04-11 14:44:22.765849 huzzy_rabbit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 huzzy_rabbit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      225 2024-04-14 00:32:05.938399 huzzy_rabbit-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 09:38:46.809735 huzzy_rabbit-0.1.2/huzzy_rabbit/__init__.py
+-rw-r--r--   0        0        0     3678 2024-04-14 00:51:20.038509 huzzy_rabbit-0.1.2/huzzy_rabbit/rabbit_mq.py
+-rw-r--r--   0        0        0      291 2024-04-13 23:47:20.855020 huzzy_rabbit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 huzzy_rabbit-0.1.2/PKG-INFO
```

### Comparing `huzzy_rabbit-0.1.1/huzzy_rabbit/rabbit_mq.py` & `huzzy_rabbit-0.1.2/huzzy_rabbit/rabbit_mq.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 
 class RabbitMQ:
     exchanges = {}
     channel = None
     # Adding a dummy comment here
 
     @staticmethod
-    async def publish(message_dict: dict, exchange_name: str, routing_key: str, message = None):
+    async def publish(message_dict: dict, exchange_name: str, routing_key: str, message: Message = None, routing_action: str = None):
         if message is None:
+
             message_body = json.dumps(message_dict).encode()
             message = Message(
                 message_body,
                 delivery_mode=DeliveryMode.PERSISTENT,
             )
         
         try:
             exchange: AbstractExchange = RabbitMQ.exchanges[exchange_name]
         except KeyError:
             # exchange = await RabbitMQ.declare_exchange(exchange_name)
             raise Exception(f"Exchange {exchange_name} not found")
-
+        
+        message.headers = {
+            "action": routing_action
+        }
         # Sending the message
         await exchange.publish(message, routing_key=routing_key)
 
     @staticmethod
     async def connect(connection_url: str):
         # Creating a connection
         # example url = "amqp://guest:guest@localhost/"
@@ -37,45 +41,50 @@
         RabbitMQ.channel = await connection.channel()
         await RabbitMQ.channel.set_qos(prefetch_count=1)
 
     @staticmethod
     async def declare_exchange(exchange_name: str):
         exchange = await RabbitMQ.channel.declare_exchange(
             exchange_name,
-            type=ExchangeType.FANOUT,
+            type=ExchangeType.DIRECT,
             durable=True,
         )
         # Register exchange
         RabbitMQ.exchanges[exchange_name] = exchange
         return exchange
 
     @staticmethod
-    async def declare_queue_and_bind(queue_name: str, exchange_name: str, app_listener):
+    async def declare_queue_and_bind(queue_name: str, exchange_name: str, app_listener, routing_key: str = None):
         queue = await RabbitMQ.channel.declare_queue(queue_name, durable=True)
  
         try:
             exchange: AbstractExchange = RabbitMQ.exchanges[exchange_name]
         except KeyError:
             # exchange = await RabbitMQ.declare_exchange(exchange_name)
             raise Exception(f"Exchange {exchange_name} not found")
 
+        routing_key = routing_key if routing_key else queue_name
+
         # Binding the queue to the exchange
-        await queue.bind(exchange)
+        await queue.bind(exchange, routing_key)
         await queue.consume(app_listener)
 
     @staticmethod
-    async def declare_queue(queue_name: str, exchange_name: str):
+    async def declare_queue(queue_name: str, exchange_name: str, routing_key: str = None):
         queue = await RabbitMQ.channel.declare_queue(queue_name, durable=True)
 
         try:
             exchange: AbstractExchange = RabbitMQ.exchanges[exchange_name]
         except KeyError:
             # exchange = await RabbitMQ.declare_exchange(exchange_name)
             raise Exception(f"Exchange {exchange_name} not found")
-        await queue.bind(exchange)
+        
+        routing_key = routing_key if routing_key else queue_name
+
+        await queue.bind(exchange, routing_key)
         
     async def remote_procedure_call(queue_name: str, on_response: Callable, correlation_id: str, message_dict: dict):
         message_body = json.dumps(message_dict).encode()
         queue = await RabbitMQ.channel.declare_queue(queue_name, durable=True)
         message = Message(
             message_body,
             delivery_mode=DeliveryMode.PERSISTENT,
```

