# Comparing `tmp/tsugu-0.3.4.tar.gz` & `tmp/tsugu-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.3.4.tar", last modified: Fri Apr 12 07:11:19 2024, max compression
+gzip compressed data, was "tsugu-0.3.5.tar", last modified: Sun Apr 14 08:26:24 2024, max compression
```

## Comparing `tsugu-0.3.4.tar` & `tsugu-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:11:19.226432 tsugu-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 07:11:10.000000 tsugu-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 07:11:19.226432 tsugu-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-12 07:11:10.000000 tsugu-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:11:19.226432 tsugu-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 07:11:10.000000 tsugu-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:11:19.226432 tsugu-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-12 07:11:10.000000 tsugu-0.3.4/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:11:19.226432 tsugu-0.3.4/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 07:11:10.000000 tsugu-0.3.4/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-12 07:11:10.000000 tsugu-0.3.4/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-12 07:11:10.000000 tsugu-0.3.4/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-12 07:11:10.000000 tsugu-0.3.4/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-04-12 07:11:10.000000 tsugu-0.3.4/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:11:19.226432 tsugu-0.3.4/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-12 07:11:18.000000 tsugu-0.3.4/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 07:11:19.000000 tsugu-0.3.4/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:11:18.000000 tsugu-0.3.4/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 07:11:18.000000 tsugu-0.3.4/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 07:11:18.000000 tsugu-0.3.4/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.142280 tsugu-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-14 08:26:10.000000 tsugu-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 08:26:24.142280 tsugu-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-14 08:26:10.000000 tsugu-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 08:26:24.142280 tsugu-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-14 08:26:10.000000 tsugu-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.138280 tsugu-0.3.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-14 08:26:10.000000 tsugu-0.3.5/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.138280 tsugu-0.3.5/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.138280 tsugu-0.3.5/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 08:26:24.000000 tsugu-0.3.5/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.3.4/LICENSE` & `tsugu-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.4/PKG-INFO` & `tsugu-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.4 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.5 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.3.4/README.md` & `tsugu-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.4/setup.py` & `tsugu-0.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.3.4',
+    version='0.3.5',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.3.4/test/test_main.py` & `tsugu-0.3.5/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.4/tsugu/bot.py` & `tsugu-0.3.5/tsugu/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,18 +30,19 @@
             return player_status(user_id, platform, int(arg_))
         # 如果用户输入了服务器名
         if server_exists(r_ := query_server_info(arg_)):
             return player_status(user_id, platform, arg_)
         else:
             return text_response('未找到绑定记录')
 
-
-    if message.startswith('绑定玩家') and len(message.replace('绑定玩家', '').strip()) < 4:
-        # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
-        return bind_player_request(platform, user_id)
+    if message.startswith('绑定玩家'):
+        if server_exists(query_server_info(message[4:].strip())) or message[4:].strip() == '':
+            return bind_player_request(platform, user_id)
+        else:
+            return text_response(f'未找到名为 {(message[4:]).strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"绑定玩家"即可')
 
     if message.startswith('验证'):
         arg = message.replace('验证', '').strip()
         # 正则出数字
         player_ids = re.findall(r'\d+', arg)
         if not player_ids or len(player_ids) > 1:
             return text_response('请确保输入正确(例如: 验证 10000xxxxx cn)')
@@ -91,29 +92,29 @@
         # 如果匹配 玩家状态 则查询默认服务器的玩家状态 如果用户输入了服务器名 则查询对应服务器的玩家状态，如果服务器名无效则返回None
         return Remote.player_status(user_id, platform) if (arg_ := message[4:].strip()) == '' else (Remote.player_status(user_id, platform, r_) if server_exists(r_ := query_server_info(arg_)) else None)
 
     if message.startswith('绑定玩家'):
         # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
         server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if server_exists(r_ := query_server_info(message[4:])) else None)
         if not server_exists(server):
-            return text_response(f'未找到名为 {message[4:]} 的服务器信息，请确保输入是服务器名而不是玩家ID，通常情况发送"绑定玩家"或"绑定玩家 服务器"即可')
+            return text_response(f'未找到名为 {(message[4:]).strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"绑定玩家"即可')
 
         res = Remote.bind_player_request(platform, user_id, server, True)
         if res.get('status') != 'success':
             # print(res)
             # {'status': 'success', 'data': {'verifyCode': 12492}}
             return text_response(res.get('data'))
         # if not res.get('status') == 'failed':
         #     return text_response('未知错误喵')
         return text_response(f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{res.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 + 空格 + 玩家ID 来完成本次身份验证\n验证 10000xxxx 国服''')
 
     if message.startswith('解除绑定'):
         server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if (config.server_list(r_ := query_server_info(message[4:]))) else None)
         if server_exists(server) is False:
-            return text_response(f'未找到名为 {message[4:].strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"解除绑定"即可')
+            return text_response(f'未找到名为 {(message[4:]).strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"绑定玩家"即可')
         response = Remote.bind_player_request(platform, user_id, server, False)  # 获取响应
         if response.get('status') == 'failed':  # 检查状态
             return text_response(response.get('data'))
         # 如果是200
         return text_response(f'''正在解除，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{response.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证解绑 {server}\n来完成本次身份验证(没错只需要加上 {server} 来确定需要解绑的服务器)''')
 
     if message.startswith('验证解绑'):
```

### Comparing `tsugu-0.3.4/tsugu/config.py` & `tsugu-0.3.5/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.4/tsugu/router.py` & `tsugu-0.3.5/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.4/tsugu/utils.py` & `tsugu-0.3.5/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.4/tsugu.egg-info/PKG-INFO` & `tsugu-0.3.5/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.4
+Version: 0.3.5
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.4 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.5 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

