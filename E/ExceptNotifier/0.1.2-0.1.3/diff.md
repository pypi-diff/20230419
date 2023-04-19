# Comparing `tmp/ExceptNotifier-0.1.2.tar.gz` & `tmp/ExceptNotifier-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.2.tar", last modified: Wed Apr 19 10:33:47 2023, max compression
+gzip compressed data, was "ExceptNotifier-0.1.3.tar", last modified: Wed Apr 19 11:19:21 2023, max compression
```

## Comparing `ExceptNotifier-0.1.2.tar` & `ExceptNotifier-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 10:33:47.806156 ExceptNotifier-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-19 10:33:47.778097 ExceptNotifier-0.1.2/ExceptNotifier/
--rw-rw-rw-   0        0        0     2569 2023-04-19 10:32:22.000000 ExceptNotifier-0.1.2/ExceptNotifier/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-04-19 10:33:31.000000 ExceptNotifier-0.1.2/ExceptNotifier/__main__.py
--rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.2/ExceptNotifier/beep_notifier.py
--rw-rw-rw-   0        0        0     6104 2023-04-19 10:16:55.000000 ExceptNotifier-0.1.2/ExceptNotifier/chime_notifier.py
--rw-rw-rw-   0        0        0     5196 2023-04-19 10:29:29.000000 ExceptNotifier-0.1.2/ExceptNotifier/desktop_notifier.py
--rw-rw-rw-   0        0        0     5644 2023-04-19 10:28:50.000000 ExceptNotifier-0.1.2/ExceptNotifier/discord_notifier.py
--rw-rw-rw-   0        0        0     5950 2023-04-19 10:17:01.000000 ExceptNotifier-0.1.2/ExceptNotifier/kakao_notifier.py
--rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.2/ExceptNotifier/line_notifier.py
--rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.2/ExceptNotifier/mail_notifier.py
--rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.2/ExceptNotifier/slack_notifier.py
--rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.2/ExceptNotifier/sms_notifier.py
--rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.2/ExceptNotifier/teams_notifier.py
--rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.2/ExceptNotifier/telegram_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 10:33:47.802011 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0     6500 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6500 2023-04-19 10:33:47.805020 ExceptNotifier-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5401 2023-04-19 10:27:50.000000 ExceptNotifier-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 10:33:47.806156 ExceptNotifier-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1965 2023-04-19 10:32:00.000000 ExceptNotifier-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.727497 ExceptNotifier-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.674508 ExceptNotifier-0.1.3/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2571 2023-04-19 11:16:02.000000 ExceptNotifier-0.1.3/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.720386 ExceptNotifier-0.1.3/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1150 2023-04-19 11:17:44.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      572 2023-04-19 10:29:57.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0      763 2023-04-19 10:30:03.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      680 2023-04-19 10:16:30.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1364 2023-04-19 10:16:29.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      889 2023-04-19 10:16:25.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/whatsapp_sender.py
+-rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.3/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6533 2023-04-19 11:14:16.000000 ExceptNotifier-0.1.3/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     5231 2023-04-19 11:12:07.000000 ExceptNotifier-0.1.3/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     5667 2023-04-19 11:12:12.000000 ExceptNotifier-0.1.3/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     5973 2023-04-19 11:12:18.000000 ExceptNotifier-0.1.3/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.3/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.3/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.3/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.3/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.3/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.3/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.724491 ExceptNotifier-0.1.3/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      246 2023-04-19 11:17:46.000000 ExceptNotifier-0.1.3/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.3/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.692463 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0     6500 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6500 2023-04-19 11:19:21.726498 ExceptNotifier-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5401 2023-04-19 10:27:50.000000 ExceptNotifier-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:19:21.728500 ExceptNotifier-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1965 2023-04-19 11:19:10.000000 ExceptNotifier-0.1.3/setup.py
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/__init__.py` & `ExceptNotifier-0.1.3/ExceptNotifier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #-*- coding: utf-8 -*- 
 # Copyright 2023 parkminwoo
 
+
 from ExceptNotifier.utils.kakao_token import get_authorize_code, save_token
 
 from ExceptNotifier.base.kakao_sender import send_kakao_msg
 from ExceptNotifier.base.mail_sender import send_gmail_msg
 from ExceptNotifier.base.slack_sender import send_slack_msg
 from ExceptNotifier.base.telegram_sender import send_telegram_msg
 from ExceptNotifier.base.chime_sender import send_chime_msg
@@ -33,9 +34,9 @@
            'send_kakao_msg', 'send_gmail', 'send_slack_msg', 'send_telegram_msg',
            'SuccessChime', 'ExceptChime', 'SendChime',  'SuccessDiscord', 'ExceptDiscord', 'SendDiscord',
            'SuccessKakao', 'ExceptKakao', 'SendKakao',  'SuccessLine', 'ExceptLine', 'SendLine',
            'SuccessTeams', 'ExceptTeams', 'SendTeams', 'send_chime_msg', 'send_discord_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg',
            'SuccessSMS', 'ExceptSMS', 'SendSMS', 'send_sms_msg',  'SuccessBeep', 'ExceptBeep', 'SendBeep', 'receive_openai_advice', 'beep', 'send_gmail_msg'
            ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/beep_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/chime_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/chime_notifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 import urllib3
 import json
-from ExceptNotifier import send_chime_msg, receive_openai_advice
+from ExceptNotifier.base.chime_sender import send_chime_msg
+from ExceptNotifier.base.openai_receiver import receive_openai_advice
+
 
 
 http = urllib3.PoolManager()
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 class ExceptChime(BaseException):
     def __init__(self, *args: object) -> None:
@@ -54,19 +56,22 @@
                 except:
                     exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
 
         print(exceptNotifier['BODY'])
         
         data = {'text':exceptNotifier['SUBJECT']+exceptNotifier['BODY']}
         send_chime_msg(_CHIME_WEBHOOK_URL, data['text'])
-        _OPEN_AI_MODEL, _OPEN_AI_API = None, None
-        if _OPEN_AI_API is not None and _OPEN_AI_API is not None:
-            advice_msg = receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, exceptNotifier['BODY'][:100])
-        send_chime_msg(_CHIME_WEBHOOK_URL, advice_msg)
-        
+
+        try:
+            error_message = f'error_type=={excType} error_type_document=={etype.__doc__} error_value=={value} stack infomation=={stack} code name=={frame.f_code.co_name}file name=={frame.f_code.co_filename} file_number=={frame.f_lineno}'
+            advice_msg = '\tFile: "%s"\n\t\t%s %s: %s\n' % (line[0], line[2], line[1], line[3])
+            advice_msg += receive_openai_advice(_OPEN_AI_MODEL, _OPEN_AI_API, error_message[:150])
+            send_chime_msg(_CHIME_WEBHOOK_URL, advice_msg)
+        except:
+            pass
 
 
 
     @staticmethod
     def send_chime_msg(_CHIME_WEBHOOK_URL: str, msg: str) -> dict:
         """Send message to chat room through chime app's webhook url.
 
@@ -132,15 +137,16 @@
     
     # Get your slcak bot and enter _CHIME_WEBHOOK_URL
     """Get your Webhook _CHIME_WEBHOOK_URL from your chatroom. 
     https://docs.aws.amazon.com/chime/latest/ag/webhooks.html"""
 
     global _CHIME_WEBHOOK_URL 
     _CHIME_WEBHOOK_URL = "https://hooks.chime.aws/incomingwebhooks/72970d5c-7ed1-4e05-bf39-305b860e7e13?token=VWxFRm1IOVh8MXxzQ2VWZVBjQ3EzNE1Oa29Wa0doeDRBWFNEZWJYdkZnSHdjbnlkRDV0TW40"
-    
+    _OPEN_AI_API = "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"
+    _OPEN_AI_MODEL = "gpt-3.5-turbo"
     sys.excepthook = ExceptChime.__call__
 
     try:
         print(1/0)  
         SuccessChime().__call__() #1 success sender          
 
     except ExceptChime as e:      #2 except sender
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/desktop_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/desktop_notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 from plyer import notification
-from ExceptNotifier import send_desktop_msg
+from ExceptNotifier import send_desktop_msg, receive_openai_advice
  
 
 
 
 class ExceptDesktop(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
@@ -54,14 +54,16 @@
                 except:
                     exceptNotifier['BODY'] += '<ERROR WHILE PRINTING VALUE>'
 
         
         print(exceptNotifier['BODY'])
                     
         send_desktop_msg(title = exceptNotifier['SUBJECT'][:20], message=exceptNotifier['BODY'][:200])
+
+        
         
         
 
 
     @staticmethod
     def send_desktop_msg(title_msg: str, body_msg: str, DISP_TIME=5) -> None:
         """Sending notification to desktop
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/discord_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/discord_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright 2023 parkminwoo
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 from discord import Webhook, RequestsWebhookAdapter
-from ExceptNotifier import send_discord_msg
+from ExceptNotifier import send_discord_msg, receive_openai_advice
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 class ExceptDiscord(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
     def __call__(etype, value, tb):
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/kakao_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/kakao_notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
 import json
-from ExceptNotifier import send_kakao_msg
+from ExceptNotifier import send_kakao_msg, receive_openai_advice
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 class ExceptKakao(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/line_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/line_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/mail_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/slack_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/sms_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/teams_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier/telegram_notifier.py` & `ExceptNotifier-0.1.3/ExceptNotifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier.egg-info/PKG-INFO` & `ExceptNotifier-0.1.3/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.2
+Version: 0.1.3
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ExceptNotifier-0.1.2/ExceptNotifier.egg-info/SOURCES.txt` & `ExceptNotifier-0.1.3/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 ExceptNotifier/__init__.py
-ExceptNotifier/__main__.py
 ExceptNotifier/beep_notifier.py
 ExceptNotifier/chime_notifier.py
 ExceptNotifier/desktop_notifier.py
 ExceptNotifier/discord_notifier.py
 ExceptNotifier/kakao_notifier.py
 ExceptNotifier/line_notifier.py
 ExceptNotifier/mail_notifier.py
@@ -15,8 +14,24 @@
 ExceptNotifier/teams_notifier.py
 ExceptNotifier/telegram_notifier.py
 ExceptNotifier.egg-info/PKG-INFO
 ExceptNotifier.egg-info/SOURCES.txt
 ExceptNotifier.egg-info/dependency_links.txt
 ExceptNotifier.egg-info/entry_points.txt
 ExceptNotifier.egg-info/requires.txt
-ExceptNotifier.egg-info/top_level.txt
+ExceptNotifier.egg-info/top_level.txt
+ExceptNotifier/base/__init__.py
+ExceptNotifier/base/beep_sender.py
+ExceptNotifier/base/chime_sender.py
+ExceptNotifier/base/desktop_sender.py
+ExceptNotifier/base/discord_sender.py
+ExceptNotifier/base/kakao_sender.py
+ExceptNotifier/base/line_sender.py
+ExceptNotifier/base/mail_sender.py
+ExceptNotifier/base/openai_receiver.py
+ExceptNotifier/base/slack_sender.py
+ExceptNotifier/base/sms_sender.py
+ExceptNotifier/base/teams_sender.py
+ExceptNotifier/base/telegram_sender.py
+ExceptNotifier/base/whatsapp_sender.py
+ExceptNotifier/utils/__init__.py
+ExceptNotifier/utils/kakao_token.py
```

### Comparing `ExceptNotifier-0.1.2/LICENSE` & `ExceptNotifier-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/PKG-INFO` & `ExceptNotifier-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.2
+Version: 0.1.3
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ExceptNotifier-0.1.2/README.md` & `ExceptNotifier-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.2/setup.py` & `ExceptNotifier-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="ExceptNotifier",
-    version="0.1.2",
+    version="0.1.3",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```

