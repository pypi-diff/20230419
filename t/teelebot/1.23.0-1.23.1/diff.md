# Comparing `tmp/teelebot-1.23.0-py3-none-any.whl.zip` & `tmp/teelebot-1.23.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 50456 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     3990 b- defN 23-Apr-11 12:57 teelebot/__init__.py
+Zip file size: 50493 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     3989 b- defN 23-Apr-19 01:18 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      163 b- defN 21-Sep-11 03:28 teelebot/__main__.py
 -rw-rw-rw-  2.0 fat     7352 b- defN 21-Sep-11 03:28 teelebot/buffer.py
--rw-rw-rw-  2.0 fat    19293 b- defN 23-Apr-11 13:11 teelebot/handler.py
+-rw-rw-rw-  2.0 fat    19354 b- defN 23-Apr-19 01:22 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1808 b- defN 21-Sep-11 03:28 teelebot/logger.py
 -rw-rw-rw-  2.0 fat      619 b- defN 22-Aug-14 05:17 teelebot/polling.py
 -rw-rw-rw-  2.0 fat     4304 b- defN 23-Apr-11 13:55 teelebot/request.py
 -rw-rw-rw-  2.0 fat     3876 b- defN 21-Sep-11 03:28 teelebot/schedule.py
--rw-rw-rw-  2.0 fat   125830 b- defN 23-Apr-18 02:19 teelebot/teelebot.py
--rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-18 02:19 teelebot/version.py
+-rw-rw-rw-  2.0 fat   125962 b- defN 23-Apr-19 01:18 teelebot/teelebot.py
+-rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-19 01:17 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 22-Aug-14 10:03 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    14712 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1420 b- defN 23-Apr-18 02:32 teelebot-1.23.0.dist-info/RECORD
-18 files, 222479 bytes uncompressed, 48154 bytes compressed:  78.4%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    14712 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1420 b- defN 23-Apr-19 01:37 teelebot-1.23.1.dist-info/RECORD
+18 files, 222671 bytes uncompressed, 48191 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/LICENSE
+Filename: teelebot-1.23.1.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/METADATA
+Filename: teelebot-1.23.1.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/WHEEL
+Filename: teelebot-1.23.1.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/entry_points.txt
+Filename: teelebot-1.23.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/top_level.txt
+Filename: teelebot-1.23.1.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/zip-safe
+Filename: teelebot-1.23.1.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-1.23.0.dist-info/RECORD
+Filename: teelebot-1.23.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/__init__.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 """
 @creation date: 2019-08-23
-@last modification: 2023-04-11
+@last modification: 2023-04-19
 """
 import os
 import requests
 import urllib3
 
 from .polling import _runUpdates
 from .webhook import _runWebhook
@@ -30,15 +30,15 @@
         "    __            __     __          __  " + "\n" + \
         "   / /____  ___  / /__  / /_  ____  / /_ " + "\n" + \
         "  / __/ _ \/ _ \/ / _ \/ __ \/ __ \/ __/ " + "\n" + \
         " / /_/  __/  __/ /  __/ /_/ / /_/ / /_   " + "\n" + \
         " \__/\___/\___/_/\___/_.___/\____/\__/   " + "\n"
     )
     print(" * Self-checking...", end="\r")
-    req = requests.post(url=bot._url + "getWebhookInfo", verify=False, proxies=bot._proxies)
+    req = requests.post(url=bot._url + "getWebhookInfo", verify=False, proxies=bot.proxies)
     if not req.json().get("ok"):
         if (req.json().get("error_code") == 401 and \
             req.json().get("description") == "Unauthorized"):
             print("\nif you already logout the bot from the cloud Bot API server,please wait at least 10 minutes and try again.")
         else:
             print("\nfailed to get running mode!")
         os._exit(0)
```

## teelebot/handler.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2023-04-11
+@last modification: 2023-04-19
 '''
 import configparser
 import argparse
 import os
 import sys
 import shutil
 import requests
@@ -211,14 +211,15 @@
                         "    # version = bot.version\n" + \
                         "    # plugin_dir = bot.plugin_dir\n" + \
                         "    # plugin_bridge = bot.plugin_bridge\n" + \
                         "    # uptime = bot.uptime\n" + \
                         "    # response_times = bot.response_times\n" + \
                         "    # response_chats = bot.response_chats\n" + \
                         "    # response_users = bot.response_users\n" + \
+                        "    # proxies = bot.proxies\n" + \
                         "\n" + \
                         '    chat_id = message["chat"]["id"]\n' + \
                         '    user_id = message["from"]["id"]\n' + \
                         '    message_id = message["message_id"]\n' + \
                         "\n" + \
                         '    message_type = message["message_type"]\n' + \
                         '    chat_type = message["chat"]["type"]\n' + \
```

## teelebot/teelebot.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-08-13
-@last modification: 2023-04-18
+@last modification: 2023-04-19
 @author: Pluto (github:plutobell)
-@version: 1.23.0
+@version: 1.23.1
 """
 import inspect
 import time
 import sys
 import os
 import json
 import string
@@ -35,15 +35,15 @@
         config = _config()
 
         if key != "":
             self._key = key
         elif key == "":
             self._key = config["key"]
         
-        self._proxies = config["proxies"]
+        self.__proxies = config["proxies"]
 
         self._cloud_api_server = config["cloud_api_server"]
         self._local_api_server = config["local_api_server"]
         if self._local_api_server != "False":
             self._basic_url = config["local_api_server"]
         else:
             self._basic_url = self._cloud_api_server
@@ -98,15 +98,15 @@
         self.__start_time = int(time.time())
         self.__response_times = 0
         self.__response_chats = []
         self.__response_users = []
 
         thread_pool_size = round(int(self._pool_size) * 2 / 3)
         schedule_queue_size = int(self._pool_size) - thread_pool_size
-        self.request = _Request(thread_pool_size, self._url, self._debug, self._proxies)
+        self.request = _Request(thread_pool_size, self._url, self._debug, self.__proxies)
         self.schedule = _Schedule(schedule_queue_size)
         self.buffer = _Buffer(int(self._buffer_size) * 1024 * 1024,
             self.__plugin_bridge.keys(), self.__plugin_dir)
 
         self.__thread_pool = ThreadPoolExecutor(
             max_workers=thread_pool_size)
         self.__timer_thread_pool = ThreadPoolExecutor(
@@ -622,14 +622,21 @@
 
     @property
     def response_users(self):
         """
         获取框架启动后响应的所有用户ID
         """
         return self.__response_users
+    
+    @property
+    def proxies(self):
+        """
+        获取代理信息
+        """
+        return self.__proxies
 
     def getChatCreator(self, chat_id):
         """
         获取群组创建者信息
         """
         if str(chat_id)[0] == "-":
             req = self.getChatAdministrators(str(chat_id))
```

## teelebot/version.py

```diff
@@ -1,15 +1,15 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
-@last modification: 2023-04-18
+@last modification: 2023-04-19
 @author: Pluto (github:plutobell)
-@version: 1.23.0
+@version: 1.23.1
 """
 
-__version__ = "1.23.0"
+__version__ = "1.23.1"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

## Comparing `teelebot-1.23.0.dist-info/LICENSE` & `teelebot-1.23.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-1.23.0.dist-info/METADATA` & `teelebot-1.23.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 1.23.0
+Version: 1.23.1
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
```

## Comparing `teelebot-1.23.0.dist-info/RECORD` & `teelebot-1.23.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-teelebot/__init__.py,sha256=EldJeJVnSdTl8FRjC4QCHJ9trFjt_9W_W_XeHHkkgvg,3990
+teelebot/__init__.py,sha256=EllxG9NIQvaLa3cFBHh4_uTWcPDiHKV8mD_-oEuy8pM,3989
 teelebot/__main__.py,sha256=SRKzFAyri9IQ-2Ox_xM3h_o9KrU4Qb2SikEGl-fhun8,163
 teelebot/buffer.py,sha256=YFYDSt7wQzko4Fuzg16PdwyjpXLpvBIK_ZHenv5gD4s,7352
-teelebot/handler.py,sha256=GQPNT3IUvzdrQpF5_VKbjO_tXqpVhgtTjAR0IgimdRo,19293
+teelebot/handler.py,sha256=JPF71of7h1DBxDzjHfcjqPieO3lZh4cLMZXoo1oEjjs,19354
 teelebot/logger.py,sha256=WALHg4p9zKuBTuI9ciND-8z-dZ04kVIwgdBmQx2lk0M,1808
 teelebot/polling.py,sha256=KyfGkXHUpPBkDzB2bQRZ8btJm0EOOXoTFZpRZS0b4nM,619
 teelebot/request.py,sha256=WntfQMyHqjGFtiekGx6O-YOZV9Ljqayvr0D1hsruNs8,4304
 teelebot/schedule.py,sha256=K5eecKJD-M9h_ZXqXMlgXlo3Bq8h6unqmTWt37LZhXg,3876
-teelebot/teelebot.py,sha256=SSw0sHnQfZepuLYrNocFSYnN6lb2Tz0KatDQSyE1h24,125830
-teelebot/version.py,sha256=q5rHZe7sqob66__s95ZKKO37SUR1jiRT4oNgrSyxvLI,478
+teelebot/teelebot.py,sha256=pUFK0vr4AWzQzTNCrmFJPVeN_4el74KteUhlkYIFWBo,125962
+teelebot/version.py,sha256=XYjk2mOgOCX2ZjK74JQ569xQI-2m02tNpWQ96pnyUYg,478
 teelebot/webhook.py,sha256=LQ51F722XOJW1mdErKw-rA9AhotGJnsvR8RStDotpVM,2665
-teelebot-1.23.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-1.23.0.dist-info/METADATA,sha256=8VE1PQz7gMDhyjbaYOo5NJWd57xPES9ddIGLSnf3bJQ,14712
-teelebot-1.23.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-1.23.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-1.23.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-1.23.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-1.23.0.dist-info/RECORD,,
+teelebot-1.23.1.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-1.23.1.dist-info/METADATA,sha256=zEj93Q12GwnYlwJS-92GIBLjCJk_yghMr-HS6k4l8Mw,14712
+teelebot-1.23.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-1.23.1.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-1.23.1.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-1.23.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-1.23.1.dist-info/RECORD,,
```

