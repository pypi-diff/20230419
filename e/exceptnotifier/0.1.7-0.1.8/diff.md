# Comparing `tmp/ExceptNotifier-0.1.7.tar.gz` & `tmp/exceptnotifier-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.7.tar", last modified: Wed Apr 19 17:58:22 2023, max compression
+gzip compressed data, was "exceptnotifier-0.1.8.tar", last modified: Wed Apr 19 18:24:09 2023, max compression
```

## Comparing `ExceptNotifier-0.1.7.tar` & `exceptnotifier-0.1.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:58:22.035144 ExceptNotifier-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-04-19 17:58:21.965150 ExceptNotifier-0.1.7/ExceptNotifier/
--rw-rw-rw-   0        0        0     2714 2023-04-19 17:36:16.000000 ExceptNotifier-0.1.7/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:58:22.027462 ExceptNotifier-0.1.7/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1232 2023-04-19 17:36:33.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      583 2023-04-19 12:04:52.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0      975 2023-04-19 12:04:07.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      680 2023-04-19 12:02:25.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1364 2023-04-19 12:03:24.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      908 2023-04-19 14:11:30.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0      548 2023-04-19 17:11:23.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/wechat_sender.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/whatsapp_sender.py
--rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.7/ExceptNotifier/beep_notifier.py
--rw-rw-rw-   0        0        0     6393 2023-04-19 13:25:44.000000 ExceptNotifier-0.1.7/ExceptNotifier/chime_notifier.py
--rw-rw-rw-   0        0        0     5769 2023-04-19 15:47:40.000000 ExceptNotifier-0.1.7/ExceptNotifier/desktop_notifier.py
--rw-rw-rw-   0        0        0     6479 2023-04-19 13:24:37.000000 ExceptNotifier-0.1.7/ExceptNotifier/discord_notifier.py
--rw-rw-rw-   0        0        0     6563 2023-04-19 13:24:31.000000 ExceptNotifier-0.1.7/ExceptNotifier/kakao_notifier.py
--rw-rw-rw-   0        0        0     6033 2023-04-19 13:24:27.000000 ExceptNotifier-0.1.7/ExceptNotifier/line_notifier.py
--rw-rw-rw-   0        0        0     7746 2023-04-19 13:24:20.000000 ExceptNotifier-0.1.7/ExceptNotifier/mail_notifier.py
--rw-rw-rw-   0        0        0     6094 2023-04-19 13:24:12.000000 ExceptNotifier-0.1.7/ExceptNotifier/slack_notifier.py
--rw-rw-rw-   0        0        0     6085 2023-04-19 15:32:02.000000 ExceptNotifier-0.1.7/ExceptNotifier/sms_notifier.py
--rw-rw-rw-   0        0        0     6020 2023-04-19 14:03:49.000000 ExceptNotifier-0.1.7/ExceptNotifier/teams_notifier.py
--rw-rw-rw-   0        0        0     6275 2023-04-19 14:10:48.000000 ExceptNotifier-0.1.7/ExceptNotifier/telegram_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:58:22.031939 ExceptNotifier-0.1.7/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      263 2023-04-19 15:56:09.000000 ExceptNotifier-0.1.7/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.7/ExceptNotifier/utils/kakao_token.py
--rw-rw-rw-   0        0        0     6148 2023-04-19 17:33:09.000000 ExceptNotifier-0.1.7/ExceptNotifier/wechat_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:58:21.995512 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    22838 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1296 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.7/LICENSE
--rw-rw-rw-   0        0        0    22838 2023-04-19 17:58:22.034144 ExceptNotifier-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    21790 2023-04-19 17:35:03.000000 ExceptNotifier-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 17:58:22.035144 ExceptNotifier-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1926 2023-04-19 17:36:24.000000 ExceptNotifier-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.306756 exceptnotifier-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.237726 exceptnotifier-0.1.8/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2714 2023-04-19 17:36:16.000000 exceptnotifier-0.1.8/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.296358 exceptnotifier-0.1.8/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1232 2023-04-19 18:19:59.000000 exceptnotifier-0.1.8/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 exceptnotifier-0.1.8/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 exceptnotifier-0.1.8/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      583 2023-04-19 12:04:52.000000 exceptnotifier-0.1.8/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0      975 2023-04-19 12:04:07.000000 exceptnotifier-0.1.8/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 exceptnotifier-0.1.8/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 exceptnotifier-0.1.8/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 exceptnotifier-0.1.8/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 exceptnotifier-0.1.8/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      680 2023-04-19 12:02:25.000000 exceptnotifier-0.1.8/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1364 2023-04-19 12:03:24.000000 exceptnotifier-0.1.8/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 exceptnotifier-0.1.8/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      908 2023-04-19 14:11:30.000000 exceptnotifier-0.1.8/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      548 2023-04-19 17:11:23.000000 exceptnotifier-0.1.8/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 exceptnotifier-0.1.8/ExceptNotifier/base/whatsapp_sender.py
+-rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 exceptnotifier-0.1.8/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6393 2023-04-19 13:25:44.000000 exceptnotifier-0.1.8/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     5769 2023-04-19 15:47:40.000000 exceptnotifier-0.1.8/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     6479 2023-04-19 13:24:37.000000 exceptnotifier-0.1.8/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     6563 2023-04-19 13:24:31.000000 exceptnotifier-0.1.8/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     6033 2023-04-19 13:24:27.000000 exceptnotifier-0.1.8/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     7746 2023-04-19 13:24:20.000000 exceptnotifier-0.1.8/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     6094 2023-04-19 13:24:12.000000 exceptnotifier-0.1.8/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     6085 2023-04-19 15:32:02.000000 exceptnotifier-0.1.8/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     6020 2023-04-19 14:03:49.000000 exceptnotifier-0.1.8/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     6275 2023-04-19 14:10:48.000000 exceptnotifier-0.1.8/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.300359 exceptnotifier-0.1.8/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      263 2023-04-19 15:56:09.000000 exceptnotifier-0.1.8/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 exceptnotifier-0.1.8/ExceptNotifier/utils/kakao_token.py
+-rw-rw-rw-   0        0        0     6148 2023-04-19 17:33:09.000000 exceptnotifier-0.1.8/ExceptNotifier/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 18:24:09.263963 exceptnotifier-0.1.8/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    23587 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1526 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 18:24:09.000000 exceptnotifier-0.1.8/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 exceptnotifier-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0    23587 2023-04-19 18:24:09.305750 exceptnotifier-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    22539 2023-04-19 18:15:27.000000 exceptnotifier-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 18:24:09.306756 exceptnotifier-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1926 2023-04-19 18:23:49.000000 exceptnotifier-0.1.8/setup.py
```

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/__init__.py` & `exceptnotifier-0.1.8/ExceptNotifier/__init__.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/__init__.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,9 +16,9 @@
 from ExceptNotifier.base.wechat_sender import send_wechat_msg
 
 
 __all__ = ['send_kakao_msg', 'send_gmail_msg', 'send_slack_msg', 'send_telegram_msg', 'send_chime_msg', 'send_discord_msg',
            'send_line_msg', 'send_wechat_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg', 'send_sms_msg', 'beep', 'receive_openai_advice'
            ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/beep_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/chime_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/desktop_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/discord_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/discord_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/kakao_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/line_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/mail_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/openai_receiver.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/slack_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/sms_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/teams_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/telegram_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/wechat_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/wechat_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/base/whatsapp_sender.py` & `exceptnotifier-0.1.8/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/beep_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/chime_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/chime_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/desktop_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/desktop_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/discord_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/discord_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/kakao_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/kakao_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/line_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/line_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/mail_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/slack_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/sms_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/teams_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/telegram_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/utils/kakao_token.py` & `exceptnotifier-0.1.8/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier/wechat_notifier.py` & `exceptnotifier-0.1.8/ExceptNotifier/wechat_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier.egg-info/PKG-INFO` & `exceptnotifier-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: ExceptNotifier
-Version: 0.1.7
-Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
-Home-page: https://github.com/dsdanielpark/ExceptNotifier
-Author: daniel park
-Author-email: parkminwoo1991@gmail.com
-Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ExceptNotifier_logo.png)
 
 <h3 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h3>
 
@@ -60,14 +38,15 @@
 - [Discord](https://discord.com/)
 - [Slack](https://slack.com/)
 - [Google Mail](https://mail.google.com/)
 - [Line](https://line.me/en/)
 - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/)
 - [Microsoft Teams](https://www.microsoft.com/en/microsoft-teams/download-app)
 - [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
+- [Wecaht](https://www.wechat.com/)
 - SMS Sending using [Twilio](https://www.twilio.com/en-us)
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 
 <Br>
 
 ### AI Debugging using OpenAI API
@@ -204,31 +183,33 @@
 ```
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ex4.png)
 
 
 <br><br>
 
-# 2. Features
+# Feature
+
+## Notifier
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 
 
-## 2-1. *Telegram Notifier*
+### 2-1. *Telegram Notifier*
 
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
 - b. Type /newbot to create a new bot <br>
 - c. Give your bot a name & a username <br>
 - d. Copy your new Telegram bot’s token <br>
 
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
 <br><br>
  
-### a. Without OpenAI API
+#### a. Without OpenAI API
 
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys
 sys.excepthook = ExceptTelegram.__call__
 
 _TELEGRAM_TOKEN = "xxxx"
@@ -243,15 +224,15 @@
 SendTelegram().__call__()        #3. customized sender     
 ```
 
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/fig44.png)
 
 
-### b. With OpenAI API
+#### b. With OpenAI API
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys
 sys.excepthook = ExceptTelegram.__call__
 
 _TELEGRAM_TOKEN = "xxxx"
 _OPEN_AI_MODEL="gpt-3.5-turbo"
@@ -265,15 +246,15 @@
     sys.exit()
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
-## 2-2. *Mail Notifier*
+### 2-2. *Mail Notifier*
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en). 
 
 ```python
 import sys
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail
@@ -347,15 +328,15 @@
 
 SendMail().__call__() 
 ```
 </details>
 
 <br>
 
-## 2-3. *Discord Notifier*
+### 2-3. *Discord Notifier*
 - a. Select the channel to receive notifications.
 - b. Click "Edit Channel" in the upper right corner of the chat window.
 - c. Click Integrations - Webhook - New Webhook.
 - d. Then click Copy Webhook.
 
 ```python
 import sys
@@ -375,15 +356,15 @@
     sys.exit()
 
 SendDiscord().__call__()        #3 customized sender       
 ```
 
 <br>
 
-## 2-4. *Chime Notifier*
+### 2-4. *Chime Notifier*
 - a. Select the Chat room to receive notifications.
 - b. Click "Room Setting" in the upper right corner.
 - c. Click "Manage Webhook and bot."
 - d. Create Add Webhook, set it up, then click Copy Webhook.
 ```python
 import sys
 from ExceptNotifier import SuccessChime, ExceptChime, SendChime
@@ -401,15 +382,15 @@
 except ExceptChime as e:      #2 except sender            
     sys.exit()
 
 SendChime().__call__()        #3 customized sender       
 ```
 <br>
 
-## 2-5. *Slack Notifier*
+### 2-5. *Slack Notifier*
 - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App`
 - c. Add webhook: Click `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace
 - d. Copy `Webhook URL`
 
 ```python
 import sys
@@ -427,15 +408,15 @@
 except ExceptSlack as e:      #2 except sender            
     sys.exit()
 
 SendSlack().__call__()        #3 customized sender     
 ```
 <Br>
 
-## 2-6. *Line Notifier*
+### 2-6. *Line Notifier*
 - a. Register [https://notify-bot.line.me/](https://notify-bot.line.me/)
 - b. Go to mypage [https://notify-bot.line.me/my/](https://notify-bot.line.me/my/)
 - c. Click `Generate Token`, enter Service Name and click `1-on-1 chat with LINE` (anything you like)
 - d. Copy Token.
 
 ```python
 import sys
@@ -454,15 +435,15 @@
     sys.exit()
 
 SendLine().__call__()        #3 customized sender          
 ```
 
 <Br>
 
-## 2-7. *SMS Notifier*
+### 2-7. *SMS Notifier*
 - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://www.twilio.com/en-us)
 - b. Click Console in the upper right corner.
 - c. Copy the variables provided in the console.
 
 ```python
 import sys
 from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS
@@ -482,15 +463,15 @@
 except ExceptSMS as e:      #2 except sender
     sys.exit()
 
 SendSMS().__call__()        #3 customized sender        
 ```
 <Br>
 
-## 2-8. *Teams Notifier*
+### 2-8. *Teams Notifier*
 - a. Create the channel that you want to notify.
 - b. App - Search: webhook - Incoming Webhook [https://teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog)
 - c. Click `Request Approval` <br>
 After you can use webhook incomming. Proceed to next steps.
 Microsoft Teams allows limited application access per organization, so it can only be used if the webhook incoming application is available.
 - c. Go to the team channel to receive notifications, and click `Connectors` in Settings.
 - d. `Connectors` After configuring webhook incoming in Connector, copy the webhook URL.
@@ -512,15 +493,15 @@
     sys.exit()
 
 SendTeams().__call__()        #3 customized sender        
 ```
 
 <Br>
 
-## 2-9. *Kakaotalk Notifier*
+### 2-9. *Kakaotalk Notifier*
 - a. Sign up at the following site: [https://developers.kakao.com/](https://developers.kakao.com/)
 - b. Click "My Application" on the top bar.
 - c. Click "Add an application," set a name, and create it.
 - d. Click "Kakao Login" in the left menu, then change the State of "Kakao Login Activation" to ON on the resulting page.
 - e. In My Application > Product Settings > Kakao Login, be sure to set Redirect URI as follows: [https://example.com/oauth](https://example.com/oauth)
 - f. In the left Consent Items menu, set "Send message in KakaoTalk" to selective agreement.
 - g. Copy the REST API Key in My Application > App Settings > Summary, and go to the following document.
@@ -544,17 +525,40 @@
     SuccessKakao().__call__() #1 success sender          
 except ExceptKakao as e:      #2 except sender            
     sys.exit()
 
 SendKakao().__call__()        #3 customized sender         
 ```
 
+
+### 2-10. *Wechat Notifier*
+a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+
+```python
+import sys
+from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat
+
+# Define the next two variables optionally when using OpenAI's API.
+# _OPEN_AI_MODEL="gpt-3.5-turbo"    
+# _OPEN_AI_API="sk-xxxxxx"
+_WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__
+
+try:
+    print(1/0)  
+    SuccessWechat().__call__() #1 success sender          
+except ExceptWechat as e:      #2 except sender            
+    sys.exit()
+
+SendWechat().__call__()        #3 customized sender       
+```
+
 <Br>
 
-## 2-10. *Beep Notifier*
+### 2-11. *Beep Notifier*
 No setup is required. Use as follows.
 
 ```python
 from Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep()
 BEEP_TIME = 1
 sys.excepthook = ExceptBeep.__call__
 
@@ -570,15 +574,15 @@
 beep()
 
 ```
 
 <Br>
 
 
-## 2-11. *Desktop Notifier*
+### 2-12. *Desktop Notifier*
 No setup is required. Use as follows.
 
 ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__
 # Define the next two variables optionally when using OpenAI's API.
 # _OPEN_AI_MODEL="gpt-3.5-turbo"    
@@ -590,14 +594,20 @@
 
 except ExceptDesktop as e:      #2 except sender            
     sys.exit()
 
 SendDesktop().__call__()        #3 customized sender         
 ```
 
+<br>
+
+## Sender
+
+
+
 <Br><br><br>
 
 # License
 MIT
 
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
```

#### html2text {}

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1 Name: ExceptNotifier Version: 0.1.7 Summary: With
-Python's try-except to receive notifications about Errors or Successes in your
-code through messenger app or email. Home-page: https://github.com/
-dsdanielpark/ExceptNotifier Author: daniel park Author-email:
-parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
-Alarm,Error notifications,Customizable notifications,Traceback
-management,Single line alarm Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research Classifier: Natural Language
-:: English Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE Development Status :: 3 - Alpha
+Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
 ExceptNotifier_logo.png)
   **** Integrates AI-assisted debugging notifications into Python try-except
               statements for various messaging applications. ****
               [PyPI] [Downloads] [conda-forge] [Code_style:_black]
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
@@ -36,18 +22,18 @@
 (https://img.shields.io/badge/pypi-ExceptNotifier-orange) ```
 
 ### Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
 (https://discord.com/) - [Slack](https://slack.com/) - [Google Mail](https://
 mail.google.com/) - [Line](https://line.me/en/) - [AWS Chime](https://
 aws.amazon.com/ko/chime/download-chime/) - [Microsoft Teams](https://
 www.microsoft.com/en/microsoft-teams/download-app) - [Kakao Talk](https://
-www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - SMS Sending using
-[Twilio](https://www.twilio.com/en-us) - Desktop Notification using [Plyer]
-(https://github.com/kivy/plyer) - Beep Sound from [system](https://
-docs.python.org/3/library/winsound.html)
+www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - [Wecaht](https://
+www.wechat.com/) - SMS Sending using [Twilio](https://www.twilio.com/en-us) -
+Desktop Notification using [Plyer](https://github.com/kivy/plyer) - Beep Sound
+from [system](https://docs.python.org/3/library/winsound.html)
 ### AI Debugging using OpenAI API If you have OpenAI API Key and model name,
 you can get information and code examples for debugging in any application. -
 [OPEN AI API](https://platform.openai.com/docs/introduction)
 
 # Quick Start ```bash pip install ExceptNotifier pip install exceptnotifier
 conda install ExceptNotifier conda install exceptnotifier ```
 # App Setup Overview - The variables in the following table must not be
@@ -123,38 +109,39 @@
 SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack,
 SendTeams, SendDesktope, SendBeep ``` *Example* ```python from ExceptNotifier
 import SendTelgeram _TELEGRAM_TOKEN = "xxxx" SendTelegram().__call__() #
 sending message to telegram noti = SendTelegram() noti() # sending message to
 telegram ``` ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/
 assets/imgs/ex4.png)
 
-# 2. Features You can receive debugging information from ChatGPT via OpenAI's
-API when using the Except statement. The syntax remains the same, but you'll
-need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API` ## 2-1.
-*Telegram Notifier* - a. Open your telegram app and search for BotFather. (A
-built-in Telegram bot that helps users create custom Telegram bots)
+# Feature ## Notifier You can receive debugging information from ChatGPT via
+OpenAI's API when using the Except statement. The syntax remains the same, but
+you'll need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API`
+### 2-1. *Telegram Notifier* - a. Open your telegram app and search for
+BotFather. (A built-in Telegram bot that helps users create custom Telegram
+bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/
 bots/api)
 
-### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
+#### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
 SuccessTelegram, SendTelegram import sys sys.excepthook =
 ExceptTelegram.__call__ _TELEGRAM_TOKEN = "xxxx" try: print(1/0)
 SuccessTelegram().__call__() #1. success sender except ExceptTelegram as e: #2.
 except sender sys.exit() SendTelegram().__call__() #3. customized sender ``` !
 [](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-fig44.png) ### b. With OpenAI API ```python from ExceptNotifier import
+fig44.png) #### b. With OpenAI API ```python from ExceptNotifier import
 ExceptTelegram, SuccessTelegram, SendTelegram import sys sys.excepthook =
 ExceptTelegram.__call__ _TELEGRAM_TOKEN = "xxxx" _OPEN_AI_MODEL="gpt-3.5-turbo"
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
 success sender except ExceptTelegram as e: #2. except sender sys.exit()
 SendTelegram().__call__() #3. customized sender ```
-## 2-2. *Mail Notifier* In the except statement, an email is sent along with
+### 2-2. *Mail Notifier* In the except statement, an email is sent along with
 the error message. Additionally, you can send emails from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
 (https://myaccount.google.com/u/3/apppasswords?utm_source=google-
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
@@ -177,64 +164,64 @@
 for Python developers... ```python import sys from ExceptNotifier import
 ExceptMail, SuccessMail, SendMail sys.excepthook = ExceptMail.__call__ # Define
 the next two variables optionally when using OpenAI's API. #
 _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-xxxxxx" _GAMIL_RECIPIENT_ADDR
 = 'xxxxxxx@gmail.com' _GMAIL_SENDER_ADDR = 'yyyyyy@gmail.com'
 _GMAIL_APP_PASSWORD_OF_SENDER = 'zzzzzz' try: 'your code' SuccessMail
 ().__call__() except ExceptMail: pass SendMail().__call__() ```
-## 2-3. *Discord Notifier* - a. Select the channel to receive notifications. -
+### 2-3. *Discord Notifier* - a. Select the channel to receive notifications. -
 b. Click "Edit Channel" in the upper right corner of the chat window. - c.
 Click Integrations - Webhook - New Webhook. - d. Then click Copy Webhook.
 ```python import sys from ExceptNotifier import ExceptDiscord, SuccessDiscord,
 SendDiscord sys.excepthook = ExceptDiscord.__call__ # Define the next two
 variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo"
 # _OPEN_AI_API="sk-xxxxxx" _DISCORD_WEBHOOK_URL = "xxxxxxxxxxxxxxxxx" try:
 print(1/20) SuccessDiscord().__call__() #1 success sender except ExceptDiscord
 as e: #2 except sender sys.exit() SendDiscord().__call__() #3 customized sender
 ```
-## 2-4. *Chime Notifier* - a. Select the Chat room to receive notifications. -
+### 2-4. *Chime Notifier* - a. Select the Chat room to receive notifications. -
 b. Click "Room Setting" in the upper right corner. - c. Click "Manage Webhook
 and bot." - d. Create Add Webhook, set it up, then click Copy Webhook.
 ```python import sys from ExceptNotifier import SuccessChime, ExceptChime,
 SendChime sys.excepthook = ExceptChime.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _CHIME_WEBHOOK_URL = "xxxxxxxxxxxxxxxxxx" try: print
 (1/0) SuccessChime().__call__() #1 success sender except ExceptChime as e: #2
 except sender sys.exit() SendChime().__call__() #3 customized sender ```
-## 2-5. *Slack Notifier* - a. visit https://api.slack.com/ - b. `Create an app`
-- `From scratch` - `Create App` - c. Add webhook: Click `Incoming Webhooks` -
-Activate Incomming `On` - Add New Webhook to Workspace - d. Copy `Webhook URL`
-```python import sys from ExceptNotifier import ExceptSlack, SuccessSlcak,
-SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next two variables
-optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
-_OPEN_AI_API="sk-xxxxxx" _SLACK_WEBHOOK_URL = 'https://hooks.slack.com/
-services/xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlcak().__call__() #1
-success sender except ExceptSlack as e: #2 except sender sys.exit() SendSlack
-().__call__() #3 customized sender ```
-## 2-6. *Line Notifier* - a. Register [https://notify-bot.line.me/](https://
+### 2-5. *Slack Notifier* - a. visit https://api.slack.com/ - b. `Create an
+app` - `From scratch` - `Create App` - c. Add webhook: Click `Incoming
+Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace - d. Copy
+`Webhook URL` ```python import sys from ExceptNotifier import ExceptSlack,
+SuccessSlcak, SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next
+two variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-
+turbo" # _OPEN_AI_API="sk-xxxxxx" _SLACK_WEBHOOK_URL = 'https://
+hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlcak
+().__call__() #1 success sender except ExceptSlack as e: #2 except sender
+sys.exit() SendSlack().__call__() #3 customized sender ```
+### 2-6. *Line Notifier* - a. Register [https://notify-bot.line.me/](https://
 notify-bot.line.me/) - b. Go to mypage [https://notify-bot.line.me/my/](https:/
 /notify-bot.line.me/my/) - c. Click `Generate Token`, enter Service Name and
 click `1-on-1 chat with LINE` (anything you like) - d. Copy Token. ```python
 import sys from ExceptNotifier import ExceptLine, SuccessLine, SendLine
 sys.excepthook = ExceptLine.__call__ # Define the next two variables optionally
 when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-
 xxxxxx" _LINE_NOTIFY_API_TOKEN = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
 ().__call__() #1 success sender except ExceptLine as e: #2 except sender
 sys.exit() SendLine().__call__() #3 customized sender ```
-## 2-7. *SMS Notifier* - a. Sign up for Twilio. [https://www.twilio.com/en-us]
+### 2-7. *SMS Notifier* - a. Sign up for Twilio. [https://www.twilio.com/en-us]
 (https://www.twilio.com/en-us) - b. Click Console in the upper right corner. -
 c. Copy the variables provided in the console. ```python import sys from
 ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
 ExceptSMS.__call__ # Define the next two variables optionally when using
 OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-xxxxxx"
 _TWILIO_SID = 'xxxx' _TWILIO_TOKEN = 'yyyyyy'
 _RECIPIENT_PHONE_NUMBER="+aaaaaa", _SENDER_PHONE_NUMBER="+bbbbbb", try: print
 (1/10) SuccessSMS().__call__() #1 success sender except ExceptSMS as e: #2
 except sender sys.exit() SendSMS().__call__() #3 customized sender ```
-## 2-8. *Teams Notifier* - a. Create the channel that you want to notify. - b.
+### 2-8. *Teams Notifier* - a. Create the channel that you want to notify. - b.
 App - Search: webhook - Incoming Webhook [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
 the webhook incoming application is available. - c. Go to the team channel to
@@ -243,15 +230,15 @@
 ```python import sys from ExceptNotifier import ExceptTeams, SuccessTeams,
 SendTeams sys.excepthook = ExceptTeams.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _TEAMS_WEBHOOK_URL = 'microsoft webhook
 _TEAMS_WEBHOOK_URL' try: print(1/20) SuccessTeams().__call__() #1 success
 sender except ExceptTeams as e: #2 except sender sys.exit() SendTeams
 ().__call__() #3 customized sender ```
-## 2-9. *Kakaotalk Notifier* - a. Sign up at the following site: [https://
+### 2-9. *Kakaotalk Notifier* - a. Sign up at the following site: [https://
 developers.kakao.com/](https://developers.kakao.com/) - b. Click "My
 Application" on the top bar. - c. Click "Add an application," set a name, and
 create it. - d. Click "Kakao Login" in the left menu, then change the State of
 "Kakao Login Activation" to ON on the resulting page. - e. In My Application >
 Product Settings > Kakao Login, be sure to set Redirect URI as follows: [https:
 //example.com/oauth](https://example.com/oauth) - f. In the left Consent Items
 menu, set "Send message in KakaoTalk" to selective agreement. - g. Copy the
@@ -263,27 +250,36 @@
 creating and removing a test application, but for security reasons, your API
 key should not be exposed to the outside world.**
 ```python import sys from ExceptNotifier import ExceptKakao, SuccessKakao,
 SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _KAKAO_TOKEN_PATH = 'xxxx/xxx/xxx.json'' try: print(1/
 0) SuccessKakao().__call__() #1 success sender except ExceptKakao as e: #2
-except sender sys.exit() SendKakao().__call__() #3 customized sender ```
-## 2-10. *Beep Notifier* No setup is required. Use as follows. ```python from
+except sender sys.exit() SendKakao().__call__() #3 customized sender ``` ### 2-
+10. *Wechat Notifier* a. Get Webhook URL by visiting [here](https://
+work.weixin.qq.com/api/doc/90000/90136/91770) ```python import sys from
+ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat # Define the next
+two variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-
+turbo" # _OPEN_AI_API="sk-xxxxxx" _WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__
+() #1 success sender except ExceptWechat as e: #2 except sender sys.exit()
+SendWechat().__call__() #3 customized sender ```
+### 2-11. *Beep Notifier* No setup is required. Use as follows. ```python from
 Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep() BEEP_TIME = 1
 sys.excepthook = ExceptBeep.__call__ try: print(1/20) SuccessBeep().__call__()
 #1 success beep-beep except ExceptBeep as e: #2 except beep-beep sys.exit()
 SendBeep().__call__() #3 customized beep-beep beep() ```
-## 2-11. *Desktop Notifier* No setup is required. Use as follows. ```python
+### 2-12. *Desktop Notifier* No setup is required. Use as follows. ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1 success
 sender except ExceptDesktop as e: #2 except sender sys.exit() SendDesktop
 ().__call__() #3 customized sender ```
+## Sender
 
 
 # License MIT # Code of Conduct Everyone participating in the `ExceptNotifier`
 project, and in particular in the issue tracker, pull requests, and social
 media activity, is expected to treat other people with respect and more
 generally to follow the guidelines articulated in [the Python Community Code of
 Conduct](https://www.python.org/psf/conduct/). ##### The package is currently
```

### Comparing `ExceptNotifier-0.1.7/ExceptNotifier.egg-info/SOURCES.txt` & `exceptnotifier-0.1.8/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,14 @@
 ExceptNotifier/base/slack_sender.py
 ExceptNotifier/base/sms_sender.py
 ExceptNotifier/base/teams_sender.py
 ExceptNotifier/base/telegram_sender.py
 ExceptNotifier/base/wechat_sender.py
 ExceptNotifier/base/whatsapp_sender.py
 ExceptNotifier/utils/__init__.py
-ExceptNotifier/utils/kakao_token.py
+ExceptNotifier/utils/kakao_token.py
+exceptnotifier.egg-info/PKG-INFO
+exceptnotifier.egg-info/SOURCES.txt
+exceptnotifier.egg-info/dependency_links.txt
+exceptnotifier.egg-info/entry_points.txt
+exceptnotifier.egg-info/requires.txt
+exceptnotifier.egg-info/top_level.txt
```

### Comparing `ExceptNotifier-0.1.7/LICENSE` & `exceptnotifier-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.7/PKG-INFO` & `exceptnotifier-0.1.8/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ExceptNotifier
-Version: 0.1.7
+Name: exceptnotifier
+Version: 0.1.8
 Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
 Home-page: https://github.com/dsdanielpark/ExceptNotifier
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -60,14 +60,15 @@
 - [Discord](https://discord.com/)
 - [Slack](https://slack.com/)
 - [Google Mail](https://mail.google.com/)
 - [Line](https://line.me/en/)
 - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/)
 - [Microsoft Teams](https://www.microsoft.com/en/microsoft-teams/download-app)
 - [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
+- [Wecaht](https://www.wechat.com/)
 - SMS Sending using [Twilio](https://www.twilio.com/en-us)
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 
 <Br>
 
 ### AI Debugging using OpenAI API
@@ -204,31 +205,33 @@
 ```
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ex4.png)
 
 
 <br><br>
 
-# 2. Features
+# Feature
+
+## Notifier
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 
 
-## 2-1. *Telegram Notifier*
+### 2-1. *Telegram Notifier*
 
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
 - b. Type /newbot to create a new bot <br>
 - c. Give your bot a name & a username <br>
 - d. Copy your new Telegram bot’s token <br>
 
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
 <br><br>
  
-### a. Without OpenAI API
+#### a. Without OpenAI API
 
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys
 sys.excepthook = ExceptTelegram.__call__
 
 _TELEGRAM_TOKEN = "xxxx"
@@ -243,15 +246,15 @@
 SendTelegram().__call__()        #3. customized sender     
 ```
 
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/fig44.png)
 
 
-### b. With OpenAI API
+#### b. With OpenAI API
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys
 sys.excepthook = ExceptTelegram.__call__
 
 _TELEGRAM_TOKEN = "xxxx"
 _OPEN_AI_MODEL="gpt-3.5-turbo"
@@ -265,15 +268,15 @@
     sys.exit()
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
-## 2-2. *Mail Notifier*
+### 2-2. *Mail Notifier*
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en). 
 
 ```python
 import sys
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail
@@ -347,15 +350,15 @@
 
 SendMail().__call__() 
 ```
 </details>
 
 <br>
 
-## 2-3. *Discord Notifier*
+### 2-3. *Discord Notifier*
 - a. Select the channel to receive notifications.
 - b. Click "Edit Channel" in the upper right corner of the chat window.
 - c. Click Integrations - Webhook - New Webhook.
 - d. Then click Copy Webhook.
 
 ```python
 import sys
@@ -375,15 +378,15 @@
     sys.exit()
 
 SendDiscord().__call__()        #3 customized sender       
 ```
 
 <br>
 
-## 2-4. *Chime Notifier*
+### 2-4. *Chime Notifier*
 - a. Select the Chat room to receive notifications.
 - b. Click "Room Setting" in the upper right corner.
 - c. Click "Manage Webhook and bot."
 - d. Create Add Webhook, set it up, then click Copy Webhook.
 ```python
 import sys
 from ExceptNotifier import SuccessChime, ExceptChime, SendChime
@@ -401,15 +404,15 @@
 except ExceptChime as e:      #2 except sender            
     sys.exit()
 
 SendChime().__call__()        #3 customized sender       
 ```
 <br>
 
-## 2-5. *Slack Notifier*
+### 2-5. *Slack Notifier*
 - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App`
 - c. Add webhook: Click `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace
 - d. Copy `Webhook URL`
 
 ```python
 import sys
@@ -427,15 +430,15 @@
 except ExceptSlack as e:      #2 except sender            
     sys.exit()
 
 SendSlack().__call__()        #3 customized sender     
 ```
 <Br>
 
-## 2-6. *Line Notifier*
+### 2-6. *Line Notifier*
 - a. Register [https://notify-bot.line.me/](https://notify-bot.line.me/)
 - b. Go to mypage [https://notify-bot.line.me/my/](https://notify-bot.line.me/my/)
 - c. Click `Generate Token`, enter Service Name and click `1-on-1 chat with LINE` (anything you like)
 - d. Copy Token.
 
 ```python
 import sys
@@ -454,15 +457,15 @@
     sys.exit()
 
 SendLine().__call__()        #3 customized sender          
 ```
 
 <Br>
 
-## 2-7. *SMS Notifier*
+### 2-7. *SMS Notifier*
 - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://www.twilio.com/en-us)
 - b. Click Console in the upper right corner.
 - c. Copy the variables provided in the console.
 
 ```python
 import sys
 from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS
@@ -482,15 +485,15 @@
 except ExceptSMS as e:      #2 except sender
     sys.exit()
 
 SendSMS().__call__()        #3 customized sender        
 ```
 <Br>
 
-## 2-8. *Teams Notifier*
+### 2-8. *Teams Notifier*
 - a. Create the channel that you want to notify.
 - b. App - Search: webhook - Incoming Webhook [https://teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog)
 - c. Click `Request Approval` <br>
 After you can use webhook incomming. Proceed to next steps.
 Microsoft Teams allows limited application access per organization, so it can only be used if the webhook incoming application is available.
 - c. Go to the team channel to receive notifications, and click `Connectors` in Settings.
 - d. `Connectors` After configuring webhook incoming in Connector, copy the webhook URL.
@@ -512,15 +515,15 @@
     sys.exit()
 
 SendTeams().__call__()        #3 customized sender        
 ```
 
 <Br>
 
-## 2-9. *Kakaotalk Notifier*
+### 2-9. *Kakaotalk Notifier*
 - a. Sign up at the following site: [https://developers.kakao.com/](https://developers.kakao.com/)
 - b. Click "My Application" on the top bar.
 - c. Click "Add an application," set a name, and create it.
 - d. Click "Kakao Login" in the left menu, then change the State of "Kakao Login Activation" to ON on the resulting page.
 - e. In My Application > Product Settings > Kakao Login, be sure to set Redirect URI as follows: [https://example.com/oauth](https://example.com/oauth)
 - f. In the left Consent Items menu, set "Send message in KakaoTalk" to selective agreement.
 - g. Copy the REST API Key in My Application > App Settings > Summary, and go to the following document.
@@ -544,17 +547,40 @@
     SuccessKakao().__call__() #1 success sender          
 except ExceptKakao as e:      #2 except sender            
     sys.exit()
 
 SendKakao().__call__()        #3 customized sender         
 ```
 
+
+### 2-10. *Wechat Notifier*
+a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+
+```python
+import sys
+from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat
+
+# Define the next two variables optionally when using OpenAI's API.
+# _OPEN_AI_MODEL="gpt-3.5-turbo"    
+# _OPEN_AI_API="sk-xxxxxx"
+_WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__
+
+try:
+    print(1/0)  
+    SuccessWechat().__call__() #1 success sender          
+except ExceptWechat as e:      #2 except sender            
+    sys.exit()
+
+SendWechat().__call__()        #3 customized sender       
+```
+
 <Br>
 
-## 2-10. *Beep Notifier*
+### 2-11. *Beep Notifier*
 No setup is required. Use as follows.
 
 ```python
 from Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep()
 BEEP_TIME = 1
 sys.excepthook = ExceptBeep.__call__
 
@@ -570,15 +596,15 @@
 beep()
 
 ```
 
 <Br>
 
 
-## 2-11. *Desktop Notifier*
+### 2-12. *Desktop Notifier*
 No setup is required. Use as follows.
 
 ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__
 # Define the next two variables optionally when using OpenAI's API.
 # _OPEN_AI_MODEL="gpt-3.5-turbo"    
@@ -590,14 +616,20 @@
 
 except ExceptDesktop as e:      #2 except sender            
     sys.exit()
 
 SendDesktop().__call__()        #3 customized sender         
 ```
 
+<br>
+
+## Sender
+
+
+
 <Br><br><br>
 
 # License
 MIT
 
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ExceptNotifier Version: 0.1.7 Summary: With
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.1.8 Summary: With
 Python's try-except to receive notifications about Errors or Successes in your
 code through messenger app or email. Home-page: https://github.com/
 dsdanielpark/ExceptNotifier Author: daniel park Author-email:
 parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
 Alarm,Error notifications,Customizable notifications,Traceback
 management,Single line alarm Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research Classifier: Natural Language
@@ -36,18 +36,18 @@
 (https://img.shields.io/badge/pypi-ExceptNotifier-orange) ```
 
 ### Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
 (https://discord.com/) - [Slack](https://slack.com/) - [Google Mail](https://
 mail.google.com/) - [Line](https://line.me/en/) - [AWS Chime](https://
 aws.amazon.com/ko/chime/download-chime/) - [Microsoft Teams](https://
 www.microsoft.com/en/microsoft-teams/download-app) - [Kakao Talk](https://
-www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - SMS Sending using
-[Twilio](https://www.twilio.com/en-us) - Desktop Notification using [Plyer]
-(https://github.com/kivy/plyer) - Beep Sound from [system](https://
-docs.python.org/3/library/winsound.html)
+www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - [Wecaht](https://
+www.wechat.com/) - SMS Sending using [Twilio](https://www.twilio.com/en-us) -
+Desktop Notification using [Plyer](https://github.com/kivy/plyer) - Beep Sound
+from [system](https://docs.python.org/3/library/winsound.html)
 ### AI Debugging using OpenAI API If you have OpenAI API Key and model name,
 you can get information and code examples for debugging in any application. -
 [OPEN AI API](https://platform.openai.com/docs/introduction)
 
 # Quick Start ```bash pip install ExceptNotifier pip install exceptnotifier
 conda install ExceptNotifier conda install exceptnotifier ```
 # App Setup Overview - The variables in the following table must not be
@@ -123,38 +123,39 @@
 SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack,
 SendTeams, SendDesktope, SendBeep ``` *Example* ```python from ExceptNotifier
 import SendTelgeram _TELEGRAM_TOKEN = "xxxx" SendTelegram().__call__() #
 sending message to telegram noti = SendTelegram() noti() # sending message to
 telegram ``` ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/
 assets/imgs/ex4.png)
 
-# 2. Features You can receive debugging information from ChatGPT via OpenAI's
-API when using the Except statement. The syntax remains the same, but you'll
-need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API` ## 2-1.
-*Telegram Notifier* - a. Open your telegram app and search for BotFather. (A
-built-in Telegram bot that helps users create custom Telegram bots)
+# Feature ## Notifier You can receive debugging information from ChatGPT via
+OpenAI's API when using the Except statement. The syntax remains the same, but
+you'll need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API`
+### 2-1. *Telegram Notifier* - a. Open your telegram app and search for
+BotFather. (A built-in Telegram bot that helps users create custom Telegram
+bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/
 bots/api)
 
-### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
+#### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
 SuccessTelegram, SendTelegram import sys sys.excepthook =
 ExceptTelegram.__call__ _TELEGRAM_TOKEN = "xxxx" try: print(1/0)
 SuccessTelegram().__call__() #1. success sender except ExceptTelegram as e: #2.
 except sender sys.exit() SendTelegram().__call__() #3. customized sender ``` !
 [](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-fig44.png) ### b. With OpenAI API ```python from ExceptNotifier import
+fig44.png) #### b. With OpenAI API ```python from ExceptNotifier import
 ExceptTelegram, SuccessTelegram, SendTelegram import sys sys.excepthook =
 ExceptTelegram.__call__ _TELEGRAM_TOKEN = "xxxx" _OPEN_AI_MODEL="gpt-3.5-turbo"
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
 success sender except ExceptTelegram as e: #2. except sender sys.exit()
 SendTelegram().__call__() #3. customized sender ```
-## 2-2. *Mail Notifier* In the except statement, an email is sent along with
+### 2-2. *Mail Notifier* In the except statement, an email is sent along with
 the error message. Additionally, you can send emails from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
 (https://myaccount.google.com/u/3/apppasswords?utm_source=google-
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
@@ -177,64 +178,64 @@
 for Python developers... ```python import sys from ExceptNotifier import
 ExceptMail, SuccessMail, SendMail sys.excepthook = ExceptMail.__call__ # Define
 the next two variables optionally when using OpenAI's API. #
 _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-xxxxxx" _GAMIL_RECIPIENT_ADDR
 = 'xxxxxxx@gmail.com' _GMAIL_SENDER_ADDR = 'yyyyyy@gmail.com'
 _GMAIL_APP_PASSWORD_OF_SENDER = 'zzzzzz' try: 'your code' SuccessMail
 ().__call__() except ExceptMail: pass SendMail().__call__() ```
-## 2-3. *Discord Notifier* - a. Select the channel to receive notifications. -
+### 2-3. *Discord Notifier* - a. Select the channel to receive notifications. -
 b. Click "Edit Channel" in the upper right corner of the chat window. - c.
 Click Integrations - Webhook - New Webhook. - d. Then click Copy Webhook.
 ```python import sys from ExceptNotifier import ExceptDiscord, SuccessDiscord,
 SendDiscord sys.excepthook = ExceptDiscord.__call__ # Define the next two
 variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo"
 # _OPEN_AI_API="sk-xxxxxx" _DISCORD_WEBHOOK_URL = "xxxxxxxxxxxxxxxxx" try:
 print(1/20) SuccessDiscord().__call__() #1 success sender except ExceptDiscord
 as e: #2 except sender sys.exit() SendDiscord().__call__() #3 customized sender
 ```
-## 2-4. *Chime Notifier* - a. Select the Chat room to receive notifications. -
+### 2-4. *Chime Notifier* - a. Select the Chat room to receive notifications. -
 b. Click "Room Setting" in the upper right corner. - c. Click "Manage Webhook
 and bot." - d. Create Add Webhook, set it up, then click Copy Webhook.
 ```python import sys from ExceptNotifier import SuccessChime, ExceptChime,
 SendChime sys.excepthook = ExceptChime.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _CHIME_WEBHOOK_URL = "xxxxxxxxxxxxxxxxxx" try: print
 (1/0) SuccessChime().__call__() #1 success sender except ExceptChime as e: #2
 except sender sys.exit() SendChime().__call__() #3 customized sender ```
-## 2-5. *Slack Notifier* - a. visit https://api.slack.com/ - b. `Create an app`
-- `From scratch` - `Create App` - c. Add webhook: Click `Incoming Webhooks` -
-Activate Incomming `On` - Add New Webhook to Workspace - d. Copy `Webhook URL`
-```python import sys from ExceptNotifier import ExceptSlack, SuccessSlcak,
-SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next two variables
-optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
-_OPEN_AI_API="sk-xxxxxx" _SLACK_WEBHOOK_URL = 'https://hooks.slack.com/
-services/xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlcak().__call__() #1
-success sender except ExceptSlack as e: #2 except sender sys.exit() SendSlack
-().__call__() #3 customized sender ```
-## 2-6. *Line Notifier* - a. Register [https://notify-bot.line.me/](https://
+### 2-5. *Slack Notifier* - a. visit https://api.slack.com/ - b. `Create an
+app` - `From scratch` - `Create App` - c. Add webhook: Click `Incoming
+Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace - d. Copy
+`Webhook URL` ```python import sys from ExceptNotifier import ExceptSlack,
+SuccessSlcak, SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next
+two variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-
+turbo" # _OPEN_AI_API="sk-xxxxxx" _SLACK_WEBHOOK_URL = 'https://
+hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlcak
+().__call__() #1 success sender except ExceptSlack as e: #2 except sender
+sys.exit() SendSlack().__call__() #3 customized sender ```
+### 2-6. *Line Notifier* - a. Register [https://notify-bot.line.me/](https://
 notify-bot.line.me/) - b. Go to mypage [https://notify-bot.line.me/my/](https:/
 /notify-bot.line.me/my/) - c. Click `Generate Token`, enter Service Name and
 click `1-on-1 chat with LINE` (anything you like) - d. Copy Token. ```python
 import sys from ExceptNotifier import ExceptLine, SuccessLine, SendLine
 sys.excepthook = ExceptLine.__call__ # Define the next two variables optionally
 when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-
 xxxxxx" _LINE_NOTIFY_API_TOKEN = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
 ().__call__() #1 success sender except ExceptLine as e: #2 except sender
 sys.exit() SendLine().__call__() #3 customized sender ```
-## 2-7. *SMS Notifier* - a. Sign up for Twilio. [https://www.twilio.com/en-us]
+### 2-7. *SMS Notifier* - a. Sign up for Twilio. [https://www.twilio.com/en-us]
 (https://www.twilio.com/en-us) - b. Click Console in the upper right corner. -
 c. Copy the variables provided in the console. ```python import sys from
 ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
 ExceptSMS.__call__ # Define the next two variables optionally when using
 OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-xxxxxx"
 _TWILIO_SID = 'xxxx' _TWILIO_TOKEN = 'yyyyyy'
 _RECIPIENT_PHONE_NUMBER="+aaaaaa", _SENDER_PHONE_NUMBER="+bbbbbb", try: print
 (1/10) SuccessSMS().__call__() #1 success sender except ExceptSMS as e: #2
 except sender sys.exit() SendSMS().__call__() #3 customized sender ```
-## 2-8. *Teams Notifier* - a. Create the channel that you want to notify. - b.
+### 2-8. *Teams Notifier* - a. Create the channel that you want to notify. - b.
 App - Search: webhook - Incoming Webhook [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
 the webhook incoming application is available. - c. Go to the team channel to
@@ -243,15 +244,15 @@
 ```python import sys from ExceptNotifier import ExceptTeams, SuccessTeams,
 SendTeams sys.excepthook = ExceptTeams.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _TEAMS_WEBHOOK_URL = 'microsoft webhook
 _TEAMS_WEBHOOK_URL' try: print(1/20) SuccessTeams().__call__() #1 success
 sender except ExceptTeams as e: #2 except sender sys.exit() SendTeams
 ().__call__() #3 customized sender ```
-## 2-9. *Kakaotalk Notifier* - a. Sign up at the following site: [https://
+### 2-9. *Kakaotalk Notifier* - a. Sign up at the following site: [https://
 developers.kakao.com/](https://developers.kakao.com/) - b. Click "My
 Application" on the top bar. - c. Click "Add an application," set a name, and
 create it. - d. Click "Kakao Login" in the left menu, then change the State of
 "Kakao Login Activation" to ON on the resulting page. - e. In My Application >
 Product Settings > Kakao Login, be sure to set Redirect URI as follows: [https:
 //example.com/oauth](https://example.com/oauth) - f. In the left Consent Items
 menu, set "Send message in KakaoTalk" to selective agreement. - g. Copy the
@@ -263,27 +264,36 @@
 creating and removing a test application, but for security reasons, your API
 key should not be exposed to the outside world.**
 ```python import sys from ExceptNotifier import ExceptKakao, SuccessKakao,
 SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _KAKAO_TOKEN_PATH = 'xxxx/xxx/xxx.json'' try: print(1/
 0) SuccessKakao().__call__() #1 success sender except ExceptKakao as e: #2
-except sender sys.exit() SendKakao().__call__() #3 customized sender ```
-## 2-10. *Beep Notifier* No setup is required. Use as follows. ```python from
+except sender sys.exit() SendKakao().__call__() #3 customized sender ``` ### 2-
+10. *Wechat Notifier* a. Get Webhook URL by visiting [here](https://
+work.weixin.qq.com/api/doc/90000/90136/91770) ```python import sys from
+ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat # Define the next
+two variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-
+turbo" # _OPEN_AI_API="sk-xxxxxx" _WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__
+() #1 success sender except ExceptWechat as e: #2 except sender sys.exit()
+SendWechat().__call__() #3 customized sender ```
+### 2-11. *Beep Notifier* No setup is required. Use as follows. ```python from
 Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep() BEEP_TIME = 1
 sys.excepthook = ExceptBeep.__call__ try: print(1/20) SuccessBeep().__call__()
 #1 success beep-beep except ExceptBeep as e: #2 except beep-beep sys.exit()
 SendBeep().__call__() #3 customized beep-beep beep() ```
-## 2-11. *Desktop Notifier* No setup is required. Use as follows. ```python
+### 2-12. *Desktop Notifier* No setup is required. Use as follows. ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1 success
 sender except ExceptDesktop as e: #2 except sender sys.exit() SendDesktop
 ().__call__() #3 customized sender ```
+## Sender
 
 
 # License MIT # Code of Conduct Everyone participating in the `ExceptNotifier`
 project, and in particular in the issue tracker, pull requests, and social
 media activity, is expected to treat other people with respect and more
 generally to follow the guidelines articulated in [the Python Community Code of
 Conduct](https://www.python.org/psf/conduct/). ##### The package is currently
```

### Comparing `ExceptNotifier-0.1.7/README.md` & `exceptnotifier-0.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: exceptnotifier
+Version: 0.1.8
+Summary: With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.
+Home-page: https://github.com/dsdanielpark/ExceptNotifier
+Author: daniel park
+Author-email: parkminwoo1991@gmail.com
+Keywords: Exception,Python,Python Exception Alarm,Error notifications,Customizable notifications,Traceback management,Single line alarm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Development Status :: 3 - Alpha <br>
 *Copyright (c) 2023 MinWoo Park, South Korea*
 <br>
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ExceptNotifier_logo.png)
 
 <h3 align="center">Integrates AI-assisted debugging notifications into Python try-except statements for various messaging applications. </h3>
 
@@ -38,14 +60,15 @@
 - [Discord](https://discord.com/)
 - [Slack](https://slack.com/)
 - [Google Mail](https://mail.google.com/)
 - [Line](https://line.me/en/)
 - [AWS Chime](https://aws.amazon.com/ko/chime/download-chime/)
 - [Microsoft Teams](https://www.microsoft.com/en/microsoft-teams/download-app)
 - [Kakao Talk](https://www.kakaocorp.com/page/service/service/KakaoTalk?lang=en)
+- [Wecaht](https://www.wechat.com/)
 - SMS Sending using [Twilio](https://www.twilio.com/en-us)
 - Desktop Notification using [Plyer](https://github.com/kivy/plyer)
 - Beep Sound from [system](https://docs.python.org/3/library/winsound.html)
 
 <Br>
 
 ### AI Debugging using OpenAI API
@@ -182,31 +205,33 @@
 ```
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/ex4.png)
 
 
 <br><br>
 
-# 2. Features
+# Feature
+
+## Notifier
 You can receive debugging information from ChatGPT via OpenAI's API when using the Except statement. The syntax remains the same, but you'll need to configure these two variables:
 `_OPEN_AI_MODEL`,`_OPEN_AI_API`
 
 
 
-## 2-1. *Telegram Notifier*
+### 2-1. *Telegram Notifier*
 
 - a. Open your telegram app and search for BotFather. (A built-in Telegram bot that helps users create custom Telegram bots) <br>
 - b. Type /newbot to create a new bot <br>
 - c. Give your bot a name & a username <br>
 - d. Copy your new Telegram bot’s token <br>
 
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/bots/api)
 <br><br>
  
-### a. Without OpenAI API
+#### a. Without OpenAI API
 
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys
 sys.excepthook = ExceptTelegram.__call__
 
 _TELEGRAM_TOKEN = "xxxx"
@@ -221,15 +246,15 @@
 SendTelegram().__call__()        #3. customized sender     
 ```
 
 
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/fig44.png)
 
 
-### b. With OpenAI API
+#### b. With OpenAI API
 ```python
 from ExceptNotifier import ExceptTelegram, SuccessTelegram, SendTelegram
 import sys
 sys.excepthook = ExceptTelegram.__call__
 
 _TELEGRAM_TOKEN = "xxxx"
 _OPEN_AI_MODEL="gpt-3.5-turbo"
@@ -243,15 +268,15 @@
     sys.exit()
 
 SendTelegram().__call__()        #3. customized sender     
 
 ```
 <br>
 
-## 2-2. *Mail Notifier*
+### 2-2. *Mail Notifier*
 In the except statement, an email is sent along with the error message. Additionally, you can send emails from any desired line. <br>
 - a. Log in with the sender's email ID. <br>
 - b. Obtain an app password for sending Google Mail at the following [link](https://myaccount.google.com/u/3/apppasswords?utm_source=google-account&utm_medium=myaccountsecurity&utm_campaign=tsv-settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw) or [google document](https://support.google.com/accounts/answer/185833?hl=en). 
 
 ```python
 import sys
 from ExceptNotifier import ExceptMail, SuccessMail, SendMail
@@ -325,15 +350,15 @@
 
 SendMail().__call__() 
 ```
 </details>
 
 <br>
 
-## 2-3. *Discord Notifier*
+### 2-3. *Discord Notifier*
 - a. Select the channel to receive notifications.
 - b. Click "Edit Channel" in the upper right corner of the chat window.
 - c. Click Integrations - Webhook - New Webhook.
 - d. Then click Copy Webhook.
 
 ```python
 import sys
@@ -353,15 +378,15 @@
     sys.exit()
 
 SendDiscord().__call__()        #3 customized sender       
 ```
 
 <br>
 
-## 2-4. *Chime Notifier*
+### 2-4. *Chime Notifier*
 - a. Select the Chat room to receive notifications.
 - b. Click "Room Setting" in the upper right corner.
 - c. Click "Manage Webhook and bot."
 - d. Create Add Webhook, set it up, then click Copy Webhook.
 ```python
 import sys
 from ExceptNotifier import SuccessChime, ExceptChime, SendChime
@@ -379,15 +404,15 @@
 except ExceptChime as e:      #2 except sender            
     sys.exit()
 
 SendChime().__call__()        #3 customized sender       
 ```
 <br>
 
-## 2-5. *Slack Notifier*
+### 2-5. *Slack Notifier*
 - a. visit https://api.slack.com/
 - b. `Create an app` - `From scratch` - `Create App`
 - c. Add webhook: Click `Incoming Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace
 - d. Copy `Webhook URL`
 
 ```python
 import sys
@@ -405,15 +430,15 @@
 except ExceptSlack as e:      #2 except sender            
     sys.exit()
 
 SendSlack().__call__()        #3 customized sender     
 ```
 <Br>
 
-## 2-6. *Line Notifier*
+### 2-6. *Line Notifier*
 - a. Register [https://notify-bot.line.me/](https://notify-bot.line.me/)
 - b. Go to mypage [https://notify-bot.line.me/my/](https://notify-bot.line.me/my/)
 - c. Click `Generate Token`, enter Service Name and click `1-on-1 chat with LINE` (anything you like)
 - d. Copy Token.
 
 ```python
 import sys
@@ -432,15 +457,15 @@
     sys.exit()
 
 SendLine().__call__()        #3 customized sender          
 ```
 
 <Br>
 
-## 2-7. *SMS Notifier*
+### 2-7. *SMS Notifier*
 - a. Sign up for Twilio. [https://www.twilio.com/en-us](https://www.twilio.com/en-us)
 - b. Click Console in the upper right corner.
 - c. Copy the variables provided in the console.
 
 ```python
 import sys
 from ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS
@@ -460,15 +485,15 @@
 except ExceptSMS as e:      #2 except sender
     sys.exit()
 
 SendSMS().__call__()        #3 customized sender        
 ```
 <Br>
 
-## 2-8. *Teams Notifier*
+### 2-8. *Teams Notifier*
 - a. Create the channel that you want to notify.
 - b. App - Search: webhook - Incoming Webhook [https://teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog)
 - c. Click `Request Approval` <br>
 After you can use webhook incomming. Proceed to next steps.
 Microsoft Teams allows limited application access per organization, so it can only be used if the webhook incoming application is available.
 - c. Go to the team channel to receive notifications, and click `Connectors` in Settings.
 - d. `Connectors` After configuring webhook incoming in Connector, copy the webhook URL.
@@ -490,15 +515,15 @@
     sys.exit()
 
 SendTeams().__call__()        #3 customized sender        
 ```
 
 <Br>
 
-## 2-9. *Kakaotalk Notifier*
+### 2-9. *Kakaotalk Notifier*
 - a. Sign up at the following site: [https://developers.kakao.com/](https://developers.kakao.com/)
 - b. Click "My Application" on the top bar.
 - c. Click "Add an application," set a name, and create it.
 - d. Click "Kakao Login" in the left menu, then change the State of "Kakao Login Activation" to ON on the resulting page.
 - e. In My Application > Product Settings > Kakao Login, be sure to set Redirect URI as follows: [https://example.com/oauth](https://example.com/oauth)
 - f. In the left Consent Items menu, set "Send message in KakaoTalk" to selective agreement.
 - g. Copy the REST API Key in My Application > App Settings > Summary, and go to the following document.
@@ -522,17 +547,40 @@
     SuccessKakao().__call__() #1 success sender          
 except ExceptKakao as e:      #2 except sender            
     sys.exit()
 
 SendKakao().__call__()        #3 customized sender         
 ```
 
+
+### 2-10. *Wechat Notifier*
+a. Get Webhook URL by visiting [here](https://work.weixin.qq.com/api/doc/90000/90136/91770)
+
+```python
+import sys
+from ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat
+
+# Define the next two variables optionally when using OpenAI's API.
+# _OPEN_AI_MODEL="gpt-3.5-turbo"    
+# _OPEN_AI_API="sk-xxxxxx"
+_WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__
+
+try:
+    print(1/0)  
+    SuccessWechat().__call__() #1 success sender          
+except ExceptWechat as e:      #2 except sender            
+    sys.exit()
+
+SendWechat().__call__()        #3 customized sender       
+```
+
 <Br>
 
-## 2-10. *Beep Notifier*
+### 2-11. *Beep Notifier*
 No setup is required. Use as follows.
 
 ```python
 from Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep()
 BEEP_TIME = 1
 sys.excepthook = ExceptBeep.__call__
 
@@ -548,15 +596,15 @@
 beep()
 
 ```
 
 <Br>
 
 
-## 2-11. *Desktop Notifier*
+### 2-12. *Desktop Notifier*
 No setup is required. Use as follows.
 
 ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__
 # Define the next two variables optionally when using OpenAI's API.
 # _OPEN_AI_MODEL="gpt-3.5-turbo"    
@@ -568,14 +616,20 @@
 
 except ExceptDesktop as e:      #2 except sender            
     sys.exit()
 
 SendDesktop().__call__()        #3 customized sender         
 ```
 
+<br>
+
+## Sender
+
+
+
 <Br><br><br>
 
 # License
 MIT
 
 # Code of Conduct
 Everyone participating in the `ExceptNotifier` project, and in particular in the issue tracker, pull requests, and social media activity, is expected to treat other people with respect and more generally to follow the guidelines articulated in [the Python Community Code of Conduct](https://www.python.org/psf/conduct/).
```

#### html2text {}

```diff
@@ -1,8 +1,22 @@
-Development Status :: 3 - Alpha
+Metadata-Version: 2.1 Name: exceptnotifier Version: 0.1.8 Summary: With
+Python's try-except to receive notifications about Errors or Successes in your
+code through messenger app or email. Home-page: https://github.com/
+dsdanielpark/ExceptNotifier Author: daniel park Author-email:
+parkminwoo1991@gmail.com Keywords: Exception,Python,Python Exception
+Alarm,Error notifications,Customizable notifications,Traceback
+management,Single line alarm Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research Classifier: Natural Language
+:: English Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE Development Status :: 3 - Alpha
 *Copyright (c) 2023 MinWoo Park, South Korea*
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
 ExceptNotifier_logo.png)
   **** Integrates AI-assisted debugging notifications into Python try-except
               statements for various messaging applications. ****
               [PyPI] [Downloads] [conda-forge] [Code_style:_black]
 ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
@@ -22,18 +36,18 @@
 (https://img.shields.io/badge/pypi-ExceptNotifier-orange) ```
 
 ### Supporting Applications - [Telegram](https://telegram.org/) - [Discord]
 (https://discord.com/) - [Slack](https://slack.com/) - [Google Mail](https://
 mail.google.com/) - [Line](https://line.me/en/) - [AWS Chime](https://
 aws.amazon.com/ko/chime/download-chime/) - [Microsoft Teams](https://
 www.microsoft.com/en/microsoft-teams/download-app) - [Kakao Talk](https://
-www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - SMS Sending using
-[Twilio](https://www.twilio.com/en-us) - Desktop Notification using [Plyer]
-(https://github.com/kivy/plyer) - Beep Sound from [system](https://
-docs.python.org/3/library/winsound.html)
+www.kakaocorp.com/page/service/service/KakaoTalk?lang=en) - [Wecaht](https://
+www.wechat.com/) - SMS Sending using [Twilio](https://www.twilio.com/en-us) -
+Desktop Notification using [Plyer](https://github.com/kivy/plyer) - Beep Sound
+from [system](https://docs.python.org/3/library/winsound.html)
 ### AI Debugging using OpenAI API If you have OpenAI API Key and model name,
 you can get information and code examples for debugging in any application. -
 [OPEN AI API](https://platform.openai.com/docs/introduction)
 
 # Quick Start ```bash pip install ExceptNotifier pip install exceptnotifier
 conda install ExceptNotifier conda install exceptnotifier ```
 # App Setup Overview - The variables in the following table must not be
@@ -109,38 +123,39 @@
 SendTelegram, SendDiscord, SendSMS, SendMail, SendKakao, SendLine, SendSlack,
 SendTeams, SendDesktope, SendBeep ``` *Example* ```python from ExceptNotifier
 import SendTelgeram _TELEGRAM_TOKEN = "xxxx" SendTelegram().__call__() #
 sending message to telegram noti = SendTelegram() noti() # sending message to
 telegram ``` ![](https://github.com/dsdanielpark/ExceptNotifier/blob/main/
 assets/imgs/ex4.png)
 
-# 2. Features You can receive debugging information from ChatGPT via OpenAI's
-API when using the Except statement. The syntax remains the same, but you'll
-need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API` ## 2-1.
-*Telegram Notifier* - a. Open your telegram app and search for BotFather. (A
-built-in Telegram bot that helps users create custom Telegram bots)
+# Feature ## Notifier You can receive debugging information from ChatGPT via
+OpenAI's API when using the Except statement. The syntax remains the same, but
+you'll need to configure these two variables: `_OPEN_AI_MODEL`,`_OPEN_AI_API`
+### 2-1. *Telegram Notifier* - a. Open your telegram app and search for
+BotFather. (A built-in Telegram bot that helps users create custom Telegram
+bots)
 - b. Type /newbot to create a new bot
 - c. Give your bot a name & a username
 - d. Copy your new Telegram botâs token
 For more infomation, visit [Telegram Bot Father API](https://core.telegram.org/
 bots/api)
 
-### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
+#### a. Without OpenAI API ```python from ExceptNotifier import ExceptTelegram,
 SuccessTelegram, SendTelegram import sys sys.excepthook =
 ExceptTelegram.__call__ _TELEGRAM_TOKEN = "xxxx" try: print(1/0)
 SuccessTelegram().__call__() #1. success sender except ExceptTelegram as e: #2.
 except sender sys.exit() SendTelegram().__call__() #3. customized sender ``` !
 [](https://github.com/dsdanielpark/ExceptNotifier/blob/main/assets/imgs/
-fig44.png) ### b. With OpenAI API ```python from ExceptNotifier import
+fig44.png) #### b. With OpenAI API ```python from ExceptNotifier import
 ExceptTelegram, SuccessTelegram, SendTelegram import sys sys.excepthook =
 ExceptTelegram.__call__ _TELEGRAM_TOKEN = "xxxx" _OPEN_AI_MODEL="gpt-3.5-turbo"
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessTelegram().__call__() #1.
 success sender except ExceptTelegram as e: #2. except sender sys.exit()
 SendTelegram().__call__() #3. customized sender ```
-## 2-2. *Mail Notifier* In the except statement, an email is sent along with
+### 2-2. *Mail Notifier* In the except statement, an email is sent along with
 the error message. Additionally, you can send emails from any desired line.
 - a. Log in with the sender's email ID.
 - b. Obtain an app password for sending Google Mail at the following [link]
 (https://myaccount.google.com/u/3/apppasswords?utm_source=google-
 account&utm_medium=myaccountsecurity&utm_campaign=tsv-
 settings&rapt=AEjHL4N2bMRWO46VaMp_jP06zQK14BWNPv66l2o59iJ99CkO8BjYnmoRUe9dtSchkkbubHZMUhevkAnwVJRHb9ygO3afispNlw)
 or [google document](https://support.google.com/accounts/answer/185833?hl=en).
@@ -163,64 +178,64 @@
 for Python developers... ```python import sys from ExceptNotifier import
 ExceptMail, SuccessMail, SendMail sys.excepthook = ExceptMail.__call__ # Define
 the next two variables optionally when using OpenAI's API. #
 _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-xxxxxx" _GAMIL_RECIPIENT_ADDR
 = 'xxxxxxx@gmail.com' _GMAIL_SENDER_ADDR = 'yyyyyy@gmail.com'
 _GMAIL_APP_PASSWORD_OF_SENDER = 'zzzzzz' try: 'your code' SuccessMail
 ().__call__() except ExceptMail: pass SendMail().__call__() ```
-## 2-3. *Discord Notifier* - a. Select the channel to receive notifications. -
+### 2-3. *Discord Notifier* - a. Select the channel to receive notifications. -
 b. Click "Edit Channel" in the upper right corner of the chat window. - c.
 Click Integrations - Webhook - New Webhook. - d. Then click Copy Webhook.
 ```python import sys from ExceptNotifier import ExceptDiscord, SuccessDiscord,
 SendDiscord sys.excepthook = ExceptDiscord.__call__ # Define the next two
 variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo"
 # _OPEN_AI_API="sk-xxxxxx" _DISCORD_WEBHOOK_URL = "xxxxxxxxxxxxxxxxx" try:
 print(1/20) SuccessDiscord().__call__() #1 success sender except ExceptDiscord
 as e: #2 except sender sys.exit() SendDiscord().__call__() #3 customized sender
 ```
-## 2-4. *Chime Notifier* - a. Select the Chat room to receive notifications. -
+### 2-4. *Chime Notifier* - a. Select the Chat room to receive notifications. -
 b. Click "Room Setting" in the upper right corner. - c. Click "Manage Webhook
 and bot." - d. Create Add Webhook, set it up, then click Copy Webhook.
 ```python import sys from ExceptNotifier import SuccessChime, ExceptChime,
 SendChime sys.excepthook = ExceptChime.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _CHIME_WEBHOOK_URL = "xxxxxxxxxxxxxxxxxx" try: print
 (1/0) SuccessChime().__call__() #1 success sender except ExceptChime as e: #2
 except sender sys.exit() SendChime().__call__() #3 customized sender ```
-## 2-5. *Slack Notifier* - a. visit https://api.slack.com/ - b. `Create an app`
-- `From scratch` - `Create App` - c. Add webhook: Click `Incoming Webhooks` -
-Activate Incomming `On` - Add New Webhook to Workspace - d. Copy `Webhook URL`
-```python import sys from ExceptNotifier import ExceptSlack, SuccessSlcak,
-SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next two variables
-optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
-_OPEN_AI_API="sk-xxxxxx" _SLACK_WEBHOOK_URL = 'https://hooks.slack.com/
-services/xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlcak().__call__() #1
-success sender except ExceptSlack as e: #2 except sender sys.exit() SendSlack
-().__call__() #3 customized sender ```
-## 2-6. *Line Notifier* - a. Register [https://notify-bot.line.me/](https://
+### 2-5. *Slack Notifier* - a. visit https://api.slack.com/ - b. `Create an
+app` - `From scratch` - `Create App` - c. Add webhook: Click `Incoming
+Webhooks` - Activate Incomming `On` - Add New Webhook to Workspace - d. Copy
+`Webhook URL` ```python import sys from ExceptNotifier import ExceptSlack,
+SuccessSlcak, SendSlack sys.excepthook = ExceptSlack.__call__ # Define the next
+two variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-
+turbo" # _OPEN_AI_API="sk-xxxxxx" _SLACK_WEBHOOK_URL = 'https://
+hooks.slack.com/services/xxxxxxxxxxxxxxxxxxx' try: print(1/0) SuccessSlcak
+().__call__() #1 success sender except ExceptSlack as e: #2 except sender
+sys.exit() SendSlack().__call__() #3 customized sender ```
+### 2-6. *Line Notifier* - a. Register [https://notify-bot.line.me/](https://
 notify-bot.line.me/) - b. Go to mypage [https://notify-bot.line.me/my/](https:/
 /notify-bot.line.me/my/) - c. Click `Generate Token`, enter Service Name and
 click `1-on-1 chat with LINE` (anything you like) - d. Copy Token. ```python
 import sys from ExceptNotifier import ExceptLine, SuccessLine, SendLine
 sys.excepthook = ExceptLine.__call__ # Define the next two variables optionally
 when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-
 xxxxxx" _LINE_NOTIFY_API_TOKEN = 'xxxxxxxxxxx' try: print(1/20) SuccessLine
 ().__call__() #1 success sender except ExceptLine as e: #2 except sender
 sys.exit() SendLine().__call__() #3 customized sender ```
-## 2-7. *SMS Notifier* - a. Sign up for Twilio. [https://www.twilio.com/en-us]
+### 2-7. *SMS Notifier* - a. Sign up for Twilio. [https://www.twilio.com/en-us]
 (https://www.twilio.com/en-us) - b. Click Console in the upper right corner. -
 c. Copy the variables provided in the console. ```python import sys from
 ExceptNotifier import ExceptSMS, SuccessSMS, SendSMS sys.excepthook =
 ExceptSMS.__call__ # Define the next two variables optionally when using
 OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" # _OPEN_AI_API="sk-xxxxxx"
 _TWILIO_SID = 'xxxx' _TWILIO_TOKEN = 'yyyyyy'
 _RECIPIENT_PHONE_NUMBER="+aaaaaa", _SENDER_PHONE_NUMBER="+bbbbbb", try: print
 (1/10) SuccessSMS().__call__() #1 success sender except ExceptSMS as e: #2
 except sender sys.exit() SendSMS().__call__() #3 customized sender ```
-## 2-8. *Teams Notifier* - a. Create the channel that you want to notify. - b.
+### 2-8. *Teams Notifier* - a. Create the channel that you want to notify. - b.
 App - Search: webhook - Incoming Webhook [https://teams.microsoft.com/l/app/
 203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-details-dialog](https://
 teams.microsoft.com/l/app/203a1e2c-26cc-47ca-83ae-be98f960b6b2?source=app-
 details-dialog) - c. Click `Request Approval`
 After you can use webhook incomming. Proceed to next steps. Microsoft Teams
 allows limited application access per organization, so it can only be used if
 the webhook incoming application is available. - c. Go to the team channel to
@@ -229,15 +244,15 @@
 ```python import sys from ExceptNotifier import ExceptTeams, SuccessTeams,
 SendTeams sys.excepthook = ExceptTeams.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _TEAMS_WEBHOOK_URL = 'microsoft webhook
 _TEAMS_WEBHOOK_URL' try: print(1/20) SuccessTeams().__call__() #1 success
 sender except ExceptTeams as e: #2 except sender sys.exit() SendTeams
 ().__call__() #3 customized sender ```
-## 2-9. *Kakaotalk Notifier* - a. Sign up at the following site: [https://
+### 2-9. *Kakaotalk Notifier* - a. Sign up at the following site: [https://
 developers.kakao.com/](https://developers.kakao.com/) - b. Click "My
 Application" on the top bar. - c. Click "Add an application," set a name, and
 create it. - d. Click "Kakao Login" in the left menu, then change the State of
 "Kakao Login Activation" to ON on the resulting page. - e. In My Application >
 Product Settings > Kakao Login, be sure to set Redirect URI as follows: [https:
 //example.com/oauth](https://example.com/oauth) - f. In the left Consent Items
 menu, set "Send message in KakaoTalk" to selective agreement. - g. Copy the
@@ -249,27 +264,36 @@
 creating and removing a test application, but for security reasons, your API
 key should not be exposed to the outside world.**
 ```python import sys from ExceptNotifier import ExceptKakao, SuccessKakao,
 SendKakao sys.excepthook = ExceptKakao.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" _KAKAO_TOKEN_PATH = 'xxxx/xxx/xxx.json'' try: print(1/
 0) SuccessKakao().__call__() #1 success sender except ExceptKakao as e: #2
-except sender sys.exit() SendKakao().__call__() #3 customized sender ```
-## 2-10. *Beep Notifier* No setup is required. Use as follows. ```python from
+except sender sys.exit() SendKakao().__call__() #3 customized sender ``` ### 2-
+10. *Wechat Notifier* a. Get Webhook URL by visiting [here](https://
+work.weixin.qq.com/api/doc/90000/90136/91770) ```python import sys from
+ExceptNotifier import ExceptWechat, SuccessWechat, SendWechat # Define the next
+two variables optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-
+turbo" # _OPEN_AI_API="sk-xxxxxx" _WECHAT_WEBHOOK_URL = "xxxxxxxxxxx"
+sys.excepthook = ExceptWechat.__call__ try: print(1/0) SuccessWechat().__call__
+() #1 success sender except ExceptWechat as e: #2 except sender sys.exit()
+SendWechat().__call__() #3 customized sender ```
+### 2-11. *Beep Notifier* No setup is required. Use as follows. ```python from
 Exceptnotifier import ExceptBeep, SuccessBeep, SendBeep(), beep() BEEP_TIME = 1
 sys.excepthook = ExceptBeep.__call__ try: print(1/20) SuccessBeep().__call__()
 #1 success beep-beep except ExceptBeep as e: #2 except beep-beep sys.exit()
 SendBeep().__call__() #3 customized beep-beep beep() ```
-## 2-11. *Desktop Notifier* No setup is required. Use as follows. ```python
+### 2-12. *Desktop Notifier* No setup is required. Use as follows. ```python
 from ExceptNotifier import ExceptDesktop, SuccessDesktop, SendDesktop
 sys.excepthook = ExceptDesktop.__call__ # Define the next two variables
 optionally when using OpenAI's API. # _OPEN_AI_MODEL="gpt-3.5-turbo" #
 _OPEN_AI_API="sk-xxxxxx" try: print(1/0) SuccessDesktop().__call__() #1 success
 sender except ExceptDesktop as e: #2 except sender sys.exit() SendDesktop
 ().__call__() #3 customized sender ```
+## Sender
 
 
 # License MIT # Code of Conduct Everyone participating in the `ExceptNotifier`
 project, and in particular in the issue tracker, pull requests, and social
 media activity, is expected to treat other people with respect and more
 generally to follow the guidelines articulated in [the Python Community Code of
 Conduct](https://www.python.org/psf/conduct/). ##### The package is currently
```

### Comparing `ExceptNotifier-0.1.7/setup.py` & `exceptnotifier-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         return long_description
 
 
 version = get_version()
 
 
 setup(
-    name="ExceptNotifier",
-    version="0.1.7",
+    name="exceptnotifier",
+    version="0.1.8",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```

