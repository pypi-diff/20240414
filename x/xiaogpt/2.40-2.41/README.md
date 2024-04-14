# Comparing `tmp/xiaogpt-2.40.tar.gz` & `tmp/xiaogpt-2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.40.tar", last modified: Sat Apr 13 03:42:50 2024, max compression
+gzip compressed data, was "xiaogpt-2.41.tar", last modified: Sun Apr 14 15:05:56 2024, max compression
```

## Comparing `xiaogpt-2.40.tar` & `xiaogpt-2.41.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1063 2024-04-13 03:42:47.363728 xiaogpt-2.40/LICENSE
--rw-r--r--   0        0        0    22684 2024-04-13 03:42:47.363728 xiaogpt-2.40/README.md
--rw-r--r--   0        0        0     1265 2024-04-13 03:42:50.747706 xiaogpt-2.40/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/__main__.py
--rw-r--r--   0        0        0      919 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3656 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1840 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0     2289 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3657 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0     4738 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/cli.py
--rw-r--r--   0        0        0     6301 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      220 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     3979 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/tts/azure.py
--rw-r--r--   0        0        0     4660 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1172 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/tts/edge.py
--rw-r--r--   0        0        0     1096 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1533 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/tts/openai.py
--rw-r--r--   0        0        0     2072 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/utils.py
--rw-r--r--   0        0        0    15337 2024-04-13 03:42:47.363728 xiaogpt-2.40/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    23668 1970-01-01 00:00:00.000000 xiaogpt-2.40/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-14 15:05:43.143656 xiaogpt-2.41/LICENSE
+-rw-r--r--   0        0        0    23007 2024-04-14 15:05:43.143656 xiaogpt-2.41/README.md
+-rw-r--r--   0        0        0     1265 2024-04-14 15:05:56.551629 xiaogpt-2.41/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      919 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3656 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1840 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0     2289 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3657 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0     4738 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6301 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      220 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     3979 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/tts/azure.py
+-rw-r--r--   0        0        0     4660 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1172 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/tts/edge.py
+-rw-r--r--   0        0        0     1096 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1533 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/tts/openai.py
+-rw-r--r--   0        0        0     2072 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/utils.py
+-rw-r--r--   0        0        0    15337 2024-04-14 15:05:43.147656 xiaogpt-2.41/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    23991 1970-01-01 00:00:00.000000 xiaogpt-2.41/PKG-INFO
```

### Comparing `xiaogpt-2.40/LICENSE` & `xiaogpt-2.41/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/README.md` & `xiaogpt-2.41/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -267,17 +267,19 @@
 
 ```shell
  docker buildx build --platform=linux/amd64 -t xiaogpt-x86 .
 ```
 
 ### 第三方 TTS
 
-我们目前支持两种第三方 TTS：edge/openai
+我们目前支持是三种第三方 TTS：edge/openai/azure
 
 [edge-tts](https://github.com/rany2/edge-tts) 提供了类似微软tts的能力
+[azure-tts](https://techcommunity.microsoft.com/t5/ai-azure-ai-services-blog/9-more-realistic-ai-voices-for-conversations-now-generally/ba-p/4099471) 提供了微软 azure tts 的能力
+[openai-tts](https://platform.openai.com/docs/guides/text-to-speech) 提供了类似 openai tts 的能力
 
 #### Usage
 
 你可以通过参数 `tts`, 来启用它
 
 ```json
 {
@@ -288,15 +290,15 @@
 
 查看更多语言支持, 从中选择一个
 
 ```shell
 edge-tts --list-voices
 ```
 
-#### 在容器中使用edge-tts
+#### 在容器中使用 edge-tts/azure-tts/openai-tts
 
 由于 Edge TTS 启动了一个本地的 HTTP 服务，所以需要将容器的端口映射到宿主机上，并且指定本地机器的 hostname:
 
 ```shell
 docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.json
 ```
```

### Comparing `xiaogpt-2.40/pyproject.toml` & `xiaogpt-2.41/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "numexpr>=2.8.6",
     "dashscope==1.10.0",
     "httpcore==0.15.0",
     "idna==3.7",
     "azure-cognitiveservices-speech>=1.37.0",
 ]
 dynamic = []
-version = "2.40"
+version = "2.41"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-2.40/xiaogpt/bot/__init__.py` & `xiaogpt-2.41/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/base_bot.py` & `xiaogpt-2.41/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.41/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.41/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.41/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.41/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/newbing_bot.py` & `xiaogpt-2.41/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.41/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/cli.py` & `xiaogpt-2.41/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/config.py` & `xiaogpt-2.41/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.41/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/langchain/chain.py` & `xiaogpt-2.41/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.41/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.41/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/tts/azure.py` & `xiaogpt-2.41/xiaogpt/tts/azure.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/tts/base.py` & `xiaogpt-2.41/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/tts/edge.py` & `xiaogpt-2.41/xiaogpt/tts/edge.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/tts/mi.py` & `xiaogpt-2.41/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/tts/openai.py` & `xiaogpt-2.41/xiaogpt/tts/openai.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/utils.py` & `xiaogpt-2.41/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/xiaogpt/xiaogpt.py` & `xiaogpt-2.41/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.40/PKG-INFO` & `xiaogpt-2.41/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.40
+Version: 2.41
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -297,17 +297,19 @@
 
 ```shell
  docker buildx build --platform=linux/amd64 -t xiaogpt-x86 .
 ```
 
 ### 第三方 TTS
 
-我们目前支持两种第三方 TTS：edge/openai
+我们目前支持是三种第三方 TTS：edge/openai/azure
 
 [edge-tts](https://github.com/rany2/edge-tts) 提供了类似微软tts的能力
+[azure-tts](https://techcommunity.microsoft.com/t5/ai-azure-ai-services-blog/9-more-realistic-ai-voices-for-conversations-now-generally/ba-p/4099471) 提供了微软 azure tts 的能力
+[openai-tts](https://platform.openai.com/docs/guides/text-to-speech) 提供了类似 openai tts 的能力
 
 #### Usage
 
 你可以通过参数 `tts`, 来启用它
 
 ```json
 {
@@ -318,15 +320,15 @@
 
 查看更多语言支持, 从中选择一个
 
 ```shell
 edge-tts --list-voices
 ```
 
-#### 在容器中使用edge-tts
+#### 在容器中使用 edge-tts/azure-tts/openai-tts
 
 由于 Edge TTS 启动了一个本地的 HTTP 服务，所以需要将容器的端口映射到宿主机上，并且指定本地机器的 hostname:
 
 ```shell
 docker run -v <your-config-dir>:/config -p 9527:9527 -e XIAOGPT_HOSTNAME=<your ip> yihong0618/xiaogpt --config=/config/config.json
 ```
```

