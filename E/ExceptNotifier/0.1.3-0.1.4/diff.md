# Comparing `tmp/ExceptNotifier-0.1.3.tar.gz` & `tmp/ExceptNotifier-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.3.tar", last modified: Wed Apr 19 11:19:21 2023, max compression
+gzip compressed data, was "ExceptNotifier-0.1.4.tar", last modified: Wed Apr 19 11:26:47 2023, max compression
```

## Comparing `ExceptNotifier-0.1.3.tar` & `ExceptNotifier-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.727497 ExceptNotifier-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.674508 ExceptNotifier-0.1.3/ExceptNotifier/
--rw-rw-rw-   0        0        0     2571 2023-04-19 11:16:02.000000 ExceptNotifier-0.1.3/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.720386 ExceptNotifier-0.1.3/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1150 2023-04-19 11:17:44.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      572 2023-04-19 10:29:57.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0      763 2023-04-19 10:30:03.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      680 2023-04-19 10:16:30.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1364 2023-04-19 10:16:29.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      889 2023-04-19 10:16:25.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.3/ExceptNotifier/base/whatsapp_sender.py
--rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.3/ExceptNotifier/beep_notifier.py
--rw-rw-rw-   0        0        0     6533 2023-04-19 11:14:16.000000 ExceptNotifier-0.1.3/ExceptNotifier/chime_notifier.py
--rw-rw-rw-   0        0        0     5231 2023-04-19 11:12:07.000000 ExceptNotifier-0.1.3/ExceptNotifier/desktop_notifier.py
--rw-rw-rw-   0        0        0     5667 2023-04-19 11:12:12.000000 ExceptNotifier-0.1.3/ExceptNotifier/discord_notifier.py
--rw-rw-rw-   0        0        0     5973 2023-04-19 11:12:18.000000 ExceptNotifier-0.1.3/ExceptNotifier/kakao_notifier.py
--rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.3/ExceptNotifier/line_notifier.py
--rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.3/ExceptNotifier/mail_notifier.py
--rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.3/ExceptNotifier/slack_notifier.py
--rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.3/ExceptNotifier/sms_notifier.py
--rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.3/ExceptNotifier/teams_notifier.py
--rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.3/ExceptNotifier/telegram_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.724491 ExceptNotifier-0.1.3/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      246 2023-04-19 11:17:46.000000 ExceptNotifier-0.1.3/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.3/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-19 11:19:21.692463 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0     6500 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 11:19:21.000000 ExceptNotifier-0.1.3/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6500 2023-04-19 11:19:21.726498 ExceptNotifier-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5401 2023-04-19 10:27:50.000000 ExceptNotifier-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 11:19:21.728500 ExceptNotifier-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1965 2023-04-19 11:19:10.000000 ExceptNotifier-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.296941 ExceptNotifier-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.229471 ExceptNotifier-0.1.4/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2571 2023-04-19 11:26:11.000000 ExceptNotifier-0.1.4/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.289227 ExceptNotifier-0.1.4/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1150 2023-04-19 11:26:17.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      572 2023-04-19 10:29:57.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0      763 2023-04-19 10:30:03.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      680 2023-04-19 10:16:30.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1364 2023-04-19 10:16:29.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      889 2023-04-19 10:16:25.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.4/ExceptNotifier/base/whatsapp_sender.py
+-rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.4/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6533 2023-04-19 11:23:31.000000 ExceptNotifier-0.1.4/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     5231 2023-04-19 11:12:07.000000 ExceptNotifier-0.1.4/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     5667 2023-04-19 11:23:03.000000 ExceptNotifier-0.1.4/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     5973 2023-04-19 11:12:18.000000 ExceptNotifier-0.1.4/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.4/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.4/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.4/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.4/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.4/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.4/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.293505 ExceptNotifier-0.1.4/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      246 2023-04-19 11:17:46.000000 ExceptNotifier-0.1.4/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.4/ExceptNotifier/utils/kakao_token.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:26:47.252086 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0     6500 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 11:26:47.000000 ExceptNotifier-0.1.4/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6500 2023-04-19 11:26:47.295508 ExceptNotifier-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5401 2023-04-19 10:27:50.000000 ExceptNotifier-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:26:47.297958 ExceptNotifier-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2023-04-19 11:26:24.000000 ExceptNotifier-0.1.4/setup.py
```

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/__init__.py` & `ExceptNotifier-0.1.4/ExceptNotifier/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,9 +34,9 @@
            'send_kakao_msg', 'send_gmail', 'send_slack_msg', 'send_telegram_msg',
            'SuccessChime', 'ExceptChime', 'SendChime',  'SuccessDiscord', 'ExceptDiscord', 'SendDiscord',
            'SuccessKakao', 'ExceptKakao', 'SendKakao',  'SuccessLine', 'ExceptLine', 'SendLine',
            'SuccessTeams', 'ExceptTeams', 'SendTeams', 'send_chime_msg', 'send_discord_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg',
            'SuccessSMS', 'ExceptSMS', 'SendSMS', 'send_sms_msg',  'SuccessBeep', 'ExceptBeep', 'SendBeep', 'receive_openai_advice', 'beep', 'send_gmail_msg'
            ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/__init__.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
 
 
 __all__ = ['send_kakao_msg', 'send_gmail_msg', 'send_slack_msg', 'send_telegram_msg', 'send_chime_msg', 'send_discord_msg',
            'send_line_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg', 'send_sms_msg', 'beep', 'receive_openai_advice'
            ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/beep_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/chime_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/desktop_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/discord_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/discord_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/kakao_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/line_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/mail_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/openai_receiver.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/slack_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/sms_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/teams_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/telegram_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/base/whatsapp_sender.py` & `ExceptNotifier-0.1.4/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/beep_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/chime_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/chime_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/desktop_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/desktop_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/discord_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/discord_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/kakao_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/kakao_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/line_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/line_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/mail_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/slack_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/sms_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/teams_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/telegram_notifier.py` & `ExceptNotifier-0.1.4/ExceptNotifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier/utils/kakao_token.py` & `ExceptNotifier-0.1.4/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier.egg-info/PKG-INFO` & `ExceptNotifier-0.1.4/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.3
+Version: 0.1.4
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ExceptNotifier-0.1.3/ExceptNotifier.egg-info/SOURCES.txt` & `ExceptNotifier-0.1.4/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/LICENSE` & `ExceptNotifier-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/PKG-INFO` & `ExceptNotifier-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExceptNotifier
-Version: 0.1.3
+Version: 0.1.4
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ExceptNotifier-0.1.3/README.md` & `ExceptNotifier-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.3/setup.py` & `ExceptNotifier-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 
 
 version = get_version()
 
 
 setup(
     name="ExceptNotifier",
-    version="0.1.3",
+    version="0.1.4",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=['twilio', 'plyer', 'openai'],
+    install_requires=['twilio', 'plyer', 'openai', 'discord'],
     keywords="Exception, Python, Python Exception Alarm, Error notifications, Customizable notifications, Traceback management, Single line alarm",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
```

