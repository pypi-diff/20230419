# Comparing `tmp/ExceptNotifier-0.1.4.tar.gz` & `tmp/ExceptNotifier-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.4.tar", last modified: Wed Apr 19 11:26:47 2023, max compression
+gzip compressed data, was "ExceptNotifier-0.1.5.tar", last modified: Wed Apr 19 11:47:17 2023, max compression
```

## Comparing `ExceptNotifier-0.1.4.tar` & `ExceptNotifier-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.296941 ExceptNotifier-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.229471 ExceptNotifier-0.1.4/ExceptNotifier/
--rw-rw-rw-   0        0        0     2571 2023-04-19 11:26:11.000000 ExceptNotifier-0.1.4/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.289227 ExceptNotifier-0.1.4/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1150 2023-04-19 11:26:17.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      572 2023-04-19 10:29:57.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0      763 2023-04-19 10:30:03.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      680 2023-04-19 10:16:30.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1364 2023-04-19 10:16:29.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      889 2023-04-19 10:16:25.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/whatsapp_sender.py
--rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.4/ExceptNotifier/beep_notifier.py
--rw-rw-rw-   0        0        0     6533 2023-04-19 11:23:31.000000 ExceptNotifier-0.1.4/ExceptNotifier/chime_notifier.py
--rw-rw-rw-   0        0        0     5231 2023-04-19 11:12:07.000000 ExceptNotifier-0.1.4/ExceptNotifier/desktop_notifier.py
--rw-rw-rw-   0        0        0     5667 2023-04-19 11:23:03.000000 ExceptNotifier-0.1.4/ExceptNotifier/discord_notifier.py
--rw-rw-rw-   0        0        0     5973 2023-04-19 11:12:18.000000 ExceptNotifier-0.1.4/ExceptNotifier/kakao_notifier.py
--rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.4/ExceptNotifier/line_notifier.py
--rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.4/ExceptNotifier/mail_notifier.py
--rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.4/ExceptNotifier/slack_notifier.py
--rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.4/ExceptNotifier/sms_notifier.py
--rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.4/ExceptNotifier/teams_notifier.py
--rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.4/ExceptNotifier/telegram_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.293505 ExceptNotifier-0.1.4/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      246 2023-04-19 11:17:46.000000 ExceptNotifier-0.1.4/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.4/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.252086 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0     6500 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6500 2023-04-19 11:26:47.295508 ExceptNotifier-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5401 2023-04-19 10:27:50.000000 ExceptNotifier-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 11:26:47.297958 ExceptNotifier-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1976 2023-04-19 11:26:24.000000 ExceptNotifier-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:47:17.993147 ExceptNotifier-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:47:17.921256 ExceptNotifier-0.1.5/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2571 2023-04-19 11:45:41.000000 ExceptNotifier-0.1.5/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:47:17.981087 ExceptNotifier-0.1.5/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1150 2023-04-19 11:45:48.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      572 2023-04-19 10:29:57.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0      963 2023-04-19 11:44:26.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      680 2023-04-19 10:16:30.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1364 2023-04-19 10:16:29.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      889 2023-04-19 10:16:25.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.5/ExceptNotifier/base/whatsapp_sender.py
+-rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.5/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6533 2023-04-19 11:23:31.000000 ExceptNotifier-0.1.5/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     5231 2023-04-19 11:12:07.000000 ExceptNotifier-0.1.5/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     5891 2023-04-19 11:45:00.000000 ExceptNotifier-0.1.5/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     5973 2023-04-19 11:12:18.000000 ExceptNotifier-0.1.5/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.5/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.5/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.5/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.5/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.5/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.5/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:47:17.990149 ExceptNotifier-0.1.5/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      267 2023-04-19 11:45:56.000000 ExceptNotifier-0.1.5/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.5/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:47:17.943900 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0     6487 2023-04-19 11:47:17.000000 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2023-04-19 11:47:17.000000 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:47:17.000000 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 11:47:17.000000 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 11:47:17.000000 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 11:47:17.000000 ExceptNotifier-0.1.5/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6487 2023-04-19 11:47:17.993147 ExceptNotifier-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5439 2023-04-19 11:45:21.000000 ExceptNotifier-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:47:17.993147 ExceptNotifier-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1926 2023-04-19 11:45:39.000000 ExceptNotifier-0.1.5/setup.py
```

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/__init__.py` & `ExceptNotifier-0.1.5/ExceptNotifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,9 +34,9 @@
            'send_kakao_msg', 'send_gmail', 'send_slack_msg', 'send_telegram_msg',
            'SuccessChime', 'ExceptChime', 'SendChime',  'SuccessDiscord', 'ExceptDiscord', 'SendDiscord',
            'SuccessKakao', 'ExceptKakao', 'SendKakao',  'SuccessLine', 'ExceptLine', 'SendLine',
            'SuccessTeams', 'ExceptTeams', 'SendTeams', 'send_chime_msg', 'send_discord_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg',
            'SuccessSMS', 'ExceptSMS', 'SendSMS', 'send_sms_msg',  'SuccessBeep', 'ExceptBeep', 'SendBeep', 'receive_openai_advice', 'beep', 'send_gmail_msg'
            ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/__init__.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 __all__ = ['send_kakao_msg', 'send_gmail_msg', 'send_slack_msg', 'send_telegram_msg', 'send_chime_msg', 'send_discord_msg',
            'send_line_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg', 'send_sms_msg', 'beep', 'receive_openai_advice'
            ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/beep_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/chime_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/desktop_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/discord_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/discord_sender.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 #-*- coding: utf-8 -*- 
 # Copyright 2023 parkminwoo
-from discord import Webhook, RequestsWebhookAdapter
 
 
 def send_discord_msg(_DISCORD_WEBHOOK_URL: str, msg: str) -> dict:
     """Send message to chat room through discord app's webhook url.
 
     :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
     :type _DISCORD_WEBHOOK_URL: str
     :param msg: Message text
     :type msg: str
     :return: Response according to REST API request
     :rtype: dict
     """
-
-    webhook = Webhook.from_url(_DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter())
-    resp = webhook.send(msg)
+    try: 
+        from discord import Webhook, RequestsWebhookAdapter
+        webhook = Webhook.from_url(_DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter())
+        resp = webhook.send(msg)
+    except:
+        from discord import SyncWebhook
+        webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL) # Initializing webhook
+        webhook.send(content=msg) 
     return resp
 
 
 
 if __name__ =="__main__":
     _DISCORD_WEBHOOK_URL = "xxxxx"
     msg = "Sending Test"
```

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/kakao_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/line_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/mail_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/openai_receiver.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/slack_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/sms_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/teams_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/telegram_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/base/whatsapp_sender.py` & `ExceptNotifier-0.1.5/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/beep_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/chime_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/chime_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/desktop_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/desktop_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/discord_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/discord_notifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #-*- coding: utf-8 -*- 
 # Copyright 2023 parkminwoo
 import traceback
 import re
 import datetime
 from email.message import EmailMessage
 import sys
-from discord import Webhook, RequestsWebhookAdapter
 from ExceptNotifier import send_discord_msg, receive_openai_advice
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 class ExceptDiscord(BaseException):
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
@@ -63,17 +62,22 @@
         :param _DISCORD_WEBHOOK_URL: Webhook url from discord app
         :type _DISCORD_WEBHOOK_URL: str
         :param msg: Message text
         :type msg: str
         :return: Response according to REST API request
         :rtype: dict
         """
-
-        webhook = Webhook.from_url(_DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter())
-        resp = webhook.send(msg)
+        try: 
+            from discord import Webhook, RequestsWebhookAdapter
+            webhook = Webhook.from_url(_DISCORD_WEBHOOK_URL, adapter=RequestsWebhookAdapter())
+            resp = webhook.send(msg)
+        except:
+            from discord import SyncWebhook
+            webhook = SyncWebhook.from_url(_DISCORD_WEBHOOK_URL) # Initializing webhook
+            webhook.send(content=msg) 
         return resp
 
 
 
 
 class SuccessDiscord:
     def __init__(self) -> None:
```

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/kakao_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/kakao_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/line_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/line_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/mail_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/slack_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/sms_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/teams_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/telegram_notifier.py` & `ExceptNotifier-0.1.5/ExceptNotifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier/utils/kakao_token.py` & `ExceptNotifier-0.1.5/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier.egg-info/PKG-INFO` & `ExceptNotifier-0.1.5/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.4
+Version: 0.1.5
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
 
 # Python Package: ExceptNotifier
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ![Pypi Version](https://img.shields.io/pypi/v/ExceptNotifier.svg)
-[![Python Version](https://img.shields.io/badge/python-3.6%20to%203.9-black)](code_of_conduct.md)
+[![Python Version](https://img.shields.io/badge/python-3.6%20to%203.7-black)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 ##### Provides a notification from the application shown in the following screen,
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main2.png)
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
@@ -55,16 +54,18 @@
 
 <br><br>
 
 # Quick Start
 ```
 pip install ExceptNotifier
 ```
-
-
+or
+```
+pip install exceptnotifier
+```
 
 <br>
 
 # Features
 ### *Telegram Notifier*
 
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
```

### Comparing `ExceptNotifier-0.1.4/ExceptNotifier.egg-info/SOURCES.txt` & `ExceptNotifier-0.1.5/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/LICENSE` & `ExceptNotifier-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.4/PKG-INFO` & `ExceptNotifier-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.4
+Version: 0.1.5
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
 
 # Python Package: ExceptNotifier
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ![Pypi Version](https://img.shields.io/pypi/v/ExceptNotifier.svg)
-[![Python Version](https://img.shields.io/badge/python-3.6%20to%203.9-black)](code_of_conduct.md)
+[![Python Version](https://img.shields.io/badge/python-3.6%20to%203.7-black)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 ##### Provides a notification from the application shown in the following screen,
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main2.png)
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
@@ -55,16 +54,18 @@
 
 <br><br>
 
 # Quick Start
 ```
 pip install ExceptNotifier
 ```
-
-
+or
+```
+pip install exceptnotifier
+```
 
 <br>
 
 # Features
 ### *Telegram Notifier*
 
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
```

### Comparing `ExceptNotifier-0.1.4/README.md` & `ExceptNotifier-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
 
 # Python Package: ExceptNotifier
 ![Except-Notifier](https://img.shields.io/badge/pypi-ExceptNotifier-orange)
 ![Pypi Version](https://img.shields.io/pypi/v/ExceptNotifier.svg)
-[![Python Version](https://img.shields.io/badge/python-3.6%20to%203.9-black)](code_of_conduct.md)
+[![Python Version](https://img.shields.io/badge/python-3.6%20to%203.7-black)](code_of_conduct.md)
 ![Code convention](https://img.shields.io/badge/code%20convention-pep8-black)
 ##### Provides a notification from the application shown in the following screen,
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/main2.png)
  The `ExceptNotifier` Python package offers a flexible approach to receiving notifications by enhancing Python's try-except statement. This package enables you to receive alerts through various messaging applications or emails.
 <Br><br>
 With `ExceptNotifier`, you can obtain detailed compilation errors, including debug information, sent directly to your preferred messaging platform or email. By integrating OpenAI's ChatGPT, you can receive additional error code information as long as you provide the required API model name and key. This feature ensures that error handling and notifications are more informative and accessible, streamlining your debugging process.
@@ -32,16 +32,18 @@
 
 <br><br>
 
 # Quick Start
 ```
 pip install ExceptNotifier
 ```
-
-
+or
+```
+pip install exceptnotifier
+```
 
 <br>
 
 # Features
 ### *Telegram Notifier*
 
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
```

### Comparing `ExceptNotifier-0.1.4/setup.py` & `ExceptNotifier-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="ExceptNotifier",
-    version="0.1.4",
+    version="0.1.5",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
@@ -40,14 +40,13 @@
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     entry_points={"console_scripts": ["ExceptNotifier=ExceptNotifier.cli:main"]},
 )
```

