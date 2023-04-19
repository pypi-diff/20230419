# Comparing `tmp/ExceptNotifier-0.1.6.tar.gz` & `tmp/ExceptNotifier-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.6.tar", last modified: Wed Apr 19 15:56:24 2023, max compression
+gzip compressed data, was "ExceptNotifier-0.1.7.tar", last modified: Wed Apr 19 17:58:22 2023, max compression
```

## Comparing `ExceptNotifier-0.1.6.tar` & `ExceptNotifier-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:56:24.806031 ExceptNotifier-0.1.6/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:56:24.729853 ExceptNotifier-0.1.6/ExceptNotifier/
--rw-rw-rw-   0        0        0     2571 2023-04-19 15:56:03.000000 ExceptNotifier-0.1.6/ExceptNotifier/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:56:24.794034 ExceptNotifier-0.1.6/ExceptNotifier/base/
--rw-rw-rw-   0        0        0     1146 2023-04-19 15:56:06.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/__init__.py
--rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/beep_sender.py
--rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/chime_sender.py
--rw-rw-rw-   0        0        0      583 2023-04-19 12:04:52.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/desktop_sender.py
--rw-rw-rw-   0        0        0      975 2023-04-19 12:04:07.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/discord_sender.py
--rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/kakao_sender.py
--rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/line_sender.py
--rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/mail_sender.py
--rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/openai_receiver.py
--rw-rw-rw-   0        0        0      680 2023-04-19 12:02:25.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/slack_sender.py
--rw-rw-rw-   0        0        0     1364 2023-04-19 12:03:24.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/sms_sender.py
--rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/teams_sender.py
--rw-rw-rw-   0        0        0      908 2023-04-19 14:11:30.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/telegram_sender.py
--rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.6/ExceptNotifier/base/whatsapp_sender.py
--rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.6/ExceptNotifier/beep_notifier.py
--rw-rw-rw-   0        0        0     6393 2023-04-19 13:25:44.000000 ExceptNotifier-0.1.6/ExceptNotifier/chime_notifier.py
--rw-rw-rw-   0        0        0     5769 2023-04-19 15:47:40.000000 ExceptNotifier-0.1.6/ExceptNotifier/desktop_notifier.py
--rw-rw-rw-   0        0        0     6479 2023-04-19 13:24:37.000000 ExceptNotifier-0.1.6/ExceptNotifier/discord_notifier.py
--rw-rw-rw-   0        0        0     6563 2023-04-19 13:24:31.000000 ExceptNotifier-0.1.6/ExceptNotifier/kakao_notifier.py
--rw-rw-rw-   0        0        0     6033 2023-04-19 13:24:27.000000 ExceptNotifier-0.1.6/ExceptNotifier/line_notifier.py
--rw-rw-rw-   0        0        0     7746 2023-04-19 13:24:20.000000 ExceptNotifier-0.1.6/ExceptNotifier/mail_notifier.py
--rw-rw-rw-   0        0        0     6094 2023-04-19 13:24:12.000000 ExceptNotifier-0.1.6/ExceptNotifier/slack_notifier.py
--rw-rw-rw-   0        0        0     6085 2023-04-19 15:32:02.000000 ExceptNotifier-0.1.6/ExceptNotifier/sms_notifier.py
--rw-rw-rw-   0        0        0     6020 2023-04-19 14:03:49.000000 ExceptNotifier-0.1.6/ExceptNotifier/teams_notifier.py
--rw-rw-rw-   0        0        0     6275 2023-04-19 14:10:48.000000 ExceptNotifier-0.1.6/ExceptNotifier/telegram_notifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:56:24.803031 ExceptNotifier-0.1.6/ExceptNotifier/utils/
--rw-rw-rw-   0        0        0      263 2023-04-19 15:56:09.000000 ExceptNotifier-0.1.6/ExceptNotifier/utils/__init__.py
--rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.6/ExceptNotifier/utils/kakao_token.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:56:24.757612 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0    22161 2023-04-19 15:56:24.000000 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2023-04-19 15:56:24.000000 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:56:24.000000 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-19 15:56:24.000000 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2023-04-19 15:56:24.000000 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 15:56:24.000000 ExceptNotifier-0.1.6/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.6/LICENSE
--rw-rw-rw-   0        0        0    22161 2023-04-19 15:56:24.805033 ExceptNotifier-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    21113 2023-04-19 15:53:06.000000 ExceptNotifier-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-19 15:56:24.806031 ExceptNotifier-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1926 2023-04-19 15:56:00.000000 ExceptNotifier-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:58:22.035144 ExceptNotifier-0.1.7/
+drwxrwxrwx   0        0        0        0 2023-04-19 17:58:21.965150 ExceptNotifier-0.1.7/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2714 2023-04-19 17:36:16.000000 ExceptNotifier-0.1.7/ExceptNotifier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:58:22.027462 ExceptNotifier-0.1.7/ExceptNotifier/base/
+-rw-rw-rw-   0        0        0     1232 2023-04-19 17:36:33.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-04-19 10:16:44.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/beep_sender.py
+-rw-rw-rw-   0        0        0      788 2023-04-19 10:29:50.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/chime_sender.py
+-rw-rw-rw-   0        0        0      583 2023-04-19 12:04:52.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/desktop_sender.py
+-rw-rw-rw-   0        0        0      975 2023-04-19 12:04:07.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/discord_sender.py
+-rw-rw-rw-   0        0        0     1305 2023-04-19 10:16:37.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/kakao_sender.py
+-rw-rw-rw-   0        0        0      881 2023-04-19 10:16:35.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/line_sender.py
+-rw-rw-rw-   0        0        0     1759 2023-04-19 10:16:33.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/mail_sender.py
+-rw-rw-rw-   0        0        0     1058 2023-04-19 11:05:15.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/openai_receiver.py
+-rw-rw-rw-   0        0        0      680 2023-04-19 12:02:25.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/slack_sender.py
+-rw-rw-rw-   0        0        0     1364 2023-04-19 12:03:24.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/sms_sender.py
+-rw-rw-rw-   0        0        0      671 2023-04-19 10:16:27.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/teams_sender.py
+-rw-rw-rw-   0        0        0      908 2023-04-19 14:11:30.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/telegram_sender.py
+-rw-rw-rw-   0        0        0      548 2023-04-19 17:11:23.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/wechat_sender.py
+-rw-rw-rw-   0        0        0     1596 2023-04-19 10:30:27.000000 ExceptNotifier-0.1.7/ExceptNotifier/base/whatsapp_sender.py
+-rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.7/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6393 2023-04-19 13:25:44.000000 ExceptNotifier-0.1.7/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     5769 2023-04-19 15:47:40.000000 ExceptNotifier-0.1.7/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     6479 2023-04-19 13:24:37.000000 ExceptNotifier-0.1.7/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     6563 2023-04-19 13:24:31.000000 ExceptNotifier-0.1.7/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     6033 2023-04-19 13:24:27.000000 ExceptNotifier-0.1.7/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     7746 2023-04-19 13:24:20.000000 ExceptNotifier-0.1.7/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     6094 2023-04-19 13:24:12.000000 ExceptNotifier-0.1.7/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     6085 2023-04-19 15:32:02.000000 ExceptNotifier-0.1.7/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     6020 2023-04-19 14:03:49.000000 ExceptNotifier-0.1.7/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     6275 2023-04-19 14:10:48.000000 ExceptNotifier-0.1.7/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:58:22.031939 ExceptNotifier-0.1.7/ExceptNotifier/utils/
+-rw-rw-rw-   0        0        0      263 2023-04-19 15:56:09.000000 ExceptNotifier-0.1.7/ExceptNotifier/utils/__init__.py
+-rw-rw-rw-   0        0        0     1391 2023-04-17 11:33:59.000000 ExceptNotifier-0.1.7/ExceptNotifier/utils/kakao_token.py
+-rw-rw-rw-   0        0        0     6148 2023-04-19 17:33:09.000000 ExceptNotifier-0.1.7/ExceptNotifier/wechat_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:58:21.995512 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0    22838 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1296 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 17:58:21.000000 ExceptNotifier-0.1.7/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0    22838 2023-04-19 17:58:22.034144 ExceptNotifier-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    21790 2023-04-19 17:35:03.000000 ExceptNotifier-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:58:22.035144 ExceptNotifier-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1926 2023-04-19 17:36:24.000000 ExceptNotifier-0.1.7/setup.py
```

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/__init__.py` & `ExceptNotifier-0.1.7/ExceptNotifier/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 from ExceptNotifier.chime_notifier import SuccessChime, ExceptChime, SendChime
 from ExceptNotifier.discord_notifier import SuccessDiscord, ExceptDiscord, SendDiscord
 from ExceptNotifier.kakao_notifier import SuccessKakao, ExceptKakao, SendKakao
 from ExceptNotifier.line_notifier import SuccessLine, ExceptLine, SendLine
 from ExceptNotifier.teams_notifier import SuccessTeams, ExceptTeams, SendTeams
 from ExceptNotifier.sms_notifier import SuccessSMS, ExceptSMS, SendSMS
 from ExceptNotifier.beep_notifier import SuccessBeep, ExceptBeep, SendBeep
-
+from ExceptNotifier.wechat_notifier import SuccessWechat, ExceptWechat, SendWechat 
 
 __all__ = ['SuccessMail', 'ExceptMail', 'SendMail', 'SuccessSlcak', 'ExceptSlack', 'SendSlack', 
            'SuccessTelegram', 'ExceptTelegram', 'SendTelegram', 'get_authorize_code', 'save_token', 
            'send_kakao_msg', 'send_gmail', 'send_slack_msg', 'send_telegram_msg',
            'SuccessChime', 'ExceptChime', 'SendChime',  'SuccessDiscord', 'ExceptDiscord', 'SendDiscord',
            'SuccessKakao', 'ExceptKakao', 'SendKakao',  'SuccessLine', 'ExceptLine', 'SendLine',
            'SuccessTeams', 'ExceptTeams', 'SendTeams', 'send_chime_msg', 'send_discord_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg',
-           'SuccessSMS', 'ExceptSMS', 'SendSMS', 'send_sms_msg',  'SuccessBeep', 'ExceptBeep', 'SendBeep', 'receive_openai_advice', 'beep', 'send_gmail_msg'
+           'SuccessSMS', 'ExceptSMS', 'SendSMS', 'send_sms_msg',  'SuccessBeep', 'ExceptBeep', 'SendBeep', 'receive_openai_advice', 'beep', 'send_gmail_msg',
+           'SuccessWechat', 'ExceptWechat', 'SendWechat' 
            ]
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/__init__.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from ExceptNotifier.base.discord_sender import send_discord_msg
 from ExceptNotifier.base.line_sender import send_line_msg
 from ExceptNotifier.base.teams_sender import send_teams_msg
 from ExceptNotifier.base.whatsapp_sender import send_whatsapp_msg
 from ExceptNotifier.base.sms_sender import send_sms_msg
 from ExceptNotifier.base.beep_sender import beep
 from ExceptNotifier.base.openai_receiver import receive_openai_advice
+from ExceptNotifier.base.wechat_sender import send_wechat_msg
 
 
 __all__ = ['send_kakao_msg', 'send_gmail_msg', 'send_slack_msg', 'send_telegram_msg', 'send_chime_msg', 'send_discord_msg',
-           'send_line_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg', 'send_sms_msg', 'beep', 'receive_openai_advice'
+           'send_line_msg', 'send_wechat_msg', 'send_line_msg', 'send_teams_msg', 'send_whatsapp_msg', 'send_sms_msg', 'beep', 'receive_openai_advice'
            ]
 
-__version__ = "6"
+__version__ = "0.1.7"
 __author__ = "daniel park <parkminwoo1991@gmail.com>"
```

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/beep_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/beep_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/chime_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/chime_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/desktop_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/desktop_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/discord_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/discord_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/kakao_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/kakao_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/line_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/line_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/mail_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/mail_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/openai_receiver.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/openai_receiver.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/slack_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/slack_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/sms_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/sms_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/teams_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/teams_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/telegram_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/telegram_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/base/whatsapp_sender.py` & `ExceptNotifier-0.1.7/ExceptNotifier/base/whatsapp_sender.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/beep_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/beep_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/chime_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/chime_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/desktop_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/desktop_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/discord_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/discord_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/kakao_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/kakao_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/line_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/line_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/mail_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/slack_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/sms_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/sms_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/teams_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/teams_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/telegram_notifier.py` & `ExceptNotifier-0.1.7/ExceptNotifier/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier/utils/kakao_token.py` & `ExceptNotifier-0.1.7/ExceptNotifier/utils/kakao_token.py`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier.egg-info/PKG-INFO` & `ExceptNotifier-0.1.7/ExceptNotifier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2045 7863  : 2.1..Name: Exc
 00000020: 6570 744e 6f74 6966 6965 720d 0a56 6572  eptNotifier..Ver
-00000030: 7369 6f6e 3a20 302e 312e 360d 0a53 756d  sion: 0.1.6..Sum
+00000030: 7369 6f6e 3a20 302e 312e 370d 0a53 756d  sion: 0.1.7..Sum
 00000040: 6d61 7279 3a20 5769 7468 2050 7974 686f  mary: With Pytho
 00000050: 6e27 7320 7472 792d 6578 6365 7074 2074  n's try-except t
 00000060: 6f20 7265 6365 6976 6520 6e6f 7469 6669  o receive notifi
 00000070: 6361 7469 6f6e 7320 6162 6f75 7420 4572  cations about Er
 00000080: 726f 7273 206f 7220 5375 6363 6573 7365  rors or Successe
 00000090: 7320 696e 2079 6f75 7220 636f 6465 2074  s in your code t
 000000a0: 6872 6f75 6768 206d 6573 7365 6e67 6572  hrough messenger
@@ -65,1322 +65,1364 @@
 00000400: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
 00000410: 454e 5345 0d0a 0d0a 4465 7665 6c6f 706d  ENSE....Developm
 00000420: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
 00000430: 2d20 416c 7068 6120 3c62 723e 0d0a 2a43  - Alpha <br>..*C
 00000440: 6f70 7972 6967 6874 2028 6329 2032 3032  opyright (c) 202
 00000450: 3320 4d69 6e57 6f6f 2050 6172 6b2c 2053  3 MinWoo Park, S
 00000460: 6f75 7468 204b 6f72 6561 2a0d 0a3c 6272  outh Korea*..<br
-00000470: 3e0d 0a0d 0a23 2050 7974 686f 6e20 5061  >....# Python Pa
-00000480: 636b 6167 653a 2045 7863 6570 744e 6f74  ckage: ExceptNot
-00000490: 6966 6965 720d 0a21 5b45 7863 6570 742d  ifier..![Except-
-000004a0: 4e6f 7469 6669 6572 5d28 6874 7470 733a  Notifier](https:
-000004b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000004c0: 2f62 6164 6765 2f70 7970 692d 4578 6365  /badge/pypi-Exce
-000004d0: 7074 4e6f 7469 6669 6572 2d6f 7261 6e67  ptNotifier-orang
-000004e0: 6529 0d0a 215b 5079 7069 2056 6572 7369  e)..![Pypi Versi
-000004f0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000500: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000510: 762f 4578 6365 7074 4e6f 7469 6669 6572  v/ExceptNotifier
-00000520: 2e73 7667 290d 0a5b 215b 5079 7468 6f6e  .svg)..[![Python
-00000530: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
-00000540: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000550: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
-00000560: 3625 3230 746f 2532 3033 2e37 2d62 6c61  6%20to%203.7-bla
-00000570: 636b 295d 2863 6f64 655f 6f66 5f63 6f6e  ck)](code_of_con
-00000580: 6475 6374 2e6d 6429 0d0a 215b 436f 6465  duct.md)..![Code
-00000590: 2063 6f6e 7665 6e74 696f 6e5d 2868 7474   convention](htt
-000005a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000005b0: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
-000005c0: 3063 6f6e 7665 6e74 696f 6e2d 7065 7038  0convention-pep8
-000005d0: 2d62 6c61 636b 290d 0a23 2323 2323 2050  -black)..##### P
-000005e0: 726f 7669 6465 7320 6120 6e6f 7469 6669  rovides a notifi
-000005f0: 6361 7469 6f6e 2066 726f 6d20 7468 6520  cation from the 
-00000600: 6170 706c 6963 6174 696f 6e20 7368 6f77  application show
-00000610: 6e20 696e 2074 6865 2066 6f6c 6c6f 7769  n in the followi
-00000620: 6e67 2073 6372 6565 6e2c 0d0a 0d0a 215b  ng screen,....![
-00000630: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000640: 2e63 6f6d 2f64 7364 616e 6965 6c70 6172  .com/dsdanielpar
-00000650: 6b2f 4578 6365 7074 4e6f 7469 6669 6572  k/ExceptNotifier
-00000660: 2f62 6c6f 622f 6d61 696e 2f61 7373 6574  /blob/main/asset
-00000670: 732f 696d 6773 2f6d 6169 6e32 2e70 6e67  s/imgs/main2.png
-00000680: 290d 0a20 5468 6520 6045 7863 6570 744e  ).. The `ExceptN
-00000690: 6f74 6966 6965 7260 2050 7974 686f 6e20  otifier` Python 
-000006a0: 7061 636b 6167 6520 6f66 6665 7273 2061  package offers a
-000006b0: 2066 6c65 7869 626c 6520 6170 7072 6f61   flexible approa
-000006c0: 6368 2074 6f20 7265 6365 6976 696e 6720  ch to receiving 
-000006d0: 6e6f 7469 6669 6361 7469 6f6e 7320 6279  notifications by
-000006e0: 2065 6e68 616e 6369 6e67 2050 7974 686f   enhancing Pytho
-000006f0: 6e27 7320 7472 792d 6578 6365 7074 2073  n's try-except s
-00000700: 7461 7465 6d65 6e74 2e20 5468 6973 2070  tatement. This p
-00000710: 6163 6b61 6765 2065 6e61 626c 6573 2079  ackage enables y
-00000720: 6f75 2074 6f20 7265 6365 6976 6520 616c  ou to receive al
-00000730: 6572 7473 2074 6872 6f75 6768 2076 6172  erts through var
-00000740: 696f 7573 206d 6573 7361 6769 6e67 2061  ious messaging a
-00000750: 7070 6c69 6361 7469 6f6e 7320 6f72 2065  pplications or e
-00000760: 6d61 696c 732e 0d0a 3c42 723e 3c62 723e  mails...<Br><br>
-00000770: 0d0a 5769 7468 2060 4578 6365 7074 4e6f  ..With `ExceptNo
-00000780: 7469 6669 6572 602c 2079 6f75 2063 616e  tifier`, you can
-00000790: 206f 6274 6169 6e20 6465 7461 696c 6564   obtain detailed
-000007a0: 2063 6f6d 7069 6c61 7469 6f6e 2065 7272   compilation err
-000007b0: 6f72 732c 2069 6e63 6c75 6469 6e67 2064  ors, including d
-000007c0: 6562 7567 2069 6e66 6f72 6d61 7469 6f6e  ebug information
-000007d0: 2c20 7365 6e74 2064 6972 6563 746c 7920  , sent directly 
-000007e0: 746f 2079 6f75 7220 7072 6566 6572 7265  to your preferre
-000007f0: 6420 6d65 7373 6167 696e 6720 706c 6174  d messaging plat
-00000800: 666f 726d 206f 7220 656d 6169 6c2e 2042  form or email. B
-00000810: 7920 696e 7465 6772 6174 696e 6720 4f70  y integrating Op
-00000820: 656e 4149 2773 2043 6861 7447 5054 2c20  enAI's ChatGPT, 
-00000830: 796f 7520 6361 6e20 7265 6365 6976 6520  you can receive 
-00000840: 6164 6469 7469 6f6e 616c 2065 7272 6f72  additional error
-00000850: 2063 6f64 6520 696e 666f 726d 6174 696f   code informatio
-00000860: 6e20 6173 206c 6f6e 6720 6173 2079 6f75  n as long as you
-00000870: 2070 726f 7669 6465 2074 6865 2072 6571   provide the req
-00000880: 7569 7265 6420 4150 4920 6d6f 6465 6c20  uired API model 
-00000890: 6e61 6d65 2061 6e64 206b 6579 2e20 5468  name and key. Th
-000008a0: 6973 2066 6561 7475 7265 2065 6e73 7572  is feature ensur
-000008b0: 6573 2074 6861 7420 6572 726f 7220 6861  es that error ha
-000008c0: 6e64 6c69 6e67 2061 6e64 206e 6f74 6966  ndling and notif
-000008d0: 6963 6174 696f 6e73 2061 7265 206d 6f72  ications are mor
-000008e0: 6520 696e 666f 726d 6174 6976 6520 616e  e informative an
-000008f0: 6420 6163 6365 7373 6962 6c65 2c20 7374  d accessible, st
-00000900: 7265 616d 6c69 6e69 6e67 2079 6f75 7220  reamlining your 
-00000910: 6465 6275 6767 696e 6720 7072 6f63 6573  debugging proces
-00000920: 732e 0d0a 0d0a 3c62 723e 3c62 723e 0d0a  s.....<br><br>..
-00000930: 0d0a 2323 2320 5375 7070 6f72 7469 6e67  ..### Supporting
-00000940: 2041 7070 6c69 6361 7469 6f6e 730d 0a0d   Applications...
-00000950: 0a2d 205b 5465 6c65 6772 616d 5d28 6874  .- [Telegram](ht
-00000960: 7470 733a 2f2f 7465 6c65 6772 616d 2e6f  tps://telegram.o
-00000970: 7267 2f29 0d0a 2d20 5b44 6973 636f 7264  rg/)..- [Discord
-00000980: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
-00000990: 642e 636f 6d2f 290d 0a2d 205b 536c 6163  d.com/)..- [Slac
-000009a0: 6b5d 2868 7474 7073 3a2f 2f73 6c61 636b  k](https://slack
-000009b0: 2e63 6f6d 2f29 0d0a 2d20 5b47 6f6f 676c  .com/)..- [Googl
-000009c0: 6520 4d61 696c 5d28 6874 7470 733a 2f2f  e Mail](https://
-000009d0: 6d61 696c 2e67 6f6f 676c 652e 636f 6d2f  mail.google.com/
-000009e0: 290d 0a2d 2053 4d53 2053 656e 6469 6e67  )..- SMS Sending
-000009f0: 2075 7369 6e67 205b 5477 696c 696f 5d28   using [Twilio](
-00000a00: 6874 7470 733a 2f2f 7777 772e 7477 696c  https://www.twil
-00000a10: 696f 2e63 6f6d 2f65 6e2d 7573 290d 0a2d  io.com/en-us)..-
-00000a20: 2044 6573 6b74 6f70 204e 6f74 6966 6963   Desktop Notific
-00000a30: 6174 696f 6e20 7573 696e 6720 5b50 6c79  ation using [Ply
-00000a40: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-00000a50: 7562 2e63 6f6d 2f6b 6976 792f 706c 7965  ub.com/kivy/plye
-00000a60: 7229 0d0a 2d20 5b4c 696e 655d 2868 7474  r)..- [Line](htt
-00000a70: 7073 3a2f 2f6c 696e 652e 6d65 2f65 6e2f  ps://line.me/en/
-00000a80: 290d 0a2d 205b 4157 5320 4368 696d 655d  )..- [AWS Chime]
-00000a90: 2868 7474 7073 3a2f 2f61 7773 2e61 6d61  (https://aws.ama
-00000aa0: 7a6f 6e2e 636f 6d2f 6b6f 2f63 6869 6d65  zon.com/ko/chime
-00000ab0: 2f64 6f77 6e6c 6f61 642d 6368 696d 652f  /download-chime/
-00000ac0: 290d 0a2d 205b 4d69 6372 6f73 6f66 7420  )..- [Microsoft 
-00000ad0: 5465 616d 735d 2868 7474 7073 3a2f 2f77  Teams](https://w
-00000ae0: 7777 2e6d 6963 726f 736f 6674 2e63 6f6d  ww.microsoft.com
-00000af0: 2f65 6e2f 6d69 6372 6f73 6f66 742d 7465  /en/microsoft-te
-00000b00: 616d 732f 646f 776e 6c6f 6164 2d61 7070  ams/download-app
-00000b10: 290d 0a2d 205b 4b61 6b61 6f20 5461 6c6b  )..- [Kakao Talk
-00000b20: 5d28 6874 7470 733a 2f2f 7777 772e 6b61  ](https://www.ka
-00000b30: 6b61 6f63 6f72 702e 636f 6d2f 7061 6765  kaocorp.com/page
-00000b40: 2f73 6572 7669 6365 2f73 6572 7669 6365  /service/service
-00000b50: 2f4b 616b 616f 5461 6c6b 3f6c 616e 673d  /KakaoTalk?lang=
-00000b60: 656e 290d 0a2d 2042 6565 7020 536f 756e  en)..- Beep Soun
-00000b70: 6420 6672 6f6d 205b 7379 7374 656d 5d28  d from [system](
-00000b80: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-00000b90: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
-00000ba0: 792f 7769 6e73 6f75 6e64 2e68 746d 6c29  y/winsound.html)
-00000bb0: 0d0a 0d0a 3c42 723e 0d0a 0d0a 2323 2320  ....<Br>....### 
-00000bc0: 4149 2044 6562 7567 6769 6e67 0d0a 4966  AI Debugging..If
-00000bd0: 2079 6f75 2068 6176 6520 4f70 656e 4149   you have OpenAI
-00000be0: 2041 5049 204b 6579 2061 6e64 206d 6f64   API Key and mod
-00000bf0: 656c 206e 616d 652c 2079 6f75 2063 616e  el name, you can
-00000c00: 2067 6574 2069 6e66 6f72 6d61 7469 6f6e   get information
-00000c10: 2061 6e64 2063 6f64 6520 6578 616d 706c   and code exampl
-00000c20: 6573 2066 6f72 2064 6562 7567 6769 6e67  es for debugging
-00000c30: 2069 6e20 616e 7920 6170 706c 6963 6174   in any applicat
-00000c40: 696f 6e2e 0d0a 2d20 5b4f 5045 4e20 4149  ion...- [OPEN AI
-00000c50: 2041 5049 5d28 6874 7470 733a 2f2f 706c   API](https://pl
-00000c60: 6174 666f 726d 2e6f 7065 6e61 692e 636f  atform.openai.co
-00000c70: 6d2f 646f 6373 2f69 6e74 726f 6475 6374  m/docs/introduct
-00000c80: 696f 6e29 0d0a 0d0a 0d0a 3c62 723e 3c62  ion)......<br><b
-00000c90: 723e 0d0a 0d0a 2320 5175 6963 6b20 5374  r>....# Quick St
-00000ca0: 6172 740d 0a60 6060 6261 7368 0d0a 7069  art..```bash..pi
-00000cb0: 7020 696e 7374 616c 6c20 4578 6365 7074  p install Except
-00000cc0: 4e6f 7469 6669 6572 0d0a 7069 7020 696e  Notifier..pip in
-00000cd0: 7374 616c 6c20 6578 6365 7074 6e6f 7469  stall exceptnoti
-00000ce0: 6669 6572 0d0a 0d0a 636f 6e64 6120 696e  fier....conda in
-00000cf0: 7374 616c 6c20 4578 6365 7074 4e6f 7469  stall ExceptNoti
-00000d00: 6669 6572 0d0a 636f 6e64 6120 696e 7374  fier..conda inst
-00000d10: 616c 6c20 6578 6365 7074 6e6f 7469 6669  all exceptnotifi
-00000d20: 6572 0d0a 6060 600d 0a0d 0a3c 6272 3e0d  er..```....<br>.
-00000d30: 0a0d 0a0d 0a23 2041 7070 2053 6574 7570  .....# App Setup
-00000d40: 204f 7665 7276 6965 770d 0a0d 0a2d 2054   Overview....- T
-00000d50: 6865 2076 6172 6961 626c 6573 2069 6e20  he variables in 
-00000d60: 7468 6520 666f 6c6c 6f77 696e 6720 7461  the following ta
-00000d70: 626c 6520 6d75 7374 206e 6f74 2062 6520  ble must not be 
-00000d80: 636f 6e74 616d 696e 6174 6564 2e0d 0a2d  contaminated...-
-00000d90: 2044 6570 656e 6469 6e67 206f 6e20 7468   Depending on th
-00000da0: 6520 7369 7475 6174 696f 6e2c 2063 6f6e  e situation, con
-00000db0: 7369 6465 7220 6465 7369 676e 6174 696e  sider designatin
-00000dc0: 6720 7468 656d 2061 7320 676c 6f62 616c  g them as global
-00000dd0: 2076 6172 6961 626c 6573 2066 6f72 2075   variables for u
-00000de0: 7365 2e0d 0a2d 2049 6620 796f 7520 6172  se...- If you ar
-00000df0: 6520 7573 696e 6720 5465 6c65 6772 616d  e using Telegram
-00000e00: 2c20 616e 2065 7861 6d70 6c65 2069 7320  , an example is 
-00000e10: 6174 7461 6368 6564 2061 7320 616e 2069  attached as an i
-00000e20: 6d61 6765 2e0d 0a2d 2041 7320 796f 7520  mage...- As you 
-00000e30: 616c 7265 6164 7920 6b6e 6f77 2c20 4150  already know, AP
-00000e40: 4920 4b65 7973 206f 7220 7365 6375 7269  I Keys or securi
-00000e50: 7479 2074 6f6b 656e 7320 6d75 7374 2062  ty tokens must b
-00000e60: 6520 7365 6375 7265 642e 204e 6f74 6520  e secured. Note 
-00000e70: 7468 6174 2074 6865 206b 6579 2076 616c  that the key val
-00000e80: 7565 7320 7768 6963 6820 6578 706f 7375  ues which exposu
-00000e90: 7265 6420 696e 2067 6974 6875 6220 7769  red in github wi
-00000ea0: 6c6c 2062 6520 6578 7069 7265 6420 6166  ll be expired af
-00000eb0: 7465 7220 696e 7365 6375 7265 642e 0d0a  ter insecured...
-00000ec0: 0d0a 7c20 4170 7020 7c20 5265 7175 6972  ..| App | Requir
-00000ed0: 6564 2056 6172 6961 626c 6573 207c 2046  ed Variables | F
-00000ee0: 7265 6520 6f72 2050 6169 6420 7c20 4561  ree or Paid | Ea
-00000ef0: 7365 206f 6620 5365 7475 7020 7c20 5469  se of Setup | Ti
-00000f00: 6d65 2052 6571 7569 7265 6420 666f 7220  me Required for 
-00000f10: 5365 7475 707c 4775 6964 6520 5475 746f  Setup|Guide Tuto
-00000f20: 7269 616c 204c 696e 6b7c 0d0a 7c3a 2d2d  rial Link|..|:--
-00000f30: 3a7c 3a2d 2d7c 3a2d 2d3a 7c3a 2d2d 3a7c  :|:--|:--:|:--:|
-00000f40: 3a2d 2d3a 7c3a 2d2d 2d3a 7c0d 0a7c 4265  :--:|:---:|..|Be
-00000f50: 6570 7c4e 2f41 7c46 7265 657c 4e2f 417c  ep|N/A|Free|N/A|
-00000f60: 3020 6d69 6e7c 5b45 7863 6570 7442 6565  0 min|[ExceptBee
-00000f70: 705d 2868 7474 7073 3a2f 2f67 6974 6875  p](https://githu
-00000f80: 622e 636f 6d2f 6473 6461 6e69 656c 7061  b.com/dsdanielpa
-00000f90: 726b 2f45 7863 6570 744e 6f74 6966 6965  rk/ExceptNotifie
-00000fa0: 722f 626c 6f62 2f6d 6169 6e2f 646f 6375  r/blob/main/docu
-00000fb0: 6d65 6e74 732f 4578 6365 7074 4265 6570  ments/ExceptBeep
-00000fc0: 2f47 5549 4445 2e6d 6429 7c0d 0a7c 4465  /GUIDE.md)|..|De
-00000fd0: 736b 746f 707c 4e2f 417c 4672 6565 7c4e  sktop|N/A|Free|N
-00000fe0: 2f41 7c30 206d 696e 7c5b 4578 6365 7074  /A|0 min|[Except
-00000ff0: 4465 736b 746f 705d 2868 7474 7073 3a2f  Desktop](https:/
-00001000: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
-00001010: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
-00001020: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
-00001030: 6e2f 646f 6375 6d65 6e74 732f 4578 6365  n/documents/Exce
-00001040: 7074 4465 736b 746f 702f 4755 4944 452e  ptDesktop/GUIDE.
-00001050: 6d64 297c 0d0a 7c54 656c 6567 7261 6d7c  md)|..|Telegram|
-00001060: 605f 5445 4c45 4752 414d 5f54 4f4b 454e  `_TELEGRAM_TOKEN
-00001070: 607c 4672 6565 6d69 756d 7c45 6173 797c  `|Freemium|Easy|
-00001080: 326d 696e 7c5b 4578 6365 7074 5465 6c65  2min|[ExceptTele
-00001090: 6772 616d 5d28 6874 7470 733a 2f2f 6769  gram](https://gi
-000010a0: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
-000010b0: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
-000010c0: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
-000010d0: 6f63 756d 656e 7473 2f45 7863 6570 7454  ocuments/ExceptT
-000010e0: 656c 6567 7261 6d2f 4755 4944 452e 6d64  elegram/GUIDE.md
-000010f0: 297c 0d0a 7c44 6973 636f 7264 7c60 5f44  )|..|Discord|`_D
-00001100: 4953 434f 5244 5f57 4542 484f 4f4b 5f55  ISCORD_WEBHOOK_U
-00001110: 524c 607c 4672 6565 6d69 756d 7c45 6173  RL`|Freemium|Eas
-00001120: 797c 316d 696e 7c5b 4578 6365 7074 4469  y|1min|[ExceptDi
-00001130: 7363 6f72 645d 2868 7474 7073 3a2f 2f67  scord](https://g
-00001140: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00001150: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00001160: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00001170: 646f 6375 6d65 6e74 732f 4578 6365 7074  documents/Except
-00001180: 5465 6c65 6772 616d 2f47 5549 4445 2e6d  Telegram/GUIDE.m
-00001190: 6429 7c0d 0a7c 4157 5320 4368 696d 657c  d)|..|AWS Chime|
-000011a0: 605f 4348 494d 455f 5745 4248 4f4f 4b5f  `_CHIME_WEBHOOK_
-000011b0: 5552 4c60 7c46 7265 656d 6975 6d7c 4561  URL`|Freemium|Ea
-000011c0: 7379 7c31 6d69 6e7c 5b45 7863 6570 7443  sy|1min|[ExceptC
-000011d0: 6869 6d65 5d28 6874 7470 733a 2f2f 6769  hime](https://gi
-000011e0: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
-000011f0: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
-00001200: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
-00001210: 6f63 756d 656e 7473 2f45 7863 6570 7443  ocuments/ExceptC
-00001220: 6869 6d65 2f47 5549 4445 2e6d 6429 7c0d  hime/GUIDE.md)|.
-00001230: 0a7c 536c 6163 6b7c 605f 534c 4143 4b5f  .|Slack|`_SLACK_
-00001240: 5745 4248 4f4f 4b5f 5552 4c60 7c46 7265  WEBHOOK_URL`|Fre
-00001250: 656d 6975 6d7c 4561 7379 7c33 6d69 6e7c  emium|Easy|3min|
-00001260: 5b45 7863 6570 7453 6c61 636b 5d28 6874  [ExceptSlack](ht
-00001270: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001280: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
-00001290: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
-000012a0: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
-000012b0: 2f45 7863 6570 7453 6c61 636b 2f47 5549  /ExceptSlack/GUI
-000012c0: 4445 2e6d 6429 7c0d 0a7c 472d 4d61 696c  DE.md)|..|G-Mail
-000012d0: 7c60 5f47 414d 494c 5f52 4543 4950 4945  |`_GAMIL_RECIPIE
-000012e0: 4e54 5f41 4444 5260 2c20 605f 474d 4149  NT_ADDR`, `_GMAI
-000012f0: 4c5f 5345 4e44 4552 5f41 4444 5260 2c20  L_SENDER_ADDR`, 
-00001300: 605f 474d 4149 4c5f 4150 505f 5041 5353  `_GMAIL_APP_PASS
-00001310: 574f 5244 5f4f 465f 5345 4e44 4552 6020  WORD_OF_SENDER` 
-00001320: 7c52 6573 7472 6963 7465 6420 6672 6565  |Restricted free
-00001330: 7c4d 6564 6975 6d7c 336d 696e 7c5b 4578  |Medium|3min|[Ex
-00001340: 6365 7074 4d61 696c 5d28 6874 7470 733a  ceptMail](https:
-00001350: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7364  //github.com/dsd
-00001360: 616e 6965 6c70 6172 6b2f 4578 6365 7074  anielpark/Except
-00001370: 4e6f 7469 6669 6572 2f62 6c6f 622f 6d61  Notifier/blob/ma
-00001380: 696e 2f64 6f63 756d 656e 7473 2f45 7863  in/documents/Exc
-00001390: 6570 744d 6169 6c2f 4755 4944 452e 6d64  eptMail/GUIDE.md
-000013a0: 297c 0d0a 7c4c 696e 657c 605f 4c49 4e45  )|..|Line|`_LINE
-000013b0: 5f4e 4f54 4946 595f 4150 495f 544f 4b45  _NOTIFY_API_TOKE
-000013c0: 4e60 7c46 7265 656d 6975 6d7c 4d65 6469  N`|Freemium|Medi
-000013d0: 756d 7c34 6d69 6e7c 5b45 7863 6570 744c  um|4min|[ExceptL
-000013e0: 696e 655d 2868 7474 7073 3a2f 2f67 6974  ine](https://git
-000013f0: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
-00001400: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
-00001410: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
-00001420: 6375 6d65 6e74 732f 4578 6365 7074 4c69  cuments/ExceptLi
-00001430: 6e65 2f47 5549 4445 2e6d 6429 7c0d 0a7c  ne/GUIDE.md)|..|
-00001440: 534d 537c 605f 5457 494c 494f 5f53 4944  SMS|`_TWILIO_SID
-00001450: 602c 2060 5f54 5749 4c49 4f5f 544f 4b45  `, `_TWILIO_TOKE
-00001460: 4e60 2c20 605f 5245 4349 5049 454e 545f  N`, `_RECIPIENT_
-00001470: 5048 4f4e 455f 4e55 4d42 4552 602c 2060  PHONE_NUMBER`, `
-00001480: 5f53 454e 4445 525f 5048 4f4e 455f 4e55  _SENDER_PHONE_NU
-00001490: 4d42 4552 607c 4e6f 7420 6672 6565 7c4d  MBER`|Not free|M
-000014a0: 6564 6975 6d7c 356d 696e 7c5b 4578 6365  edium|5min|[Exce
-000014b0: 7074 534d 535d 2868 7474 7073 3a2f 2f67  ptSMS](https://g
-000014c0: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-000014d0: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-000014e0: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-000014f0: 646f 6375 6d65 6e74 732f 4578 6365 7074  documents/Except
-00001500: 534d 532f 4755 4944 452e 6d64 297c 0d0a  SMS/GUIDE.md)|..
-00001510: 7c4d 6963 726f 736f 6674 2054 6561 6d73  |Microsoft Teams
-00001520: 7c60 5f54 4541 4d53 5f57 4542 484f 4f4b  |`_TEAMS_WEBHOOK
-00001530: 5f55 524c 607c 4e6f 7420 4672 6565 7c4d  _URL`|Not Free|M
-00001540: 6564 6975 6d7c 356d 696e 7c5b 4578 6365  edium|5min|[Exce
-00001550: 7074 5465 616d 735d 2868 7474 7073 3a2f  ptTeams](https:/
-00001560: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
-00001570: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
-00001580: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
-00001590: 6e2f 646f 6375 6d65 6e74 732f 4578 6365  n/documents/Exce
-000015a0: 7074 5465 616d 732f 4755 4944 452e 6d64  ptTeams/GUIDE.md
-000015b0: 297c 0d0a 7c4b 616b 616f 5461 6c6b 7c60  )|..|KakaoTalk|`
-000015c0: 5f4b 414b 414f 5f54 4f4b 454e 5f50 4154  _KAKAO_TOKEN_PAT
-000015d0: 4860 7c46 7265 656d 6975 6d7c 4865 6c6c  H`|Freemium|Hell
-000015e0: 7c3e 3d31 306d 696e 2854 6f6b 656e 2072  |>=10min(Token r
-000015f0: 6566 7265 7368 6573 2064 6169 6c79 2e29  efreshes daily.)
-00001600: 7c5b 4578 6365 7074 4b61 6b61 6f5d 2868  |[ExceptKakao](h
-00001610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001620: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00001630: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00001640: 6f62 2f6d 6169 6e2f 646f 6375 6d65 6e74  ob/main/document
-00001650: 732f 4578 6365 7074 4b61 6b61 6f2f 4755  s/ExceptKakao/GU
-00001660: 4944 452e 6d64 297c 0d0a 0d0a 0d0a 4966  IDE.md)|......If
-00001670: 2079 6f75 2061 6464 2074 6865 2066 6f6c   you add the fol
-00001680: 6c6f 7769 6e67 2074 776f 2076 6172 6961  lowing two varia
-00001690: 626c 6573 2074 6f20 7468 6520 7265 7175  bles to the requ
-000016a0: 6972 6564 2076 6172 6961 626c 6573 2066  ired variables f
-000016b0: 6f72 2065 6163 6820 6170 706c 6963 6174  or each applicat
-000016c0: 696f 6e20 696e 2074 6865 2074 6162 6c65  ion in the table
-000016d0: 2061 626f 7665 2c20 796f 7520 6361 6e20   above, you can 
-000016e0: 7265 6365 6976 6520 6572 726f 7220 6c6f  receive error lo
-000016f0: 6361 7469 6f6e 2061 6e64 2065 7870 6c61  cation and expla
-00001700: 6e61 7469 6f6e 2c20 6173 2077 656c 6c20  nation, as well 
-00001710: 6173 2065 7861 6d70 6c65 732c 2066 726f  as examples, fro
-00001720: 6d20 4f70 656e 4149 2773 206d 6f64 656c  m OpenAI's model
-00001730: 0d0a 0d0a 7c20 4150 4920 7c20 5265 7175  ....| API | Requ
-00001740: 6972 6564 2056 6172 6961 626c 6573 207c  ired Variables |
-00001750: 2046 7265 6520 6f72 2050 6169 6420 7c20   Free or Paid | 
-00001760: 4561 7365 206f 6620 5365 7475 7020 7c20  Ease of Setup | 
-00001770: 5469 6d65 2052 6571 7569 7265 6420 666f  Time Required fo
-00001780: 7220 5365 7475 707c 4775 6964 6520 5475  r Setup|Guide Tu
-00001790: 746f 7269 616c 204c 696e 6b7c 0d0a 7c3a  torial Link|..|:
-000017a0: 2d2d 3a7c 3a2d 2d7c 3a2d 2d3a 7c3a 2d2d  --:|:--|:--:|:--
-000017b0: 3a7c 3a2d 2d3a 7c3a 2d2d 2d3a 7c0d 0a7c  :|:--:|:---:|..|
-000017c0: 204f 7065 6e41 4920 4150 4920 7c60 5265   OpenAI API |`Re
-000017d0: 7175 6972 6564 2076 6172 6961 626c 6573  quired variables
-000017e0: 2066 6f72 2065 6163 6820 6170 706c 6963   for each applic
-000017f0: 6174 696f 6e60 2b20 605f 4f50 454e 5f41  ation`+ `_OPEN_A
-00001800: 495f 4d4f 4445 4c60 2c60 5f4f 5045 4e5f  I_MODEL`,`_OPEN_
-00001810: 4149 5f41 5049 607c 4e6f 7420 6672 6565  AI_API`|Not free
-00001820: 7c45 6173 797c 326d 696e 7c5b 4150 494f  |Easy|2min|[APIO
-00001830: 7065 6e41 495d 2868 7474 7073 3a2f 2f67  penAI](https://g
-00001840: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00001850: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00001860: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00001870: 646f 6375 6d65 6e74 732f 4150 494f 7065  documents/APIOpe
-00001880: 6e41 492f 4755 4944 452e 6d64 297c 0d0a  nAI/GUIDE.md)|..
-00001890: 0d0a 0d0a 3c62 723e 3c62 723e 0d0a 0d0a  ....<br><br>....
-000018a0: 2320 312e 204b 6579 2046 6561 7475 7265  # 1. Key Feature
-000018b0: 730d 0a54 6f20 7573 6520 7468 6520 6465  s..To use the de
-000018c0: 7369 7265 6420 6170 706c 6963 6174 696f  sired applicatio
-000018d0: 6e2c 2079 6f75 206d 7573 7420 6465 6669  n, you must defi
-000018e0: 6e65 2074 6865 206e 6563 6573 7361 7279  ne the necessary
-000018f0: 2076 6172 6961 626c 6573 2e20 456e 7375   variables. Ensu
-00001900: 7265 2074 6861 7420 7468 6520 7661 7269  re that the vari
-00001910: 6162 6c65 206e 616d 6573 2072 656d 6169  able names remai
-00001920: 6e20 756e 6368 616e 6765 642c 2061 6e64  n unchanged, and
-00001930: 2079 6f75 2063 616e 2075 7365 2065 6974   you can use eit
-00001940: 6865 7220 6c6f 6361 6c20 6f72 2067 6c6f  her local or glo
-00001950: 6261 6c20 7661 7269 6162 6c65 732e 2049  bal variables. I
-00001960: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
-00001970: 6054 656c 6567 7261 6d60 2c20 616e 2065  `Telegram`, an e
-00001980: 7861 6d70 6c65 2069 7320 6174 7461 6368  xample is attach
-00001990: 6564 2061 7320 616e 2069 6d61 6765 2e0d  ed as an image..
-000019a0: 0a0d 0a23 2320 312d 312e 2045 7863 6570  ...## 1-1. Excep
-000019b0: 7460 5b61 7070 4e61 6d65 5d60 0d0a 4966  t`[appName]`..If
-000019c0: 2079 6f75 2075 7365 2050 7974 686f 6e27   you use Python'
-000019d0: 7320 7472 7920 6578 6365 7074 2073 7461  s try except sta
-000019e0: 7465 6d65 6e74 2061 7320 6974 2069 732c  tement as it is,
-000019f0: 2062 7574 2063 6861 6e67 6520 6578 6365   but change exce
-00001a00: 7074 2061 7320 666f 6c6c 6f77 732c 2079  pt as follows, y
-00001a10: 6f75 2063 616e 2072 6563 6569 7665 206e  ou can receive n
-00001a20: 6f74 6966 6963 6174 696f 6e73 2074 6872  otifications thr
-00001a30: 6f75 6768 2079 6f75 7220 6170 706c 6963  ough your applic
-00001a40: 6174 696f 6e2e 0d0a 6060 600d 0a45 7863  ation...```..Exc
-00001a50: 6570 7443 6869 6d65 2c20 4578 6365 7074  eptChime, Except
-00001a60: 5465 6c65 6772 616d 2c20 4578 6365 7074  Telegram, Except
-00001a70: 4469 7363 6f72 642c 2045 7863 6570 7453  Discord, ExceptS
-00001a80: 4d53 2c20 4578 6365 7074 4d61 696c 2c20  MS, ExceptMail, 
-00001a90: 4578 6365 7074 4b61 6b61 6f2c 2045 7863  ExceptKakao, Exc
-00001aa0: 6570 744c 696e 652c 2045 7863 6570 7453  eptLine, ExceptS
-00001ab0: 6c61 636b 2c20 4578 6365 7074 5465 616d  lack, ExceptTeam
-00001ac0: 732c 2045 7863 6570 7444 6573 6b74 6f70  s, ExceptDesktop
-00001ad0: 652c 2045 7863 6570 7442 6565 700d 0a60  e, ExceptBeep..`
-00001ae0: 6060 0d0a 0d0a 2a45 7861 6d70 6c65 2a0d  ``....*Example*.
-00001af0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00001b00: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
-00001b10: 696d 706f 7274 2045 7863 6570 7454 656c  import ExceptTel
-00001b20: 6765 7261 6d0d 0a5f 5445 4c45 4752 414d  geram.._TELEGRAM
-00001b30: 5f54 4f4b 454e 203d 2022 7878 7878 220d  _TOKEN = "xxxx".
-00001b40: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
-00001b50: 6e74 2831 2f30 290d 0a65 7863 6570 7420  nt(1/0)..except 
-00001b60: 4578 6365 7074 5465 6c65 6772 616d 3a20  ExceptTelegram: 
-00001b70: 2020 2023 2073 656e 6469 6e67 2065 7863     # sending exc
-00001b80: 6570 7420 6d65 7373 6167 6520 746f 2074  ept message to t
-00001b90: 656c 6567 7261 6d0d 0a20 2020 2073 7973  elegram..    sys
-00001ba0: 2e65 7869 7428 290d 0a60 6060 0d0a 215b  .exit()..```..![
-00001bb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001bc0: 2e63 6f6d 2f64 7364 616e 6965 6c70 6172  .com/dsdanielpar
-00001bd0: 6b2f 4578 6365 7074 4e6f 7469 6669 6572  k/ExceptNotifier
-00001be0: 2f62 6c6f 622f 6d61 696e 2f61 7373 6574  /blob/main/asset
-00001bf0: 732f 696d 6773 2f65 7831 2e70 6e67 290d  s/imgs/ex1.png).
-00001c00: 0a0d 0a3c 6272 3e0d 0a0d 0a23 2320 312d  ...<br>....## 1-
-00001c10: 322e 2041 4920 4465 6262 7567 6769 6e67  2. AI Debbugging
-00001c20: 2049 6e66 6f6d 6174 696f 6e20 4e6f 7469   Infomation Noti
-00001c30: 6669 6361 7469 6f6e 0d0a 596f 7520 6361  fication..You ca
-00001c40: 6e20 7265 6365 6976 6520 6465 6275 6767  n receive debugg
-00001c50: 696e 6720 696e 666f 726d 6174 696f 6e20  ing information 
-00001c60: 6672 6f6d 2043 6861 7447 5054 2076 6961  from ChatGPT via
-00001c70: 204f 7065 6e41 4927 7320 4150 4920 7768   OpenAI's API wh
-00001c80: 656e 2075 7369 6e67 2074 6865 2045 7863  en using the Exc
-00001c90: 6570 7420 7374 6174 656d 656e 742e 2054  ept statement. T
-00001ca0: 6865 2073 796e 7461 7820 7265 6d61 696e  he syntax remain
-00001cb0: 7320 7468 6520 7361 6d65 2c20 6275 7420  s the same, but 
-00001cc0: 796f 7527 6c6c 206e 6565 6420 746f 2063  you'll need to c
-00001cd0: 6f6e 6669 6775 7265 2074 6865 7365 2074  onfigure these t
-00001ce0: 776f 2076 6172 6961 626c 6573 3a0d 0a60  wo variables:..`
-00001cf0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 602c  _OPEN_AI_MODEL`,
-00001d00: 605f 4f50 454e 5f41 495f 4150 4960 0d0a  `_OPEN_AI_API`..
-00001d10: 0d0a 2a45 7861 6d70 6c65 2a0d 0a60 6060  ..*Example*..```
-00001d20: 7079 7468 6f6e 0d0a 6672 6f6d 2045 7863  python..from Exc
-00001d30: 6570 744e 6f74 6966 6965 7220 696d 706f  eptNotifier impo
-00001d40: 7274 2045 7863 6570 7454 656c 6765 7261  rt ExceptTelgera
-00001d50: 6d0d 0a5f 5445 4c45 4752 414d 5f54 4f4b  m.._TELEGRAM_TOK
-00001d60: 454e 203d 2022 7878 7878 220d 0a5f 4f50  EN = "xxxx".._OP
-00001d70: 454e 5f41 495f 4d4f 4445 4c3d 2267 7074  EN_AI_MODEL="gpt
-00001d80: 2d33 2e35 2d74 7572 626f 220d 0a5f 4f50  -3.5-turbo".._OP
-00001d90: 454e 5f41 495f 4150 493d 2273 6b2d 7878  EN_AI_API="sk-xx
-00001da0: 7878 7878 220d 0a0d 0a74 7279 3a0d 0a20  xxxx"....try:.. 
-00001db0: 2020 2070 7269 6e74 2831 2f30 290d 0a65     print(1/0)..e
-00001dc0: 7863 6570 7420 4578 6365 7074 5465 6c65  xcept ExceptTele
-00001dd0: 6772 616d 3a20 2320 7365 6e64 696e 6720  gram: # sending 
-00001de0: 6d73 6720 5749 5448 2041 4920 4445 4255  msg WITH AI DEBU
-00001df0: 4747 494e 4720 746f 2074 656c 6567 7261  GGING to telegra
-00001e00: 6d0d 0a20 2020 2073 7973 2e65 7869 7428  m..    sys.exit(
-00001e10: 290d 0a60 6060 0d0a 0d0a 215b 5d28 6874  )..```....![](ht
-00001e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001e30: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
-00001e40: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
-00001e50: 622f 6d61 696e 2f61 7373 6574 732f 696d  b/main/assets/im
-00001e60: 6773 2f65 7832 2e70 6e67 290d 0a0d 0a3c  gs/ex2.png)....<
-00001e70: 6272 3e0d 0a0d 0a23 2320 312d 332e 2053  br>....## 1-3. S
-00001e80: 7563 6365 7373 605b 6170 704e 616d 655d  uccess`[appName]
-00001e90: 600d 0a42 7920 706c 6163 696e 6720 7468  `..By placing th
-00001ea0: 6520 7472 7920 6578 6365 7074 2069 6e20  e try except in 
-00001eb0: 7079 7468 6f6e 2061 7420 7468 6520 656e  python at the en
-00001ec0: 6420 6f66 2074 6865 2074 7279 2073 7461  d of the try sta
-00001ed0: 7465 6d65 6e74 2c20 6170 706c 6963 6174  tement, applicat
-00001ee0: 696f 6e73 2063 616e 2062 6520 6e6f 7469  ions can be noti
-00001ef0: 6669 6564 2074 6861 7420 7468 6520 7472  fied that the tr
-00001f00: 7920 7374 6174 656d 656e 7420 776f 726b  y statement work
-00001f10: 6564 206e 6f72 6d61 6c6c 792e 0d0a 6060  ed normally...``
-00001f20: 600d 0a53 7563 6365 7373 4368 696d 652c  `..SuccessChime,
-00001f30: 2053 7563 6365 7373 5465 6c65 6772 616d   SuccessTelegram
-00001f40: 2c20 5375 6363 6573 7344 6973 636f 7264  , SuccessDiscord
-00001f50: 2c20 5375 6363 6573 7353 4d53 2c20 5375  , SuccessSMS, Su
-00001f60: 6363 6573 734d 6169 6c2c 2053 7563 6365  ccessMail, Succe
-00001f70: 7373 4b61 6b61 6f2c 2053 7563 6365 7373  ssKakao, Success
-00001f80: 4c69 6e65 2c20 5375 6363 6573 7353 6c61  Line, SuccessSla
-00001f90: 636b 2c20 5375 6363 6573 7354 6561 6d73  ck, SuccessTeams
-00001fa0: 2c20 5375 6363 6573 7344 6573 6b74 6f70  , SuccessDesktop
-00001fb0: 652c 2053 7563 6365 7373 4265 6570 0d0a  e, SuccessBeep..
-00001fc0: 6060 600d 0a2a 4578 616d 706c 652a 0d0a  ```..*Example*..
-00001fd0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00001fe0: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
-00001ff0: 2069 6d70 6f72 7420 5375 6363 6573 7354   import SuccessT
-00002000: 656c 6765 7261 6d0d 0a5f 5445 4c45 4752  elgeram.._TELEGR
-00002010: 414d 5f54 4f4b 454e 203d 2022 7878 7878  AM_TOKEN = "xxxx
-00002020: 220d 0a0d 0a74 7279 3a0d 0a20 2020 2070  "....try:..    p
-00002030: 7269 6e74 2831 2f32 3029 0d0a 2020 2020  rint(1/20)..    
-00002040: 5375 6363 6573 7354 656c 6765 7261 6d28  SuccessTelgeram(
-00002050: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2320  ).__call__()  # 
-00002060: 7365 6e64 696e 6720 7375 6363 6573 7320  sending success 
-00002070: 6d65 7373 6167 6520 746f 2074 656c 6567  message to teleg
-00002080: 7261 6d0d 0a65 7863 6570 743a 0d0a 2020  ram..except:..  
-00002090: 2020 7379 732e 6578 6974 2829 0d0a 6060    sys.exit()..``
-000020a0: 600d 0a0d 0a21 5b5d 2868 7474 7073 3a2f  `....![](https:/
-000020b0: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
-000020c0: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
-000020d0: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
-000020e0: 6e2f 6173 7365 7473 2f69 6d67 732f 6578  n/assets/imgs/ex
-000020f0: 332e 706e 6729 0d0a 0d0a 3c42 723e 0d0a  3.png)....<Br>..
-00002100: 0d0a 2323 2031 2d34 2e20 5365 6e64 605b  ..## 1-4. Send`[
-00002110: 6170 704e 616d 655d 600d 0a50 6c61 6365  appName]`..Place
-00002120: 2069 7420 616e 7977 6865 7265 206f 6e20   it anywhere on 
-00002130: 7468 6520 6c69 6e65 206f 6620 636f 6465  the line of code
-00002140: 2079 6f75 2077 616e 742c 2061 6e64 2079   you want, and y
-00002150: 6f75 276c 6c20 6265 206e 6f74 6966 6965  ou'll be notifie
-00002160: 6420 7768 656e 2074 6861 7420 6c69 6e65  d when that line
-00002170: 206f 6620 636f 6465 2069 7320 7265 6163   of code is reac
-00002180: 6865 642e 0d0a 6060 600d 0a53 656e 6443  hed...```..SendC
-00002190: 6869 6d65 2c20 5365 6e64 5465 6c65 6772  hime, SendTelegr
-000021a0: 616d 2c20 5365 6e64 4469 7363 6f72 642c  am, SendDiscord,
-000021b0: 2053 656e 6453 4d53 2c20 5365 6e64 4d61   SendSMS, SendMa
-000021c0: 696c 2c20 5365 6e64 4b61 6b61 6f2c 2053  il, SendKakao, S
-000021d0: 656e 644c 696e 652c 2053 656e 6453 6c61  endLine, SendSla
-000021e0: 636b 2c20 5365 6e64 5465 616d 732c 2053  ck, SendTeams, S
-000021f0: 656e 6444 6573 6b74 6f70 652c 2053 656e  endDesktope, Sen
-00002200: 6442 6565 700d 0a60 6060 0d0a 2a45 7861  dBeep..```..*Exa
-00002210: 6d70 6c65 2a0d 0a0d 0a60 6060 7079 7468  mple*....```pyth
-00002220: 6f6e 0d0a 6672 6f6d 2045 7863 6570 744e  on..from ExceptN
-00002230: 6f74 6966 6965 7220 696d 706f 7274 2053  otifier import S
-00002240: 656e 6454 656c 6765 7261 6d0d 0a5f 5445  endTelgeram.._TE
-00002250: 4c45 4752 414d 5f54 4f4b 454e 203d 2022  LEGRAM_TOKEN = "
-00002260: 7878 7878 220d 0a0d 0a53 656e 6454 656c  xxxx"....SendTel
-00002270: 6567 7261 6d28 292e 5f5f 6361 6c6c 5f5f  egram().__call__
-00002280: 2829 2023 2073 656e 6469 6e67 206d 6573  () # sending mes
-00002290: 7361 6765 2074 6f20 7465 6c65 6772 616d  sage to telegram
-000022a0: 0d0a 0d0a 6e6f 7469 203d 2053 656e 6454  ....noti = SendT
-000022b0: 656c 6567 7261 6d28 290d 0a6e 6f74 6928  elegram()..noti(
-000022c0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-000022d0: 2020 2020 2023 2073 656e 6469 6e67 206d       # sending m
-000022e0: 6573 7361 6765 2074 6f20 7465 6c65 6772  essage to telegr
-000022f0: 616d 0d0a 6060 600d 0a0d 0a21 5b5d 2868  am..```....![](h
-00002300: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002310: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00002320: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00002330: 6f62 2f6d 6169 6e2f 6173 7365 7473 2f69  ob/main/assets/i
-00002340: 6d67 732f 6578 342e 706e 6729 0d0a 0d0a  mgs/ex4.png)....
-00002350: 0d0a 3c62 723e 3c62 723e 0d0a 0d0a 2320  ..<br><br>....# 
-00002360: 322e 2046 6561 7475 7265 730d 0a59 6f75  2. Features..You
-00002370: 2063 616e 2072 6563 6569 7665 2064 6562   can receive deb
-00002380: 7567 6769 6e67 2069 6e66 6f72 6d61 7469  ugging informati
-00002390: 6f6e 2066 726f 6d20 4368 6174 4750 5420  on from ChatGPT 
-000023a0: 7669 6120 4f70 656e 4149 2773 2041 5049  via OpenAI's API
-000023b0: 2077 6865 6e20 7573 696e 6720 7468 6520   when using the 
-000023c0: 4578 6365 7074 2073 7461 7465 6d65 6e74  Except statement
-000023d0: 2e20 5468 6520 7379 6e74 6178 2072 656d  . The syntax rem
-000023e0: 6169 6e73 2074 6865 2073 616d 652c 2062  ains the same, b
-000023f0: 7574 2079 6f75 276c 6c20 6e65 6564 2074  ut you'll need t
-00002400: 6f20 636f 6e66 6967 7572 6520 7468 6573  o configure thes
-00002410: 6520 7477 6f20 7661 7269 6162 6c65 733a  e two variables:
-00002420: 0d0a 605f 4f50 454e 5f41 495f 4d4f 4445  ..`_OPEN_AI_MODE
-00002430: 4c60 2c60 5f4f 5045 4e5f 4149 5f41 5049  L`,`_OPEN_AI_API
-00002440: 600d 0a0d 0a0d 0a0d 0a23 2320 322d 312e  `........## 2-1.
-00002450: 202a 5465 6c65 6772 616d 204e 6f74 6966   *Telegram Notif
-00002460: 6965 722a 0d0a 0d0a 2d20 612e 204f 7065  ier*....- a. Ope
-00002470: 6e20 796f 7572 2074 656c 6567 7261 6d20  n your telegram 
-00002480: 6170 7020 616e 6420 7365 6172 6368 2066  app and search f
-00002490: 6f72 2042 6f74 4661 7468 6572 2e20 2841  or BotFather. (A
-000024a0: 2062 7569 6c74 2d69 6e20 5465 6c65 6772   built-in Telegr
-000024b0: 616d 2062 6f74 2074 6861 7420 6865 6c70  am bot that help
-000024c0: 7320 7573 6572 7320 6372 6561 7465 2063  s users create c
-000024d0: 7573 746f 6d20 5465 6c65 6772 616d 2062  ustom Telegram b
-000024e0: 6f74 7329 203c 6272 3e0d 0a2d 2062 2e20  ots) <br>..- b. 
-000024f0: 5479 7065 202f 6e65 7762 6f74 2074 6f20  Type /newbot to 
-00002500: 6372 6561 7465 2061 206e 6577 2062 6f74  create a new bot
-00002510: 203c 6272 3e0d 0a2d 2063 2e20 4769 7665   <br>..- c. Give
-00002520: 2079 6f75 7220 626f 7420 6120 6e61 6d65   your bot a name
-00002530: 2026 2061 2075 7365 726e 616d 6520 3c62   & a username <b
-00002540: 723e 0d0a 2d20 642e 2043 6f70 7920 796f  r>..- d. Copy yo
-00002550: 7572 206e 6577 2054 656c 6567 7261 6d20  ur new Telegram 
-00002560: 626f 74e2 8099 7320 746f 6b65 6e20 3c62  bot...s token <b
-00002570: 723e 0d0a 0d0a 466f 7220 6d6f 7265 2069  r>....For more i
-00002580: 6e66 6f6d 6174 696f 6e2c 2076 6973 6974  nfomation, visit
-00002590: 205b 5465 6c65 6772 616d 2042 6f74 2046   [Telegram Bot F
-000025a0: 6174 6865 7220 4150 495d 2868 7474 7073  ather API](https
-000025b0: 3a2f 2f63 6f72 652e 7465 6c65 6772 616d  ://core.telegram
-000025c0: 2e6f 7267 2f62 6f74 732f 6170 6929 0d0a  .org/bots/api)..
-000025d0: 3c62 723e 3c62 723e 0d0a 200d 0a23 2323  <br><br>.. ..###
-000025e0: 2061 2e20 5769 7468 6f75 7420 4f70 656e   a. Without Open
-000025f0: 4149 2041 5049 0d0a 0d0a 6060 6070 7974  AI API....```pyt
-00002600: 686f 6e0d 0a66 726f 6d20 4578 6365 7074  hon..from Except
-00002610: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
-00002620: 4578 6365 7074 5465 6c65 6772 616d 2c20  ExceptTelegram, 
-00002630: 5375 6363 6573 7354 656c 6567 7261 6d2c  SuccessTelegram,
-00002640: 2053 656e 6454 656c 6567 7261 6d0d 0a69   SendTelegram..i
-00002650: 6d70 6f72 7420 7379 730d 0a73 7973 2e65  mport sys..sys.e
-00002660: 7863 6570 7468 6f6f 6b20 3d20 4578 6365  xcepthook = Exce
-00002670: 7074 5465 6c65 6772 616d 2e5f 5f63 616c  ptTelegram.__cal
-00002680: 6c5f 5f0d 0a0d 0a5f 5445 4c45 4752 414d  l__...._TELEGRAM
-00002690: 5f54 4f4b 454e 203d 2022 7878 7878 220d  _TOKEN = "xxxx".
-000026a0: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
-000026b0: 6e74 2831 2f30 2920 200d 0a20 2020 2053  nt(1/0)  ..    S
-000026c0: 7563 6365 7373 5465 6c65 6772 616d 2829  uccessTelegram()
-000026d0: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2e20  .__call__() #1. 
-000026e0: 7375 6363 6573 7320 7365 6e64 6572 2020  success sender  
-000026f0: 2020 2020 2020 2020 0d0a 0d0a 6578 6365          ....exce
-00002700: 7074 2045 7863 6570 7454 656c 6567 7261  pt ExceptTelegra
-00002710: 6d20 6173 2065 3a20 2020 2020 2023 322e  m as e:      #2.
-00002720: 2065 7863 6570 7420 7365 6e64 6572 2020   except sender  
-00002730: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002740: 7379 732e 6578 6974 2829 0d0a 0d0a 5365  sys.exit()....Se
-00002750: 6e64 5465 6c65 6772 616d 2829 2e5f 5f63  ndTelegram().__c
-00002760: 616c 6c5f 5f28 2920 2020 2020 2020 2023  all__()        #
-00002770: 332e 2063 7573 746f 6d69 7a65 6420 7365  3. customized se
-00002780: 6e64 6572 2020 2020 200d 0a60 6060 0d0a  nder     ..```..
-00002790: 0d0a 0d0a 215b 5d28 6874 7470 733a 2f2f  ....![](https://
-000027a0: 6769 7468 7562 2e63 6f6d 2f64 7364 616e  github.com/dsdan
-000027b0: 6965 6c70 6172 6b2f 4578 6365 7074 4e6f  ielpark/ExceptNo
-000027c0: 7469 6669 6572 2f62 6c6f 622f 6d61 696e  tifier/blob/main
-000027d0: 2f61 7373 6574 732f 696d 6773 2f66 6967  /assets/imgs/fig
-000027e0: 3434 2e70 6e67 290d 0a0d 0a0d 0a23 2323  44.png)......###
-000027f0: 2062 2e20 5769 7468 204f 7065 6e41 4920   b. With OpenAI 
-00002800: 4150 490d 0a60 6060 7079 7468 6f6e 0d0a  API..```python..
-00002810: 6672 6f6d 2045 7863 6570 744e 6f74 6966  from ExceptNotif
-00002820: 6965 7220 696d 706f 7274 2045 7863 6570  ier import Excep
-00002830: 7454 656c 6567 7261 6d2c 2053 7563 6365  tTelegram, Succe
-00002840: 7373 5465 6c65 6772 616d 2c20 5365 6e64  ssTelegram, Send
-00002850: 5465 6c65 6772 616d 0d0a 696d 706f 7274  Telegram..import
-00002860: 2073 7973 0d0a 7379 732e 6578 6365 7074   sys..sys.except
-00002870: 686f 6f6b 203d 2045 7863 6570 7454 656c  hook = ExceptTel
-00002880: 6567 7261 6d2e 5f5f 6361 6c6c 5f5f 0d0a  egram.__call__..
-00002890: 0d0a 5f54 454c 4547 5241 4d5f 544f 4b45  .._TELEGRAM_TOKE
-000028a0: 4e20 3d20 2278 7878 7822 0d0a 5f4f 5045  N = "xxxx".._OPE
-000028b0: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-000028c0: 332e 352d 7475 7262 6f22 0d0a 5f4f 5045  3.5-turbo".._OPE
-000028d0: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
-000028e0: 7878 7822 0d0a 0d0a 7472 793a 0d0a 2020  xxx"....try:..  
-000028f0: 2020 7072 696e 7428 312f 3029 2020 0d0a    print(1/0)  ..
-00002900: 2020 2020 5375 6363 6573 7354 656c 6567      SuccessTeleg
-00002910: 7261 6d28 292e 5f5f 6361 6c6c 5f5f 2829  ram().__call__()
-00002920: 2023 312e 2073 7563 6365 7373 2073 656e   #1. success sen
-00002930: 6465 7220 2020 2020 2020 2020 200d 0a0d  der          ...
-00002940: 0a65 7863 6570 7420 4578 6365 7074 5465  .except ExceptTe
-00002950: 6c65 6772 616d 2061 7320 653a 2020 2020  legram as e:    
-00002960: 2020 2332 2e20 6578 6365 7074 2073 656e    #2. except sen
-00002970: 6465 7220 2020 2020 2020 2020 2020 200d  der            .
-00002980: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
-00002990: 0a0d 0a53 656e 6454 656c 6567 7261 6d28  ...SendTelegram(
-000029a0: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
-000029b0: 2020 2020 2333 2e20 6375 7374 6f6d 697a      #3. customiz
-000029c0: 6564 2073 656e 6465 7220 2020 2020 0d0a  ed sender     ..
-000029d0: 0d0a 6060 600d 0a3c 6272 3e0d 0a0d 0a23  ..```..<br>....#
-000029e0: 2320 322d 322e 202a 4d61 696c 204e 6f74  # 2-2. *Mail Not
-000029f0: 6966 6965 722a 0d0a 496e 2074 6865 2065  ifier*..In the e
-00002a00: 7863 6570 7420 7374 6174 656d 656e 742c  xcept statement,
-00002a10: 2061 6e20 656d 6169 6c20 6973 2073 656e   an email is sen
-00002a20: 7420 616c 6f6e 6720 7769 7468 2074 6865  t along with the
-00002a30: 2065 7272 6f72 206d 6573 7361 6765 2e20   error message. 
-00002a40: 4164 6469 7469 6f6e 616c 6c79 2c20 796f  Additionally, yo
-00002a50: 7520 6361 6e20 7365 6e64 2065 6d61 696c  u can send email
-00002a60: 7320 6672 6f6d 2061 6e79 2064 6573 6972  s from any desir
-00002a70: 6564 206c 696e 652e 203c 6272 3e0d 0a2d  ed line. <br>..-
-00002a80: 2061 2e20 4c6f 6720 696e 2077 6974 6820   a. Log in with 
-00002a90: 7468 6520 7365 6e64 6572 2773 2065 6d61  the sender's ema
-00002aa0: 696c 2049 442e 203c 6272 3e0d 0a2d 2062  il ID. <br>..- b
-00002ab0: 2e20 4f62 7461 696e 2061 6e20 6170 7020  . Obtain an app 
-00002ac0: 7061 7373 776f 7264 2066 6f72 2073 656e  password for sen
-00002ad0: 6469 6e67 2047 6f6f 676c 6520 4d61 696c  ding Google Mail
-00002ae0: 2061 7420 7468 6520 666f 6c6c 6f77 696e   at the followin
-00002af0: 6720 5b6c 696e 6b5d 2868 7474 7073 3a2f  g [link](https:/
-00002b00: 2f6d 7961 6363 6f75 6e74 2e67 6f6f 676c  /myaccount.googl
-00002b10: 652e 636f 6d2f 752f 332f 6170 7070 6173  e.com/u/3/apppas
-00002b20: 7377 6f72 6473 3f75 746d 5f73 6f75 7263  swords?utm_sourc
-00002b30: 653d 676f 6f67 6c65 2d61 6363 6f75 6e74  e=google-account
-00002b40: 2675 746d 5f6d 6564 6975 6d3d 6d79 6163  &utm_medium=myac
-00002b50: 636f 756e 7473 6563 7572 6974 7926 7574  countsecurity&ut
-00002b60: 6d5f 6361 6d70 6169 676e 3d74 7376 2d73  m_campaign=tsv-s
-00002b70: 6574 7469 6e67 7326 7261 7074 3d41 456a  ettings&rapt=AEj
-00002b80: 484c 344e 3262 4d52 574f 3436 5661 4d70  HL4N2bMRWO46VaMp
-00002b90: 5f6a 5030 367a 514b 3134 4257 4e50 7636  _jP06zQK14BWNPv6
-00002ba0: 366c 326f 3539 694a 3939 436b 4f38 426a  6l2o59iJ99CkO8Bj
-00002bb0: 596e 6d6f 5255 6539 6474 5363 686b 6b62  YnmoRUe9dtSchkkb
-00002bc0: 7562 485a 4d55 6865 766b 416e 7756 4a52  ubHZMUhevkAnwVJR
-00002bd0: 4862 3979 674f 3361 6669 7370 4e6c 7729  Hb9ygO3afispNlw)
-00002be0: 206f 7220 5b67 6f6f 676c 6520 646f 6375   or [google docu
-00002bf0: 6d65 6e74 5d28 6874 7470 733a 2f2f 7375  ment](https://su
-00002c00: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
-00002c10: 2f61 6363 6f75 6e74 732f 616e 7377 6572  /accounts/answer
-00002c20: 2f31 3835 3833 333f 686c 3d65 6e29 2e20  /185833?hl=en). 
-00002c30: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00002c40: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00002c50: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00002c60: 6d70 6f72 7420 4578 6365 7074 4d61 696c  mport ExceptMail
-00002c70: 2c20 5375 6363 6573 734d 6169 6c2c 2053  , SuccessMail, S
-00002c80: 656e 644d 6169 6c0d 0a73 7973 2e65 7863  endMail..sys.exc
-00002c90: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
-00002ca0: 4d61 696c 2e5f 5f63 616c 6c5f 5f0d 0a0d  Mail.__call__...
-00002cb0: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
-00002cc0: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
-00002cd0: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
-00002ce0: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
-00002cf0: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
-00002d00: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
-00002d10: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
-00002d20: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
-00002d30: 7878 7878 7822 0d0a 5f47 414d 494c 5f52  xxxxx".._GAMIL_R
-00002d40: 4543 4950 4945 4e54 5f41 4444 5220 3d20  ECIPIENT_ADDR = 
-00002d50: 2778 7878 7878 7878 4067 6d61 696c 2e63  'xxxxxxx@gmail.c
-00002d60: 6f6d 270d 0a5f 474d 4149 4c5f 5345 4e44  om'.._GMAIL_SEND
-00002d70: 4552 5f41 4444 5220 3d20 2779 7979 7979  ER_ADDR = 'yyyyy
-00002d80: 7940 676d 6169 6c2e 636f 6d27 0d0a 5f47  y@gmail.com'.._G
-00002d90: 4d41 494c 5f41 5050 5f50 4153 5357 4f52  MAIL_APP_PASSWOR
-00002da0: 445f 4f46 5f53 454e 4445 5220 3d20 277a  D_OF_SENDER = 'z
-00002db0: 7a7a 7a7a 7a27 0d0a 0d0a 7472 793a 0d0a  zzzzz'....try:..
-00002dc0: 2020 2020 6d61 696e 2829 2020 2020 2020      main()      
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2320 596f 7572 2043 6f64 6520 4865 7265  # Your Code Here
-00002df0: 0d0a 2020 2020 5375 6363 6573 734d 6169  ..    SuccessMai
-00002e00: 6c28 292e 5f5f 6361 6c6c 5f5f 2829 2020  l().__call__()  
-00002e10: 2020 2320 4e6f 2045 7863 6570 7469 6f6e    # No Exception
-00002e20: 202d 3e20 5365 6e64 2053 7563 6365 7373   -> Send Success
-00002e30: 206d 6169 6c2e 0d0a 6578 6365 7074 2045   mail...except E
-00002e40: 7863 6570 744d 6169 6c3a 2020 2020 2020  xceptMail:      
-00002e50: 2020 2020 2020 2020 2320 4578 6365 7074          # Except
-00002e60: 696f 6e20 2d3e 2053 656e 6420 4661 696c  ion -> Send Fail
-00002e70: 206d 6169 6c2e 0d0a 2020 2020 7061 7373   mail...    pass
-00002e80: 0d0a 0d0a 5365 6e64 4d61 696c 2829 2e5f  ....SendMail()._
-00002e90: 5f63 616c 6c5f 5f28 2920 2020 2020 2020  _call__()       
-00002ea0: 2020 2020 2320 5768 656e 2050 726f 6365      # When Proce
-00002eb0: 7373 2045 6e64 6564 202d 3e20 416e 7920  ss Ended -> Any 
-00002ec0: 4c69 6e65 206d 6169 6c2e 0d0a 6060 600d  Line mail...```.
-00002ed0: 0a0d 0a3c 6465 7461 696c 733e 0d0a 3c73  ...<details>..<s
-00002ee0: 756d 6d61 7279 3e20 5365 6520 4578 616d  ummary> See Exam
-00002ef0: 706c 652e 2e2e 3c2f 7375 6d6d 6172 793e  ple...</summary>
-00002f00: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00002f10: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00002f20: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00002f30: 6d70 6f72 7420 4578 6365 7074 4d61 696c  mport ExceptMail
-00002f40: 2c20 5375 6363 6573 734d 6169 6c2c 2053  , SuccessMail, S
-00002f50: 656e 644d 6169 6c0d 0a0d 0a23 2044 6566  endMail....# Def
-00002f60: 696e 6520 7468 6520 6e65 7874 2074 776f  ine the next two
-00002f70: 2076 6172 6961 626c 6573 206f 7074 696f   variables optio
-00002f80: 6e61 6c6c 7920 7768 656e 2075 7369 6e67  nally when using
-00002f90: 204f 7065 6e41 4927 7320 4150 492e 0d0a   OpenAI's API...
-00002fa0: 2320 5f4f 5045 4e5f 4149 5f4d 4f44 454c  # _OPEN_AI_MODEL
-00002fb0: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
-00002fc0: 2020 2020 0d0a 2320 5f4f 5045 4e5f 4149      ..# _OPEN_AI
-00002fd0: 5f41 5049 3d22 736b 2d78 7878 7878 7822  _API="sk-xxxxxx"
-00002fe0: 0d0a 5f47 414d 494c 5f52 4543 4950 4945  .._GAMIL_RECIPIE
-00002ff0: 4e54 5f41 4444 5220 3d20 2778 7878 7878  NT_ADDR = 'xxxxx
-00003000: 7878 4067 6d61 696c 2e63 6f6d 270d 0a5f  xx@gmail.com'.._
-00003010: 474d 4149 4c5f 5345 4e44 4552 5f41 4444  GMAIL_SENDER_ADD
-00003020: 5220 3d20 2779 7979 7979 7940 676d 6169  R = 'yyyyyy@gmai
-00003030: 6c2e 636f 6d27 0d0a 5f47 4d41 494c 5f41  l.com'.._GMAIL_A
-00003040: 5050 5f50 4153 5357 4f52 445f 4f46 5f53  PP_PASSWORD_OF_S
-00003050: 454e 4445 5220 3d20 277a 7a7a 7a7a 7a27  ENDER = 'zzzzzz'
-00003060: 0d0a 0d0a 7379 732e 6578 6365 7074 686f  ....sys.exceptho
-00003070: 6f6b 203d 2045 7863 6570 744d 6169 6c2e  ok = ExceptMail.
-00003080: 5f5f 6361 6c6c 5f5f 0d0a 0d0a 7472 793a  __call__....try:
-00003090: 0d0a 2020 2020 2320 3032 2e4c 6f63 6174  ..    # 02.Locat
-000030a0: 6520 796f 7572 2063 6f64 650d 0a20 2020  e your code..   
-000030b0: 2070 7269 6e74 2831 2f30 2920 2020 0d0a   print(1/0)   ..
-000030c0: 2020 2020 5375 6363 6573 734d 6169 6c28      SuccessMail(
-000030d0: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2023  ).__call__()   #
-000030e0: 2053 7563 6365 7373 204d 6169 6c0d 0a0d   Success Mail...
-000030f0: 0a65 7863 6570 7420 4578 6365 7074 4d61  .except ExceptMa
-00003100: 696c 2061 7320 653a 2020 2020 2020 2020  il as e:        
-00003110: 2320 4578 6365 7074 696f 6e20 4d61 696c  # Exception Mail
-00003120: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-00003130: 2e65 7869 7428 290d 0a20 2020 2070 7269  .exit()..    pri
-00003140: 6e74 2865 290d 0a0d 0a53 656e 644d 6169  nt(e)....SendMai
-00003150: 6c28 292e 5f5f 6361 6c6c 5f5f 2829 2020  l().__call__()  
-00003160: 2020 2020 2020 2020 2320 5075 7420 416e          # Put An
-00003170: 7920 4c69 6e65 3a20 5365 6e64 696e 6720  y Line: Sending 
-00003180: 6d61 696c 0d0a 6060 600d 0a3c 2f64 6574  mail..```..</det
-00003190: 6169 6c73 3e0d 0a0d 0a3c 6465 7461 696c  ails>....<detail
-000031a0: 733e 0d0a 3c73 756d 6d61 7279 3e20 536e  s>..<summary> Sn
-000031b0: 6970 7065 7420 666f 7220 5079 7468 6f6e  ippet for Python
-000031c0: 2064 6576 656c 6f70 6572 732e 2e2e 3c2f   developers...</
-000031d0: 7375 6d6d 6172 793e 0d0a 0d0a 6060 6070  summary>....```p
-000031e0: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
-000031f0: 730d 0a66 726f 6d20 4578 6365 7074 4e6f  s..from ExceptNo
-00003200: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
-00003210: 6365 7074 4d61 696c 2c20 5375 6363 6573  ceptMail, Succes
-00003220: 734d 6169 6c2c 2053 656e 644d 6169 6c0d  sMail, SendMail.
-00003230: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
-00003240: 3d20 4578 6365 7074 4d61 696c 2e5f 5f63  = ExceptMail.__c
-00003250: 616c 6c5f 5f0d 0a0d 0a23 2044 6566 696e  all__....# Defin
-00003260: 6520 7468 6520 6e65 7874 2074 776f 2076  e the next two v
-00003270: 6172 6961 626c 6573 206f 7074 696f 6e61  ariables optiona
-00003280: 6c6c 7920 7768 656e 2075 7369 6e67 204f  lly when using O
-00003290: 7065 6e41 4927 7320 4150 492e 0d0a 2320  penAI's API...# 
-000032a0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 3d22  _OPEN_AI_MODEL="
-000032b0: 6770 742d 332e 352d 7475 7262 6f22 2020  gpt-3.5-turbo"  
-000032c0: 2020 0d0a 2320 5f4f 5045 4e5f 4149 5f41    ..# _OPEN_AI_A
-000032d0: 5049 3d22 736b 2d78 7878 7878 7822 0d0a  PI="sk-xxxxxx"..
-000032e0: 5f47 414d 494c 5f52 4543 4950 4945 4e54  _GAMIL_RECIPIENT
-000032f0: 5f41 4444 5220 3d20 2778 7878 7878 7878  _ADDR = 'xxxxxxx
-00003300: 4067 6d61 696c 2e63 6f6d 270d 0a5f 474d  @gmail.com'.._GM
-00003310: 4149 4c5f 5345 4e44 4552 5f41 4444 5220  AIL_SENDER_ADDR 
-00003320: 3d20 2779 7979 7979 7940 676d 6169 6c2e  = 'yyyyyy@gmail.
-00003330: 636f 6d27 0d0a 5f47 4d41 494c 5f41 5050  com'.._GMAIL_APP
-00003340: 5f50 4153 5357 4f52 445f 4f46 5f53 454e  _PASSWORD_OF_SEN
-00003350: 4445 5220 3d20 277a 7a7a 7a7a 7a27 0d0a  DER = 'zzzzzz'..
-00003360: 0d0a 7472 793a 0d0a 2020 2020 2779 6f75  ..try:..    'you
-00003370: 7220 636f 6465 270d 0a20 2020 2053 7563  r code'..    Suc
-00003380: 6365 7373 4d61 696c 2829 2e5f 5f63 616c  cessMail().__cal
-00003390: 6c5f 5f28 290d 0a65 7863 6570 7420 4578  l__()..except Ex
-000033a0: 6365 7074 4d61 696c 3a0d 0a20 2020 2070  ceptMail:..    p
-000033b0: 6173 730d 0a0d 0a53 656e 644d 6169 6c28  ass....SendMail(
-000033c0: 292e 5f5f 6361 6c6c 5f5f 2829 200d 0a60  ).__call__() ..`
-000033d0: 6060 0d0a 3c2f 6465 7461 696c 733e 0d0a  ``..</details>..
-000033e0: 0d0a 3c62 723e 0d0a 0d0a 2323 2032 2d33  ..<br>....## 2-3
-000033f0: 2e20 2a44 6973 636f 7264 204e 6f74 6966  . *Discord Notif
-00003400: 6965 722a 0d0a 2d20 612e 2053 656c 6563  ier*..- a. Selec
-00003410: 7420 7468 6520 6368 616e 6e65 6c20 746f  t the channel to
-00003420: 2072 6563 6569 7665 206e 6f74 6966 6963   receive notific
-00003430: 6174 696f 6e73 2e0d 0a2d 2062 2e20 436c  ations...- b. Cl
-00003440: 6963 6b20 2245 6469 7420 4368 616e 6e65  ick "Edit Channe
-00003450: 6c22 2069 6e20 7468 6520 7570 7065 7220  l" in the upper 
-00003460: 7269 6768 7420 636f 726e 6572 206f 6620  right corner of 
-00003470: 7468 6520 6368 6174 2077 696e 646f 772e  the chat window.
-00003480: 0d0a 2d20 632e 2043 6c69 636b 2049 6e74  ..- c. Click Int
-00003490: 6567 7261 7469 6f6e 7320 2d20 5765 6268  egrations - Webh
-000034a0: 6f6f 6b20 2d20 4e65 7720 5765 6268 6f6f  ook - New Webhoo
-000034b0: 6b2e 0d0a 2d20 642e 2054 6865 6e20 636c  k...- d. Then cl
-000034c0: 6963 6b20 436f 7079 2057 6562 686f 6f6b  ick Copy Webhook
-000034d0: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
-000034e0: 696d 706f 7274 2073 7973 0d0a 6672 6f6d  import sys..from
-000034f0: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
-00003500: 696d 706f 7274 2045 7863 6570 7444 6973  import ExceptDis
-00003510: 636f 7264 2c20 5375 6363 6573 7344 6973  cord, SuccessDis
-00003520: 636f 7264 2c20 5365 6e64 4469 7363 6f72  cord, SendDiscor
-00003530: 640d 0a73 7973 2e65 7863 6570 7468 6f6f  d..sys.excepthoo
-00003540: 6b20 3d20 4578 6365 7074 4469 7363 6f72  k = ExceptDiscor
-00003550: 642e 5f5f 6361 6c6c 5f5f 0d0a 0d0a 2320  d.__call__....# 
-00003560: 4465 6669 6e65 2074 6865 206e 6578 7420  Define the next 
-00003570: 7477 6f20 7661 7269 6162 6c65 7320 6f70  two variables op
-00003580: 7469 6f6e 616c 6c79 2077 6865 6e20 7573  tionally when us
-00003590: 696e 6720 4f70 656e 4149 2773 2041 5049  ing OpenAI's API
-000035a0: 2e0d 0a23 205f 4f50 454e 5f41 495f 4d4f  ...# _OPEN_AI_MO
-000035b0: 4445 4c3d 2267 7074 2d33 2e35 2d74 7572  DEL="gpt-3.5-tur
-000035c0: 626f 2220 2020 200d 0a23 205f 4f50 454e  bo"    ..# _OPEN
-000035d0: 5f41 495f 4150 493d 2273 6b2d 7878 7878  _AI_API="sk-xxxx
-000035e0: 7878 220d 0a5f 4449 5343 4f52 445f 5745  xx".._DISCORD_WE
-000035f0: 4248 4f4f 4b5f 5552 4c20 3d20 2278 7878  BHOOK_URL = "xxx
-00003600: 7878 7878 7878 7878 7878 7878 7878 220d  xxxxxxxxxxxxxx".
-00003610: 0a0d 0a0d 0a74 7279 3a0d 0a20 2020 2070  .....try:..    p
-00003620: 7269 6e74 2831 2f32 3029 2020 0d0a 2020  rint(1/20)  ..  
-00003630: 2020 5375 6363 6573 7344 6973 636f 7264    SuccessDiscord
-00003640: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2331  ().__call__() #1
-00003650: 2073 7563 6365 7373 2073 656e 6465 7220   success sender 
-00003660: 2020 2020 2020 2020 200d 0a65 7863 6570           ..excep
-00003670: 7420 4578 6365 7074 4469 7363 6f72 6420  t ExceptDiscord 
-00003680: 6173 2065 3a20 2020 2020 2023 3220 6578  as e:      #2 ex
-00003690: 6365 7074 2073 656e 6465 7220 2020 2020  cept sender     
-000036a0: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-000036b0: 2e65 7869 7428 290d 0a0d 0a53 656e 6444  .exit()....SendD
-000036c0: 6973 636f 7264 2829 2e5f 5f63 616c 6c5f  iscord().__call_
-000036d0: 5f28 2920 2020 2020 2020 2023 3320 6375  _()        #3 cu
-000036e0: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
-000036f0: 2020 2020 2020 0d0a 6060 600d 0a0d 0a3c        ..```....<
-00003700: 6272 3e0d 0a0d 0a23 2320 322d 342e 202a  br>....## 2-4. *
-00003710: 4368 696d 6520 4e6f 7469 6669 6572 2a0d  Chime Notifier*.
-00003720: 0a2d 2061 2e20 5365 6c65 6374 2074 6865  .- a. Select the
-00003730: 2043 6861 7420 726f 6f6d 2074 6f20 7265   Chat room to re
-00003740: 6365 6976 6520 6e6f 7469 6669 6361 7469  ceive notificati
-00003750: 6f6e 732e 0d0a 2d20 622e 2043 6c69 636b  ons...- b. Click
-00003760: 2022 526f 6f6d 2053 6574 7469 6e67 2220   "Room Setting" 
-00003770: 696e 2074 6865 2075 7070 6572 2072 6967  in the upper rig
-00003780: 6874 2063 6f72 6e65 722e 0d0a 2d20 632e  ht corner...- c.
-00003790: 2043 6c69 636b 2022 4d61 6e61 6765 2057   Click "Manage W
-000037a0: 6562 686f 6f6b 2061 6e64 2062 6f74 2e22  ebhook and bot."
-000037b0: 0d0a 2d20 642e 2043 7265 6174 6520 4164  ..- d. Create Ad
-000037c0: 6420 5765 6268 6f6f 6b2c 2073 6574 2069  d Webhook, set i
-000037d0: 7420 7570 2c20 7468 656e 2063 6c69 636b  t up, then click
-000037e0: 2043 6f70 7920 5765 6268 6f6f 6b2e 0d0a   Copy Webhook...
-000037f0: 6060 6070 7974 686f 6e0d 0a69 6d70 6f72  ```python..impor
-00003800: 7420 7379 730d 0a66 726f 6d20 4578 6365  t sys..from Exce
-00003810: 7074 4e6f 7469 6669 6572 2069 6d70 6f72  ptNotifier impor
-00003820: 7420 5375 6363 6573 7343 6869 6d65 2c20  t SuccessChime, 
-00003830: 4578 6365 7074 4368 696d 652c 2053 656e  ExceptChime, Sen
-00003840: 6443 6869 6d65 0d0a 7379 732e 6578 6365  dChime..sys.exce
-00003850: 7074 686f 6f6b 203d 2045 7863 6570 7443  pthook = ExceptC
-00003860: 6869 6d65 2e5f 5f63 616c 6c5f 5f0d 0a0d  hime.__call__...
-00003870: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
-00003880: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
-00003890: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
-000038a0: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
-000038b0: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
-000038c0: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
-000038d0: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
-000038e0: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
-000038f0: 7878 7878 7822 0d0a 5f43 4849 4d45 5f57  xxxxx".._CHIME_W
-00003900: 4542 484f 4f4b 5f55 524c 203d 2022 7878  EBHOOK_URL = "xx
-00003910: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
-00003920: 220d 0a0d 0a0d 0a74 7279 3a0d 0a20 2020  "......try:..   
-00003930: 2070 7269 6e74 2831 2f30 2920 200d 0a20   print(1/0)  .. 
-00003940: 2020 2053 7563 6365 7373 4368 696d 6528     SuccessChime(
-00003950: 292e 5f5f 6361 6c6c 5f5f 2829 2023 3120  ).__call__() #1 
-00003960: 7375 6363 6573 7320 7365 6e64 6572 2020  success sender  
-00003970: 2020 2020 2020 2020 0d0a 6578 6365 7074          ..except
-00003980: 2045 7863 6570 7443 6869 6d65 2061 7320   ExceptChime as 
-00003990: 653a 2020 2020 2020 2332 2065 7863 6570  e:      #2 excep
-000039a0: 7420 7365 6e64 6572 2020 2020 2020 2020  t sender        
-000039b0: 2020 2020 0d0a 2020 2020 7379 732e 6578      ..    sys.ex
-000039c0: 6974 2829 0d0a 0d0a 5365 6e64 4368 696d  it()....SendChim
-000039d0: 6528 292e 5f5f 6361 6c6c 5f5f 2829 2020  e().__call__()  
-000039e0: 2020 2020 2020 2333 2063 7573 746f 6d69        #3 customi
-000039f0: 7a65 6420 7365 6e64 6572 2020 2020 2020  zed sender      
-00003a00: 200d 0a60 6060 0d0a 3c62 723e 0d0a 0d0a   ..```..<br>....
-00003a10: 2323 2032 2d35 2e20 2a53 6c61 636b 204e  ## 2-5. *Slack N
-00003a20: 6f74 6966 6965 722a 0d0a 2d20 612e 2076  otifier*..- a. v
-00003a30: 6973 6974 2068 7474 7073 3a2f 2f61 7069  isit https://api
-00003a40: 2e73 6c61 636b 2e63 6f6d 2f0d 0a2d 2062  .slack.com/..- b
-00003a50: 2e20 6043 7265 6174 6520 616e 2061 7070  . `Create an app
-00003a60: 6020 2d20 6046 726f 6d20 7363 7261 7463  ` - `From scratc
-00003a70: 6860 202d 2060 4372 6561 7465 2041 7070  h` - `Create App
-00003a80: 600d 0a2d 2063 2e20 4164 6420 7765 6268  `..- c. Add webh
-00003a90: 6f6f 6b3a 2043 6c69 636b 2060 496e 636f  ook: Click `Inco
-00003aa0: 6d69 6e67 2057 6562 686f 6f6b 7360 202d  ming Webhooks` -
-00003ab0: 2041 6374 6976 6174 6520 496e 636f 6d6d   Activate Incomm
-00003ac0: 696e 6720 604f 6e60 202d 2041 6464 204e  ing `On` - Add N
-00003ad0: 6577 2057 6562 686f 6f6b 2074 6f20 576f  ew Webhook to Wo
-00003ae0: 726b 7370 6163 650d 0a2d 2064 2e20 436f  rkspace..- d. Co
-00003af0: 7079 2060 5765 6268 6f6f 6b20 5552 4c60  py `Webhook URL`
-00003b00: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00003b10: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00003b20: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00003b30: 6d70 6f72 7420 4578 6365 7074 536c 6163  mport ExceptSlac
-00003b40: 6b2c 2053 7563 6365 7373 536c 6361 6b2c  k, SuccessSlcak,
-00003b50: 2053 656e 6453 6c61 636b 0d0a 7379 732e   SendSlack..sys.
-00003b60: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-00003b70: 6570 7453 6c61 636b 2e5f 5f63 616c 6c5f  eptSlack.__call_
-00003b80: 5f0d 0a0d 0a23 2044 6566 696e 6520 7468  _....# Define th
-00003b90: 6520 6e65 7874 2074 776f 2076 6172 6961  e next two varia
-00003ba0: 626c 6573 206f 7074 696f 6e61 6c6c 7920  bles optionally 
-00003bb0: 7768 656e 2075 7369 6e67 204f 7065 6e41  when using OpenA
-00003bc0: 4927 7320 4150 492e 0d0a 2320 5f4f 5045  I's API...# _OPE
-00003bd0: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-00003be0: 332e 352d 7475 7262 6f22 2020 2020 0d0a  3.5-turbo"    ..
-00003bf0: 2320 5f4f 5045 4e5f 4149 5f41 5049 3d22  # _OPEN_AI_API="
-00003c00: 736b 2d78 7878 7878 7822 0d0a 5f53 4c41  sk-xxxxxx".._SLA
-00003c10: 434b 5f57 4542 484f 4f4b 5f55 524c 203d  CK_WEBHOOK_URL =
-00003c20: 2027 6874 7470 733a 2f2f 686f 6f6b 732e   'https://hooks.
-00003c30: 736c 6163 6b2e 636f 6d2f 7365 7276 6963  slack.com/servic
-00003c40: 6573 2f78 7878 7878 7878 7878 7878 7878  es/xxxxxxxxxxxxx
-00003c50: 7878 7878 7878 270d 0a0d 0a74 7279 3a0d  xxxxxx'....try:.
-00003c60: 0a20 2020 2070 7269 6e74 2831 2f30 2920  .    print(1/0) 
-00003c70: 200d 0a20 2020 2053 7563 6365 7373 536c   ..    SuccessSl
-00003c80: 6361 6b28 292e 5f5f 6361 6c6c 5f5f 2829  cak().__call__()
-00003c90: 2023 3120 7375 6363 6573 7320 7365 6e64   #1 success send
-00003ca0: 6572 2020 2020 2020 2020 2020 0d0a 6578  er          ..ex
-00003cb0: 6365 7074 2045 7863 6570 7453 6c61 636b  cept ExceptSlack
-00003cc0: 2061 7320 653a 2020 2020 2020 2332 2065   as e:      #2 e
-00003cd0: 7863 6570 7420 7365 6e64 6572 2020 2020  xcept sender    
-00003ce0: 2020 2020 2020 2020 0d0a 2020 2020 7379          ..    sy
-00003cf0: 732e 6578 6974 2829 0d0a 0d0a 5365 6e64  s.exit()....Send
-00003d00: 536c 6163 6b28 292e 5f5f 6361 6c6c 5f5f  Slack().__call__
-00003d10: 2829 2020 2020 2020 2020 2333 2063 7573  ()        #3 cus
-00003d20: 746f 6d69 7a65 6420 7365 6e64 6572 2020  tomized sender  
-00003d30: 2020 200d 0a60 6060 0d0a 3c42 723e 0d0a     ..```..<Br>..
-00003d40: 0d0a 2323 2032 2d36 2e20 2a4c 696e 6520  ..## 2-6. *Line 
-00003d50: 4e6f 7469 6669 6572 2a0d 0a2d 2061 2e20  Notifier*..- a. 
-00003d60: 5265 6769 7374 6572 205b 6874 7470 733a  Register [https:
-00003d70: 2f2f 6e6f 7469 6679 2d62 6f74 2e6c 696e  //notify-bot.lin
-00003d80: 652e 6d65 2f5d 2868 7474 7073 3a2f 2f6e  e.me/](https://n
-00003d90: 6f74 6966 792d 626f 742e 6c69 6e65 2e6d  otify-bot.line.m
-00003da0: 652f 292e 0d0a 2d20 622e 2047 6f20 746f  e/)...- b. Go to
-00003db0: 206d 7970 6167 6520 5b68 7474 7073 3a2f   mypage [https:/
-00003dc0: 2f6e 6f74 6966 792d 626f 742e 6c69 6e65  /notify-bot.line
-00003dd0: 2e6d 652f 6d79 2f5d 2868 7474 7073 3a2f  .me/my/](https:/
-00003de0: 2f6e 6f74 6966 792d 626f 742e 6c69 6e65  /notify-bot.line
-00003df0: 2e6d 652f 6d79 2f29 2e0d 0a2d 2063 2e20  .me/my/)...- c. 
-00003e00: 436c 6963 6b20 6047 656e 6572 6174 6520  Click `Generate 
-00003e10: 546f 6b65 6e60 2c20 656e 7465 7220 5365  Token`, enter Se
-00003e20: 7276 6963 6520 4e61 6d65 2061 6e64 2063  rvice Name and c
-00003e30: 6c69 636b 2060 312d 6f6e 2d31 2063 6861  lick `1-on-1 cha
-00003e40: 7420 7769 7468 204c 494e 4560 2028 616e  t with LINE` (an
-00003e50: 7974 6869 6e67 2079 6f75 206c 696b 6529  ything you like)
-00003e60: 2e0d 0a2d 2064 2e20 436f 7079 2054 6f6b  ...- d. Copy Tok
-00003e70: 656e 2e0d 0a0d 0a60 6060 7079 7468 6f6e  en.....```python
-00003e80: 0d0a 696d 706f 7274 2073 7973 0d0a 6672  ..import sys..fr
-00003e90: 6f6d 2045 7863 6570 744e 6f74 6966 6965  om ExceptNotifie
-00003ea0: 7220 696d 706f 7274 2045 7863 6570 744c  r import ExceptL
-00003eb0: 696e 652c 2053 7563 6365 7373 4c69 6e65  ine, SuccessLine
-00003ec0: 2c20 5365 6e64 4c69 6e65 0d0a 7379 732e  , SendLine..sys.
-00003ed0: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-00003ee0: 6570 744c 696e 652e 5f5f 6361 6c6c 5f5f  eptLine.__call__
-00003ef0: 0d0a 0d0a 2320 4465 6669 6e65 2074 6865  ....# Define the
-00003f00: 206e 6578 7420 7477 6f20 7661 7269 6162   next two variab
-00003f10: 6c65 7320 6f70 7469 6f6e 616c 6c79 2077  les optionally w
-00003f20: 6865 6e20 7573 696e 6720 4f70 656e 4149  hen using OpenAI
-00003f30: 2773 2041 5049 2e0d 0a23 205f 4f50 454e  's API...# _OPEN
-00003f40: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
-00003f50: 2e35 2d74 7572 626f 2220 2020 200d 0a23  .5-turbo"    ..#
-00003f60: 205f 4f50 454e 5f41 495f 4150 493d 2273   _OPEN_AI_API="s
-00003f70: 6b2d 7878 7878 7878 220d 0a5f 4c49 4e45  k-xxxxxx".._LINE
-00003f80: 5f4e 4f54 4946 595f 4150 495f 544f 4b45  _NOTIFY_API_TOKE
-00003f90: 4e20 3d20 2778 7878 7878 7878 7878 7878  N = 'xxxxxxxxxxx
-00003fa0: 270d 0a0d 0a74 7279 3a0d 0a20 2020 2070  '....try:..    p
-00003fb0: 7269 6e74 2831 2f32 3029 2020 0d0a 2020  rint(1/20)  ..  
-00003fc0: 2020 5375 6363 6573 734c 696e 6528 292e    SuccessLine().
-00003fd0: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
-00003fe0: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
-00003ff0: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
-00004000: 7863 6570 744c 696e 6520 6173 2065 3a20  xceptLine as e: 
-00004010: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
-00004020: 656e 6465 7220 2020 2020 2020 2020 2020  ender           
-00004030: 200d 0a20 2020 2073 7973 2e65 7869 7428   ..    sys.exit(
-00004040: 290d 0a0d 0a53 656e 644c 696e 6528 292e  )....SendLine().
-00004050: 5f5f 6361 6c6c 5f5f 2829 2020 2020 2020  __call__()      
-00004060: 2020 2333 2063 7573 746f 6d69 7a65 6420    #3 customized 
-00004070: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00004080: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
-00004090: 0a23 2320 322d 372e 202a 534d 5320 4e6f  .## 2-7. *SMS No
-000040a0: 7469 6669 6572 2a0d 0a2d 2061 2e20 5369  tifier*..- a. Si
-000040b0: 676e 2075 7020 666f 7220 5477 696c 696f  gn up for Twilio
-000040c0: 2e20 5b68 7474 7073 3a2f 2f77 7777 2e74  . [https://www.t
-000040d0: 7769 6c69 6f2e 636f 6d2f 656e 2d75 735d  wilio.com/en-us]
-000040e0: 2868 7474 7073 3a2f 2f77 7777 2e74 7769  (https://www.twi
-000040f0: 6c69 6f2e 636f 6d2f 656e 2d75 7329 2e0d  lio.com/en-us)..
-00004100: 0a2d 2062 2e20 436c 6963 6b20 436f 6e73  .- b. Click Cons
-00004110: 6f6c 6520 696e 2074 6865 2075 7070 6572  ole in the upper
-00004120: 2072 6967 6874 2063 6f72 6e65 722e 0d0a   right corner...
-00004130: 2d20 632e 2043 6f70 7920 7468 6520 7661  - c. Copy the va
-00004140: 7269 6162 6c65 7320 7072 6f76 6964 6564  riables provided
-00004150: 2069 6e20 7468 6520 636f 6e73 6f6c 652e   in the console.
-00004160: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00004170: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00004180: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00004190: 6d70 6f72 7420 4578 6365 7074 534d 532c  mport ExceptSMS,
-000041a0: 2053 7563 6365 7373 534d 532c 2053 656e   SuccessSMS, Sen
-000041b0: 6453 4d53 0d0a 7379 732e 6578 6365 7074  dSMS..sys.except
-000041c0: 686f 6f6b 203d 2045 7863 6570 7453 4d53  hook = ExceptSMS
-000041d0: 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23 2044  .__call__....# D
-000041e0: 6566 696e 6520 7468 6520 6e65 7874 2074  efine the next t
-000041f0: 776f 2076 6172 6961 626c 6573 206f 7074  wo variables opt
-00004200: 696f 6e61 6c6c 7920 7768 656e 2075 7369  ionally when usi
-00004210: 6e67 204f 7065 6e41 4927 7320 4150 492e  ng OpenAI's API.
-00004220: 0d0a 2320 5f4f 5045 4e5f 4149 5f4d 4f44  ..# _OPEN_AI_MOD
-00004230: 454c 3d22 6770 742d 332e 352d 7475 7262  EL="gpt-3.5-turb
-00004240: 6f22 2020 2020 0d0a 2320 5f4f 5045 4e5f  o"    ..# _OPEN_
-00004250: 4149 5f41 5049 3d22 736b 2d78 7878 7878  AI_API="sk-xxxxx
-00004260: 7822 0d0a 5f54 5749 4c49 4f5f 5349 4420  x".._TWILIO_SID 
-00004270: 3d20 2778 7878 7827 0d0a 5f54 5749 4c49  = 'xxxx'.._TWILI
-00004280: 4f5f 544f 4b45 4e20 3d20 2779 7979 7979  O_TOKEN = 'yyyyy
-00004290: 7927 0d0a 5f52 4543 4950 4945 4e54 5f50  y'.._RECIPIENT_P
-000042a0: 484f 4e45 5f4e 554d 4245 523d 222b 6161  HONE_NUMBER="+aa
-000042b0: 6161 6161 222c 0d0a 5f53 454e 4445 525f  aaaa",.._SENDER_
-000042c0: 5048 4f4e 455f 4e55 4d42 4552 3d22 2b62  PHONE_NUMBER="+b
-000042d0: 6262 6262 6222 2c20 200d 0a0d 0a74 7279  bbbbb",  ....try
-000042e0: 3a0d 0a20 2020 2070 7269 6e74 2831 2f31  :..    print(1/1
-000042f0: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
-00004300: 7353 4d53 2829 2e5f 5f63 616c 6c5f 5f28  sSMS().__call__(
-00004310: 2920 2331 2073 7563 6365 7373 2073 656e  ) #1 success sen
-00004320: 6465 7220 2020 2020 2020 2020 200d 0a65  der          ..e
-00004330: 7863 6570 7420 4578 6365 7074 534d 5320  xcept ExceptSMS 
-00004340: 6173 2065 3a20 2020 2020 2023 3220 6578  as e:      #2 ex
-00004350: 6365 7074 2073 656e 6465 720d 0a20 2020  cept sender..   
-00004360: 2073 7973 2e65 7869 7428 290d 0a0d 0a53   sys.exit()....S
-00004370: 656e 6453 4d53 2829 2e5f 5f63 616c 6c5f  endSMS().__call_
-00004380: 5f28 2920 2020 2020 2020 2023 3320 6375  _()        #3 cu
-00004390: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
-000043a0: 2020 2020 2020 200d 0a60 6060 0d0a 3c42         ..```..<B
-000043b0: 723e 0d0a 0d0a 2323 2032 2d38 2e20 2a54  r>....## 2-8. *T
-000043c0: 6561 6d73 204e 6f74 6966 6965 722a 0d0a  eams Notifier*..
-000043d0: 2d20 612e 2043 7265 6174 6520 7468 6520  - a. Create the 
-000043e0: 6368 616e 6e65 6c20 7468 6174 2079 6f75  channel that you
-000043f0: 2077 616e 7420 746f 206e 6f74 6966 792e   want to notify.
-00004400: 0d0a 2d20 622e 2041 7070 202d 2053 6561  ..- b. App - Sea
-00004410: 7263 683a 2077 6562 686f 6f6b 202d 2049  rch: webhook - I
-00004420: 6e63 6f6d 696e 6720 5765 6268 6f6f 6b20  ncoming Webhook 
-00004430: 5b68 7474 7073 3a2f 2f74 6561 6d73 2e6d  [https://teams.m
-00004440: 6963 726f 736f 6674 2e63 6f6d 2f6c 2f61  icrosoft.com/l/a
-00004450: 7070 2f32 3033 6131 6532 632d 3236 6363  pp/203a1e2c-26cc
-00004460: 2d34 3763 612d 3833 6165 2d62 6539 3866  -47ca-83ae-be98f
-00004470: 3936 3062 3662 323f 736f 7572 6365 3d61  960b6b2?source=a
-00004480: 7070 2d64 6574 6169 6c73 2d64 6961 6c6f  pp-details-dialo
-00004490: 675d 2868 7474 7073 3a2f 2f74 6561 6d73  g](https://teams
-000044a0: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6c  .microsoft.com/l
-000044b0: 2f61 7070 2f32 3033 6131 6532 632d 3236  /app/203a1e2c-26
-000044c0: 6363 2d34 3763 612d 3833 6165 2d62 6539  cc-47ca-83ae-be9
-000044d0: 3866 3936 3062 3662 323f 736f 7572 6365  8f960b6b2?source
-000044e0: 3d61 7070 2d64 6574 6169 6c73 2d64 6961  =app-details-dia
-000044f0: 6c6f 6729 2e0d 0a2d 2063 2e20 436c 6963  log)...- c. Clic
-00004500: 6b20 6052 6571 7565 7374 2041 7070 726f  k `Request Appro
-00004510: 7661 6c60 203c 6272 3e0d 0a41 6674 6572  val` <br>..After
-00004520: 2079 6f75 2063 616e 2075 7365 2077 6562   you can use web
-00004530: 686f 6f6b 2069 6e63 6f6d 6d69 6e67 2e20  hook incomming. 
-00004540: 5072 6f63 6565 6420 746f 206e 6578 7420  Proceed to next 
-00004550: 7374 6570 732e 0d0a 4d69 6372 6f73 6f66  steps...Microsof
-00004560: 7420 5465 616d 7320 616c 6c6f 7773 206c  t Teams allows l
-00004570: 696d 6974 6564 2061 7070 6c69 6361 7469  imited applicati
-00004580: 6f6e 2061 6363 6573 7320 7065 7220 6f72  on access per or
-00004590: 6761 6e69 7a61 7469 6f6e 2c20 736f 2069  ganization, so i
-000045a0: 7420 6361 6e20 6f6e 6c79 2062 6520 7573  t can only be us
-000045b0: 6564 2069 6620 7468 6520 7765 6268 6f6f  ed if the webhoo
-000045c0: 6b20 696e 636f 6d69 6e67 2061 7070 6c69  k incoming appli
-000045d0: 6361 7469 6f6e 2069 7320 6176 6169 6c61  cation is availa
-000045e0: 626c 652e 0d0a 2d20 632e 2047 6f20 746f  ble...- c. Go to
-000045f0: 2074 6865 2074 6561 6d20 6368 616e 6e65   the team channe
-00004600: 6c20 746f 2072 6563 6569 7665 206e 6f74  l to receive not
-00004610: 6966 6963 6174 696f 6e73 2c20 616e 6420  ifications, and 
-00004620: 636c 6963 6b20 6043 6f6e 6e65 6374 6f72  click `Connector
-00004630: 7360 2069 6e20 5365 7474 696e 6773 2e0d  s` in Settings..
-00004640: 0a2d 2064 2e20 6043 6f6e 6e65 6374 6f72  .- d. `Connector
-00004650: 7360 2041 6674 6572 2063 6f6e 6669 6775  s` After configu
-00004660: 7269 6e67 2077 6562 686f 6f6b 2069 6e63  ring webhook inc
-00004670: 6f6d 696e 6720 696e 2043 6f6e 6e65 6374  oming in Connect
-00004680: 6f72 2c20 636f 7079 2074 6865 2077 6562  or, copy the web
-00004690: 686f 6f6b 2055 524c 2e0d 0a0d 0a60 6060  hook URL.....```
-000046a0: 7079 7468 6f6e 0d0a 696d 706f 7274 2073  python..import s
-000046b0: 7973 0d0a 6672 6f6d 2045 7863 6570 744e  ys..from ExceptN
-000046c0: 6f74 6966 6965 7220 696d 706f 7274 2045  otifier import E
-000046d0: 7863 6570 7454 6561 6d73 2c20 5375 6363  xceptTeams, Succ
-000046e0: 6573 7354 6561 6d73 2c20 5365 6e64 5465  essTeams, SendTe
-000046f0: 616d 730d 0a73 7973 2e65 7863 6570 7468  ams..sys.excepth
-00004700: 6f6f 6b20 3d20 4578 6365 7074 5465 616d  ook = ExceptTeam
-00004710: 732e 5f5f 6361 6c6c 5f5f 0d0a 0d0a 2320  s.__call__....# 
-00004720: 4465 6669 6e65 2074 6865 206e 6578 7420  Define the next 
-00004730: 7477 6f20 7661 7269 6162 6c65 7320 6f70  two variables op
-00004740: 7469 6f6e 616c 6c79 2077 6865 6e20 7573  tionally when us
-00004750: 696e 6720 4f70 656e 4149 2773 2041 5049  ing OpenAI's API
-00004760: 2e0d 0a23 205f 4f50 454e 5f41 495f 4d4f  ...# _OPEN_AI_MO
-00004770: 4445 4c3d 2267 7074 2d33 2e35 2d74 7572  DEL="gpt-3.5-tur
-00004780: 626f 2220 2020 200d 0a23 205f 4f50 454e  bo"    ..# _OPEN
-00004790: 5f41 495f 4150 493d 2273 6b2d 7878 7878  _AI_API="sk-xxxx
-000047a0: 7878 220d 0a5f 5445 414d 535f 5745 4248  xx".._TEAMS_WEBH
-000047b0: 4f4f 4b5f 5552 4c20 3d20 276d 6963 726f  OOK_URL = 'micro
-000047c0: 736f 6674 2077 6562 686f 6f6b 205f 5445  soft webhook _TE
-000047d0: 414d 535f 5745 4248 4f4f 4b5f 5552 4c27  AMS_WEBHOOK_URL'
-000047e0: 0d0a 0d0a 7472 793a 0d0a 2020 2020 7072  ....try:..    pr
-000047f0: 696e 7428 312f 3230 2920 200d 0a20 2020  int(1/20)  ..   
-00004800: 2053 7563 6365 7373 5465 616d 7328 292e   SuccessTeams().
-00004810: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
-00004820: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
-00004830: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
-00004840: 7863 6570 7454 6561 6d73 2061 7320 653a  xceptTeams as e:
-00004850: 2020 2020 2020 2332 2065 7863 6570 7420        #2 except 
-00004860: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00004870: 2020 0d0a 2020 2020 7379 732e 6578 6974    ..    sys.exit
-00004880: 2829 0d0a 0d0a 5365 6e64 5465 616d 7328  ()....SendTeams(
-00004890: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
-000048a0: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
-000048b0: 6420 7365 6e64 6572 2020 2020 2020 2020  d sender        
-000048c0: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
-000048d0: 0a23 2320 322d 392e 202a 4b61 6b61 6f74  .## 2-9. *Kakaot
-000048e0: 616c 6b20 4e6f 7469 6669 6572 2a0d 0a2d  alk Notifier*..-
-000048f0: 2061 2e20 5369 676e 2075 7020 6174 2074   a. Sign up at t
-00004900: 6865 2066 6f6c 6c6f 7769 6e67 2073 6974  he following sit
-00004910: 653a 205b 6874 7470 733a 2f2f 6465 7665  e: [https://deve
-00004920: 6c6f 7065 7273 2e6b 616b 616f 2e63 6f6d  lopers.kakao.com
-00004930: 2f5d 2868 7474 7073 3a2f 2f64 6576 656c  /](https://devel
-00004940: 6f70 6572 732e 6b61 6b61 6f2e 636f 6d2f  opers.kakao.com/
-00004950: 292e 0d0a 2d20 622e 2043 6c69 636b 2022  )...- b. Click "
-00004960: 4d79 2041 7070 6c69 6361 7469 6f6e 2220  My Application" 
-00004970: 6f6e 2074 6865 2074 6f70 2062 6172 2e0d  on the top bar..
-00004980: 0a2d 2063 2e20 436c 6963 6b20 2241 6464  .- c. Click "Add
-00004990: 2061 6e20 6170 706c 6963 6174 696f 6e2c   an application,
-000049a0: 2220 7365 7420 6120 6e61 6d65 2c20 616e  " set a name, an
-000049b0: 6420 6372 6561 7465 2069 742e 0d0a 2d20  d create it...- 
-000049c0: 642e 2043 6c69 636b 2022 4b61 6b61 6f20  d. Click "Kakao 
-000049d0: 4c6f 6769 6e22 2069 6e20 7468 6520 6c65  Login" in the le
-000049e0: 6674 206d 656e 752c 2074 6865 6e20 6368  ft menu, then ch
-000049f0: 616e 6765 2074 6865 2053 7461 7465 206f  ange the State o
-00004a00: 6620 224b 616b 616f 204c 6f67 696e 2041  f "Kakao Login A
-00004a10: 6374 6976 6174 696f 6e22 2074 6f20 4f4e  ctivation" to ON
-00004a20: 206f 6e20 7468 6520 7265 7375 6c74 696e   on the resultin
-00004a30: 6720 7061 6765 2e0d 0a2d 2065 2e20 496e  g page...- e. In
-00004a40: 204d 7920 4170 706c 6963 6174 696f 6e20   My Application 
-00004a50: 3e20 5072 6f64 7563 7420 5365 7474 696e  > Product Settin
-00004a60: 6773 203e 204b 616b 616f 204c 6f67 696e  gs > Kakao Login
-00004a70: 2c20 6265 2073 7572 6520 746f 2073 6574  , be sure to set
-00004a80: 2052 6564 6972 6563 7420 5552 4920 6173   Redirect URI as
-00004a90: 2066 6f6c 6c6f 7773 3a20 5b68 7474 7073   follows: [https
-00004aa0: 3a2f 2f65 7861 6d70 6c65 2e63 6f6d 2f6f  ://example.com/o
-00004ab0: 6175 7468 5d28 6874 7470 733a 2f2f 6578  auth](https://ex
-00004ac0: 616d 706c 652e 636f 6d2f 6f61 7574 6829  ample.com/oauth)
-00004ad0: 2e0d 0a2d 2066 2e20 496e 2074 6865 206c  ...- f. In the l
-00004ae0: 6566 7420 436f 6e73 656e 7420 4974 656d  eft Consent Item
-00004af0: 7320 6d65 6e75 2c20 7365 7420 2253 656e  s menu, set "Sen
-00004b00: 6420 6d65 7373 6167 6520 696e 204b 616b  d message in Kak
-00004b10: 616f 5461 6c6b 2220 746f 2073 656c 6563  aoTalk" to selec
-00004b20: 7469 7665 2061 6772 6565 6d65 6e74 2e0d  tive agreement..
-00004b30: 0a2d 2067 2e20 436f 7079 2074 6865 2052  .- g. Copy the R
-00004b40: 4553 5420 4150 4920 4b65 7920 696e 204d  EST API Key in M
-00004b50: 7920 4170 706c 6963 6174 696f 6e20 3e20  y Application > 
-00004b60: 4170 7020 5365 7474 696e 6773 203e 2053  App Settings > S
-00004b70: 756d 6d61 7279 2c20 616e 6420 676f 2074  ummary, and go t
-00004b80: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
-00004b90: 646f 6375 6d65 6e74 2e0d 0a2d 2068 2e20  document...- h. 
-00004ba0: 4966 2079 6f75 2068 6176 6520 7375 6363  If you have succ
-00004bb0: 6573 7366 756c 6c79 2063 6f6d 706c 6574  essfully complet
-00004bc0: 6564 2061 6c6c 206f 6620 7468 6520 6162  ed all of the ab
-00004bd0: 6f76 6520 7374 6570 732c 2067 6f20 746f  ove steps, go to
-00004be0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00004bf0: 6f63 756d 656e 7420 616e 6420 666f 6c6c  ocument and foll
-00004c00: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-00004c10: 6f6e 733a 0d0a 2068 7474 7073 3a2f 2f67  ons:.. https://g
-00004c20: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00004c30: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00004c40: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00004c50: 7475 746f 7269 616c 732f 6b61 6b61 6f5f  tutorials/kakao_
-00004c60: 746f 6b65 6e5f 6765 6e65 7261 746f 722e  token_generator.
-00004c70: 6970 796e 620d 0a20 2a2a 496e 2074 6869  ipynb.. **In thi
-00004c80: 7320 6578 616d 706c 652c 2073 6f6d 6520  s example, some 
-00004c90: 4150 4920 6b65 7973 2077 6572 6520 6578  API keys were ex
-00004ca0: 706f 7365 6420 6279 2063 7265 6174 696e  posed by creatin
-00004cb0: 6720 616e 6420 7265 6d6f 7669 6e67 2061  g and removing a
-00004cc0: 2074 6573 7420 6170 706c 6963 6174 696f   test applicatio
-00004cd0: 6e2c 2062 7574 2066 6f72 2073 6563 7572  n, but for secur
-00004ce0: 6974 7920 7265 6173 6f6e 732c 2079 6f75  ity reasons, you
-00004cf0: 7220 4150 4920 6b65 7920 7368 6f75 6c64  r API key should
-00004d00: 206e 6f74 2062 6520 6578 706f 7365 6420   not be exposed 
-00004d10: 746f 2074 6865 206f 7574 7369 6465 2077  to the outside w
-00004d20: 6f72 6c64 2e2a 2a0d 0a3c 4272 3e0d 0a0d  orld.**..<Br>...
-00004d30: 0a60 6060 7079 7468 6f6e 0d0a 696d 706f  .```python..impo
-00004d40: 7274 2073 7973 0d0a 6672 6f6d 2045 7863  rt sys..from Exc
-00004d50: 6570 744e 6f74 6966 6965 7220 696d 706f  eptNotifier impo
-00004d60: 7274 2045 7863 6570 744b 616b 616f 2c20  rt ExceptKakao, 
-00004d70: 5375 6363 6573 734b 616b 616f 2c20 5365  SuccessKakao, Se
-00004d80: 6e64 4b61 6b61 6f0d 0a73 7973 2e65 7863  ndKakao..sys.exc
-00004d90: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
-00004da0: 4b61 6b61 6f2e 5f5f 6361 6c6c 5f5f 0d0a  Kakao.__call__..
-00004db0: 0d0a 2320 4465 6669 6e65 2074 6865 206e  ..# Define the n
-00004dc0: 6578 7420 7477 6f20 7661 7269 6162 6c65  ext two variable
-00004dd0: 7320 6f70 7469 6f6e 616c 6c79 2077 6865  s optionally whe
-00004de0: 6e20 7573 696e 6720 4f70 656e 4149 2773  n using OpenAI's
-00004df0: 2041 5049 2e0d 0a23 205f 4f50 454e 5f41   API...# _OPEN_A
-00004e00: 495f 4d4f 4445 4c3d 2267 7074 2d33 2e35  I_MODEL="gpt-3.5
-00004e10: 2d74 7572 626f 2220 2020 200d 0a23 205f  -turbo"    ..# _
-00004e20: 4f50 454e 5f41 495f 4150 493d 2273 6b2d  OPEN_AI_API="sk-
-00004e30: 7878 7878 7878 220d 0a5f 4b41 4b41 4f5f  xxxxxx".._KAKAO_
-00004e40: 544f 4b45 4e5f 5041 5448 203d 2027 7878  TOKEN_PATH = 'xx
-00004e50: 7878 2f78 7878 2f78 7878 2e6a 736f 6e27  xx/xxx/xxx.json'
-00004e60: 270d 0a0d 0a74 7279 3a0d 0a20 2020 2070  '....try:..    p
-00004e70: 7269 6e74 2831 2f30 2920 200d 0a20 2020  rint(1/0)  ..   
-00004e80: 2053 7563 6365 7373 4b61 6b61 6f28 292e   SuccessKakao().
-00004e90: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
-00004ea0: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
-00004eb0: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
-00004ec0: 7863 6570 744b 616b 616f 2061 7320 653a  xceptKakao as e:
-00004ed0: 2020 2020 2020 2332 2065 7863 6570 7420        #2 except 
-00004ee0: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00004ef0: 2020 0d0a 2020 2020 7379 732e 6578 6974    ..    sys.exit
-00004f00: 2829 0d0a 0d0a 5365 6e64 4b61 6b61 6f28  ()....SendKakao(
-00004f10: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
-00004f20: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
-00004f30: 6420 7365 6e64 6572 2020 2020 2020 2020  d sender        
-00004f40: 200d 0a60 6060 0d0a 0d0a 3c42 723e 0d0a   ..```....<Br>..
-00004f50: 0d0a 2323 2032 2d31 302e 202a 4265 6570  ..## 2-10. *Beep
-00004f60: 204e 6f74 6966 6965 722a 0d0a 4e6f 2073   Notifier*..No s
-00004f70: 6574 7570 2069 7320 7265 7175 6972 6564  etup is required
-00004f80: 2e20 5573 6520 6173 2066 6f6c 6c6f 7773  . Use as follows
-00004f90: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
-00004fa0: 6672 6f6d 2045 7863 6570 746e 6f74 6966  from Exceptnotif
-00004fb0: 6965 7220 696d 706f 7274 2045 7863 6570  ier import Excep
-00004fc0: 7442 6565 702c 2053 7563 6365 7373 4265  tBeep, SuccessBe
-00004fd0: 6570 2c20 5365 6e64 4265 6570 2829 2c20  ep, SendBeep(), 
-00004fe0: 6265 6570 2829 0d0a 4245 4550 5f54 494d  beep()..BEEP_TIM
-00004ff0: 4520 3d20 310d 0a73 7973 2e65 7863 6570  E = 1..sys.excep
-00005000: 7468 6f6f 6b20 3d20 4578 6365 7074 4265  thook = ExceptBe
-00005010: 6570 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a74  ep.__call__....t
-00005020: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
-00005030: 2f32 3029 2020 0d0a 2020 2020 5375 6363  /20)  ..    Succ
-00005040: 6573 7342 6565 7028 292e 5f5f 6361 6c6c  essBeep().__call
-00005050: 5f5f 2829 2023 3120 7375 6363 6573 7320  __() #1 success 
-00005060: 6265 6570 2d62 6565 7020 2020 2020 2020  beep-beep       
-00005070: 2020 200d 0a0d 0a65 7863 6570 7420 4578     ....except Ex
-00005080: 6365 7074 4265 6570 2061 7320 653a 2020  ceptBeep as e:  
-00005090: 2020 2020 2332 2065 7863 6570 7420 6265      #2 except be
-000050a0: 6570 2d62 6565 7020 2020 2020 2020 2020  ep-beep         
-000050b0: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-000050c0: 2e65 7869 7428 290d 0a0d 0a53 656e 6442  .exit()....SendB
-000050d0: 6565 7028 292e 5f5f 6361 6c6c 5f5f 2829  eep().__call__()
-000050e0: 2020 2020 2020 2020 2333 2063 7573 746f          #3 custo
-000050f0: 6d69 7a65 6420 6265 6570 2d62 6565 7020  mized beep-beep 
-00005100: 2020 2020 200d 0a0d 0a62 6565 7028 290d       ....beep().
-00005110: 0a0d 0a60 6060 0d0a 0d0a 3c42 723e 0d0a  ...```....<Br>..
-00005120: 0d0a 0d0a 2323 2032 2d31 312e 202a 4465  ....## 2-11. *De
-00005130: 736b 746f 7020 4e6f 7469 6669 6572 2a0d  sktop Notifier*.
-00005140: 0a4e 6f20 7365 7475 7020 6973 2072 6571  .No setup is req
-00005150: 7569 7265 642e 2055 7365 2061 7320 666f  uired. Use as fo
-00005160: 6c6c 6f77 732e 0d0a 0d0a 6060 6070 7974  llows.....```pyt
-00005170: 686f 6e0d 0a66 726f 6d20 4578 6365 7074  hon..from Except
-00005180: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
-00005190: 4578 6365 7074 4465 736b 746f 702c 2053  ExceptDesktop, S
-000051a0: 7563 6365 7373 4465 736b 746f 702c 2053  uccessDesktop, S
-000051b0: 656e 6444 6573 6b74 6f70 0d0a 7379 732e  endDesktop..sys.
-000051c0: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-000051d0: 6570 7444 6573 6b74 6f70 2e5f 5f63 616c  eptDesktop.__cal
-000051e0: 6c5f 5f0d 0a23 2044 6566 696e 6520 7468  l__..# Define th
-000051f0: 6520 6e65 7874 2074 776f 2076 6172 6961  e next two varia
-00005200: 626c 6573 206f 7074 696f 6e61 6c6c 7920  bles optionally 
-00005210: 7768 656e 2075 7369 6e67 204f 7065 6e41  when using OpenA
-00005220: 4927 7320 4150 492e 0d0a 2320 5f4f 5045  I's API...# _OPE
-00005230: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-00005240: 332e 352d 7475 7262 6f22 2020 2020 0d0a  3.5-turbo"    ..
-00005250: 2320 5f4f 5045 4e5f 4149 5f41 5049 3d22  # _OPEN_AI_API="
-00005260: 736b 2d78 7878 7878 7822 0d0a 0d0a 7472  sk-xxxxxx"....tr
-00005270: 793a 0d0a 2020 2020 7072 696e 7428 312f  y:..    print(1/
-00005280: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
-00005290: 7344 6573 6b74 6f70 2829 2e5f 5f63 616c  sDesktop().__cal
-000052a0: 6c5f 5f28 2920 2331 2073 7563 6365 7373  l__() #1 success
-000052b0: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
-000052c0: 200d 0a0d 0a65 7863 6570 7420 4578 6365   ....except Exce
-000052d0: 7074 4465 736b 746f 7020 6173 2065 3a20  ptDesktop as e: 
-000052e0: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
-000052f0: 656e 6465 7220 2020 2020 2020 2020 2020  ender           
-00005300: 200d 0a20 2020 2073 7973 2e65 7869 7428   ..    sys.exit(
-00005310: 290d 0a0d 0a53 656e 6444 6573 6b74 6f70  )....SendDesktop
-00005320: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
-00005330: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
-00005340: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
-00005350: 2020 0d0a 6060 600d 0a0d 0a3c 4272 3e3c    ..```....<Br><
-00005360: 6272 3e3c 6272 3e0d 0a0d 0a23 2323 2049  br><br>....### I
-00005370: 6e73 7069 7269 6e67 0d0a 2d20 5468 616e  nspiring..- Than
-00005380: 6b73 2074 6f20 5b4d 7975 6e67 6861 6b20  ks to [Myunghak 
-00005390: 4c65 655d 2868 7474 7073 3a2f 2f67 6974  Lee](https://git
-000053a0: 6875 622e 636f 6d2f 6d79 656f 6e67 6861  hub.com/myeongha
-000053b0: 6b29 2066 6f72 2070 726f 7669 6469 6e67  k) for providing
-000053c0: 2067 7265 6174 2069 6465 6173 206f 6e20   great ideas on 
-000053d0: 7072 6f76 6964 696e 6720 6465 6275 6767  providing debugg
-000053e0: 696e 6720 696e 666f 726d 6174 696f 6e20  ing information 
-000053f0: 7468 726f 7567 6820 6f70 656e 2061 6920  through open ai 
-00005400: 4150 492e 0d0a 0d0a 2323 2320 436f 6e74  API.....### Cont
-00005410: 6163 7473 0d0a 2d20 4d61 696e 7461 696e  acts..- Maintain
-00005420: 6572 205b 4461 6e69 656c 2050 6172 6b2c  er [Daniel Park,
-00005430: 2053 6f75 7468 204b 6f72 6561 5d28 6874   South Korea](ht
-00005440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005450: 2f44 5344 616e 6965 6c50 6172 6b29 203c  /DSDanielPark) <
-00005460: 6272 3e0d 0a2d 2045 6d61 696c 2070 6172  br>..- Email par
-00005470: 6b6d 696e 776f 6f31 3939 3140 676d 6169  kminwoo1991@gmai
-00005480: 6c2e 636f 6d0d 0a0d 0a23 2323 2323 2054  l.com....##### T
-00005490: 6865 2070 6163 6b61 6765 2069 7320 6375  he package is cu
-000054a0: 7272 656e 746c 7920 696e 2074 6865 2064  rrently in the d
-000054b0: 6576 656c 6f70 6d65 6e74 2061 6e64 2051  evelopment and Q
-000054c0: 4120 7374 6167 6573 2c20 616e 6420 7468  A stages, and th
-000054d0: 6520 6465 7665 6c6f 706d 656e 7420 7374  e development st
-000054e0: 6167 6520 7769 6c6c 2062 6520 7570 6461  age will be upda
-000054f0: 7465 6420 6174 2074 6865 2074 6f70 206f  ted at the top o
-00005500: 6620 7468 6973 2070 6167 652e 2049 6620  f this page. If 
-00005510: 6974 2069 7320 6465 7465 726d 696e 6564  it is determined
-00005520: 2074 6861 7420 7468 6520 7072 6f64 7563   that the produc
-00005530: 7420 6973 2073 7461 626c 6520 7468 726f  t is stable thro
-00005540: 7567 6820 6665 6174 7572 6520 696d 7072  ugh feature impr
-00005550: 6f76 656d 656e 742c 2061 6464 6974 696f  ovement, additio
-00005560: 6e2c 2061 6e64 2069 7373 7565 2072 6573  n, and issue res
-00005570: 6f6c 7574 696f 6e2c 2074 6865 2064 6576  olution, the dev
-00005580: 656c 6f70 6d65 6e74 2073 7461 6765 2077  elopment stage w
-00005590: 696c 6c20 7265 6163 6820 7374 6167 6520  ill reach stage 
-000055a0: 352e 2049 6620 6e6f 206e 6577 2075 7064  5. If no new upd
-000055b0: 6174 6573 206f 7220 6973 7375 6573 2061  ates or issues a
-000055c0: 7269 7365 2c20 6974 2077 696c 6c20 6265  rise, it will be
-000055d0: 2061 646a 7573 7465 6420 7570 7761 7264   adjusted upward
-000055e0: 2074 6f20 7374 6167 6520 3620 6f72 2068   to stage 6 or h
-000055f0: 6967 6865 722e 0d0a 0d0a 2323 2323 2043  igher.....#### C
-00005600: 6f75 6c64 2079 6f75 206b 696e 646c 7920  ould you kindly 
-00005610: 6164 6420 7468 6973 2062 6164 6765 2074  add this badge t
-00005620: 6f20 796f 7572 2072 6570 6f73 6974 6f72  o your repositor
-00005630: 793f 0d0a 0d0a 6060 600d 0a21 5b45 7863  y?....```..![Exc
-00005640: 6570 742d 4e6f 7469 6669 6572 5d28 6874  ept-Notifier](ht
-00005650: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00005660: 732e 696f 2f62 6164 6765 2f70 7970 692d  s.io/badge/pypi-
-00005670: 4578 6365 7074 4e6f 7469 6669 6572 2d6f  ExceptNotifier-o
-00005680: 7261 6e67 6529 0d0a 6060 600d 0a0d 0a0d  range)..```.....
-00005690: 0a                                       .
+00000470: 3e0d 0a21 5b5d 2868 7474 7073 3a2f 2f67  >..![](https://g
+00000480: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
+00000490: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
+000004a0: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
+000004b0: 6173 7365 7473 2f69 6d67 732f 4578 6365  assets/imgs/Exce
+000004c0: 7074 4e6f 7469 6669 6572 5f6c 6f67 6f2e  ptNotifier_logo.
+000004d0: 706e 6729 0d0a 0d0a 3c68 3320 616c 6967  png)....<h3 alig
+000004e0: 6e3d 2263 656e 7465 7222 3e49 6e74 6567  n="center">Integ
+000004f0: 7261 7465 7320 4149 2d61 7373 6973 7465  rates AI-assiste
+00000500: 6420 6465 6275 6767 696e 6720 6e6f 7469  d debugging noti
+00000510: 6669 6361 7469 6f6e 7320 696e 746f 2050  fications into P
+00000520: 7974 686f 6e20 7472 792d 6578 6365 7074  ython try-except
+00000530: 2073 7461 7465 6d65 6e74 7320 666f 7220   statements for 
+00000540: 7661 7269 6f75 7320 6d65 7373 6167 696e  various messagin
+00000550: 6720 6170 706c 6963 6174 696f 6e73 2e20  g applications. 
+00000560: 3c2f 6833 3e0d 0a0d 0a3c 7020 616c 6967  </h3>....<p alig
+00000570: 6e3d 2263 656e 7465 7222 3e0d 0a3c 6120  n="center">..<a 
+00000580: 6872 6566 3d22 2868 7474 7073 3a2f 2f69  href="(https://i
+00000590: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000005a0: 6467 652f 7079 7069 2d45 7863 6570 744e  dge/pypi-ExceptN
+000005b0: 6f74 6966 6965 722d 6f72 616e 6765 223e  otifier-orange">
+000005c0: 3c2f 613e 0d0a 3c61 2068 7265 663d 2268  </a>..<a href="h
+000005d0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000005e0: 7072 6f6a 6563 742f 6578 6365 7074 6e6f  project/exceptno
+000005f0: 7469 6669 6572 2f22 3e3c 696d 6720 616c  tifier/"><img al
+00000600: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
+00000610: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000620: 732e 696f 2f70 7970 692f 762f 6578 6365  s.io/pypi/v/exce
+00000630: 7074 6e6f 7469 6669 6572 223e 3c2f 613e  ptnotifier"></a>
+00000640: 0d0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000650: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
+00000660: 6a65 6374 2f65 7863 6570 746e 6f74 6966  ject/exceptnotif
+00000670: 6965 7222 3e3c 696d 6720 616c 743d 2244  ier"><img alt="D
+00000680: 6f77 6e6c 6f61 6473 2220 7372 633d 2268  ownloads" src="h
+00000690: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+000006a0: 2f62 6164 6765 2f65 7863 6570 746e 6f74  /badge/exceptnot
+000006b0: 6966 6965 7222 3e3c 2f61 3e0d 0a3c 6120  ifier"></a>..<a 
+000006c0: 6872 6566 3d22 6874 7470 733a 2f2f 616e  href="https://an
+000006d0: 6163 6f6e 6461 2e6f 7267 2f63 6f6e 6461  aconda.org/conda
+000006e0: 2d66 6f72 6765 2f65 7863 6570 746e 6f74  -forge/exceptnot
+000006f0: 6966 6965 722f 223e 3c69 6d67 2061 6c74  ifier/"><img alt
+00000700: 3d22 636f 6e64 612d 666f 7267 6522 2073  ="conda-forge" s
+00000710: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000720: 7368 6965 6c64 732e 696f 2f63 6f6e 6461  shields.io/conda
+00000730: 2f64 6e2f 636f 6e64 612d 666f 7267 652f  /dn/conda-forge/
+00000740: 6578 6365 7074 6e6f 7469 6669 6572 2e73  exceptnotifier.s
+00000750: 7667 3f6c 6162 656c 3d63 6f6e 6461 2d66  vg?label=conda-f
+00000760: 6f72 6765 223e 3c2f 613e 0d0a 3c61 2068  orge"></a>..<a h
+00000770: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000780: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+00000790: 6b22 3e3c 696d 6720 616c 743d 2243 6f64  k"><img alt="Cod
+000007a0: 6520 7374 796c 653a 2062 6c61 636b 2220  e style: black" 
+000007b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000007c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000007d0: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
+000007e0: 6c61 636b 2d30 3030 3030 302e 7376 6722  lack-000000.svg"
+000007f0: 3e3c 2f61 3e0d 0a3c 2f70 3e0d 0a0d 0a21  ></a>..</p>....!
+00000800: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
+00000810: 622e 636f 6d2f 6473 6461 6e69 656c 7061  b.com/dsdanielpa
+00000820: 726b 2f45 7863 6570 744e 6f74 6966 6965  rk/ExceptNotifie
+00000830: 722f 626c 6f62 2f6d 6169 6e2f 6173 7365  r/blob/main/asse
+00000840: 7473 2f69 6d67 732f 6d61 696e 322e 706e  ts/imgs/main2.pn
+00000850: 6729 0d0a 0d0a 2320 5079 7468 6f6e 2050  g)....# Python P
+00000860: 6163 6b61 6765 3a20 4578 6365 7074 4e6f  ackage: ExceptNo
+00000870: 7469 6669 6572 0d0a 2323 2323 2320 5072  tifier..##### Pr
+00000880: 6f76 6964 6573 2061 206e 6f74 6966 6963  ovides a notific
+00000890: 6174 696f 6e20 6672 6f6d 2074 6865 2061  ation from the a
+000008a0: 7070 6c69 6361 7469 6f6e 2073 686f 776e  pplication shown
+000008b0: 2069 6e20 7468 6520 6361 7074 7572 6564   in the captured
+000008c0: 2073 6372 6565 6e2e 0d0a 2054 6865 2060   screen... The `
+000008d0: 4578 6365 7074 4e6f 7469 6669 6572 6020  ExceptNotifier` 
+000008e0: 5079 7468 6f6e 2070 6163 6b61 6765 206f  Python package o
+000008f0: 6666 6572 7320 6120 666c 6578 6962 6c65  ffers a flexible
+00000900: 2061 7070 726f 6163 6820 746f 2072 6563   approach to rec
+00000910: 6569 7669 6e67 206e 6f74 6966 6963 6174  eiving notificat
+00000920: 696f 6e73 2062 7920 656e 6861 6e63 696e  ions by enhancin
+00000930: 6720 5079 7468 6f6e 2773 2074 7279 2d65  g Python's try-e
+00000940: 7863 6570 7420 7374 6174 656d 656e 742e  xcept statement.
+00000950: 2054 6869 7320 7061 636b 6167 6520 656e   This package en
+00000960: 6162 6c65 7320 796f 7520 746f 2072 6563  ables you to rec
+00000970: 6569 7665 2061 6c65 7274 7320 7468 726f  eive alerts thro
+00000980: 7567 6820 7661 7269 6f75 7320 6d65 7373  ugh various mess
+00000990: 6167 696e 6720 6170 706c 6963 6174 696f  aging applicatio
+000009a0: 6e73 206f 7220 656d 6169 6c73 2e0d 0a3c  ns or emails...<
+000009b0: 4272 3e3c 6272 3e0d 0a57 6974 6820 6045  Br><br>..With `E
+000009c0: 7863 6570 744e 6f74 6966 6965 7260 2c20  xceptNotifier`, 
+000009d0: 796f 7520 6361 6e20 6f62 7461 696e 2064  you can obtain d
+000009e0: 6574 6169 6c65 6420 636f 6d70 696c 6174  etailed compilat
+000009f0: 696f 6e20 6572 726f 7273 2c20 696e 636c  ion errors, incl
+00000a00: 7564 696e 6720 6465 6275 6720 696e 666f  uding debug info
+00000a10: 726d 6174 696f 6e2c 2073 656e 7420 6469  rmation, sent di
+00000a20: 7265 6374 6c79 2074 6f20 796f 7572 2070  rectly to your p
+00000a30: 7265 6665 7272 6564 206d 6573 7361 6769  referred messagi
+00000a40: 6e67 2070 6c61 7466 6f72 6d20 6f72 2065  ng platform or e
+00000a50: 6d61 696c 2e20 4279 2069 6e74 6567 7261  mail. By integra
+00000a60: 7469 6e67 204f 7065 6e41 4927 7320 4368  ting OpenAI's Ch
+00000a70: 6174 4750 542c 2079 6f75 2063 616e 2072  atGPT, you can r
+00000a80: 6563 6569 7665 2061 6464 6974 696f 6e61  eceive additiona
+00000a90: 6c20 6572 726f 7220 636f 6465 2069 6e66  l error code inf
+00000aa0: 6f72 6d61 7469 6f6e 2061 7320 6c6f 6e67  ormation as long
+00000ab0: 2061 7320 796f 7520 7072 6f76 6964 6520   as you provide 
+00000ac0: 7468 6520 7265 7175 6972 6564 2041 5049  the required API
+00000ad0: 206d 6f64 656c 206e 616d 6520 616e 6420   model name and 
+00000ae0: 6b65 792e 2054 6869 7320 6665 6174 7572  key. This featur
+00000af0: 6520 656e 7375 7265 7320 7468 6174 2065  e ensures that e
+00000b00: 7272 6f72 2068 616e 646c 696e 6720 616e  rror handling an
+00000b10: 6420 6e6f 7469 6669 6361 7469 6f6e 7320  d notifications 
+00000b20: 6172 6520 6d6f 7265 2069 6e66 6f72 6d61  are more informa
+00000b30: 7469 7665 2061 6e64 2061 6363 6573 7369  tive and accessi
+00000b40: 626c 652c 2073 7472 6561 6d6c 696e 696e  ble, streamlinin
+00000b50: 6720 796f 7572 2064 6562 7567 6769 6e67  g your debugging
+00000b60: 2070 726f 6365 7373 2e0d 0a0d 0a3c 4272   process.....<Br
+00000b70: 3e0d 0a0d 0a23 2323 2320 436f 756c 6420  >....#### Could 
+00000b80: 796f 7520 6b69 6e64 6c79 2061 6464 2074  you kindly add t
+00000b90: 6869 7320 6261 6467 6520 746f 2079 6f75  his badge to you
+00000ba0: 7220 7265 706f 7369 746f 7279 3f0d 0a0d  r repository?...
+00000bb0: 0a60 6060 0d0a 215b 4578 6365 7074 2d4e  .```..![Except-N
+00000bc0: 6f74 6966 6965 725d 2868 7474 7073 3a2f  otifier](https:/
+00000bd0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000be0: 6261 6467 652f 7079 7069 2d45 7863 6570  badge/pypi-Excep
+00000bf0: 744e 6f74 6966 6965 722d 6f72 616e 6765  tNotifier-orange
+00000c00: 290d 0a60 6060 0d0a 0d0a 0d0a 3c62 723e  )..```......<br>
+00000c10: 3c62 723e 0d0a 0d0a 2323 2320 5375 7070  <br>....### Supp
+00000c20: 6f72 7469 6e67 2041 7070 6c69 6361 7469  orting Applicati
+00000c30: 6f6e 730d 0a0d 0a2d 205b 5465 6c65 6772  ons....- [Telegr
+00000c40: 616d 5d28 6874 7470 733a 2f2f 7465 6c65  am](https://tele
+00000c50: 6772 616d 2e6f 7267 2f29 0d0a 2d20 5b44  gram.org/)..- [D
+00000c60: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+00000c70: 6469 7363 6f72 642e 636f 6d2f 290d 0a2d  discord.com/)..-
+00000c80: 205b 536c 6163 6b5d 2868 7474 7073 3a2f   [Slack](https:/
+00000c90: 2f73 6c61 636b 2e63 6f6d 2f29 0d0a 2d20  /slack.com/)..- 
+00000ca0: 5b47 6f6f 676c 6520 4d61 696c 5d28 6874  [Google Mail](ht
+00000cb0: 7470 733a 2f2f 6d61 696c 2e67 6f6f 676c  tps://mail.googl
+00000cc0: 652e 636f 6d2f 290d 0a2d 205b 4c69 6e65  e.com/)..- [Line
+00000cd0: 5d28 6874 7470 733a 2f2f 6c69 6e65 2e6d  ](https://line.m
+00000ce0: 652f 656e 2f29 0d0a 2d20 5b41 5753 2043  e/en/)..- [AWS C
+00000cf0: 6869 6d65 5d28 6874 7470 733a 2f2f 6177  hime](https://aw
+00000d00: 732e 616d 617a 6f6e 2e63 6f6d 2f6b 6f2f  s.amazon.com/ko/
+00000d10: 6368 696d 652f 646f 776e 6c6f 6164 2d63  chime/download-c
+00000d20: 6869 6d65 2f29 0d0a 2d20 5b4d 6963 726f  hime/)..- [Micro
+00000d30: 736f 6674 2054 6561 6d73 5d28 6874 7470  soft Teams](http
+00000d40: 733a 2f2f 7777 772e 6d69 6372 6f73 6f66  s://www.microsof
+00000d50: 742e 636f 6d2f 656e 2f6d 6963 726f 736f  t.com/en/microso
+00000d60: 6674 2d74 6561 6d73 2f64 6f77 6e6c 6f61  ft-teams/downloa
+00000d70: 642d 6170 7029 0d0a 2d20 5b4b 616b 616f  d-app)..- [Kakao
+00000d80: 2054 616c 6b5d 2868 7474 7073 3a2f 2f77   Talk](https://w
+00000d90: 7777 2e6b 616b 616f 636f 7270 2e63 6f6d  ww.kakaocorp.com
+00000da0: 2f70 6167 652f 7365 7276 6963 652f 7365  /page/service/se
+00000db0: 7276 6963 652f 4b61 6b61 6f54 616c 6b3f  rvice/KakaoTalk?
+00000dc0: 6c61 6e67 3d65 6e29 0d0a 2d20 534d 5320  lang=en)..- SMS 
+00000dd0: 5365 6e64 696e 6720 7573 696e 6720 5b54  Sending using [T
+00000de0: 7769 6c69 6f5d 2868 7474 7073 3a2f 2f77  wilio](https://w
+00000df0: 7777 2e74 7769 6c69 6f2e 636f 6d2f 656e  ww.twilio.com/en
+00000e00: 2d75 7329 0d0a 2d20 4465 736b 746f 7020  -us)..- Desktop 
+00000e10: 4e6f 7469 6669 6361 7469 6f6e 2075 7369  Notification usi
+00000e20: 6e67 205b 506c 7965 725d 2868 7474 7073  ng [Plyer](https
+00000e30: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b69  ://github.com/ki
+00000e40: 7679 2f70 6c79 6572 290d 0a2d 2042 6565  vy/plyer)..- Bee
+00000e50: 7020 536f 756e 6420 6672 6f6d 205b 7379  p Sound from [sy
+00000e60: 7374 656d 5d28 6874 7470 733a 2f2f 646f  stem](https://do
+00000e70: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+00000e80: 6c69 6272 6172 792f 7769 6e73 6f75 6e64  library/winsound
+00000e90: 2e68 746d 6c29 0d0a 0d0a 3c42 723e 0d0a  .html)....<Br>..
+00000ea0: 0d0a 2323 2320 4149 2044 6562 7567 6769  ..### AI Debuggi
+00000eb0: 6e67 2075 7369 6e67 204f 7065 6e41 4920  ng using OpenAI 
+00000ec0: 4150 490d 0a49 6620 796f 7520 6861 7665  API..If you have
+00000ed0: 204f 7065 6e41 4920 4150 4920 4b65 7920   OpenAI API Key 
+00000ee0: 616e 6420 6d6f 6465 6c20 6e61 6d65 2c20  and model name, 
+00000ef0: 796f 7520 6361 6e20 6765 7420 696e 666f  you can get info
+00000f00: 726d 6174 696f 6e20 616e 6420 636f 6465  rmation and code
+00000f10: 2065 7861 6d70 6c65 7320 666f 7220 6465   examples for de
+00000f20: 6275 6767 696e 6720 696e 2061 6e79 2061  bugging in any a
+00000f30: 7070 6c69 6361 7469 6f6e 2e0d 0a2d 205b  pplication...- [
+00000f40: 4f50 454e 2041 4920 4150 495d 2868 7474  OPEN AI API](htt
+00000f50: 7073 3a2f 2f70 6c61 7466 6f72 6d2e 6f70  ps://platform.op
+00000f60: 656e 6169 2e63 6f6d 2f64 6f63 732f 696e  enai.com/docs/in
+00000f70: 7472 6f64 7563 7469 6f6e 290d 0a0d 0a0d  troduction).....
+00000f80: 0a3c 6272 3e3c 6272 3e0d 0a0d 0a23 2051  .<br><br>....# Q
+00000f90: 7569 636b 2053 7461 7274 0d0a 6060 6062  uick Start..```b
+00000fa0: 6173 680d 0a70 6970 2069 6e73 7461 6c6c  ash..pip install
+00000fb0: 2045 7863 6570 744e 6f74 6966 6965 720d   ExceptNotifier.
+00000fc0: 0a70 6970 2069 6e73 7461 6c6c 2065 7863  .pip install exc
+00000fd0: 6570 746e 6f74 6966 6965 720d 0a0d 0a63  eptnotifier....c
+00000fe0: 6f6e 6461 2069 6e73 7461 6c6c 2045 7863  onda install Exc
+00000ff0: 6570 744e 6f74 6966 6965 720d 0a63 6f6e  eptNotifier..con
+00001000: 6461 2069 6e73 7461 6c6c 2065 7863 6570  da install excep
+00001010: 746e 6f74 6966 6965 720d 0a60 6060 0d0a  tnotifier..```..
+00001020: 0d0a 3c62 723e 0d0a 0d0a 0d0a 2320 4170  ..<br>......# Ap
+00001030: 7020 5365 7475 7020 4f76 6572 7669 6577  p Setup Overview
+00001040: 0d0a 0d0a 2d20 5468 6520 7661 7269 6162  ....- The variab
+00001050: 6c65 7320 696e 2074 6865 2066 6f6c 6c6f  les in the follo
+00001060: 7769 6e67 2074 6162 6c65 206d 7573 7420  wing table must 
+00001070: 6e6f 7420 6265 2063 6f6e 7461 6d69 6e61  not be contamina
+00001080: 7465 642e 0d0a 2d20 4465 7065 6e64 696e  ted...- Dependin
+00001090: 6720 6f6e 2074 6865 2073 6974 7561 7469  g on the situati
+000010a0: 6f6e 2c20 636f 6e73 6964 6572 2064 6573  on, consider des
+000010b0: 6967 6e61 7469 6e67 2074 6865 6d20 6173  ignating them as
+000010c0: 2067 6c6f 6261 6c20 7661 7269 6162 6c65   global variable
+000010d0: 7320 666f 7220 7573 652e 0d0a 2d20 4966  s for use...- If
+000010e0: 2079 6f75 2061 7265 2075 7369 6e67 2054   you are using T
+000010f0: 656c 6567 7261 6d2c 2061 6e20 6578 616d  elegram, an exam
+00001100: 706c 6520 6973 2061 7474 6163 6865 6420  ple is attached 
+00001110: 6173 2061 6e20 696d 6167 652e 0d0a 2d20  as an image...- 
+00001120: 4173 2079 6f75 2061 6c72 6561 6479 206b  As you already k
+00001130: 6e6f 772c 2041 5049 204b 6579 7320 6f72  now, API Keys or
+00001140: 2073 6563 7572 6974 7920 746f 6b65 6e73   security tokens
+00001150: 206d 7573 7420 6265 2073 6563 7572 6564   must be secured
+00001160: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
+00001170: 6b65 7920 7661 6c75 6573 2077 6869 6368  key values which
+00001180: 2065 7870 6f73 7572 6564 2069 6e20 6769   exposured in gi
+00001190: 7468 7562 2077 696c 6c20 6265 2065 7870  thub will be exp
+000011a0: 6972 6564 2061 6674 6572 2069 6e73 6563  ired after insec
+000011b0: 7572 6564 2e0d 0a0d 0a7c 2041 7070 207c  ured.....| App |
+000011c0: 2052 6571 7569 7265 6420 5661 7269 6162   Required Variab
+000011d0: 6c65 7320 7c20 4672 6565 206f 7220 5061  les | Free or Pa
+000011e0: 6964 207c 2045 6173 6520 6f66 2053 6574  id | Ease of Set
+000011f0: 7570 207c 2054 696d 6520 5265 7175 6972  up | Time Requir
+00001200: 6564 2066 6f72 2053 6574 7570 7c47 7569  ed for Setup|Gui
+00001210: 6465 2054 7574 6f72 6961 6c20 4c69 6e6b  de Tutorial Link
+00001220: 7c0d 0a7c 3a2d 2d3a 7c3a 2d2d 7c3a 2d2d  |..|:--:|:--|:--
+00001230: 3a7c 3a2d 2d3a 7c3a 2d2d 3a7c 3a2d 2d2d  :|:--:|:--:|:---
+00001240: 3a7c 0d0a 7c42 6565 707c 4e2f 417c 4672  :|..|Beep|N/A|Fr
+00001250: 6565 7c4e 2f41 7c30 206d 696e 7c5b 4578  ee|N/A|0 min|[Ex
+00001260: 6365 7074 4265 6570 5d28 6874 7470 733a  ceptBeep](https:
+00001270: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7364  //github.com/dsd
+00001280: 616e 6965 6c70 6172 6b2f 4578 6365 7074  anielpark/Except
+00001290: 4e6f 7469 6669 6572 2f62 6c6f 622f 6d61  Notifier/blob/ma
+000012a0: 696e 2f64 6f63 756d 656e 7473 2f45 7863  in/documents/Exc
+000012b0: 6570 7442 6565 702f 4755 4944 452e 6d64  eptBeep/GUIDE.md
+000012c0: 297c 0d0a 7c44 6573 6b74 6f70 7c4e 2f41  )|..|Desktop|N/A
+000012d0: 7c46 7265 657c 4e2f 417c 3020 6d69 6e7c  |Free|N/A|0 min|
+000012e0: 5b45 7863 6570 7444 6573 6b74 6f70 5d28  [ExceptDesktop](
+000012f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001300: 6f6d 2f64 7364 616e 6965 6c70 6172 6b2f  om/dsdanielpark/
+00001310: 4578 6365 7074 4e6f 7469 6669 6572 2f62  ExceptNotifier/b
+00001320: 6c6f 622f 6d61 696e 2f64 6f63 756d 656e  lob/main/documen
+00001330: 7473 2f45 7863 6570 7444 6573 6b74 6f70  ts/ExceptDesktop
+00001340: 2f47 5549 4445 2e6d 6429 7c0d 0a7c 5465  /GUIDE.md)|..|Te
+00001350: 6c65 6772 616d 7c60 5f54 454c 4547 5241  legram|`_TELEGRA
+00001360: 4d5f 544f 4b45 4e60 7c46 7265 656d 6975  M_TOKEN`|Freemiu
+00001370: 6d7c 4561 7379 7c32 6d69 6e7c 5b45 7863  m|Easy|2min|[Exc
+00001380: 6570 7454 656c 6567 7261 6d5d 2868 7474  eptTelegram](htt
+00001390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000013a0: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+000013b0: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+000013c0: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+000013d0: 4578 6365 7074 5465 6c65 6772 616d 2f47  ExceptTelegram/G
+000013e0: 5549 4445 2e6d 6429 7c0d 0a7c 4469 7363  UIDE.md)|..|Disc
+000013f0: 6f72 647c 605f 4449 5343 4f52 445f 5745  ord|`_DISCORD_WE
+00001400: 4248 4f4f 4b5f 5552 4c60 7c46 7265 656d  BHOOK_URL`|Freem
+00001410: 6975 6d7c 4561 7379 7c31 6d69 6e7c 5b45  ium|Easy|1min|[E
+00001420: 7863 6570 7444 6973 636f 7264 5d28 6874  xceptDiscord](ht
+00001430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001440: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+00001450: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+00001460: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
+00001470: 2f45 7863 6570 7454 656c 6567 7261 6d2f  /ExceptTelegram/
+00001480: 4755 4944 452e 6d64 297c 0d0a 7c41 5753  GUIDE.md)|..|AWS
+00001490: 2043 6869 6d65 7c60 5f43 4849 4d45 5f57   Chime|`_CHIME_W
+000014a0: 4542 484f 4f4b 5f55 524c 607c 4672 6565  EBHOOK_URL`|Free
+000014b0: 6d69 756d 7c45 6173 797c 316d 696e 7c5b  mium|Easy|1min|[
+000014c0: 4578 6365 7074 4368 696d 655d 2868 7474  ExceptChime](htt
+000014d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000014e0: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+000014f0: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00001500: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+00001510: 4578 6365 7074 4368 696d 652f 4755 4944  ExceptChime/GUID
+00001520: 452e 6d64 297c 0d0a 7c53 6c61 636b 7c60  E.md)|..|Slack|`
+00001530: 5f53 4c41 434b 5f57 4542 484f 4f4b 5f55  _SLACK_WEBHOOK_U
+00001540: 524c 607c 4672 6565 6d69 756d 7c45 6173  RL`|Freemium|Eas
+00001550: 797c 336d 696e 7c5b 4578 6365 7074 536c  y|3min|[ExceptSl
+00001560: 6163 6b5d 2868 7474 7073 3a2f 2f67 6974  ack](https://git
+00001570: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00001580: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00001590: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+000015a0: 6375 6d65 6e74 732f 4578 6365 7074 536c  cuments/ExceptSl
+000015b0: 6163 6b2f 4755 4944 452e 6d64 297c 0d0a  ack/GUIDE.md)|..
+000015c0: 7c47 2d4d 6169 6c7c 605f 4741 4d49 4c5f  |G-Mail|`_GAMIL_
+000015d0: 5245 4349 5049 454e 545f 4144 4452 602c  RECIPIENT_ADDR`,
+000015e0: 2060 5f47 4d41 494c 5f53 454e 4445 525f   `_GMAIL_SENDER_
+000015f0: 4144 4452 602c 2060 5f47 4d41 494c 5f41  ADDR`, `_GMAIL_A
+00001600: 5050 5f50 4153 5357 4f52 445f 4f46 5f53  PP_PASSWORD_OF_S
+00001610: 454e 4445 5260 207c 5265 7374 7269 6374  ENDER` |Restrict
+00001620: 6564 2066 7265 657c 4d65 6469 756d 7c33  ed free|Medium|3
+00001630: 6d69 6e7c 5b45 7863 6570 744d 6169 6c5d  min|[ExceptMail]
+00001640: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001650: 636f 6d2f 6473 6461 6e69 656c 7061 726b  com/dsdanielpark
+00001660: 2f45 7863 6570 744e 6f74 6966 6965 722f  /ExceptNotifier/
+00001670: 626c 6f62 2f6d 6169 6e2f 646f 6375 6d65  blob/main/docume
+00001680: 6e74 732f 4578 6365 7074 4d61 696c 2f47  nts/ExceptMail/G
+00001690: 5549 4445 2e6d 6429 7c0d 0a7c 4c69 6e65  UIDE.md)|..|Line
+000016a0: 7c60 5f4c 494e 455f 4e4f 5449 4659 5f41  |`_LINE_NOTIFY_A
+000016b0: 5049 5f54 4f4b 454e 607c 4672 6565 6d69  PI_TOKEN`|Freemi
+000016c0: 756d 7c4d 6564 6975 6d7c 346d 696e 7c5b  um|Medium|4min|[
+000016d0: 4578 6365 7074 4c69 6e65 5d28 6874 7470  ExceptLine](http
+000016e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000016f0: 7364 616e 6965 6c70 6172 6b2f 4578 6365  sdanielpark/Exce
+00001700: 7074 4e6f 7469 6669 6572 2f62 6c6f 622f  ptNotifier/blob/
+00001710: 6d61 696e 2f64 6f63 756d 656e 7473 2f45  main/documents/E
+00001720: 7863 6570 744c 696e 652f 4755 4944 452e  xceptLine/GUIDE.
+00001730: 6d64 297c 0d0a 7c53 4d53 7c60 5f54 5749  md)|..|SMS|`_TWI
+00001740: 4c49 4f5f 5349 4460 2c20 605f 5457 494c  LIO_SID`, `_TWIL
+00001750: 494f 5f54 4f4b 454e 602c 2060 5f52 4543  IO_TOKEN`, `_REC
+00001760: 4950 4945 4e54 5f50 484f 4e45 5f4e 554d  IPIENT_PHONE_NUM
+00001770: 4245 5260 2c20 605f 5345 4e44 4552 5f50  BER`, `_SENDER_P
+00001780: 484f 4e45 5f4e 554d 4245 5260 7c4e 6f74  HONE_NUMBER`|Not
+00001790: 2066 7265 657c 4d65 6469 756d 7c35 6d69   free|Medium|5mi
+000017a0: 6e7c 5b45 7863 6570 7453 4d53 5d28 6874  n|[ExceptSMS](ht
+000017b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000017c0: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+000017d0: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+000017e0: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
+000017f0: 2f45 7863 6570 7453 4d53 2f47 5549 4445  /ExceptSMS/GUIDE
+00001800: 2e6d 6429 7c0d 0a7c 4d69 6372 6f73 6f66  .md)|..|Microsof
+00001810: 7420 5465 616d 737c 605f 5445 414d 535f  t Teams|`_TEAMS_
+00001820: 5745 4248 4f4f 4b5f 5552 4c60 7c4e 6f74  WEBHOOK_URL`|Not
+00001830: 2046 7265 657c 4d65 6469 756d 7c35 6d69   Free|Medium|5mi
+00001840: 6e7c 5b45 7863 6570 7454 6561 6d73 5d28  n|[ExceptTeams](
+00001850: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001860: 6f6d 2f64 7364 616e 6965 6c70 6172 6b2f  om/dsdanielpark/
+00001870: 4578 6365 7074 4e6f 7469 6669 6572 2f62  ExceptNotifier/b
+00001880: 6c6f 622f 6d61 696e 2f64 6f63 756d 656e  lob/main/documen
+00001890: 7473 2f45 7863 6570 7454 6561 6d73 2f47  ts/ExceptTeams/G
+000018a0: 5549 4445 2e6d 6429 7c0d 0a7c 4b61 6b61  UIDE.md)|..|Kaka
+000018b0: 6f54 616c 6b7c 605f 4b41 4b41 4f5f 544f  oTalk|`_KAKAO_TO
+000018c0: 4b45 4e5f 5041 5448 607c 4672 6565 6d69  KEN_PATH`|Freemi
+000018d0: 756d 7c48 656c 6c7c 3e3d 3130 6d69 6e28  um|Hell|>=10min(
+000018e0: 546f 6b65 6e20 7265 6672 6573 6865 7320  Token refreshes 
+000018f0: 6461 696c 7929 7c5b 4578 6365 7074 4b61  daily)|[ExceptKa
+00001900: 6b61 6f5d 2868 7474 7073 3a2f 2f67 6974  kao](https://git
+00001910: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00001920: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00001930: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+00001940: 6375 6d65 6e74 732f 4578 6365 7074 4b61  cuments/ExceptKa
+00001950: 6b61 6f2f 4755 4944 452e 6d64 297c 0d0a  kao/GUIDE.md)|..
+00001960: 0d0a 0d0a 4966 2079 6f75 2061 6464 2074  ....If you add t
+00001970: 6865 2066 6f6c 6c6f 7769 6e67 2074 776f  he following two
+00001980: 2076 6172 6961 626c 6573 2074 6f20 7468   variables to th
+00001990: 6520 7265 7175 6972 6564 2076 6172 6961  e required varia
+000019a0: 626c 6573 2066 6f72 2065 6163 6820 6170  bles for each ap
+000019b0: 706c 6963 6174 696f 6e20 696e 2074 6865  plication in the
+000019c0: 2074 6162 6c65 2061 626f 7665 2c20 796f   table above, yo
+000019d0: 7520 6361 6e20 7265 6365 6976 6520 6572  u can receive er
+000019e0: 726f 7220 6c6f 6361 7469 6f6e 2061 6e64  ror location and
+000019f0: 2065 7870 6c61 6e61 7469 6f6e 2c20 6173   explanation, as
+00001a00: 2077 656c 6c20 6173 2065 7861 6d70 6c65   well as example
+00001a10: 732c 2066 726f 6d20 4f70 656e 4149 2773  s, from OpenAI's
+00001a20: 206d 6f64 656c 0d0a 0d0a 7c20 4150 4920   model....| API 
+00001a30: 7c20 5265 7175 6972 6564 2056 6172 6961  | Required Varia
+00001a40: 626c 6573 207c 2046 7265 6520 6f72 2050  bles | Free or P
+00001a50: 6169 6420 7c20 4561 7365 206f 6620 5365  aid | Ease of Se
+00001a60: 7475 7020 7c20 5469 6d65 2052 6571 7569  tup | Time Requi
+00001a70: 7265 6420 666f 7220 5365 7475 707c 4775  red for Setup|Gu
+00001a80: 6964 6520 5475 746f 7269 616c 204c 696e  ide Tutorial Lin
+00001a90: 6b7c 0d0a 7c3a 2d2d 3a7c 3a2d 2d7c 3a2d  k|..|:--:|:--|:-
+00001aa0: 2d3a 7c3a 2d2d 3a7c 3a2d 2d3a 7c3a 2d2d  -:|:--:|:--:|:--
+00001ab0: 2d3a 7c0d 0a7c 204f 7065 6e41 4920 4150  -:|..| OpenAI AP
+00001ac0: 4920 7c60 5265 7175 6972 6564 2076 6172  I |`Required var
+00001ad0: 6961 626c 6573 2066 6f72 2065 6163 6820  iables for each 
+00001ae0: 6170 706c 6963 6174 696f 6e60 2b20 605f  application`+ `_
+00001af0: 4f50 454e 5f41 495f 4d4f 4445 4c60 2c60  OPEN_AI_MODEL`,`
+00001b00: 5f4f 5045 4e5f 4149 5f41 5049 607c 4e6f  _OPEN_AI_API`|No
+00001b10: 7420 6672 6565 7c45 6173 797c 326d 696e  t free|Easy|2min
+00001b20: 7c5b 4150 494f 7065 6e41 495d 2868 7474  |[APIOpenAI](htt
+00001b30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001b40: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+00001b50: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00001b60: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+00001b70: 4150 494f 7065 6e41 492f 4755 4944 452e  APIOpenAI/GUIDE.
+00001b80: 6d64 297c 0d0a 0d0a 0d0a 3c62 723e 3c62  md)|......<br><b
+00001b90: 723e 0d0a 0d0a 2320 312e 204b 6579 2046  r>....# 1. Key F
+00001ba0: 6561 7475 7265 730d 0a54 6f20 7573 6520  eatures..To use 
+00001bb0: 7468 6520 6465 7369 7265 6420 6170 706c  the desired appl
+00001bc0: 6963 6174 696f 6e2c 2079 6f75 206d 7573  ication, you mus
+00001bd0: 7420 6465 6669 6e65 2074 6865 206e 6563  t define the nec
+00001be0: 6573 7361 7279 2076 6172 6961 626c 6573  essary variables
+00001bf0: 2e20 456e 7375 7265 2074 6861 7420 7468  . Ensure that th
+00001c00: 6520 7661 7269 6162 6c65 206e 616d 6573  e variable names
+00001c10: 2072 656d 6169 6e20 756e 6368 616e 6765   remain unchange
+00001c20: 642c 2061 6e64 2079 6f75 2063 616e 2075  d, and you can u
+00001c30: 7365 2065 6974 6865 7220 6c6f 6361 6c20  se either local 
+00001c40: 6f72 2067 6c6f 6261 6c20 7661 7269 6162  or global variab
+00001c50: 6c65 732e 2049 6620 796f 7520 6172 6520  les. If you are 
+00001c60: 7573 696e 6720 6054 656c 6567 7261 6d60  using `Telegram`
+00001c70: 2c20 616e 2065 7861 6d70 6c65 2069 7320  , an example is 
+00001c80: 6174 7461 6368 6564 2061 7320 616e 2069  attached as an i
+00001c90: 6d61 6765 2e0d 0a0d 0a23 2320 312d 312e  mage.....## 1-1.
+00001ca0: 2045 7863 6570 7460 5b61 7070 4e61 6d65   Except`[appName
+00001cb0: 5d60 0d0a 4966 2079 6f75 2075 7365 2050  ]`..If you use P
+00001cc0: 7974 686f 6e27 7320 7472 7920 6578 6365  ython's try exce
+00001cd0: 7074 2073 7461 7465 6d65 6e74 2061 7320  pt statement as 
+00001ce0: 6974 2069 732c 2062 7574 2063 6861 6e67  it is, but chang
+00001cf0: 6520 6578 6365 7074 2061 7320 666f 6c6c  e except as foll
+00001d00: 6f77 732c 2079 6f75 2063 616e 2072 6563  ows, you can rec
+00001d10: 6569 7665 206e 6f74 6966 6963 6174 696f  eive notificatio
+00001d20: 6e73 2074 6872 6f75 6768 2079 6f75 7220  ns through your 
+00001d30: 6170 706c 6963 6174 696f 6e2e 0d0a 6060  application...``
+00001d40: 600d 0a45 7863 6570 7443 6869 6d65 2c20  `..ExceptChime, 
+00001d50: 4578 6365 7074 5465 6c65 6772 616d 2c20  ExceptTelegram, 
+00001d60: 4578 6365 7074 4469 7363 6f72 642c 2045  ExceptDiscord, E
+00001d70: 7863 6570 7453 4d53 2c20 4578 6365 7074  xceptSMS, Except
+00001d80: 4d61 696c 2c20 4578 6365 7074 4b61 6b61  Mail, ExceptKaka
+00001d90: 6f2c 2045 7863 6570 744c 696e 652c 2045  o, ExceptLine, E
+00001da0: 7863 6570 7453 6c61 636b 2c20 4578 6365  xceptSlack, Exce
+00001db0: 7074 5465 616d 732c 2045 7863 6570 7444  ptTeams, ExceptD
+00001dc0: 6573 6b74 6f70 652c 2045 7863 6570 7442  esktope, ExceptB
+00001dd0: 6565 700d 0a60 6060 0d0a 0d0a 2a45 7861  eep..```....*Exa
+00001de0: 6d70 6c65 2a0d 0a60 6060 7079 7468 6f6e  mple*..```python
+00001df0: 0d0a 6672 6f6d 2045 7863 6570 744e 6f74  ..from ExceptNot
+00001e00: 6966 6965 7220 696d 706f 7274 2045 7863  ifier import Exc
+00001e10: 6570 7454 656c 6765 7261 6d0d 0a5f 5445  eptTelgeram.._TE
+00001e20: 4c45 4752 414d 5f54 4f4b 454e 203d 2022  LEGRAM_TOKEN = "
+00001e30: 7878 7878 220d 0a0d 0a74 7279 3a0d 0a20  xxxx"....try:.. 
+00001e40: 2020 2070 7269 6e74 2831 2f30 290d 0a65     print(1/0)..e
+00001e50: 7863 6570 7420 4578 6365 7074 5465 6c65  xcept ExceptTele
+00001e60: 6772 616d 3a20 2020 2023 2073 656e 6469  gram:    # sendi
+00001e70: 6e67 2065 7863 6570 7420 6d65 7373 6167  ng except messag
+00001e80: 6520 746f 2074 656c 6567 7261 6d0d 0a20  e to telegram.. 
+00001e90: 2020 2073 7973 2e65 7869 7428 290d 0a60     sys.exit()..`
+00001ea0: 6060 0d0a 215b 5d28 6874 7470 733a 2f2f  ``..![](https://
+00001eb0: 6769 7468 7562 2e63 6f6d 2f64 7364 616e  github.com/dsdan
+00001ec0: 6965 6c70 6172 6b2f 4578 6365 7074 4e6f  ielpark/ExceptNo
+00001ed0: 7469 6669 6572 2f62 6c6f 622f 6d61 696e  tifier/blob/main
+00001ee0: 2f61 7373 6574 732f 696d 6773 2f65 7831  /assets/imgs/ex1
+00001ef0: 2e70 6e67 290d 0a0d 0a3c 6272 3e0d 0a0d  .png)....<br>...
+00001f00: 0a23 2320 312d 322e 2041 4920 4465 6262  .## 1-2. AI Debb
+00001f10: 7567 6769 6e67 2049 6e66 6f6d 6174 696f  ugging Infomatio
+00001f20: 6e20 4e6f 7469 6669 6361 7469 6f6e 0d0a  n Notification..
+00001f30: 596f 7520 6361 6e20 7265 6365 6976 6520  You can receive 
+00001f40: 6465 6275 6767 696e 6720 696e 666f 726d  debugging inform
+00001f50: 6174 696f 6e20 6672 6f6d 2043 6861 7447  ation from ChatG
+00001f60: 5054 2076 6961 204f 7065 6e41 4927 7320  PT via OpenAI's 
+00001f70: 4150 4920 7768 656e 2075 7369 6e67 2074  API when using t
+00001f80: 6865 2045 7863 6570 7420 7374 6174 656d  he Except statem
+00001f90: 656e 742e 2054 6865 2073 796e 7461 7820  ent. The syntax 
+00001fa0: 7265 6d61 696e 7320 7468 6520 7361 6d65  remains the same
+00001fb0: 2c20 6275 7420 796f 7527 6c6c 206e 6565  , but you'll nee
+00001fc0: 6420 746f 2063 6f6e 6669 6775 7265 2074  d to configure t
+00001fd0: 6865 7365 2074 776f 2076 6172 6961 626c  hese two variabl
+00001fe0: 6573 3a0d 0a60 5f4f 5045 4e5f 4149 5f4d  es:..`_OPEN_AI_M
+00001ff0: 4f44 454c 602c 605f 4f50 454e 5f41 495f  ODEL`,`_OPEN_AI_
+00002000: 4150 4960 0d0a 0d0a 2a45 7861 6d70 6c65  API`....*Example
+00002010: 2a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  *..```python..fr
+00002020: 6f6d 2045 7863 6570 744e 6f74 6966 6965  om ExceptNotifie
+00002030: 7220 696d 706f 7274 2045 7863 6570 7454  r import ExceptT
+00002040: 656c 6765 7261 6d0d 0a5f 5445 4c45 4752  elgeram.._TELEGR
+00002050: 414d 5f54 4f4b 454e 203d 2022 7878 7878  AM_TOKEN = "xxxx
+00002060: 220d 0a5f 4f50 454e 5f41 495f 4d4f 4445  ".._OPEN_AI_MODE
+00002070: 4c3d 2267 7074 2d33 2e35 2d74 7572 626f  L="gpt-3.5-turbo
+00002080: 220d 0a5f 4f50 454e 5f41 495f 4150 493d  ".._OPEN_AI_API=
+00002090: 2273 6b2d 7878 7878 7878 220d 0a0d 0a74  "sk-xxxxxx"....t
+000020a0: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
+000020b0: 2f30 290d 0a65 7863 6570 7420 4578 6365  /0)..except Exce
+000020c0: 7074 5465 6c65 6772 616d 3a20 2320 7365  ptTelegram: # se
+000020d0: 6e64 696e 6720 6d73 6720 5749 5448 2041  nding msg WITH A
+000020e0: 4920 4445 4255 4747 494e 4720 746f 2074  I DEBUGGING to t
+000020f0: 656c 6567 7261 6d0d 0a20 2020 2073 7973  elegram..    sys
+00002100: 2e65 7869 7428 290d 0a60 6060 0d0a 0d0a  .exit()..```....
+00002110: 215b 5d28 6874 7470 733a 2f2f 6769 7468  ![](https://gith
+00002120: 7562 2e63 6f6d 2f64 7364 616e 6965 6c70  ub.com/dsdanielp
+00002130: 6172 6b2f 4578 6365 7074 4e6f 7469 6669  ark/ExceptNotifi
+00002140: 6572 2f62 6c6f 622f 6d61 696e 2f61 7373  er/blob/main/ass
+00002150: 6574 732f 696d 6773 2f65 7832 2e70 6e67  ets/imgs/ex2.png
+00002160: 290d 0a0d 0a3c 6272 3e0d 0a0d 0a23 2320  )....<br>....## 
+00002170: 312d 332e 2053 7563 6365 7373 605b 6170  1-3. Success`[ap
+00002180: 704e 616d 655d 600d 0a42 7920 706c 6163  pName]`..By plac
+00002190: 696e 6720 7468 6520 7472 7920 6578 6365  ing the try exce
+000021a0: 7074 2069 6e20 7079 7468 6f6e 2061 7420  pt in python at 
+000021b0: 7468 6520 656e 6420 6f66 2074 6865 2074  the end of the t
+000021c0: 7279 2073 7461 7465 6d65 6e74 2c20 6170  ry statement, ap
+000021d0: 706c 6963 6174 696f 6e73 2063 616e 2062  plications can b
+000021e0: 6520 6e6f 7469 6669 6564 2074 6861 7420  e notified that 
+000021f0: 7468 6520 7472 7920 7374 6174 656d 656e  the try statemen
+00002200: 7420 776f 726b 6564 206e 6f72 6d61 6c6c  t worked normall
+00002210: 792e 0d0a 6060 600d 0a53 7563 6365 7373  y...```..Success
+00002220: 4368 696d 652c 2053 7563 6365 7373 5465  Chime, SuccessTe
+00002230: 6c65 6772 616d 2c20 5375 6363 6573 7344  legram, SuccessD
+00002240: 6973 636f 7264 2c20 5375 6363 6573 7353  iscord, SuccessS
+00002250: 4d53 2c20 5375 6363 6573 734d 6169 6c2c  MS, SuccessMail,
+00002260: 2053 7563 6365 7373 4b61 6b61 6f2c 2053   SuccessKakao, S
+00002270: 7563 6365 7373 4c69 6e65 2c20 5375 6363  uccessLine, Succ
+00002280: 6573 7353 6c61 636b 2c20 5375 6363 6573  essSlack, Succes
+00002290: 7354 6561 6d73 2c20 5375 6363 6573 7344  sTeams, SuccessD
+000022a0: 6573 6b74 6f70 652c 2053 7563 6365 7373  esktope, Success
+000022b0: 4265 6570 0d0a 6060 600d 0a2a 4578 616d  Beep..```..*Exam
+000022c0: 706c 652a 0d0a 0d0a 6060 6070 7974 686f  ple*....```pytho
+000022d0: 6e0d 0a66 726f 6d20 4578 6365 7074 4e6f  n..from ExceptNo
+000022e0: 7469 6669 6572 2069 6d70 6f72 7420 5375  tifier import Su
+000022f0: 6363 6573 7354 656c 6765 7261 6d0d 0a5f  ccessTelgeram.._
+00002300: 5445 4c45 4752 414d 5f54 4f4b 454e 203d  TELEGRAM_TOKEN =
+00002310: 2022 7878 7878 220d 0a0d 0a74 7279 3a0d   "xxxx"....try:.
+00002320: 0a20 2020 2070 7269 6e74 2831 2f32 3029  .    print(1/20)
+00002330: 0d0a 2020 2020 5375 6363 6573 7354 656c  ..    SuccessTel
+00002340: 6765 7261 6d28 292e 5f5f 6361 6c6c 5f5f  geram().__call__
+00002350: 2829 2020 2320 7365 6e64 696e 6720 7375  ()  # sending su
+00002360: 6363 6573 7320 6d65 7373 6167 6520 746f  ccess message to
+00002370: 2074 656c 6567 7261 6d0d 0a65 7863 6570   telegram..excep
+00002380: 743a 0d0a 2020 2020 7379 732e 6578 6974  t:..    sys.exit
+00002390: 2829 0d0a 6060 600d 0a0d 0a21 5b5d 2868  ()..```....![](h
+000023a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000023b0: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
+000023c0: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
+000023d0: 6f62 2f6d 6169 6e2f 6173 7365 7473 2f69  ob/main/assets/i
+000023e0: 6d67 732f 6578 332e 706e 6729 0d0a 0d0a  mgs/ex3.png)....
+000023f0: 3c42 723e 0d0a 0d0a 2323 2031 2d34 2e20  <Br>....## 1-4. 
+00002400: 5365 6e64 605b 6170 704e 616d 655d 600d  Send`[appName]`.
+00002410: 0a50 6c61 6365 2069 7420 616e 7977 6865  .Place it anywhe
+00002420: 7265 206f 6e20 7468 6520 6c69 6e65 206f  re on the line o
+00002430: 6620 636f 6465 2079 6f75 2077 616e 742c  f code you want,
+00002440: 2061 6e64 2079 6f75 276c 6c20 6265 206e   and you'll be n
+00002450: 6f74 6966 6965 6420 7768 656e 2074 6861  otified when tha
+00002460: 7420 6c69 6e65 206f 6620 636f 6465 2069  t line of code i
+00002470: 7320 7265 6163 6865 642e 0d0a 6060 600d  s reached...```.
+00002480: 0a53 656e 6443 6869 6d65 2c20 5365 6e64  .SendChime, Send
+00002490: 5465 6c65 6772 616d 2c20 5365 6e64 4469  Telegram, SendDi
+000024a0: 7363 6f72 642c 2053 656e 6453 4d53 2c20  scord, SendSMS, 
+000024b0: 5365 6e64 4d61 696c 2c20 5365 6e64 4b61  SendMail, SendKa
+000024c0: 6b61 6f2c 2053 656e 644c 696e 652c 2053  kao, SendLine, S
+000024d0: 656e 6453 6c61 636b 2c20 5365 6e64 5465  endSlack, SendTe
+000024e0: 616d 732c 2053 656e 6444 6573 6b74 6f70  ams, SendDesktop
+000024f0: 652c 2053 656e 6442 6565 700d 0a60 6060  e, SendBeep..```
+00002500: 0d0a 2a45 7861 6d70 6c65 2a0d 0a0d 0a60  ..*Example*....`
+00002510: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2045  ``python..from E
+00002520: 7863 6570 744e 6f74 6966 6965 7220 696d  xceptNotifier im
+00002530: 706f 7274 2053 656e 6454 656c 6765 7261  port SendTelgera
+00002540: 6d0d 0a5f 5445 4c45 4752 414d 5f54 4f4b  m.._TELEGRAM_TOK
+00002550: 454e 203d 2022 7878 7878 220d 0a0d 0a53  EN = "xxxx"....S
+00002560: 656e 6454 656c 6567 7261 6d28 292e 5f5f  endTelegram().__
+00002570: 6361 6c6c 5f5f 2829 2023 2073 656e 6469  call__() # sendi
+00002580: 6e67 206d 6573 7361 6765 2074 6f20 7465  ng message to te
+00002590: 6c65 6772 616d 0d0a 0d0a 6e6f 7469 203d  legram....noti =
+000025a0: 2053 656e 6454 656c 6567 7261 6d28 290d   SendTelegram().
+000025b0: 0a6e 6f74 6928 2920 2020 2020 2020 2020  .noti()         
+000025c0: 2020 2020 2020 2020 2020 2023 2073 656e             # sen
+000025d0: 6469 6e67 206d 6573 7361 6765 2074 6f20  ding message to 
+000025e0: 7465 6c65 6772 616d 0d0a 6060 600d 0a0d  telegram..```...
+000025f0: 0a21 5b5d 2868 7474 7073 3a2f 2f67 6974  .![](https://git
+00002600: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00002610: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00002620: 6965 722f 626c 6f62 2f6d 6169 6e2f 6173  ier/blob/main/as
+00002630: 7365 7473 2f69 6d67 732f 6578 342e 706e  sets/imgs/ex4.pn
+00002640: 6729 0d0a 0d0a 0d0a 3c62 723e 3c62 723e  g)......<br><br>
+00002650: 0d0a 0d0a 2320 322e 2046 6561 7475 7265  ....# 2. Feature
+00002660: 730d 0a59 6f75 2063 616e 2072 6563 6569  s..You can recei
+00002670: 7665 2064 6562 7567 6769 6e67 2069 6e66  ve debugging inf
+00002680: 6f72 6d61 7469 6f6e 2066 726f 6d20 4368  ormation from Ch
+00002690: 6174 4750 5420 7669 6120 4f70 656e 4149  atGPT via OpenAI
+000026a0: 2773 2041 5049 2077 6865 6e20 7573 696e  's API when usin
+000026b0: 6720 7468 6520 4578 6365 7074 2073 7461  g the Except sta
+000026c0: 7465 6d65 6e74 2e20 5468 6520 7379 6e74  tement. The synt
+000026d0: 6178 2072 656d 6169 6e73 2074 6865 2073  ax remains the s
+000026e0: 616d 652c 2062 7574 2079 6f75 276c 6c20  ame, but you'll 
+000026f0: 6e65 6564 2074 6f20 636f 6e66 6967 7572  need to configur
+00002700: 6520 7468 6573 6520 7477 6f20 7661 7269  e these two vari
+00002710: 6162 6c65 733a 0d0a 605f 4f50 454e 5f41  ables:..`_OPEN_A
+00002720: 495f 4d4f 4445 4c60 2c60 5f4f 5045 4e5f  I_MODEL`,`_OPEN_
+00002730: 4149 5f41 5049 600d 0a0d 0a0d 0a0d 0a23  AI_API`........#
+00002740: 2320 322d 312e 202a 5465 6c65 6772 616d  # 2-1. *Telegram
+00002750: 204e 6f74 6966 6965 722a 0d0a 0d0a 2d20   Notifier*....- 
+00002760: 612e 204f 7065 6e20 796f 7572 2074 656c  a. Open your tel
+00002770: 6567 7261 6d20 6170 7020 616e 6420 7365  egram app and se
+00002780: 6172 6368 2066 6f72 2042 6f74 4661 7468  arch for BotFath
+00002790: 6572 2e20 2841 2062 7569 6c74 2d69 6e20  er. (A built-in 
+000027a0: 5465 6c65 6772 616d 2062 6f74 2074 6861  Telegram bot tha
+000027b0: 7420 6865 6c70 7320 7573 6572 7320 6372  t helps users cr
+000027c0: 6561 7465 2063 7573 746f 6d20 5465 6c65  eate custom Tele
+000027d0: 6772 616d 2062 6f74 7329 203c 6272 3e0d  gram bots) <br>.
+000027e0: 0a2d 2062 2e20 5479 7065 202f 6e65 7762  .- b. Type /newb
+000027f0: 6f74 2074 6f20 6372 6561 7465 2061 206e  ot to create a n
+00002800: 6577 2062 6f74 203c 6272 3e0d 0a2d 2063  ew bot <br>..- c
+00002810: 2e20 4769 7665 2079 6f75 7220 626f 7420  . Give your bot 
+00002820: 6120 6e61 6d65 2026 2061 2075 7365 726e  a name & a usern
+00002830: 616d 6520 3c62 723e 0d0a 2d20 642e 2043  ame <br>..- d. C
+00002840: 6f70 7920 796f 7572 206e 6577 2054 656c  opy your new Tel
+00002850: 6567 7261 6d20 626f 74e2 8099 7320 746f  egram bot...s to
+00002860: 6b65 6e20 3c62 723e 0d0a 0d0a 466f 7220  ken <br>....For 
+00002870: 6d6f 7265 2069 6e66 6f6d 6174 696f 6e2c  more infomation,
+00002880: 2076 6973 6974 205b 5465 6c65 6772 616d   visit [Telegram
+00002890: 2042 6f74 2046 6174 6865 7220 4150 495d   Bot Father API]
+000028a0: 2868 7474 7073 3a2f 2f63 6f72 652e 7465  (https://core.te
+000028b0: 6c65 6772 616d 2e6f 7267 2f62 6f74 732f  legram.org/bots/
+000028c0: 6170 6929 0d0a 3c62 723e 3c62 723e 0d0a  api)..<br><br>..
+000028d0: 200d 0a23 2323 2061 2e20 5769 7468 6f75   ..### a. Withou
+000028e0: 7420 4f70 656e 4149 2041 5049 0d0a 0d0a  t OpenAI API....
+000028f0: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00002900: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
+00002910: 6d70 6f72 7420 4578 6365 7074 5465 6c65  mport ExceptTele
+00002920: 6772 616d 2c20 5375 6363 6573 7354 656c  gram, SuccessTel
+00002930: 6567 7261 6d2c 2053 656e 6454 656c 6567  egram, SendTeleg
+00002940: 7261 6d0d 0a69 6d70 6f72 7420 7379 730d  ram..import sys.
+00002950: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
+00002960: 3d20 4578 6365 7074 5465 6c65 6772 616d  = ExceptTelegram
+00002970: 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a5f 5445  .__call__...._TE
+00002980: 4c45 4752 414d 5f54 4f4b 454e 203d 2022  LEGRAM_TOKEN = "
+00002990: 7878 7878 220d 0a0d 0a74 7279 3a0d 0a20  xxxx"....try:.. 
+000029a0: 2020 2070 7269 6e74 2831 2f30 2920 200d     print(1/0)  .
+000029b0: 0a20 2020 2053 7563 6365 7373 5465 6c65  .    SuccessTele
+000029c0: 6772 616d 2829 2e5f 5f63 616c 6c5f 5f28  gram().__call__(
+000029d0: 2920 2331 2e20 7375 6363 6573 7320 7365  ) #1. success se
+000029e0: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
+000029f0: 0d0a 6578 6365 7074 2045 7863 6570 7454  ..except ExceptT
+00002a00: 656c 6567 7261 6d20 6173 2065 3a20 2020  elegram as e:   
+00002a10: 2020 2023 322e 2065 7863 6570 7420 7365     #2. except se
+00002a20: 6e64 6572 2020 2020 2020 2020 2020 2020  nder            
+00002a30: 0d0a 2020 2020 7379 732e 6578 6974 2829  ..    sys.exit()
+00002a40: 0d0a 0d0a 5365 6e64 5465 6c65 6772 616d  ....SendTelegram
+00002a50: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00002a60: 2020 2020 2023 332e 2063 7573 746f 6d69       #3. customi
+00002a70: 7a65 6420 7365 6e64 6572 2020 2020 200d  zed sender     .
+00002a80: 0a60 6060 0d0a 0d0a 0d0a 215b 5d28 6874  .```......![](ht
+00002a90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002aa0: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+00002ab0: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+00002ac0: 622f 6d61 696e 2f61 7373 6574 732f 696d  b/main/assets/im
+00002ad0: 6773 2f66 6967 3434 2e70 6e67 290d 0a0d  gs/fig44.png)...
+00002ae0: 0a0d 0a23 2323 2062 2e20 5769 7468 204f  ...### b. With O
+00002af0: 7065 6e41 4920 4150 490d 0a60 6060 7079  penAI API..```py
+00002b00: 7468 6f6e 0d0a 6672 6f6d 2045 7863 6570  thon..from Excep
+00002b10: 744e 6f74 6966 6965 7220 696d 706f 7274  tNotifier import
+00002b20: 2045 7863 6570 7454 656c 6567 7261 6d2c   ExceptTelegram,
+00002b30: 2053 7563 6365 7373 5465 6c65 6772 616d   SuccessTelegram
+00002b40: 2c20 5365 6e64 5465 6c65 6772 616d 0d0a  , SendTelegram..
+00002b50: 696d 706f 7274 2073 7973 0d0a 7379 732e  import sys..sys.
+00002b60: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
+00002b70: 6570 7454 656c 6567 7261 6d2e 5f5f 6361  eptTelegram.__ca
+00002b80: 6c6c 5f5f 0d0a 0d0a 5f54 454c 4547 5241  ll__...._TELEGRA
+00002b90: 4d5f 544f 4b45 4e20 3d20 2278 7878 7822  M_TOKEN = "xxxx"
+00002ba0: 0d0a 5f4f 5045 4e5f 4149 5f4d 4f44 454c  .._OPEN_AI_MODEL
+00002bb0: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
+00002bc0: 0d0a 5f4f 5045 4e5f 4149 5f41 5049 3d22  .._OPEN_AI_API="
+00002bd0: 736b 2d78 7878 7878 7822 0d0a 0d0a 7472  sk-xxxxxx"....tr
+00002be0: 793a 0d0a 2020 2020 7072 696e 7428 312f  y:..    print(1/
+00002bf0: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
+00002c00: 7354 656c 6567 7261 6d28 292e 5f5f 6361  sTelegram().__ca
+00002c10: 6c6c 5f5f 2829 2023 312e 2073 7563 6365  ll__() #1. succe
+00002c20: 7373 2073 656e 6465 7220 2020 2020 2020  ss sender       
+00002c30: 2020 200d 0a0d 0a65 7863 6570 7420 4578     ....except Ex
+00002c40: 6365 7074 5465 6c65 6772 616d 2061 7320  ceptTelegram as 
+00002c50: 653a 2020 2020 2020 2332 2e20 6578 6365  e:      #2. exce
+00002c60: 7074 2073 656e 6465 7220 2020 2020 2020  pt sender       
+00002c70: 2020 2020 200d 0a20 2020 2073 7973 2e65       ..    sys.e
+00002c80: 7869 7428 290d 0a0d 0a53 656e 6454 656c  xit()....SendTel
+00002c90: 6567 7261 6d28 292e 5f5f 6361 6c6c 5f5f  egram().__call__
+00002ca0: 2829 2020 2020 2020 2020 2333 2e20 6375  ()        #3. cu
+00002cb0: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
+00002cc0: 2020 2020 0d0a 0d0a 6060 600d 0a3c 6272      ....```..<br
+00002cd0: 3e0d 0a0d 0a23 2320 322d 322e 202a 4d61  >....## 2-2. *Ma
+00002ce0: 696c 204e 6f74 6966 6965 722a 0d0a 496e  il Notifier*..In
+00002cf0: 2074 6865 2065 7863 6570 7420 7374 6174   the except stat
+00002d00: 656d 656e 742c 2061 6e20 656d 6169 6c20  ement, an email 
+00002d10: 6973 2073 656e 7420 616c 6f6e 6720 7769  is sent along wi
+00002d20: 7468 2074 6865 2065 7272 6f72 206d 6573  th the error mes
+00002d30: 7361 6765 2e20 4164 6469 7469 6f6e 616c  sage. Additional
+00002d40: 6c79 2c20 796f 7520 6361 6e20 7365 6e64  ly, you can send
+00002d50: 2065 6d61 696c 7320 6672 6f6d 2061 6e79   emails from any
+00002d60: 2064 6573 6972 6564 206c 696e 652e 203c   desired line. <
+00002d70: 6272 3e0d 0a2d 2061 2e20 4c6f 6720 696e  br>..- a. Log in
+00002d80: 2077 6974 6820 7468 6520 7365 6e64 6572   with the sender
+00002d90: 2773 2065 6d61 696c 2049 442e 203c 6272  's email ID. <br
+00002da0: 3e0d 0a2d 2062 2e20 4f62 7461 696e 2061  >..- b. Obtain a
+00002db0: 6e20 6170 7020 7061 7373 776f 7264 2066  n app password f
+00002dc0: 6f72 2073 656e 6469 6e67 2047 6f6f 676c  or sending Googl
+00002dd0: 6520 4d61 696c 2061 7420 7468 6520 666f  e Mail at the fo
+00002de0: 6c6c 6f77 696e 6720 5b6c 696e 6b5d 2868  llowing [link](h
+00002df0: 7474 7073 3a2f 2f6d 7961 6363 6f75 6e74  ttps://myaccount
+00002e00: 2e67 6f6f 676c 652e 636f 6d2f 752f 332f  .google.com/u/3/
+00002e10: 6170 7070 6173 7377 6f72 6473 3f75 746d  apppasswords?utm
+00002e20: 5f73 6f75 7263 653d 676f 6f67 6c65 2d61  _source=google-a
+00002e30: 6363 6f75 6e74 2675 746d 5f6d 6564 6975  ccount&utm_mediu
+00002e40: 6d3d 6d79 6163 636f 756e 7473 6563 7572  m=myaccountsecur
+00002e50: 6974 7926 7574 6d5f 6361 6d70 6169 676e  ity&utm_campaign
+00002e60: 3d74 7376 2d73 6574 7469 6e67 7326 7261  =tsv-settings&ra
+00002e70: 7074 3d41 456a 484c 344e 3262 4d52 574f  pt=AEjHL4N2bMRWO
+00002e80: 3436 5661 4d70 5f6a 5030 367a 514b 3134  46VaMp_jP06zQK14
+00002e90: 4257 4e50 7636 366c 326f 3539 694a 3939  BWNPv66l2o59iJ99
+00002ea0: 436b 4f38 426a 596e 6d6f 5255 6539 6474  CkO8BjYnmoRUe9dt
+00002eb0: 5363 686b 6b62 7562 485a 4d55 6865 766b  SchkkbubHZMUhevk
+00002ec0: 416e 7756 4a52 4862 3979 674f 3361 6669  AnwVJRHb9ygO3afi
+00002ed0: 7370 4e6c 7729 206f 7220 5b67 6f6f 676c  spNlw) or [googl
+00002ee0: 6520 646f 6375 6d65 6e74 5d28 6874 7470  e document](http
+00002ef0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+00002f00: 6c65 2e63 6f6d 2f61 6363 6f75 6e74 732f  le.com/accounts/
+00002f10: 616e 7377 6572 2f31 3835 3833 333f 686c  answer/185833?hl
+00002f20: 3d65 6e29 2e20 0d0a 0d0a 6060 6070 7974  =en). ....```pyt
+00002f30: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00002f40: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00002f50: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+00002f60: 7074 4d61 696c 2c20 5375 6363 6573 734d  ptMail, SuccessM
+00002f70: 6169 6c2c 2053 656e 644d 6169 6c0d 0a73  ail, SendMail..s
+00002f80: 7973 2e65 7863 6570 7468 6f6f 6b20 3d20  ys.excepthook = 
+00002f90: 4578 6365 7074 4d61 696c 2e5f 5f63 616c  ExceptMail.__cal
+00002fa0: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+00002fb0: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00002fc0: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00002fd0: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00002fe0: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00002ff0: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00003000: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00003010: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00003020: 3d22 736b 2d78 7878 7878 7822 0d0a 5f47  ="sk-xxxxxx".._G
+00003030: 414d 494c 5f52 4543 4950 4945 4e54 5f41  AMIL_RECIPIENT_A
+00003040: 4444 5220 3d20 2778 7878 7878 7878 4067  DDR = 'xxxxxxx@g
+00003050: 6d61 696c 2e63 6f6d 270d 0a5f 474d 4149  mail.com'.._GMAI
+00003060: 4c5f 5345 4e44 4552 5f41 4444 5220 3d20  L_SENDER_ADDR = 
+00003070: 2779 7979 7979 7940 676d 6169 6c2e 636f  'yyyyyy@gmail.co
+00003080: 6d27 0d0a 5f47 4d41 494c 5f41 5050 5f50  m'.._GMAIL_APP_P
+00003090: 4153 5357 4f52 445f 4f46 5f53 454e 4445  ASSWORD_OF_SENDE
+000030a0: 5220 3d20 277a 7a7a 7a7a 7a27 0d0a 0d0a  R = 'zzzzzz'....
+000030b0: 7472 793a 0d0a 2020 2020 6d61 696e 2829  try:..    main()
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 2020 2020 2320 596f 7572 2043 6f64        # Your Cod
+000030e0: 6520 4865 7265 0d0a 2020 2020 5375 6363  e Here..    Succ
+000030f0: 6573 734d 6169 6c28 292e 5f5f 6361 6c6c  essMail().__call
+00003100: 5f5f 2829 2020 2020 2320 4e6f 2045 7863  __()    # No Exc
+00003110: 6570 7469 6f6e 202d 3e20 5365 6e64 2053  eption -> Send S
+00003120: 7563 6365 7373 206d 6169 6c2e 0d0a 6578  uccess mail...ex
+00003130: 6365 7074 2045 7863 6570 744d 6169 6c3a  cept ExceptMail:
+00003140: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003150: 4578 6365 7074 696f 6e20 2d3e 2053 656e  Exception -> Sen
+00003160: 6420 4661 696c 206d 6169 6c2e 0d0a 2020  d Fail mail...  
+00003170: 2020 7061 7373 0d0a 0d0a 5365 6e64 4d61    pass....SendMa
+00003180: 696c 2829 2e5f 5f63 616c 6c5f 5f28 2920  il().__call__() 
+00003190: 2020 2020 2020 2020 2020 2320 5768 656e            # When
+000031a0: 2050 726f 6365 7373 2045 6e64 6564 202d   Process Ended -
+000031b0: 3e20 416e 7920 4c69 6e65 206d 6169 6c2e  > Any Line mail.
+000031c0: 0d0a 6060 600d 0a0d 0a3c 6465 7461 696c  ..```....<detail
+000031d0: 733e 0d0a 3c73 756d 6d61 7279 3e20 5365  s>..<summary> Se
+000031e0: 6520 4578 616d 706c 652e 2e2e 3c2f 7375  e Example...</su
+000031f0: 6d6d 6172 793e 0d0a 0d0a 6060 6070 7974  mmary>....```pyt
+00003200: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00003210: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00003220: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+00003230: 7074 4d61 696c 2c20 5375 6363 6573 734d  ptMail, SuccessM
+00003240: 6169 6c2c 2053 656e 644d 6169 6c0d 0a0d  ail, SendMail...
+00003250: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
+00003260: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
+00003270: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
+00003280: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
+00003290: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
+000032a0: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
+000032b0: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
+000032c0: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
+000032d0: 7878 7878 7822 0d0a 5f47 414d 494c 5f52  xxxxx".._GAMIL_R
+000032e0: 4543 4950 4945 4e54 5f41 4444 5220 3d20  ECIPIENT_ADDR = 
+000032f0: 2778 7878 7878 7878 4067 6d61 696c 2e63  'xxxxxxx@gmail.c
+00003300: 6f6d 270d 0a5f 474d 4149 4c5f 5345 4e44  om'.._GMAIL_SEND
+00003310: 4552 5f41 4444 5220 3d20 2779 7979 7979  ER_ADDR = 'yyyyy
+00003320: 7940 676d 6169 6c2e 636f 6d27 0d0a 5f47  y@gmail.com'.._G
+00003330: 4d41 494c 5f41 5050 5f50 4153 5357 4f52  MAIL_APP_PASSWOR
+00003340: 445f 4f46 5f53 454e 4445 5220 3d20 277a  D_OF_SENDER = 'z
+00003350: 7a7a 7a7a 7a27 0d0a 0d0a 7379 732e 6578  zzzzz'....sys.ex
+00003360: 6365 7074 686f 6f6b 203d 2045 7863 6570  cepthook = Excep
+00003370: 744d 6169 6c2e 5f5f 6361 6c6c 5f5f 0d0a  tMail.__call__..
+00003380: 0d0a 7472 793a 0d0a 2020 2020 2320 3032  ..try:..    # 02
+00003390: 2e4c 6f63 6174 6520 796f 7572 2063 6f64  .Locate your cod
+000033a0: 650d 0a20 2020 2070 7269 6e74 2831 2f30  e..    print(1/0
+000033b0: 2920 2020 0d0a 2020 2020 5375 6363 6573  )   ..    Succes
+000033c0: 734d 6169 6c28 292e 5f5f 6361 6c6c 5f5f  sMail().__call__
+000033d0: 2829 2020 2023 2053 7563 6365 7373 204d  ()   # Success M
+000033e0: 6169 6c0d 0a0d 0a65 7863 6570 7420 4578  ail....except Ex
+000033f0: 6365 7074 4d61 696c 2061 7320 653a 2020  ceptMail as e:  
+00003400: 2020 2020 2020 2320 4578 6365 7074 696f        # Exceptio
+00003410: 6e20 4d61 696c 2020 2020 2020 200d 0a20  n Mail       .. 
+00003420: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
+00003430: 2020 2070 7269 6e74 2865 290d 0a0d 0a53     print(e)....S
+00003440: 656e 644d 6169 6c28 292e 5f5f 6361 6c6c  endMail().__call
+00003450: 5f5f 2829 2020 2020 2020 2020 2020 2320  __()          # 
+00003460: 5075 7420 416e 7920 4c69 6e65 3a20 5365  Put Any Line: Se
+00003470: 6e64 696e 6720 6d61 696c 0d0a 6060 600d  nding mail..```.
+00003480: 0a3c 2f64 6574 6169 6c73 3e0d 0a0d 0a3c  .</details>....<
+00003490: 6465 7461 696c 733e 0d0a 3c73 756d 6d61  details>..<summa
+000034a0: 7279 3e20 536e 6970 7065 7420 666f 7220  ry> Snippet for 
+000034b0: 5079 7468 6f6e 2064 6576 656c 6f70 6572  Python developer
+000034c0: 732e 2e2e 3c2f 7375 6d6d 6172 793e 0d0a  s...</summary>..
+000034d0: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
+000034e0: 6f72 7420 7379 730d 0a66 726f 6d20 4578  ort sys..from Ex
+000034f0: 6365 7074 4e6f 7469 6669 6572 2069 6d70  ceptNotifier imp
+00003500: 6f72 7420 4578 6365 7074 4d61 696c 2c20  ort ExceptMail, 
+00003510: 5375 6363 6573 734d 6169 6c2c 2053 656e  SuccessMail, Sen
+00003520: 644d 6169 6c0d 0a73 7973 2e65 7863 6570  dMail..sys.excep
+00003530: 7468 6f6f 6b20 3d20 4578 6365 7074 4d61  thook = ExceptMa
+00003540: 696c 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  il.__call__....#
+00003550: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00003560: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00003570: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00003580: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00003590: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+000035a0: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+000035b0: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+000035c0: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+000035d0: 7878 7822 0d0a 5f47 414d 494c 5f52 4543  xxx".._GAMIL_REC
+000035e0: 4950 4945 4e54 5f41 4444 5220 3d20 2778  IPIENT_ADDR = 'x
+000035f0: 7878 7878 7878 4067 6d61 696c 2e63 6f6d  xxxxxx@gmail.com
+00003600: 270d 0a5f 474d 4149 4c5f 5345 4e44 4552  '.._GMAIL_SENDER
+00003610: 5f41 4444 5220 3d20 2779 7979 7979 7940  _ADDR = 'yyyyyy@
+00003620: 676d 6169 6c2e 636f 6d27 0d0a 5f47 4d41  gmail.com'.._GMA
+00003630: 494c 5f41 5050 5f50 4153 5357 4f52 445f  IL_APP_PASSWORD_
+00003640: 4f46 5f53 454e 4445 5220 3d20 277a 7a7a  OF_SENDER = 'zzz
+00003650: 7a7a 7a27 0d0a 0d0a 7472 793a 0d0a 2020  zzz'....try:..  
+00003660: 2020 2779 6f75 7220 636f 6465 270d 0a20    'your code'.. 
+00003670: 2020 2053 7563 6365 7373 4d61 696c 2829     SuccessMail()
+00003680: 2e5f 5f63 616c 6c5f 5f28 290d 0a65 7863  .__call__()..exc
+00003690: 6570 7420 4578 6365 7074 4d61 696c 3a0d  ept ExceptMail:.
+000036a0: 0a20 2020 2070 6173 730d 0a0d 0a53 656e  .    pass....Sen
+000036b0: 644d 6169 6c28 292e 5f5f 6361 6c6c 5f5f  dMail().__call__
+000036c0: 2829 200d 0a60 6060 0d0a 3c2f 6465 7461  () ..```..</deta
+000036d0: 696c 733e 0d0a 0d0a 3c62 723e 0d0a 0d0a  ils>....<br>....
+000036e0: 2323 2032 2d33 2e20 2a44 6973 636f 7264  ## 2-3. *Discord
+000036f0: 204e 6f74 6966 6965 722a 0d0a 2d20 612e   Notifier*..- a.
+00003700: 2053 656c 6563 7420 7468 6520 6368 616e   Select the chan
+00003710: 6e65 6c20 746f 2072 6563 6569 7665 206e  nel to receive n
+00003720: 6f74 6966 6963 6174 696f 6e73 2e0d 0a2d  otifications...-
+00003730: 2062 2e20 436c 6963 6b20 2245 6469 7420   b. Click "Edit 
+00003740: 4368 616e 6e65 6c22 2069 6e20 7468 6520  Channel" in the 
+00003750: 7570 7065 7220 7269 6768 7420 636f 726e  upper right corn
+00003760: 6572 206f 6620 7468 6520 6368 6174 2077  er of the chat w
+00003770: 696e 646f 772e 0d0a 2d20 632e 2043 6c69  indow...- c. Cli
+00003780: 636b 2049 6e74 6567 7261 7469 6f6e 7320  ck Integrations 
+00003790: 2d20 5765 6268 6f6f 6b20 2d20 4e65 7720  - Webhook - New 
+000037a0: 5765 6268 6f6f 6b2e 0d0a 2d20 642e 2054  Webhook...- d. T
+000037b0: 6865 6e20 636c 6963 6b20 436f 7079 2057  hen click Copy W
+000037c0: 6562 686f 6f6b 2e0d 0a0d 0a60 6060 7079  ebhook.....```py
+000037d0: 7468 6f6e 0d0a 696d 706f 7274 2073 7973  thon..import sys
+000037e0: 0d0a 6672 6f6d 2045 7863 6570 744e 6f74  ..from ExceptNot
+000037f0: 6966 6965 7220 696d 706f 7274 2045 7863  ifier import Exc
+00003800: 6570 7444 6973 636f 7264 2c20 5375 6363  eptDiscord, Succ
+00003810: 6573 7344 6973 636f 7264 2c20 5365 6e64  essDiscord, Send
+00003820: 4469 7363 6f72 640d 0a73 7973 2e65 7863  Discord..sys.exc
+00003830: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
+00003840: 4469 7363 6f72 642e 5f5f 6361 6c6c 5f5f  Discord.__call__
+00003850: 0d0a 0d0a 2320 4465 6669 6e65 2074 6865  ....# Define the
+00003860: 206e 6578 7420 7477 6f20 7661 7269 6162   next two variab
+00003870: 6c65 7320 6f70 7469 6f6e 616c 6c79 2077  les optionally w
+00003880: 6865 6e20 7573 696e 6720 4f70 656e 4149  hen using OpenAI
+00003890: 2773 2041 5049 2e0d 0a23 205f 4f50 454e  's API...# _OPEN
+000038a0: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
+000038b0: 2e35 2d74 7572 626f 2220 2020 200d 0a23  .5-turbo"    ..#
+000038c0: 205f 4f50 454e 5f41 495f 4150 493d 2273   _OPEN_AI_API="s
+000038d0: 6b2d 7878 7878 7878 220d 0a5f 4449 5343  k-xxxxxx".._DISC
+000038e0: 4f52 445f 5745 4248 4f4f 4b5f 5552 4c20  ORD_WEBHOOK_URL 
+000038f0: 3d20 2278 7878 7878 7878 7878 7878 7878  = "xxxxxxxxxxxxx
+00003900: 7878 7878 220d 0a0d 0a0d 0a74 7279 3a0d  xxxx"......try:.
+00003910: 0a20 2020 2070 7269 6e74 2831 2f32 3029  .    print(1/20)
+00003920: 2020 0d0a 2020 2020 5375 6363 6573 7344    ..    SuccessD
+00003930: 6973 636f 7264 2829 2e5f 5f63 616c 6c5f  iscord().__call_
+00003940: 5f28 2920 2331 2073 7563 6365 7373 2073  _() #1 success s
+00003950: 656e 6465 7220 2020 2020 2020 2020 200d  ender          .
+00003960: 0a65 7863 6570 7420 4578 6365 7074 4469  .except ExceptDi
+00003970: 7363 6f72 6420 6173 2065 3a20 2020 2020  scord as e:     
+00003980: 2023 3220 6578 6365 7074 2073 656e 6465   #2 except sende
+00003990: 7220 2020 2020 2020 2020 2020 200d 0a20  r            .. 
+000039a0: 2020 2073 7973 2e65 7869 7428 290d 0a0d     sys.exit()...
+000039b0: 0a53 656e 6444 6973 636f 7264 2829 2e5f  .SendDiscord()._
+000039c0: 5f63 616c 6c5f 5f28 2920 2020 2020 2020  _call__()       
+000039d0: 2023 3320 6375 7374 6f6d 697a 6564 2073   #3 customized s
+000039e0: 656e 6465 7220 2020 2020 2020 0d0a 6060  ender       ..``
+000039f0: 600d 0a0d 0a3c 6272 3e0d 0a0d 0a23 2320  `....<br>....## 
+00003a00: 322d 342e 202a 4368 696d 6520 4e6f 7469  2-4. *Chime Noti
+00003a10: 6669 6572 2a0d 0a2d 2061 2e20 5365 6c65  fier*..- a. Sele
+00003a20: 6374 2074 6865 2043 6861 7420 726f 6f6d  ct the Chat room
+00003a30: 2074 6f20 7265 6365 6976 6520 6e6f 7469   to receive noti
+00003a40: 6669 6361 7469 6f6e 732e 0d0a 2d20 622e  fications...- b.
+00003a50: 2043 6c69 636b 2022 526f 6f6d 2053 6574   Click "Room Set
+00003a60: 7469 6e67 2220 696e 2074 6865 2075 7070  ting" in the upp
+00003a70: 6572 2072 6967 6874 2063 6f72 6e65 722e  er right corner.
+00003a80: 0d0a 2d20 632e 2043 6c69 636b 2022 4d61  ..- c. Click "Ma
+00003a90: 6e61 6765 2057 6562 686f 6f6b 2061 6e64  nage Webhook and
+00003aa0: 2062 6f74 2e22 0d0a 2d20 642e 2043 7265   bot."..- d. Cre
+00003ab0: 6174 6520 4164 6420 5765 6268 6f6f 6b2c  ate Add Webhook,
+00003ac0: 2073 6574 2069 7420 7570 2c20 7468 656e   set it up, then
+00003ad0: 2063 6c69 636b 2043 6f70 7920 5765 6268   click Copy Webh
+00003ae0: 6f6f 6b2e 0d0a 6060 6070 7974 686f 6e0d  ook...```python.
+00003af0: 0a69 6d70 6f72 7420 7379 730d 0a66 726f  .import sys..fro
+00003b00: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
+00003b10: 2069 6d70 6f72 7420 5375 6363 6573 7343   import SuccessC
+00003b20: 6869 6d65 2c20 4578 6365 7074 4368 696d  hime, ExceptChim
+00003b30: 652c 2053 656e 6443 6869 6d65 0d0a 7379  e, SendChime..sy
+00003b40: 732e 6578 6365 7074 686f 6f6b 203d 2045  s.excepthook = E
+00003b50: 7863 6570 7443 6869 6d65 2e5f 5f63 616c  xceptChime.__cal
+00003b60: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+00003b70: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00003b80: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00003b90: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00003ba0: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00003bb0: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00003bc0: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00003bd0: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00003be0: 3d22 736b 2d78 7878 7878 7822 0d0a 5f43  ="sk-xxxxxx".._C
+00003bf0: 4849 4d45 5f57 4542 484f 4f4b 5f55 524c  HIME_WEBHOOK_URL
+00003c00: 203d 2022 7878 7878 7878 7878 7878 7878   = "xxxxxxxxxxxx
+00003c10: 7878 7878 7878 220d 0a0d 0a0d 0a74 7279  xxxxxx"......try
+00003c20: 3a0d 0a20 2020 2070 7269 6e74 2831 2f30  :..    print(1/0
+00003c30: 2920 200d 0a20 2020 2053 7563 6365 7373  )  ..    Success
+00003c40: 4368 696d 6528 292e 5f5f 6361 6c6c 5f5f  Chime().__call__
+00003c50: 2829 2023 3120 7375 6363 6573 7320 7365  () #1 success se
+00003c60: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
+00003c70: 6578 6365 7074 2045 7863 6570 7443 6869  except ExceptChi
+00003c80: 6d65 2061 7320 653a 2020 2020 2020 2332  me as e:      #2
+00003c90: 2065 7863 6570 7420 7365 6e64 6572 2020   except sender  
+00003ca0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00003cb0: 7379 732e 6578 6974 2829 0d0a 0d0a 5365  sys.exit()....Se
+00003cc0: 6e64 4368 696d 6528 292e 5f5f 6361 6c6c  ndChime().__call
+00003cd0: 5f5f 2829 2020 2020 2020 2020 2333 2063  __()        #3 c
+00003ce0: 7573 746f 6d69 7a65 6420 7365 6e64 6572  ustomized sender
+00003cf0: 2020 2020 2020 200d 0a60 6060 0d0a 3c62         ..```..<b
+00003d00: 723e 0d0a 0d0a 2323 2032 2d35 2e20 2a53  r>....## 2-5. *S
+00003d10: 6c61 636b 204e 6f74 6966 6965 722a 0d0a  lack Notifier*..
+00003d20: 2d20 612e 2076 6973 6974 2068 7474 7073  - a. visit https
+00003d30: 3a2f 2f61 7069 2e73 6c61 636b 2e63 6f6d  ://api.slack.com
+00003d40: 2f0d 0a2d 2062 2e20 6043 7265 6174 6520  /..- b. `Create 
+00003d50: 616e 2061 7070 6020 2d20 6046 726f 6d20  an app` - `From 
+00003d60: 7363 7261 7463 6860 202d 2060 4372 6561  scratch` - `Crea
+00003d70: 7465 2041 7070 600d 0a2d 2063 2e20 4164  te App`..- c. Ad
+00003d80: 6420 7765 6268 6f6f 6b3a 2043 6c69 636b  d webhook: Click
+00003d90: 2060 496e 636f 6d69 6e67 2057 6562 686f   `Incoming Webho
+00003da0: 6f6b 7360 202d 2041 6374 6976 6174 6520  oks` - Activate 
+00003db0: 496e 636f 6d6d 696e 6720 604f 6e60 202d  Incomming `On` -
+00003dc0: 2041 6464 204e 6577 2057 6562 686f 6f6b   Add New Webhook
+00003dd0: 2074 6f20 576f 726b 7370 6163 650d 0a2d   to Workspace..-
+00003de0: 2064 2e20 436f 7079 2060 5765 6268 6f6f   d. Copy `Webhoo
+00003df0: 6b20 5552 4c60 0d0a 0d0a 6060 6070 7974  k URL`....```pyt
+00003e00: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00003e10: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00003e20: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+00003e30: 7074 536c 6163 6b2c 2053 7563 6365 7373  ptSlack, Success
+00003e40: 536c 6361 6b2c 2053 656e 6453 6c61 636b  Slcak, SendSlack
+00003e50: 0d0a 7379 732e 6578 6365 7074 686f 6f6b  ..sys.excepthook
+00003e60: 203d 2045 7863 6570 7453 6c61 636b 2e5f   = ExceptSlack._
+00003e70: 5f63 616c 6c5f 5f0d 0a0d 0a23 2044 6566  _call__....# Def
+00003e80: 696e 6520 7468 6520 6e65 7874 2074 776f  ine the next two
+00003e90: 2076 6172 6961 626c 6573 206f 7074 696f   variables optio
+00003ea0: 6e61 6c6c 7920 7768 656e 2075 7369 6e67  nally when using
+00003eb0: 204f 7065 6e41 4927 7320 4150 492e 0d0a   OpenAI's API...
+00003ec0: 2320 5f4f 5045 4e5f 4149 5f4d 4f44 454c  # _OPEN_AI_MODEL
+00003ed0: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
+00003ee0: 2020 2020 0d0a 2320 5f4f 5045 4e5f 4149      ..# _OPEN_AI
+00003ef0: 5f41 5049 3d22 736b 2d78 7878 7878 7822  _API="sk-xxxxxx"
+00003f00: 0d0a 5f53 4c41 434b 5f57 4542 484f 4f4b  .._SLACK_WEBHOOK
+00003f10: 5f55 524c 203d 2027 6874 7470 733a 2f2f  _URL = 'https://
+00003f20: 686f 6f6b 732e 736c 6163 6b2e 636f 6d2f  hooks.slack.com/
+00003f30: 7365 7276 6963 6573 2f78 7878 7878 7878  services/xxxxxxx
+00003f40: 7878 7878 7878 7878 7878 7878 270d 0a0d  xxxxxxxxxxxx'...
+00003f50: 0a74 7279 3a0d 0a20 2020 2070 7269 6e74  .try:..    print
+00003f60: 2831 2f30 2920 200d 0a20 2020 2053 7563  (1/0)  ..    Suc
+00003f70: 6365 7373 536c 6361 6b28 292e 5f5f 6361  cessSlcak().__ca
+00003f80: 6c6c 5f5f 2829 2023 3120 7375 6363 6573  ll__() #1 succes
+00003f90: 7320 7365 6e64 6572 2020 2020 2020 2020  s sender        
+00003fa0: 2020 0d0a 6578 6365 7074 2045 7863 6570    ..except Excep
+00003fb0: 7453 6c61 636b 2061 7320 653a 2020 2020  tSlack as e:    
+00003fc0: 2020 2332 2065 7863 6570 7420 7365 6e64    #2 except send
+00003fd0: 6572 2020 2020 2020 2020 2020 2020 0d0a  er            ..
+00003fe0: 2020 2020 7379 732e 6578 6974 2829 0d0a      sys.exit()..
+00003ff0: 0d0a 5365 6e64 536c 6163 6b28 292e 5f5f  ..SendSlack().__
+00004000: 6361 6c6c 5f5f 2829 2020 2020 2020 2020  call__()        
+00004010: 2333 2063 7573 746f 6d69 7a65 6420 7365  #3 customized se
+00004020: 6e64 6572 2020 2020 200d 0a60 6060 0d0a  nder     ..```..
+00004030: 3c42 723e 0d0a 0d0a 2323 2032 2d36 2e20  <Br>....## 2-6. 
+00004040: 2a4c 696e 6520 4e6f 7469 6669 6572 2a0d  *Line Notifier*.
+00004050: 0a2d 2061 2e20 5265 6769 7374 6572 205b  .- a. Register [
+00004060: 6874 7470 733a 2f2f 6e6f 7469 6679 2d62  https://notify-b
+00004070: 6f74 2e6c 696e 652e 6d65 2f5d 2868 7474  ot.line.me/](htt
+00004080: 7073 3a2f 2f6e 6f74 6966 792d 626f 742e  ps://notify-bot.
+00004090: 6c69 6e65 2e6d 652f 290d 0a2d 2062 2e20  line.me/)..- b. 
+000040a0: 476f 2074 6f20 6d79 7061 6765 205b 6874  Go to mypage [ht
+000040b0: 7470 733a 2f2f 6e6f 7469 6679 2d62 6f74  tps://notify-bot
+000040c0: 2e6c 696e 652e 6d65 2f6d 792f 5d28 6874  .line.me/my/](ht
+000040d0: 7470 733a 2f2f 6e6f 7469 6679 2d62 6f74  tps://notify-bot
+000040e0: 2e6c 696e 652e 6d65 2f6d 792f 290d 0a2d  .line.me/my/)..-
+000040f0: 2063 2e20 436c 6963 6b20 6047 656e 6572   c. Click `Gener
+00004100: 6174 6520 546f 6b65 6e60 2c20 656e 7465  ate Token`, ente
+00004110: 7220 5365 7276 6963 6520 4e61 6d65 2061  r Service Name a
+00004120: 6e64 2063 6c69 636b 2060 312d 6f6e 2d31  nd click `1-on-1
+00004130: 2063 6861 7420 7769 7468 204c 494e 4560   chat with LINE`
+00004140: 2028 616e 7974 6869 6e67 2079 6f75 206c   (anything you l
+00004150: 696b 6529 0d0a 2d20 642e 2043 6f70 7920  ike)..- d. Copy 
+00004160: 546f 6b65 6e2e 0d0a 0d0a 6060 6070 7974  Token.....```pyt
+00004170: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00004180: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00004190: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+000041a0: 7074 4c69 6e65 2c20 5375 6363 6573 734c  ptLine, SuccessL
+000041b0: 696e 652c 2053 656e 644c 696e 650d 0a73  ine, SendLine..s
+000041c0: 7973 2e65 7863 6570 7468 6f6f 6b20 3d20  ys.excepthook = 
+000041d0: 4578 6365 7074 4c69 6e65 2e5f 5f63 616c  ExceptLine.__cal
+000041e0: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+000041f0: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00004200: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00004210: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00004220: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00004230: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00004240: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00004250: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00004260: 3d22 736b 2d78 7878 7878 7822 0d0a 5f4c  ="sk-xxxxxx".._L
+00004270: 494e 455f 4e4f 5449 4659 5f41 5049 5f54  INE_NOTIFY_API_T
+00004280: 4f4b 454e 203d 2027 7878 7878 7878 7878  OKEN = 'xxxxxxxx
+00004290: 7878 7827 0d0a 0d0a 7472 793a 0d0a 2020  xxx'....try:..  
+000042a0: 2020 7072 696e 7428 312f 3230 2920 200d    print(1/20)  .
+000042b0: 0a20 2020 2053 7563 6365 7373 4c69 6e65  .    SuccessLine
+000042c0: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2331  ().__call__() #1
+000042d0: 2073 7563 6365 7373 2073 656e 6465 7220   success sender 
+000042e0: 2020 2020 2020 2020 200d 0a65 7863 6570           ..excep
+000042f0: 7420 4578 6365 7074 4c69 6e65 2061 7320  t ExceptLine as 
+00004300: 653a 2020 2020 2020 2332 2065 7863 6570  e:      #2 excep
+00004310: 7420 7365 6e64 6572 2020 2020 2020 2020  t sender        
+00004320: 2020 2020 0d0a 2020 2020 7379 732e 6578      ..    sys.ex
+00004330: 6974 2829 0d0a 0d0a 5365 6e64 4c69 6e65  it()....SendLine
+00004340: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00004350: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
+00004360: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
+00004370: 2020 200d 0a60 6060 0d0a 0d0a 3c42 723e     ..```....<Br>
+00004380: 0d0a 0d0a 2323 2032 2d37 2e20 2a53 4d53  ....## 2-7. *SMS
+00004390: 204e 6f74 6966 6965 722a 0d0a 2d20 612e   Notifier*..- a.
+000043a0: 2053 6967 6e20 7570 2066 6f72 2054 7769   Sign up for Twi
+000043b0: 6c69 6f2e 205b 6874 7470 733a 2f2f 7777  lio. [https://ww
+000043c0: 772e 7477 696c 696f 2e63 6f6d 2f65 6e2d  w.twilio.com/en-
+000043d0: 7573 5d28 6874 7470 733a 2f2f 7777 772e  us](https://www.
+000043e0: 7477 696c 696f 2e63 6f6d 2f65 6e2d 7573  twilio.com/en-us
+000043f0: 290d 0a2d 2062 2e20 436c 6963 6b20 436f  )..- b. Click Co
+00004400: 6e73 6f6c 6520 696e 2074 6865 2075 7070  nsole in the upp
+00004410: 6572 2072 6967 6874 2063 6f72 6e65 722e  er right corner.
+00004420: 0d0a 2d20 632e 2043 6f70 7920 7468 6520  ..- c. Copy the 
+00004430: 7661 7269 6162 6c65 7320 7072 6f76 6964  variables provid
+00004440: 6564 2069 6e20 7468 6520 636f 6e73 6f6c  ed in the consol
+00004450: 652e 0d0a 0d0a 6060 6070 7974 686f 6e0d  e.....```python.
+00004460: 0a69 6d70 6f72 7420 7379 730d 0a66 726f  .import sys..fro
+00004470: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
+00004480: 2069 6d70 6f72 7420 4578 6365 7074 534d   import ExceptSM
+00004490: 532c 2053 7563 6365 7373 534d 532c 2053  S, SuccessSMS, S
+000044a0: 656e 6453 4d53 0d0a 7379 732e 6578 6365  endSMS..sys.exce
+000044b0: 7074 686f 6f6b 203d 2045 7863 6570 7453  pthook = ExceptS
+000044c0: 4d53 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  MS.__call__....#
+000044d0: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+000044e0: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+000044f0: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00004500: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00004510: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+00004520: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+00004530: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+00004540: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+00004550: 7878 7822 0d0a 5f54 5749 4c49 4f5f 5349  xxx".._TWILIO_SI
+00004560: 4420 3d20 2778 7878 7827 0d0a 5f54 5749  D = 'xxxx'.._TWI
+00004570: 4c49 4f5f 544f 4b45 4e20 3d20 2779 7979  LIO_TOKEN = 'yyy
+00004580: 7979 7927 0d0a 5f52 4543 4950 4945 4e54  yyy'.._RECIPIENT
+00004590: 5f50 484f 4e45 5f4e 554d 4245 523d 222b  _PHONE_NUMBER="+
+000045a0: 6161 6161 6161 222c 0d0a 5f53 454e 4445  aaaaaa",.._SENDE
+000045b0: 525f 5048 4f4e 455f 4e55 4d42 4552 3d22  R_PHONE_NUMBER="
+000045c0: 2b62 6262 6262 6222 2c20 200d 0a0d 0a74  +bbbbbb",  ....t
+000045d0: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
+000045e0: 2f31 3029 2020 0d0a 2020 2020 5375 6363  /10)  ..    Succ
+000045f0: 6573 7353 4d53 2829 2e5f 5f63 616c 6c5f  essSMS().__call_
+00004600: 5f28 2920 2331 2073 7563 6365 7373 2073  _() #1 success s
+00004610: 656e 6465 7220 2020 2020 2020 2020 200d  ender          .
+00004620: 0a65 7863 6570 7420 4578 6365 7074 534d  .except ExceptSM
+00004630: 5320 6173 2065 3a20 2020 2020 2023 3220  S as e:      #2 
+00004640: 6578 6365 7074 2073 656e 6465 720d 0a20  except sender.. 
+00004650: 2020 2073 7973 2e65 7869 7428 290d 0a0d     sys.exit()...
+00004660: 0a53 656e 6453 4d53 2829 2e5f 5f63 616c  .SendSMS().__cal
+00004670: 6c5f 5f28 2920 2020 2020 2020 2023 3320  l__()        #3 
+00004680: 6375 7374 6f6d 697a 6564 2073 656e 6465  customized sende
+00004690: 7220 2020 2020 2020 200d 0a60 6060 0d0a  r        ..```..
+000046a0: 3c42 723e 0d0a 0d0a 2323 2032 2d38 2e20  <Br>....## 2-8. 
+000046b0: 2a54 6561 6d73 204e 6f74 6966 6965 722a  *Teams Notifier*
+000046c0: 0d0a 2d20 612e 2043 7265 6174 6520 7468  ..- a. Create th
+000046d0: 6520 6368 616e 6e65 6c20 7468 6174 2079  e channel that y
+000046e0: 6f75 2077 616e 7420 746f 206e 6f74 6966  ou want to notif
+000046f0: 792e 0d0a 2d20 622e 2041 7070 202d 2053  y...- b. App - S
+00004700: 6561 7263 683a 2077 6562 686f 6f6b 202d  earch: webhook -
+00004710: 2049 6e63 6f6d 696e 6720 5765 6268 6f6f   Incoming Webhoo
+00004720: 6b20 5b68 7474 7073 3a2f 2f74 6561 6d73  k [https://teams
+00004730: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6c  .microsoft.com/l
+00004740: 2f61 7070 2f32 3033 6131 6532 632d 3236  /app/203a1e2c-26
+00004750: 6363 2d34 3763 612d 3833 6165 2d62 6539  cc-47ca-83ae-be9
+00004760: 3866 3936 3062 3662 323f 736f 7572 6365  8f960b6b2?source
+00004770: 3d61 7070 2d64 6574 6169 6c73 2d64 6961  =app-details-dia
+00004780: 6c6f 675d 2868 7474 7073 3a2f 2f74 6561  log](https://tea
+00004790: 6d73 2e6d 6963 726f 736f 6674 2e63 6f6d  ms.microsoft.com
+000047a0: 2f6c 2f61 7070 2f32 3033 6131 6532 632d  /l/app/203a1e2c-
+000047b0: 3236 6363 2d34 3763 612d 3833 6165 2d62  26cc-47ca-83ae-b
+000047c0: 6539 3866 3936 3062 3662 323f 736f 7572  e98f960b6b2?sour
+000047d0: 6365 3d61 7070 2d64 6574 6169 6c73 2d64  ce=app-details-d
+000047e0: 6961 6c6f 6729 0d0a 2d20 632e 2043 6c69  ialog)..- c. Cli
+000047f0: 636b 2060 5265 7175 6573 7420 4170 7072  ck `Request Appr
+00004800: 6f76 616c 6020 3c62 723e 0d0a 4166 7465  oval` <br>..Afte
+00004810: 7220 796f 7520 6361 6e20 7573 6520 7765  r you can use we
+00004820: 6268 6f6f 6b20 696e 636f 6d6d 696e 672e  bhook incomming.
+00004830: 2050 726f 6365 6564 2074 6f20 6e65 7874   Proceed to next
+00004840: 2073 7465 7073 2e0d 0a4d 6963 726f 736f   steps...Microso
+00004850: 6674 2054 6561 6d73 2061 6c6c 6f77 7320  ft Teams allows 
+00004860: 6c69 6d69 7465 6420 6170 706c 6963 6174  limited applicat
+00004870: 696f 6e20 6163 6365 7373 2070 6572 206f  ion access per o
+00004880: 7267 616e 697a 6174 696f 6e2c 2073 6f20  rganization, so 
+00004890: 6974 2063 616e 206f 6e6c 7920 6265 2075  it can only be u
+000048a0: 7365 6420 6966 2074 6865 2077 6562 686f  sed if the webho
+000048b0: 6f6b 2069 6e63 6f6d 696e 6720 6170 706c  ok incoming appl
+000048c0: 6963 6174 696f 6e20 6973 2061 7661 696c  ication is avail
+000048d0: 6162 6c65 2e0d 0a2d 2063 2e20 476f 2074  able...- c. Go t
+000048e0: 6f20 7468 6520 7465 616d 2063 6861 6e6e  o the team chann
+000048f0: 656c 2074 6f20 7265 6365 6976 6520 6e6f  el to receive no
+00004900: 7469 6669 6361 7469 6f6e 732c 2061 6e64  tifications, and
+00004910: 2063 6c69 636b 2060 436f 6e6e 6563 746f   click `Connecto
+00004920: 7273 6020 696e 2053 6574 7469 6e67 732e  rs` in Settings.
+00004930: 0d0a 2d20 642e 2060 436f 6e6e 6563 746f  ..- d. `Connecto
+00004940: 7273 6020 4166 7465 7220 636f 6e66 6967  rs` After config
+00004950: 7572 696e 6720 7765 6268 6f6f 6b20 696e  uring webhook in
+00004960: 636f 6d69 6e67 2069 6e20 436f 6e6e 6563  coming in Connec
+00004970: 746f 722c 2063 6f70 7920 7468 6520 7765  tor, copy the we
+00004980: 6268 6f6f 6b20 5552 4c2e 0d0a 0d0a 6060  bhook URL.....``
+00004990: 6070 7974 686f 6e0d 0a69 6d70 6f72 7420  `python..import 
+000049a0: 7379 730d 0a66 726f 6d20 4578 6365 7074  sys..from Except
+000049b0: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
+000049c0: 4578 6365 7074 5465 616d 732c 2053 7563  ExceptTeams, Suc
+000049d0: 6365 7373 5465 616d 732c 2053 656e 6454  cessTeams, SendT
+000049e0: 6561 6d73 0d0a 7379 732e 6578 6365 7074  eams..sys.except
+000049f0: 686f 6f6b 203d 2045 7863 6570 7454 6561  hook = ExceptTea
+00004a00: 6d73 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  ms.__call__....#
+00004a10: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00004a20: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00004a30: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00004a40: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00004a50: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+00004a60: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+00004a70: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+00004a80: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+00004a90: 7878 7822 0d0a 5f54 4541 4d53 5f57 4542  xxx".._TEAMS_WEB
+00004aa0: 484f 4f4b 5f55 524c 203d 2027 6d69 6372  HOOK_URL = 'micr
+00004ab0: 6f73 6f66 7420 7765 6268 6f6f 6b20 5f54  osoft webhook _T
+00004ac0: 4541 4d53 5f57 4542 484f 4f4b 5f55 524c  EAMS_WEBHOOK_URL
+00004ad0: 270d 0a0d 0a74 7279 3a0d 0a20 2020 2070  '....try:..    p
+00004ae0: 7269 6e74 2831 2f32 3029 2020 0d0a 2020  rint(1/20)  ..  
+00004af0: 2020 5375 6363 6573 7354 6561 6d73 2829    SuccessTeams()
+00004b00: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2073  .__call__() #1 s
+00004b10: 7563 6365 7373 2073 656e 6465 7220 2020  uccess sender   
+00004b20: 2020 2020 2020 200d 0a65 7863 6570 7420         ..except 
+00004b30: 4578 6365 7074 5465 616d 7320 6173 2065  ExceptTeams as e
+00004b40: 3a20 2020 2020 2023 3220 6578 6365 7074  :      #2 except
+00004b50: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
+00004b60: 2020 200d 0a20 2020 2073 7973 2e65 7869     ..    sys.exi
+00004b70: 7428 290d 0a0d 0a53 656e 6454 6561 6d73  t()....SendTeams
+00004b80: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00004b90: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
+00004ba0: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
+00004bb0: 200d 0a60 6060 0d0a 0d0a 3c42 723e 0d0a   ..```....<Br>..
+00004bc0: 0d0a 2323 2032 2d39 2e20 2a4b 616b 616f  ..## 2-9. *Kakao
+00004bd0: 7461 6c6b 204e 6f74 6966 6965 722a 0d0a  talk Notifier*..
+00004be0: 2d20 612e 2053 6967 6e20 7570 2061 7420  - a. Sign up at 
+00004bf0: 7468 6520 666f 6c6c 6f77 696e 6720 7369  the following si
+00004c00: 7465 3a20 5b68 7474 7073 3a2f 2f64 6576  te: [https://dev
+00004c10: 656c 6f70 6572 732e 6b61 6b61 6f2e 636f  elopers.kakao.co
+00004c20: 6d2f 5d28 6874 7470 733a 2f2f 6465 7665  m/](https://deve
+00004c30: 6c6f 7065 7273 2e6b 616b 616f 2e63 6f6d  lopers.kakao.com
+00004c40: 2f29 0d0a 2d20 622e 2043 6c69 636b 2022  /)..- b. Click "
+00004c50: 4d79 2041 7070 6c69 6361 7469 6f6e 2220  My Application" 
+00004c60: 6f6e 2074 6865 2074 6f70 2062 6172 2e0d  on the top bar..
+00004c70: 0a2d 2063 2e20 436c 6963 6b20 2241 6464  .- c. Click "Add
+00004c80: 2061 6e20 6170 706c 6963 6174 696f 6e2c   an application,
+00004c90: 2220 7365 7420 6120 6e61 6d65 2c20 616e  " set a name, an
+00004ca0: 6420 6372 6561 7465 2069 742e 0d0a 2d20  d create it...- 
+00004cb0: 642e 2043 6c69 636b 2022 4b61 6b61 6f20  d. Click "Kakao 
+00004cc0: 4c6f 6769 6e22 2069 6e20 7468 6520 6c65  Login" in the le
+00004cd0: 6674 206d 656e 752c 2074 6865 6e20 6368  ft menu, then ch
+00004ce0: 616e 6765 2074 6865 2053 7461 7465 206f  ange the State o
+00004cf0: 6620 224b 616b 616f 204c 6f67 696e 2041  f "Kakao Login A
+00004d00: 6374 6976 6174 696f 6e22 2074 6f20 4f4e  ctivation" to ON
+00004d10: 206f 6e20 7468 6520 7265 7375 6c74 696e   on the resultin
+00004d20: 6720 7061 6765 2e0d 0a2d 2065 2e20 496e  g page...- e. In
+00004d30: 204d 7920 4170 706c 6963 6174 696f 6e20   My Application 
+00004d40: 3e20 5072 6f64 7563 7420 5365 7474 696e  > Product Settin
+00004d50: 6773 203e 204b 616b 616f 204c 6f67 696e  gs > Kakao Login
+00004d60: 2c20 6265 2073 7572 6520 746f 2073 6574  , be sure to set
+00004d70: 2052 6564 6972 6563 7420 5552 4920 6173   Redirect URI as
+00004d80: 2066 6f6c 6c6f 7773 3a20 5b68 7474 7073   follows: [https
+00004d90: 3a2f 2f65 7861 6d70 6c65 2e63 6f6d 2f6f  ://example.com/o
+00004da0: 6175 7468 5d28 6874 7470 733a 2f2f 6578  auth](https://ex
+00004db0: 616d 706c 652e 636f 6d2f 6f61 7574 6829  ample.com/oauth)
+00004dc0: 0d0a 2d20 662e 2049 6e20 7468 6520 6c65  ..- f. In the le
+00004dd0: 6674 2043 6f6e 7365 6e74 2049 7465 6d73  ft Consent Items
+00004de0: 206d 656e 752c 2073 6574 2022 5365 6e64   menu, set "Send
+00004df0: 206d 6573 7361 6765 2069 6e20 4b61 6b61   message in Kaka
+00004e00: 6f54 616c 6b22 2074 6f20 7365 6c65 6374  oTalk" to select
+00004e10: 6976 6520 6167 7265 656d 656e 742e 0d0a  ive agreement...
+00004e20: 2d20 672e 2043 6f70 7920 7468 6520 5245  - g. Copy the RE
+00004e30: 5354 2041 5049 204b 6579 2069 6e20 4d79  ST API Key in My
+00004e40: 2041 7070 6c69 6361 7469 6f6e 203e 2041   Application > A
+00004e50: 7070 2053 6574 7469 6e67 7320 3e20 5375  pp Settings > Su
+00004e60: 6d6d 6172 792c 2061 6e64 2067 6f20 746f  mmary, and go to
+00004e70: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
+00004e80: 6f63 756d 656e 742e 0d0a 2d20 682e 2049  ocument...- h. I
+00004e90: 6620 796f 7520 6861 7665 2073 7563 6365  f you have succe
+00004ea0: 7373 6675 6c6c 7920 636f 6d70 6c65 7465  ssfully complete
+00004eb0: 6420 616c 6c20 6f66 2074 6865 2061 626f  d all of the abo
+00004ec0: 7665 2073 7465 7073 2c20 676f 2074 6f20  ve steps, go to 
+00004ed0: 7468 6520 666f 6c6c 6f77 696e 6720 646f  the following do
+00004ee0: 6375 6d65 6e74 2061 6e64 2066 6f6c 6c6f  cument and follo
+00004ef0: 7720 7468 6520 696e 7374 7275 6374 696f  w the instructio
+00004f00: 6e73 3a0d 0a20 6874 7470 733a 2f2f 6769  ns:.. https://gi
+00004f10: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
+00004f20: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
+00004f30: 6669 6572 2f62 6c6f 622f 6d61 696e 2f74  fier/blob/main/t
+00004f40: 7574 6f72 6961 6c73 2f6b 616b 616f 5f74  utorials/kakao_t
+00004f50: 6f6b 656e 5f67 656e 6572 6174 6f72 2e69  oken_generator.i
+00004f60: 7079 6e62 0d0a 202a 2a49 6e20 7468 6973  pynb.. **In this
+00004f70: 2065 7861 6d70 6c65 2c20 736f 6d65 2041   example, some A
+00004f80: 5049 206b 6579 7320 7765 7265 2065 7870  PI keys were exp
+00004f90: 6f73 6564 2062 7920 6372 6561 7469 6e67  osed by creating
+00004fa0: 2061 6e64 2072 656d 6f76 696e 6720 6120   and removing a 
+00004fb0: 7465 7374 2061 7070 6c69 6361 7469 6f6e  test application
+00004fc0: 2c20 6275 7420 666f 7220 7365 6375 7269  , but for securi
+00004fd0: 7479 2072 6561 736f 6e73 2c20 796f 7572  ty reasons, your
+00004fe0: 2041 5049 206b 6579 2073 686f 756c 6420   API key should 
+00004ff0: 6e6f 7420 6265 2065 7870 6f73 6564 2074  not be exposed t
+00005000: 6f20 7468 6520 6f75 7473 6964 6520 776f  o the outside wo
+00005010: 726c 642e 2a2a 0d0a 3c42 723e 0d0a 0d0a  rld.**..<Br>....
+00005020: 6060 6070 7974 686f 6e0d 0a69 6d70 6f72  ```python..impor
+00005030: 7420 7379 730d 0a66 726f 6d20 4578 6365  t sys..from Exce
+00005040: 7074 4e6f 7469 6669 6572 2069 6d70 6f72  ptNotifier impor
+00005050: 7420 4578 6365 7074 4b61 6b61 6f2c 2053  t ExceptKakao, S
+00005060: 7563 6365 7373 4b61 6b61 6f2c 2053 656e  uccessKakao, Sen
+00005070: 644b 616b 616f 0d0a 7379 732e 6578 6365  dKakao..sys.exce
+00005080: 7074 686f 6f6b 203d 2045 7863 6570 744b  pthook = ExceptK
+00005090: 616b 616f 2e5f 5f63 616c 6c5f 5f0d 0a0d  akao.__call__...
+000050a0: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
+000050b0: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
+000050c0: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
+000050d0: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
+000050e0: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
+000050f0: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
+00005100: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
+00005110: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
+00005120: 7878 7878 7822 0d0a 5f4b 414b 414f 5f54  xxxxx".._KAKAO_T
+00005130: 4f4b 454e 5f50 4154 4820 3d20 2778 7878  OKEN_PATH = 'xxx
+00005140: 782f 7878 782f 7878 782e 6a73 6f6e 2727  x/xxx/xxx.json''
+00005150: 0d0a 0d0a 7472 793a 0d0a 2020 2020 7072  ....try:..    pr
+00005160: 696e 7428 312f 3029 2020 0d0a 2020 2020  int(1/0)  ..    
+00005170: 5375 6363 6573 734b 616b 616f 2829 2e5f  SuccessKakao()._
+00005180: 5f63 616c 6c5f 5f28 2920 2331 2073 7563  _call__() #1 suc
+00005190: 6365 7373 2073 656e 6465 7220 2020 2020  cess sender     
+000051a0: 2020 2020 200d 0a65 7863 6570 7420 4578       ..except Ex
+000051b0: 6365 7074 4b61 6b61 6f20 6173 2065 3a20  ceptKakao as e: 
+000051c0: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
+000051d0: 656e 6465 7220 2020 2020 2020 2020 2020  ender           
+000051e0: 200d 0a20 2020 2073 7973 2e65 7869 7428   ..    sys.exit(
+000051f0: 290d 0a0d 0a53 656e 644b 616b 616f 2829  )....SendKakao()
+00005200: 2e5f 5f63 616c 6c5f 5f28 2920 2020 2020  .__call__()     
+00005210: 2020 2023 3320 6375 7374 6f6d 697a 6564     #3 customized
+00005220: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
+00005230: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
+00005240: 0a23 2320 322d 3130 2e20 2a42 6565 7020  .## 2-10. *Beep 
+00005250: 4e6f 7469 6669 6572 2a0d 0a4e 6f20 7365  Notifier*..No se
+00005260: 7475 7020 6973 2072 6571 7569 7265 642e  tup is required.
+00005270: 2055 7365 2061 7320 666f 6c6c 6f77 732e   Use as follows.
+00005280: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+00005290: 726f 6d20 4578 6365 7074 6e6f 7469 6669  rom Exceptnotifi
+000052a0: 6572 2069 6d70 6f72 7420 4578 6365 7074  er import Except
+000052b0: 4265 6570 2c20 5375 6363 6573 7342 6565  Beep, SuccessBee
+000052c0: 702c 2053 656e 6442 6565 7028 292c 2062  p, SendBeep(), b
+000052d0: 6565 7028 290d 0a42 4545 505f 5449 4d45  eep()..BEEP_TIME
+000052e0: 203d 2031 0d0a 7379 732e 6578 6365 7074   = 1..sys.except
+000052f0: 686f 6f6b 203d 2045 7863 6570 7442 6565  hook = ExceptBee
+00005300: 702e 5f5f 6361 6c6c 5f5f 0d0a 0d0a 7472  p.__call__....tr
+00005310: 793a 0d0a 2020 2020 7072 696e 7428 312f  y:..    print(1/
+00005320: 3230 2920 200d 0a20 2020 2053 7563 6365  20)  ..    Succe
+00005330: 7373 4265 6570 2829 2e5f 5f63 616c 6c5f  ssBeep().__call_
+00005340: 5f28 2920 2331 2073 7563 6365 7373 2062  _() #1 success b
+00005350: 6565 702d 6265 6570 2020 2020 2020 2020  eep-beep        
+00005360: 2020 0d0a 0d0a 6578 6365 7074 2045 7863    ....except Exc
+00005370: 6570 7442 6565 7020 6173 2065 3a20 2020  eptBeep as e:   
+00005380: 2020 2023 3220 6578 6365 7074 2062 6565     #2 except bee
+00005390: 702d 6265 6570 2020 2020 2020 2020 2020  p-beep          
+000053a0: 2020 2020 2020 0d0a 2020 2020 7379 732e        ..    sys.
+000053b0: 6578 6974 2829 0d0a 0d0a 5365 6e64 4265  exit()....SendBe
+000053c0: 6570 2829 2e5f 5f63 616c 6c5f 5f28 2920  ep().__call__() 
+000053d0: 2020 2020 2020 2023 3320 6375 7374 6f6d         #3 custom
+000053e0: 697a 6564 2062 6565 702d 6265 6570 2020  ized beep-beep  
+000053f0: 2020 2020 0d0a 0d0a 6265 6570 2829 0d0a      ....beep()..
+00005400: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
+00005410: 0a0d 0a23 2320 322d 3131 2e20 2a44 6573  ...## 2-11. *Des
+00005420: 6b74 6f70 204e 6f74 6966 6965 722a 0d0a  ktop Notifier*..
+00005430: 4e6f 2073 6574 7570 2069 7320 7265 7175  No setup is requ
+00005440: 6972 6564 2e20 5573 6520 6173 2066 6f6c  ired. Use as fol
+00005450: 6c6f 7773 2e0d 0a0d 0a60 6060 7079 7468  lows.....```pyth
+00005460: 6f6e 0d0a 6672 6f6d 2045 7863 6570 744e  on..from ExceptN
+00005470: 6f74 6966 6965 7220 696d 706f 7274 2045  otifier import E
+00005480: 7863 6570 7444 6573 6b74 6f70 2c20 5375  xceptDesktop, Su
+00005490: 6363 6573 7344 6573 6b74 6f70 2c20 5365  ccessDesktop, Se
+000054a0: 6e64 4465 736b 746f 700d 0a73 7973 2e65  ndDesktop..sys.e
+000054b0: 7863 6570 7468 6f6f 6b20 3d20 4578 6365  xcepthook = Exce
+000054c0: 7074 4465 736b 746f 702e 5f5f 6361 6c6c  ptDesktop.__call
+000054d0: 5f5f 0d0a 2320 4465 6669 6e65 2074 6865  __..# Define the
+000054e0: 206e 6578 7420 7477 6f20 7661 7269 6162   next two variab
+000054f0: 6c65 7320 6f70 7469 6f6e 616c 6c79 2077  les optionally w
+00005500: 6865 6e20 7573 696e 6720 4f70 656e 4149  hen using OpenAI
+00005510: 2773 2041 5049 2e0d 0a23 205f 4f50 454e  's API...# _OPEN
+00005520: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
+00005530: 2e35 2d74 7572 626f 2220 2020 200d 0a23  .5-turbo"    ..#
+00005540: 205f 4f50 454e 5f41 495f 4150 493d 2273   _OPEN_AI_API="s
+00005550: 6b2d 7878 7878 7878 220d 0a0d 0a74 7279  k-xxxxxx"....try
+00005560: 3a0d 0a20 2020 2070 7269 6e74 2831 2f30  :..    print(1/0
+00005570: 2920 200d 0a20 2020 2053 7563 6365 7373  )  ..    Success
+00005580: 4465 736b 746f 7028 292e 5f5f 6361 6c6c  Desktop().__call
+00005590: 5f5f 2829 2023 3120 7375 6363 6573 7320  __() #1 success 
+000055a0: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
+000055b0: 0d0a 0d0a 6578 6365 7074 2045 7863 6570  ....except Excep
+000055c0: 7444 6573 6b74 6f70 2061 7320 653a 2020  tDesktop as e:  
+000055d0: 2020 2020 2332 2065 7863 6570 7420 7365      #2 except se
+000055e0: 6e64 6572 2020 2020 2020 2020 2020 2020  nder            
+000055f0: 0d0a 2020 2020 7379 732e 6578 6974 2829  ..    sys.exit()
+00005600: 0d0a 0d0a 5365 6e64 4465 736b 746f 7028  ....SendDesktop(
+00005610: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
+00005620: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
+00005630: 6420 7365 6e64 6572 2020 2020 2020 2020  d sender        
+00005640: 200d 0a60 6060 0d0a 0d0a 3c42 723e 3c62   ..```....<Br><b
+00005650: 723e 3c62 723e 0d0a 0d0a 2320 4c69 6365  r><br>....# Lice
+00005660: 6e73 650d 0a4d 4954 0d0a 0d0a 2320 436f  nse..MIT....# Co
+00005670: 6465 206f 6620 436f 6e64 7563 740d 0a45  de of Conduct..E
+00005680: 7665 7279 6f6e 6520 7061 7274 6963 6970  veryone particip
+00005690: 6174 696e 6720 696e 2074 6865 2060 4578  ating in the `Ex
+000056a0: 6365 7074 4e6f 7469 6669 6572 6020 7072  ceptNotifier` pr
+000056b0: 6f6a 6563 742c 2061 6e64 2069 6e20 7061  oject, and in pa
+000056c0: 7274 6963 756c 6172 2069 6e20 7468 6520  rticular in the 
+000056d0: 6973 7375 6520 7472 6163 6b65 722c 2070  issue tracker, p
+000056e0: 756c 6c20 7265 7175 6573 7473 2c20 616e  ull requests, an
+000056f0: 6420 736f 6369 616c 206d 6564 6961 2061  d social media a
+00005700: 6374 6976 6974 792c 2069 7320 6578 7065  ctivity, is expe
+00005710: 6374 6564 2074 6f20 7472 6561 7420 6f74  cted to treat ot
+00005720: 6865 7220 7065 6f70 6c65 2077 6974 6820  her people with 
+00005730: 7265 7370 6563 7420 616e 6420 6d6f 7265  respect and more
+00005740: 2067 656e 6572 616c 6c79 2074 6f20 666f   generally to fo
+00005750: 6c6c 6f77 2074 6865 2067 7569 6465 6c69  llow the guideli
+00005760: 6e65 7320 6172 7469 6375 6c61 7465 6420  nes articulated 
+00005770: 696e 205b 7468 6520 5079 7468 6f6e 2043  in [the Python C
+00005780: 6f6d 6d75 6e69 7479 2043 6f64 6520 6f66  ommunity Code of
+00005790: 2043 6f6e 6475 6374 5d28 6874 7470 733a   Conduct](https:
+000057a0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+000057b0: 2f70 7366 2f63 6f6e 6475 6374 2f29 2e0d  /psf/conduct/)..
+000057c0: 0a0d 0a23 2323 2323 2054 6865 2070 6163  ...##### The pac
+000057d0: 6b61 6765 2069 7320 6375 7272 656e 746c  kage is currentl
+000057e0: 7920 696e 2074 6865 2064 6576 656c 6f70  y in the develop
+000057f0: 6d65 6e74 2061 6e64 2051 4120 7374 6167  ment and QA stag
+00005800: 6573 2c20 616e 6420 7468 6520 6465 7665  es, and the deve
+00005810: 6c6f 706d 656e 7420 7374 6167 6520 7769  lopment stage wi
+00005820: 6c6c 2062 6520 7570 6461 7465 6420 6174  ll be updated at
+00005830: 2074 6865 2074 6f70 206f 6620 7468 6973   the top of this
+00005840: 2070 6167 652e 2049 6620 6974 2069 7320   page. If it is 
+00005850: 6465 7465 726d 696e 6564 2074 6861 7420  determined that 
+00005860: 7468 6520 7072 6f64 7563 7420 6973 2073  the product is s
+00005870: 7461 626c 6520 7468 726f 7567 6820 6665  table through fe
+00005880: 6174 7572 6520 696d 7072 6f76 656d 656e  ature improvemen
+00005890: 742c 2061 6464 6974 696f 6e2c 2061 6e64  t, addition, and
+000058a0: 2069 7373 7565 2072 6573 6f6c 7574 696f   issue resolutio
+000058b0: 6e2c 2074 6865 2064 6576 656c 6f70 6d65  n, the developme
+000058c0: 6e74 2073 7461 6765 2077 696c 6c20 7265  nt stage will re
+000058d0: 6163 6820 7374 6167 6520 352e 2049 6620  ach stage 5. If 
+000058e0: 6e6f 206e 6577 2075 7064 6174 6573 206f  no new updates o
+000058f0: 7220 6973 7375 6573 2061 7269 7365 2c20  r issues arise, 
+00005900: 6974 2077 696c 6c20 6265 2061 646a 7573  it will be adjus
+00005910: 7465 6420 7570 7761 7264 2074 6f20 7374  ted upward to st
+00005920: 6167 6520 3620 6f72 2068 6967 6865 722e  age 6 or higher.
+00005930: 0d0a 0d0a 0d0a                           ......
```

### Comparing `ExceptNotifier-0.1.6/ExceptNotifier.egg-info/SOURCES.txt` & `ExceptNotifier-0.1.7/ExceptNotifier.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ExceptNotifier/kakao_notifier.py
 ExceptNotifier/line_notifier.py
 ExceptNotifier/mail_notifier.py
 ExceptNotifier/slack_notifier.py
 ExceptNotifier/sms_notifier.py
 ExceptNotifier/teams_notifier.py
 ExceptNotifier/telegram_notifier.py
+ExceptNotifier/wechat_notifier.py
 ExceptNotifier.egg-info/PKG-INFO
 ExceptNotifier.egg-info/SOURCES.txt
 ExceptNotifier.egg-info/dependency_links.txt
 ExceptNotifier.egg-info/entry_points.txt
 ExceptNotifier.egg-info/requires.txt
 ExceptNotifier.egg-info/top_level.txt
 ExceptNotifier/base/__init__.py
@@ -28,10 +29,11 @@
 ExceptNotifier/base/line_sender.py
 ExceptNotifier/base/mail_sender.py
 ExceptNotifier/base/openai_receiver.py
 ExceptNotifier/base/slack_sender.py
 ExceptNotifier/base/sms_sender.py
 ExceptNotifier/base/teams_sender.py
 ExceptNotifier/base/telegram_sender.py
+ExceptNotifier/base/wechat_sender.py
 ExceptNotifier/base/whatsapp_sender.py
 ExceptNotifier/utils/__init__.py
 ExceptNotifier/utils/kakao_token.py
```

### Comparing `ExceptNotifier-0.1.6/LICENSE` & `ExceptNotifier-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.6/PKG-INFO` & `ExceptNotifier-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2045 7863  : 2.1..Name: Exc
 00000020: 6570 744e 6f74 6966 6965 720d 0a56 6572  eptNotifier..Ver
-00000030: 7369 6f6e 3a20 302e 312e 360d 0a53 756d  sion: 0.1.6..Sum
+00000030: 7369 6f6e 3a20 302e 312e 370d 0a53 756d  sion: 0.1.7..Sum
 00000040: 6d61 7279 3a20 5769 7468 2050 7974 686f  mary: With Pytho
 00000050: 6e27 7320 7472 792d 6578 6365 7074 2074  n's try-except t
 00000060: 6f20 7265 6365 6976 6520 6e6f 7469 6669  o receive notifi
 00000070: 6361 7469 6f6e 7320 6162 6f75 7420 4572  cations about Er
 00000080: 726f 7273 206f 7220 5375 6363 6573 7365  rors or Successe
 00000090: 7320 696e 2079 6f75 7220 636f 6465 2074  s in your code t
 000000a0: 6872 6f75 6768 206d 6573 7365 6e67 6572  hrough messenger
@@ -65,1322 +65,1364 @@
 00000400: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
 00000410: 454e 5345 0d0a 0d0a 4465 7665 6c6f 706d  ENSE....Developm
 00000420: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
 00000430: 2d20 416c 7068 6120 3c62 723e 0d0a 2a43  - Alpha <br>..*C
 00000440: 6f70 7972 6967 6874 2028 6329 2032 3032  opyright (c) 202
 00000450: 3320 4d69 6e57 6f6f 2050 6172 6b2c 2053  3 MinWoo Park, S
 00000460: 6f75 7468 204b 6f72 6561 2a0d 0a3c 6272  outh Korea*..<br
-00000470: 3e0d 0a0d 0a23 2050 7974 686f 6e20 5061  >....# Python Pa
-00000480: 636b 6167 653a 2045 7863 6570 744e 6f74  ckage: ExceptNot
-00000490: 6966 6965 720d 0a21 5b45 7863 6570 742d  ifier..![Except-
-000004a0: 4e6f 7469 6669 6572 5d28 6874 7470 733a  Notifier](https:
-000004b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-000004c0: 2f62 6164 6765 2f70 7970 692d 4578 6365  /badge/pypi-Exce
-000004d0: 7074 4e6f 7469 6669 6572 2d6f 7261 6e67  ptNotifier-orang
-000004e0: 6529 0d0a 215b 5079 7069 2056 6572 7369  e)..![Pypi Versi
-000004f0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000500: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000510: 762f 4578 6365 7074 4e6f 7469 6669 6572  v/ExceptNotifier
-00000520: 2e73 7667 290d 0a5b 215b 5079 7468 6f6e  .svg)..[![Python
-00000530: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
-00000540: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000550: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
-00000560: 3625 3230 746f 2532 3033 2e37 2d62 6c61  6%20to%203.7-bla
-00000570: 636b 295d 2863 6f64 655f 6f66 5f63 6f6e  ck)](code_of_con
-00000580: 6475 6374 2e6d 6429 0d0a 215b 436f 6465  duct.md)..![Code
-00000590: 2063 6f6e 7665 6e74 696f 6e5d 2868 7474   convention](htt
-000005a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000005b0: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
-000005c0: 3063 6f6e 7665 6e74 696f 6e2d 7065 7038  0convention-pep8
-000005d0: 2d62 6c61 636b 290d 0a23 2323 2323 2050  -black)..##### P
-000005e0: 726f 7669 6465 7320 6120 6e6f 7469 6669  rovides a notifi
-000005f0: 6361 7469 6f6e 2066 726f 6d20 7468 6520  cation from the 
-00000600: 6170 706c 6963 6174 696f 6e20 7368 6f77  application show
-00000610: 6e20 696e 2074 6865 2066 6f6c 6c6f 7769  n in the followi
-00000620: 6e67 2073 6372 6565 6e2c 0d0a 0d0a 215b  ng screen,....![
-00000630: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000640: 2e63 6f6d 2f64 7364 616e 6965 6c70 6172  .com/dsdanielpar
-00000650: 6b2f 4578 6365 7074 4e6f 7469 6669 6572  k/ExceptNotifier
-00000660: 2f62 6c6f 622f 6d61 696e 2f61 7373 6574  /blob/main/asset
-00000670: 732f 696d 6773 2f6d 6169 6e32 2e70 6e67  s/imgs/main2.png
-00000680: 290d 0a20 5468 6520 6045 7863 6570 744e  ).. The `ExceptN
-00000690: 6f74 6966 6965 7260 2050 7974 686f 6e20  otifier` Python 
-000006a0: 7061 636b 6167 6520 6f66 6665 7273 2061  package offers a
-000006b0: 2066 6c65 7869 626c 6520 6170 7072 6f61   flexible approa
-000006c0: 6368 2074 6f20 7265 6365 6976 696e 6720  ch to receiving 
-000006d0: 6e6f 7469 6669 6361 7469 6f6e 7320 6279  notifications by
-000006e0: 2065 6e68 616e 6369 6e67 2050 7974 686f   enhancing Pytho
-000006f0: 6e27 7320 7472 792d 6578 6365 7074 2073  n's try-except s
-00000700: 7461 7465 6d65 6e74 2e20 5468 6973 2070  tatement. This p
-00000710: 6163 6b61 6765 2065 6e61 626c 6573 2079  ackage enables y
-00000720: 6f75 2074 6f20 7265 6365 6976 6520 616c  ou to receive al
-00000730: 6572 7473 2074 6872 6f75 6768 2076 6172  erts through var
-00000740: 696f 7573 206d 6573 7361 6769 6e67 2061  ious messaging a
-00000750: 7070 6c69 6361 7469 6f6e 7320 6f72 2065  pplications or e
-00000760: 6d61 696c 732e 0d0a 3c42 723e 3c62 723e  mails...<Br><br>
-00000770: 0d0a 5769 7468 2060 4578 6365 7074 4e6f  ..With `ExceptNo
-00000780: 7469 6669 6572 602c 2079 6f75 2063 616e  tifier`, you can
-00000790: 206f 6274 6169 6e20 6465 7461 696c 6564   obtain detailed
-000007a0: 2063 6f6d 7069 6c61 7469 6f6e 2065 7272   compilation err
-000007b0: 6f72 732c 2069 6e63 6c75 6469 6e67 2064  ors, including d
-000007c0: 6562 7567 2069 6e66 6f72 6d61 7469 6f6e  ebug information
-000007d0: 2c20 7365 6e74 2064 6972 6563 746c 7920  , sent directly 
-000007e0: 746f 2079 6f75 7220 7072 6566 6572 7265  to your preferre
-000007f0: 6420 6d65 7373 6167 696e 6720 706c 6174  d messaging plat
-00000800: 666f 726d 206f 7220 656d 6169 6c2e 2042  form or email. B
-00000810: 7920 696e 7465 6772 6174 696e 6720 4f70  y integrating Op
-00000820: 656e 4149 2773 2043 6861 7447 5054 2c20  enAI's ChatGPT, 
-00000830: 796f 7520 6361 6e20 7265 6365 6976 6520  you can receive 
-00000840: 6164 6469 7469 6f6e 616c 2065 7272 6f72  additional error
-00000850: 2063 6f64 6520 696e 666f 726d 6174 696f   code informatio
-00000860: 6e20 6173 206c 6f6e 6720 6173 2079 6f75  n as long as you
-00000870: 2070 726f 7669 6465 2074 6865 2072 6571   provide the req
-00000880: 7569 7265 6420 4150 4920 6d6f 6465 6c20  uired API model 
-00000890: 6e61 6d65 2061 6e64 206b 6579 2e20 5468  name and key. Th
-000008a0: 6973 2066 6561 7475 7265 2065 6e73 7572  is feature ensur
-000008b0: 6573 2074 6861 7420 6572 726f 7220 6861  es that error ha
-000008c0: 6e64 6c69 6e67 2061 6e64 206e 6f74 6966  ndling and notif
-000008d0: 6963 6174 696f 6e73 2061 7265 206d 6f72  ications are mor
-000008e0: 6520 696e 666f 726d 6174 6976 6520 616e  e informative an
-000008f0: 6420 6163 6365 7373 6962 6c65 2c20 7374  d accessible, st
-00000900: 7265 616d 6c69 6e69 6e67 2079 6f75 7220  reamlining your 
-00000910: 6465 6275 6767 696e 6720 7072 6f63 6573  debugging proces
-00000920: 732e 0d0a 0d0a 3c62 723e 3c62 723e 0d0a  s.....<br><br>..
-00000930: 0d0a 2323 2320 5375 7070 6f72 7469 6e67  ..### Supporting
-00000940: 2041 7070 6c69 6361 7469 6f6e 730d 0a0d   Applications...
-00000950: 0a2d 205b 5465 6c65 6772 616d 5d28 6874  .- [Telegram](ht
-00000960: 7470 733a 2f2f 7465 6c65 6772 616d 2e6f  tps://telegram.o
-00000970: 7267 2f29 0d0a 2d20 5b44 6973 636f 7264  rg/)..- [Discord
-00000980: 5d28 6874 7470 733a 2f2f 6469 7363 6f72  ](https://discor
-00000990: 642e 636f 6d2f 290d 0a2d 205b 536c 6163  d.com/)..- [Slac
-000009a0: 6b5d 2868 7474 7073 3a2f 2f73 6c61 636b  k](https://slack
-000009b0: 2e63 6f6d 2f29 0d0a 2d20 5b47 6f6f 676c  .com/)..- [Googl
-000009c0: 6520 4d61 696c 5d28 6874 7470 733a 2f2f  e Mail](https://
-000009d0: 6d61 696c 2e67 6f6f 676c 652e 636f 6d2f  mail.google.com/
-000009e0: 290d 0a2d 2053 4d53 2053 656e 6469 6e67  )..- SMS Sending
-000009f0: 2075 7369 6e67 205b 5477 696c 696f 5d28   using [Twilio](
-00000a00: 6874 7470 733a 2f2f 7777 772e 7477 696c  https://www.twil
-00000a10: 696f 2e63 6f6d 2f65 6e2d 7573 290d 0a2d  io.com/en-us)..-
-00000a20: 2044 6573 6b74 6f70 204e 6f74 6966 6963   Desktop Notific
-00000a30: 6174 696f 6e20 7573 696e 6720 5b50 6c79  ation using [Ply
-00000a40: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-00000a50: 7562 2e63 6f6d 2f6b 6976 792f 706c 7965  ub.com/kivy/plye
-00000a60: 7229 0d0a 2d20 5b4c 696e 655d 2868 7474  r)..- [Line](htt
-00000a70: 7073 3a2f 2f6c 696e 652e 6d65 2f65 6e2f  ps://line.me/en/
-00000a80: 290d 0a2d 205b 4157 5320 4368 696d 655d  )..- [AWS Chime]
-00000a90: 2868 7474 7073 3a2f 2f61 7773 2e61 6d61  (https://aws.ama
-00000aa0: 7a6f 6e2e 636f 6d2f 6b6f 2f63 6869 6d65  zon.com/ko/chime
-00000ab0: 2f64 6f77 6e6c 6f61 642d 6368 696d 652f  /download-chime/
-00000ac0: 290d 0a2d 205b 4d69 6372 6f73 6f66 7420  )..- [Microsoft 
-00000ad0: 5465 616d 735d 2868 7474 7073 3a2f 2f77  Teams](https://w
-00000ae0: 7777 2e6d 6963 726f 736f 6674 2e63 6f6d  ww.microsoft.com
-00000af0: 2f65 6e2f 6d69 6372 6f73 6f66 742d 7465  /en/microsoft-te
-00000b00: 616d 732f 646f 776e 6c6f 6164 2d61 7070  ams/download-app
-00000b10: 290d 0a2d 205b 4b61 6b61 6f20 5461 6c6b  )..- [Kakao Talk
-00000b20: 5d28 6874 7470 733a 2f2f 7777 772e 6b61  ](https://www.ka
-00000b30: 6b61 6f63 6f72 702e 636f 6d2f 7061 6765  kaocorp.com/page
-00000b40: 2f73 6572 7669 6365 2f73 6572 7669 6365  /service/service
-00000b50: 2f4b 616b 616f 5461 6c6b 3f6c 616e 673d  /KakaoTalk?lang=
-00000b60: 656e 290d 0a2d 2042 6565 7020 536f 756e  en)..- Beep Soun
-00000b70: 6420 6672 6f6d 205b 7379 7374 656d 5d28  d from [system](
-00000b80: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-00000b90: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
-00000ba0: 792f 7769 6e73 6f75 6e64 2e68 746d 6c29  y/winsound.html)
-00000bb0: 0d0a 0d0a 3c42 723e 0d0a 0d0a 2323 2320  ....<Br>....### 
-00000bc0: 4149 2044 6562 7567 6769 6e67 0d0a 4966  AI Debugging..If
-00000bd0: 2079 6f75 2068 6176 6520 4f70 656e 4149   you have OpenAI
-00000be0: 2041 5049 204b 6579 2061 6e64 206d 6f64   API Key and mod
-00000bf0: 656c 206e 616d 652c 2079 6f75 2063 616e  el name, you can
-00000c00: 2067 6574 2069 6e66 6f72 6d61 7469 6f6e   get information
-00000c10: 2061 6e64 2063 6f64 6520 6578 616d 706c   and code exampl
-00000c20: 6573 2066 6f72 2064 6562 7567 6769 6e67  es for debugging
-00000c30: 2069 6e20 616e 7920 6170 706c 6963 6174   in any applicat
-00000c40: 696f 6e2e 0d0a 2d20 5b4f 5045 4e20 4149  ion...- [OPEN AI
-00000c50: 2041 5049 5d28 6874 7470 733a 2f2f 706c   API](https://pl
-00000c60: 6174 666f 726d 2e6f 7065 6e61 692e 636f  atform.openai.co
-00000c70: 6d2f 646f 6373 2f69 6e74 726f 6475 6374  m/docs/introduct
-00000c80: 696f 6e29 0d0a 0d0a 0d0a 3c62 723e 3c62  ion)......<br><b
-00000c90: 723e 0d0a 0d0a 2320 5175 6963 6b20 5374  r>....# Quick St
-00000ca0: 6172 740d 0a60 6060 6261 7368 0d0a 7069  art..```bash..pi
-00000cb0: 7020 696e 7374 616c 6c20 4578 6365 7074  p install Except
-00000cc0: 4e6f 7469 6669 6572 0d0a 7069 7020 696e  Notifier..pip in
-00000cd0: 7374 616c 6c20 6578 6365 7074 6e6f 7469  stall exceptnoti
-00000ce0: 6669 6572 0d0a 0d0a 636f 6e64 6120 696e  fier....conda in
-00000cf0: 7374 616c 6c20 4578 6365 7074 4e6f 7469  stall ExceptNoti
-00000d00: 6669 6572 0d0a 636f 6e64 6120 696e 7374  fier..conda inst
-00000d10: 616c 6c20 6578 6365 7074 6e6f 7469 6669  all exceptnotifi
-00000d20: 6572 0d0a 6060 600d 0a0d 0a3c 6272 3e0d  er..```....<br>.
-00000d30: 0a0d 0a0d 0a23 2041 7070 2053 6574 7570  .....# App Setup
-00000d40: 204f 7665 7276 6965 770d 0a0d 0a2d 2054   Overview....- T
-00000d50: 6865 2076 6172 6961 626c 6573 2069 6e20  he variables in 
-00000d60: 7468 6520 666f 6c6c 6f77 696e 6720 7461  the following ta
-00000d70: 626c 6520 6d75 7374 206e 6f74 2062 6520  ble must not be 
-00000d80: 636f 6e74 616d 696e 6174 6564 2e0d 0a2d  contaminated...-
-00000d90: 2044 6570 656e 6469 6e67 206f 6e20 7468   Depending on th
-00000da0: 6520 7369 7475 6174 696f 6e2c 2063 6f6e  e situation, con
-00000db0: 7369 6465 7220 6465 7369 676e 6174 696e  sider designatin
-00000dc0: 6720 7468 656d 2061 7320 676c 6f62 616c  g them as global
-00000dd0: 2076 6172 6961 626c 6573 2066 6f72 2075   variables for u
-00000de0: 7365 2e0d 0a2d 2049 6620 796f 7520 6172  se...- If you ar
-00000df0: 6520 7573 696e 6720 5465 6c65 6772 616d  e using Telegram
-00000e00: 2c20 616e 2065 7861 6d70 6c65 2069 7320  , an example is 
-00000e10: 6174 7461 6368 6564 2061 7320 616e 2069  attached as an i
-00000e20: 6d61 6765 2e0d 0a2d 2041 7320 796f 7520  mage...- As you 
-00000e30: 616c 7265 6164 7920 6b6e 6f77 2c20 4150  already know, AP
-00000e40: 4920 4b65 7973 206f 7220 7365 6375 7269  I Keys or securi
-00000e50: 7479 2074 6f6b 656e 7320 6d75 7374 2062  ty tokens must b
-00000e60: 6520 7365 6375 7265 642e 204e 6f74 6520  e secured. Note 
-00000e70: 7468 6174 2074 6865 206b 6579 2076 616c  that the key val
-00000e80: 7565 7320 7768 6963 6820 6578 706f 7375  ues which exposu
-00000e90: 7265 6420 696e 2067 6974 6875 6220 7769  red in github wi
-00000ea0: 6c6c 2062 6520 6578 7069 7265 6420 6166  ll be expired af
-00000eb0: 7465 7220 696e 7365 6375 7265 642e 0d0a  ter insecured...
-00000ec0: 0d0a 7c20 4170 7020 7c20 5265 7175 6972  ..| App | Requir
-00000ed0: 6564 2056 6172 6961 626c 6573 207c 2046  ed Variables | F
-00000ee0: 7265 6520 6f72 2050 6169 6420 7c20 4561  ree or Paid | Ea
-00000ef0: 7365 206f 6620 5365 7475 7020 7c20 5469  se of Setup | Ti
-00000f00: 6d65 2052 6571 7569 7265 6420 666f 7220  me Required for 
-00000f10: 5365 7475 707c 4775 6964 6520 5475 746f  Setup|Guide Tuto
-00000f20: 7269 616c 204c 696e 6b7c 0d0a 7c3a 2d2d  rial Link|..|:--
-00000f30: 3a7c 3a2d 2d7c 3a2d 2d3a 7c3a 2d2d 3a7c  :|:--|:--:|:--:|
-00000f40: 3a2d 2d3a 7c3a 2d2d 2d3a 7c0d 0a7c 4265  :--:|:---:|..|Be
-00000f50: 6570 7c4e 2f41 7c46 7265 657c 4e2f 417c  ep|N/A|Free|N/A|
-00000f60: 3020 6d69 6e7c 5b45 7863 6570 7442 6565  0 min|[ExceptBee
-00000f70: 705d 2868 7474 7073 3a2f 2f67 6974 6875  p](https://githu
-00000f80: 622e 636f 6d2f 6473 6461 6e69 656c 7061  b.com/dsdanielpa
-00000f90: 726b 2f45 7863 6570 744e 6f74 6966 6965  rk/ExceptNotifie
-00000fa0: 722f 626c 6f62 2f6d 6169 6e2f 646f 6375  r/blob/main/docu
-00000fb0: 6d65 6e74 732f 4578 6365 7074 4265 6570  ments/ExceptBeep
-00000fc0: 2f47 5549 4445 2e6d 6429 7c0d 0a7c 4465  /GUIDE.md)|..|De
-00000fd0: 736b 746f 707c 4e2f 417c 4672 6565 7c4e  sktop|N/A|Free|N
-00000fe0: 2f41 7c30 206d 696e 7c5b 4578 6365 7074  /A|0 min|[Except
-00000ff0: 4465 736b 746f 705d 2868 7474 7073 3a2f  Desktop](https:/
-00001000: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
-00001010: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
-00001020: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
-00001030: 6e2f 646f 6375 6d65 6e74 732f 4578 6365  n/documents/Exce
-00001040: 7074 4465 736b 746f 702f 4755 4944 452e  ptDesktop/GUIDE.
-00001050: 6d64 297c 0d0a 7c54 656c 6567 7261 6d7c  md)|..|Telegram|
-00001060: 605f 5445 4c45 4752 414d 5f54 4f4b 454e  `_TELEGRAM_TOKEN
-00001070: 607c 4672 6565 6d69 756d 7c45 6173 797c  `|Freemium|Easy|
-00001080: 326d 696e 7c5b 4578 6365 7074 5465 6c65  2min|[ExceptTele
-00001090: 6772 616d 5d28 6874 7470 733a 2f2f 6769  gram](https://gi
-000010a0: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
-000010b0: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
-000010c0: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
-000010d0: 6f63 756d 656e 7473 2f45 7863 6570 7454  ocuments/ExceptT
-000010e0: 656c 6567 7261 6d2f 4755 4944 452e 6d64  elegram/GUIDE.md
-000010f0: 297c 0d0a 7c44 6973 636f 7264 7c60 5f44  )|..|Discord|`_D
-00001100: 4953 434f 5244 5f57 4542 484f 4f4b 5f55  ISCORD_WEBHOOK_U
-00001110: 524c 607c 4672 6565 6d69 756d 7c45 6173  RL`|Freemium|Eas
-00001120: 797c 316d 696e 7c5b 4578 6365 7074 4469  y|1min|[ExceptDi
-00001130: 7363 6f72 645d 2868 7474 7073 3a2f 2f67  scord](https://g
-00001140: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00001150: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00001160: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00001170: 646f 6375 6d65 6e74 732f 4578 6365 7074  documents/Except
-00001180: 5465 6c65 6772 616d 2f47 5549 4445 2e6d  Telegram/GUIDE.m
-00001190: 6429 7c0d 0a7c 4157 5320 4368 696d 657c  d)|..|AWS Chime|
-000011a0: 605f 4348 494d 455f 5745 4248 4f4f 4b5f  `_CHIME_WEBHOOK_
-000011b0: 5552 4c60 7c46 7265 656d 6975 6d7c 4561  URL`|Freemium|Ea
-000011c0: 7379 7c31 6d69 6e7c 5b45 7863 6570 7443  sy|1min|[ExceptC
-000011d0: 6869 6d65 5d28 6874 7470 733a 2f2f 6769  hime](https://gi
-000011e0: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
-000011f0: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
-00001200: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
-00001210: 6f63 756d 656e 7473 2f45 7863 6570 7443  ocuments/ExceptC
-00001220: 6869 6d65 2f47 5549 4445 2e6d 6429 7c0d  hime/GUIDE.md)|.
-00001230: 0a7c 536c 6163 6b7c 605f 534c 4143 4b5f  .|Slack|`_SLACK_
-00001240: 5745 4248 4f4f 4b5f 5552 4c60 7c46 7265  WEBHOOK_URL`|Fre
-00001250: 656d 6975 6d7c 4561 7379 7c33 6d69 6e7c  emium|Easy|3min|
-00001260: 5b45 7863 6570 7453 6c61 636b 5d28 6874  [ExceptSlack](ht
-00001270: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001280: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
-00001290: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
-000012a0: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
-000012b0: 2f45 7863 6570 7453 6c61 636b 2f47 5549  /ExceptSlack/GUI
-000012c0: 4445 2e6d 6429 7c0d 0a7c 472d 4d61 696c  DE.md)|..|G-Mail
-000012d0: 7c60 5f47 414d 494c 5f52 4543 4950 4945  |`_GAMIL_RECIPIE
-000012e0: 4e54 5f41 4444 5260 2c20 605f 474d 4149  NT_ADDR`, `_GMAI
-000012f0: 4c5f 5345 4e44 4552 5f41 4444 5260 2c20  L_SENDER_ADDR`, 
-00001300: 605f 474d 4149 4c5f 4150 505f 5041 5353  `_GMAIL_APP_PASS
-00001310: 574f 5244 5f4f 465f 5345 4e44 4552 6020  WORD_OF_SENDER` 
-00001320: 7c52 6573 7472 6963 7465 6420 6672 6565  |Restricted free
-00001330: 7c4d 6564 6975 6d7c 336d 696e 7c5b 4578  |Medium|3min|[Ex
-00001340: 6365 7074 4d61 696c 5d28 6874 7470 733a  ceptMail](https:
-00001350: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7364  //github.com/dsd
-00001360: 616e 6965 6c70 6172 6b2f 4578 6365 7074  anielpark/Except
-00001370: 4e6f 7469 6669 6572 2f62 6c6f 622f 6d61  Notifier/blob/ma
-00001380: 696e 2f64 6f63 756d 656e 7473 2f45 7863  in/documents/Exc
-00001390: 6570 744d 6169 6c2f 4755 4944 452e 6d64  eptMail/GUIDE.md
-000013a0: 297c 0d0a 7c4c 696e 657c 605f 4c49 4e45  )|..|Line|`_LINE
-000013b0: 5f4e 4f54 4946 595f 4150 495f 544f 4b45  _NOTIFY_API_TOKE
-000013c0: 4e60 7c46 7265 656d 6975 6d7c 4d65 6469  N`|Freemium|Medi
-000013d0: 756d 7c34 6d69 6e7c 5b45 7863 6570 744c  um|4min|[ExceptL
-000013e0: 696e 655d 2868 7474 7073 3a2f 2f67 6974  ine](https://git
-000013f0: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
-00001400: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
-00001410: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
-00001420: 6375 6d65 6e74 732f 4578 6365 7074 4c69  cuments/ExceptLi
-00001430: 6e65 2f47 5549 4445 2e6d 6429 7c0d 0a7c  ne/GUIDE.md)|..|
-00001440: 534d 537c 605f 5457 494c 494f 5f53 4944  SMS|`_TWILIO_SID
-00001450: 602c 2060 5f54 5749 4c49 4f5f 544f 4b45  `, `_TWILIO_TOKE
-00001460: 4e60 2c20 605f 5245 4349 5049 454e 545f  N`, `_RECIPIENT_
-00001470: 5048 4f4e 455f 4e55 4d42 4552 602c 2060  PHONE_NUMBER`, `
-00001480: 5f53 454e 4445 525f 5048 4f4e 455f 4e55  _SENDER_PHONE_NU
-00001490: 4d42 4552 607c 4e6f 7420 6672 6565 7c4d  MBER`|Not free|M
-000014a0: 6564 6975 6d7c 356d 696e 7c5b 4578 6365  edium|5min|[Exce
-000014b0: 7074 534d 535d 2868 7474 7073 3a2f 2f67  ptSMS](https://g
-000014c0: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-000014d0: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-000014e0: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-000014f0: 646f 6375 6d65 6e74 732f 4578 6365 7074  documents/Except
-00001500: 534d 532f 4755 4944 452e 6d64 297c 0d0a  SMS/GUIDE.md)|..
-00001510: 7c4d 6963 726f 736f 6674 2054 6561 6d73  |Microsoft Teams
-00001520: 7c60 5f54 4541 4d53 5f57 4542 484f 4f4b  |`_TEAMS_WEBHOOK
-00001530: 5f55 524c 607c 4e6f 7420 4672 6565 7c4d  _URL`|Not Free|M
-00001540: 6564 6975 6d7c 356d 696e 7c5b 4578 6365  edium|5min|[Exce
-00001550: 7074 5465 616d 735d 2868 7474 7073 3a2f  ptTeams](https:/
-00001560: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
-00001570: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
-00001580: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
-00001590: 6e2f 646f 6375 6d65 6e74 732f 4578 6365  n/documents/Exce
-000015a0: 7074 5465 616d 732f 4755 4944 452e 6d64  ptTeams/GUIDE.md
-000015b0: 297c 0d0a 7c4b 616b 616f 5461 6c6b 7c60  )|..|KakaoTalk|`
-000015c0: 5f4b 414b 414f 5f54 4f4b 454e 5f50 4154  _KAKAO_TOKEN_PAT
-000015d0: 4860 7c46 7265 656d 6975 6d7c 4865 6c6c  H`|Freemium|Hell
-000015e0: 7c3e 3d31 306d 696e 2854 6f6b 656e 2072  |>=10min(Token r
-000015f0: 6566 7265 7368 6573 2064 6169 6c79 2e29  efreshes daily.)
-00001600: 7c5b 4578 6365 7074 4b61 6b61 6f5d 2868  |[ExceptKakao](h
-00001610: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001620: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00001630: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00001640: 6f62 2f6d 6169 6e2f 646f 6375 6d65 6e74  ob/main/document
-00001650: 732f 4578 6365 7074 4b61 6b61 6f2f 4755  s/ExceptKakao/GU
-00001660: 4944 452e 6d64 297c 0d0a 0d0a 0d0a 4966  IDE.md)|......If
-00001670: 2079 6f75 2061 6464 2074 6865 2066 6f6c   you add the fol
-00001680: 6c6f 7769 6e67 2074 776f 2076 6172 6961  lowing two varia
-00001690: 626c 6573 2074 6f20 7468 6520 7265 7175  bles to the requ
-000016a0: 6972 6564 2076 6172 6961 626c 6573 2066  ired variables f
-000016b0: 6f72 2065 6163 6820 6170 706c 6963 6174  or each applicat
-000016c0: 696f 6e20 696e 2074 6865 2074 6162 6c65  ion in the table
-000016d0: 2061 626f 7665 2c20 796f 7520 6361 6e20   above, you can 
-000016e0: 7265 6365 6976 6520 6572 726f 7220 6c6f  receive error lo
-000016f0: 6361 7469 6f6e 2061 6e64 2065 7870 6c61  cation and expla
-00001700: 6e61 7469 6f6e 2c20 6173 2077 656c 6c20  nation, as well 
-00001710: 6173 2065 7861 6d70 6c65 732c 2066 726f  as examples, fro
-00001720: 6d20 4f70 656e 4149 2773 206d 6f64 656c  m OpenAI's model
-00001730: 0d0a 0d0a 7c20 4150 4920 7c20 5265 7175  ....| API | Requ
-00001740: 6972 6564 2056 6172 6961 626c 6573 207c  ired Variables |
-00001750: 2046 7265 6520 6f72 2050 6169 6420 7c20   Free or Paid | 
-00001760: 4561 7365 206f 6620 5365 7475 7020 7c20  Ease of Setup | 
-00001770: 5469 6d65 2052 6571 7569 7265 6420 666f  Time Required fo
-00001780: 7220 5365 7475 707c 4775 6964 6520 5475  r Setup|Guide Tu
-00001790: 746f 7269 616c 204c 696e 6b7c 0d0a 7c3a  torial Link|..|:
-000017a0: 2d2d 3a7c 3a2d 2d7c 3a2d 2d3a 7c3a 2d2d  --:|:--|:--:|:--
-000017b0: 3a7c 3a2d 2d3a 7c3a 2d2d 2d3a 7c0d 0a7c  :|:--:|:---:|..|
-000017c0: 204f 7065 6e41 4920 4150 4920 7c60 5265   OpenAI API |`Re
-000017d0: 7175 6972 6564 2076 6172 6961 626c 6573  quired variables
-000017e0: 2066 6f72 2065 6163 6820 6170 706c 6963   for each applic
-000017f0: 6174 696f 6e60 2b20 605f 4f50 454e 5f41  ation`+ `_OPEN_A
-00001800: 495f 4d4f 4445 4c60 2c60 5f4f 5045 4e5f  I_MODEL`,`_OPEN_
-00001810: 4149 5f41 5049 607c 4e6f 7420 6672 6565  AI_API`|Not free
-00001820: 7c45 6173 797c 326d 696e 7c5b 4150 494f  |Easy|2min|[APIO
-00001830: 7065 6e41 495d 2868 7474 7073 3a2f 2f67  penAI](https://g
-00001840: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00001850: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00001860: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00001870: 646f 6375 6d65 6e74 732f 4150 494f 7065  documents/APIOpe
-00001880: 6e41 492f 4755 4944 452e 6d64 297c 0d0a  nAI/GUIDE.md)|..
-00001890: 0d0a 0d0a 3c62 723e 3c62 723e 0d0a 0d0a  ....<br><br>....
-000018a0: 2320 312e 204b 6579 2046 6561 7475 7265  # 1. Key Feature
-000018b0: 730d 0a54 6f20 7573 6520 7468 6520 6465  s..To use the de
-000018c0: 7369 7265 6420 6170 706c 6963 6174 696f  sired applicatio
-000018d0: 6e2c 2079 6f75 206d 7573 7420 6465 6669  n, you must defi
-000018e0: 6e65 2074 6865 206e 6563 6573 7361 7279  ne the necessary
-000018f0: 2076 6172 6961 626c 6573 2e20 456e 7375   variables. Ensu
-00001900: 7265 2074 6861 7420 7468 6520 7661 7269  re that the vari
-00001910: 6162 6c65 206e 616d 6573 2072 656d 6169  able names remai
-00001920: 6e20 756e 6368 616e 6765 642c 2061 6e64  n unchanged, and
-00001930: 2079 6f75 2063 616e 2075 7365 2065 6974   you can use eit
-00001940: 6865 7220 6c6f 6361 6c20 6f72 2067 6c6f  her local or glo
-00001950: 6261 6c20 7661 7269 6162 6c65 732e 2049  bal variables. I
-00001960: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
-00001970: 6054 656c 6567 7261 6d60 2c20 616e 2065  `Telegram`, an e
-00001980: 7861 6d70 6c65 2069 7320 6174 7461 6368  xample is attach
-00001990: 6564 2061 7320 616e 2069 6d61 6765 2e0d  ed as an image..
-000019a0: 0a0d 0a23 2320 312d 312e 2045 7863 6570  ...## 1-1. Excep
-000019b0: 7460 5b61 7070 4e61 6d65 5d60 0d0a 4966  t`[appName]`..If
-000019c0: 2079 6f75 2075 7365 2050 7974 686f 6e27   you use Python'
-000019d0: 7320 7472 7920 6578 6365 7074 2073 7461  s try except sta
-000019e0: 7465 6d65 6e74 2061 7320 6974 2069 732c  tement as it is,
-000019f0: 2062 7574 2063 6861 6e67 6520 6578 6365   but change exce
-00001a00: 7074 2061 7320 666f 6c6c 6f77 732c 2079  pt as follows, y
-00001a10: 6f75 2063 616e 2072 6563 6569 7665 206e  ou can receive n
-00001a20: 6f74 6966 6963 6174 696f 6e73 2074 6872  otifications thr
-00001a30: 6f75 6768 2079 6f75 7220 6170 706c 6963  ough your applic
-00001a40: 6174 696f 6e2e 0d0a 6060 600d 0a45 7863  ation...```..Exc
-00001a50: 6570 7443 6869 6d65 2c20 4578 6365 7074  eptChime, Except
-00001a60: 5465 6c65 6772 616d 2c20 4578 6365 7074  Telegram, Except
-00001a70: 4469 7363 6f72 642c 2045 7863 6570 7453  Discord, ExceptS
-00001a80: 4d53 2c20 4578 6365 7074 4d61 696c 2c20  MS, ExceptMail, 
-00001a90: 4578 6365 7074 4b61 6b61 6f2c 2045 7863  ExceptKakao, Exc
-00001aa0: 6570 744c 696e 652c 2045 7863 6570 7453  eptLine, ExceptS
-00001ab0: 6c61 636b 2c20 4578 6365 7074 5465 616d  lack, ExceptTeam
-00001ac0: 732c 2045 7863 6570 7444 6573 6b74 6f70  s, ExceptDesktop
-00001ad0: 652c 2045 7863 6570 7442 6565 700d 0a60  e, ExceptBeep..`
-00001ae0: 6060 0d0a 0d0a 2a45 7861 6d70 6c65 2a0d  ``....*Example*.
-00001af0: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00001b00: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
-00001b10: 696d 706f 7274 2045 7863 6570 7454 656c  import ExceptTel
-00001b20: 6765 7261 6d0d 0a5f 5445 4c45 4752 414d  geram.._TELEGRAM
-00001b30: 5f54 4f4b 454e 203d 2022 7878 7878 220d  _TOKEN = "xxxx".
-00001b40: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
-00001b50: 6e74 2831 2f30 290d 0a65 7863 6570 7420  nt(1/0)..except 
-00001b60: 4578 6365 7074 5465 6c65 6772 616d 3a20  ExceptTelegram: 
-00001b70: 2020 2023 2073 656e 6469 6e67 2065 7863     # sending exc
-00001b80: 6570 7420 6d65 7373 6167 6520 746f 2074  ept message to t
-00001b90: 656c 6567 7261 6d0d 0a20 2020 2073 7973  elegram..    sys
-00001ba0: 2e65 7869 7428 290d 0a60 6060 0d0a 215b  .exit()..```..![
-00001bb0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001bc0: 2e63 6f6d 2f64 7364 616e 6965 6c70 6172  .com/dsdanielpar
-00001bd0: 6b2f 4578 6365 7074 4e6f 7469 6669 6572  k/ExceptNotifier
-00001be0: 2f62 6c6f 622f 6d61 696e 2f61 7373 6574  /blob/main/asset
-00001bf0: 732f 696d 6773 2f65 7831 2e70 6e67 290d  s/imgs/ex1.png).
-00001c00: 0a0d 0a3c 6272 3e0d 0a0d 0a23 2320 312d  ...<br>....## 1-
-00001c10: 322e 2041 4920 4465 6262 7567 6769 6e67  2. AI Debbugging
-00001c20: 2049 6e66 6f6d 6174 696f 6e20 4e6f 7469   Infomation Noti
-00001c30: 6669 6361 7469 6f6e 0d0a 596f 7520 6361  fication..You ca
-00001c40: 6e20 7265 6365 6976 6520 6465 6275 6767  n receive debugg
-00001c50: 696e 6720 696e 666f 726d 6174 696f 6e20  ing information 
-00001c60: 6672 6f6d 2043 6861 7447 5054 2076 6961  from ChatGPT via
-00001c70: 204f 7065 6e41 4927 7320 4150 4920 7768   OpenAI's API wh
-00001c80: 656e 2075 7369 6e67 2074 6865 2045 7863  en using the Exc
-00001c90: 6570 7420 7374 6174 656d 656e 742e 2054  ept statement. T
-00001ca0: 6865 2073 796e 7461 7820 7265 6d61 696e  he syntax remain
-00001cb0: 7320 7468 6520 7361 6d65 2c20 6275 7420  s the same, but 
-00001cc0: 796f 7527 6c6c 206e 6565 6420 746f 2063  you'll need to c
-00001cd0: 6f6e 6669 6775 7265 2074 6865 7365 2074  onfigure these t
-00001ce0: 776f 2076 6172 6961 626c 6573 3a0d 0a60  wo variables:..`
-00001cf0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 602c  _OPEN_AI_MODEL`,
-00001d00: 605f 4f50 454e 5f41 495f 4150 4960 0d0a  `_OPEN_AI_API`..
-00001d10: 0d0a 2a45 7861 6d70 6c65 2a0d 0a60 6060  ..*Example*..```
-00001d20: 7079 7468 6f6e 0d0a 6672 6f6d 2045 7863  python..from Exc
-00001d30: 6570 744e 6f74 6966 6965 7220 696d 706f  eptNotifier impo
-00001d40: 7274 2045 7863 6570 7454 656c 6765 7261  rt ExceptTelgera
-00001d50: 6d0d 0a5f 5445 4c45 4752 414d 5f54 4f4b  m.._TELEGRAM_TOK
-00001d60: 454e 203d 2022 7878 7878 220d 0a5f 4f50  EN = "xxxx".._OP
-00001d70: 454e 5f41 495f 4d4f 4445 4c3d 2267 7074  EN_AI_MODEL="gpt
-00001d80: 2d33 2e35 2d74 7572 626f 220d 0a5f 4f50  -3.5-turbo".._OP
-00001d90: 454e 5f41 495f 4150 493d 2273 6b2d 7878  EN_AI_API="sk-xx
-00001da0: 7878 7878 220d 0a0d 0a74 7279 3a0d 0a20  xxxx"....try:.. 
-00001db0: 2020 2070 7269 6e74 2831 2f30 290d 0a65     print(1/0)..e
-00001dc0: 7863 6570 7420 4578 6365 7074 5465 6c65  xcept ExceptTele
-00001dd0: 6772 616d 3a20 2320 7365 6e64 696e 6720  gram: # sending 
-00001de0: 6d73 6720 5749 5448 2041 4920 4445 4255  msg WITH AI DEBU
-00001df0: 4747 494e 4720 746f 2074 656c 6567 7261  GGING to telegra
-00001e00: 6d0d 0a20 2020 2073 7973 2e65 7869 7428  m..    sys.exit(
-00001e10: 290d 0a60 6060 0d0a 0d0a 215b 5d28 6874  )..```....![](ht
-00001e20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001e30: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
-00001e40: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
-00001e50: 622f 6d61 696e 2f61 7373 6574 732f 696d  b/main/assets/im
-00001e60: 6773 2f65 7832 2e70 6e67 290d 0a0d 0a3c  gs/ex2.png)....<
-00001e70: 6272 3e0d 0a0d 0a23 2320 312d 332e 2053  br>....## 1-3. S
-00001e80: 7563 6365 7373 605b 6170 704e 616d 655d  uccess`[appName]
-00001e90: 600d 0a42 7920 706c 6163 696e 6720 7468  `..By placing th
-00001ea0: 6520 7472 7920 6578 6365 7074 2069 6e20  e try except in 
-00001eb0: 7079 7468 6f6e 2061 7420 7468 6520 656e  python at the en
-00001ec0: 6420 6f66 2074 6865 2074 7279 2073 7461  d of the try sta
-00001ed0: 7465 6d65 6e74 2c20 6170 706c 6963 6174  tement, applicat
-00001ee0: 696f 6e73 2063 616e 2062 6520 6e6f 7469  ions can be noti
-00001ef0: 6669 6564 2074 6861 7420 7468 6520 7472  fied that the tr
-00001f00: 7920 7374 6174 656d 656e 7420 776f 726b  y statement work
-00001f10: 6564 206e 6f72 6d61 6c6c 792e 0d0a 6060  ed normally...``
-00001f20: 600d 0a53 7563 6365 7373 4368 696d 652c  `..SuccessChime,
-00001f30: 2053 7563 6365 7373 5465 6c65 6772 616d   SuccessTelegram
-00001f40: 2c20 5375 6363 6573 7344 6973 636f 7264  , SuccessDiscord
-00001f50: 2c20 5375 6363 6573 7353 4d53 2c20 5375  , SuccessSMS, Su
-00001f60: 6363 6573 734d 6169 6c2c 2053 7563 6365  ccessMail, Succe
-00001f70: 7373 4b61 6b61 6f2c 2053 7563 6365 7373  ssKakao, Success
-00001f80: 4c69 6e65 2c20 5375 6363 6573 7353 6c61  Line, SuccessSla
-00001f90: 636b 2c20 5375 6363 6573 7354 6561 6d73  ck, SuccessTeams
-00001fa0: 2c20 5375 6363 6573 7344 6573 6b74 6f70  , SuccessDesktop
-00001fb0: 652c 2053 7563 6365 7373 4265 6570 0d0a  e, SuccessBeep..
-00001fc0: 6060 600d 0a2a 4578 616d 706c 652a 0d0a  ```..*Example*..
-00001fd0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00001fe0: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
-00001ff0: 2069 6d70 6f72 7420 5375 6363 6573 7354   import SuccessT
-00002000: 656c 6765 7261 6d0d 0a5f 5445 4c45 4752  elgeram.._TELEGR
-00002010: 414d 5f54 4f4b 454e 203d 2022 7878 7878  AM_TOKEN = "xxxx
-00002020: 220d 0a0d 0a74 7279 3a0d 0a20 2020 2070  "....try:..    p
-00002030: 7269 6e74 2831 2f32 3029 0d0a 2020 2020  rint(1/20)..    
-00002040: 5375 6363 6573 7354 656c 6765 7261 6d28  SuccessTelgeram(
-00002050: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2320  ).__call__()  # 
-00002060: 7365 6e64 696e 6720 7375 6363 6573 7320  sending success 
-00002070: 6d65 7373 6167 6520 746f 2074 656c 6567  message to teleg
-00002080: 7261 6d0d 0a65 7863 6570 743a 0d0a 2020  ram..except:..  
-00002090: 2020 7379 732e 6578 6974 2829 0d0a 6060    sys.exit()..``
-000020a0: 600d 0a0d 0a21 5b5d 2868 7474 7073 3a2f  `....![](https:/
-000020b0: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
-000020c0: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
-000020d0: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
-000020e0: 6e2f 6173 7365 7473 2f69 6d67 732f 6578  n/assets/imgs/ex
-000020f0: 332e 706e 6729 0d0a 0d0a 3c42 723e 0d0a  3.png)....<Br>..
-00002100: 0d0a 2323 2031 2d34 2e20 5365 6e64 605b  ..## 1-4. Send`[
-00002110: 6170 704e 616d 655d 600d 0a50 6c61 6365  appName]`..Place
-00002120: 2069 7420 616e 7977 6865 7265 206f 6e20   it anywhere on 
-00002130: 7468 6520 6c69 6e65 206f 6620 636f 6465  the line of code
-00002140: 2079 6f75 2077 616e 742c 2061 6e64 2079   you want, and y
-00002150: 6f75 276c 6c20 6265 206e 6f74 6966 6965  ou'll be notifie
-00002160: 6420 7768 656e 2074 6861 7420 6c69 6e65  d when that line
-00002170: 206f 6620 636f 6465 2069 7320 7265 6163   of code is reac
-00002180: 6865 642e 0d0a 6060 600d 0a53 656e 6443  hed...```..SendC
-00002190: 6869 6d65 2c20 5365 6e64 5465 6c65 6772  hime, SendTelegr
-000021a0: 616d 2c20 5365 6e64 4469 7363 6f72 642c  am, SendDiscord,
-000021b0: 2053 656e 6453 4d53 2c20 5365 6e64 4d61   SendSMS, SendMa
-000021c0: 696c 2c20 5365 6e64 4b61 6b61 6f2c 2053  il, SendKakao, S
-000021d0: 656e 644c 696e 652c 2053 656e 6453 6c61  endLine, SendSla
-000021e0: 636b 2c20 5365 6e64 5465 616d 732c 2053  ck, SendTeams, S
-000021f0: 656e 6444 6573 6b74 6f70 652c 2053 656e  endDesktope, Sen
-00002200: 6442 6565 700d 0a60 6060 0d0a 2a45 7861  dBeep..```..*Exa
-00002210: 6d70 6c65 2a0d 0a0d 0a60 6060 7079 7468  mple*....```pyth
-00002220: 6f6e 0d0a 6672 6f6d 2045 7863 6570 744e  on..from ExceptN
-00002230: 6f74 6966 6965 7220 696d 706f 7274 2053  otifier import S
-00002240: 656e 6454 656c 6765 7261 6d0d 0a5f 5445  endTelgeram.._TE
-00002250: 4c45 4752 414d 5f54 4f4b 454e 203d 2022  LEGRAM_TOKEN = "
-00002260: 7878 7878 220d 0a0d 0a53 656e 6454 656c  xxxx"....SendTel
-00002270: 6567 7261 6d28 292e 5f5f 6361 6c6c 5f5f  egram().__call__
-00002280: 2829 2023 2073 656e 6469 6e67 206d 6573  () # sending mes
-00002290: 7361 6765 2074 6f20 7465 6c65 6772 616d  sage to telegram
-000022a0: 0d0a 0d0a 6e6f 7469 203d 2053 656e 6454  ....noti = SendT
-000022b0: 656c 6567 7261 6d28 290d 0a6e 6f74 6928  elegram()..noti(
-000022c0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-000022d0: 2020 2020 2023 2073 656e 6469 6e67 206d       # sending m
-000022e0: 6573 7361 6765 2074 6f20 7465 6c65 6772  essage to telegr
-000022f0: 616d 0d0a 6060 600d 0a0d 0a21 5b5d 2868  am..```....![](h
-00002300: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002310: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00002320: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00002330: 6f62 2f6d 6169 6e2f 6173 7365 7473 2f69  ob/main/assets/i
-00002340: 6d67 732f 6578 342e 706e 6729 0d0a 0d0a  mgs/ex4.png)....
-00002350: 0d0a 3c62 723e 3c62 723e 0d0a 0d0a 2320  ..<br><br>....# 
-00002360: 322e 2046 6561 7475 7265 730d 0a59 6f75  2. Features..You
-00002370: 2063 616e 2072 6563 6569 7665 2064 6562   can receive deb
-00002380: 7567 6769 6e67 2069 6e66 6f72 6d61 7469  ugging informati
-00002390: 6f6e 2066 726f 6d20 4368 6174 4750 5420  on from ChatGPT 
-000023a0: 7669 6120 4f70 656e 4149 2773 2041 5049  via OpenAI's API
-000023b0: 2077 6865 6e20 7573 696e 6720 7468 6520   when using the 
-000023c0: 4578 6365 7074 2073 7461 7465 6d65 6e74  Except statement
-000023d0: 2e20 5468 6520 7379 6e74 6178 2072 656d  . The syntax rem
-000023e0: 6169 6e73 2074 6865 2073 616d 652c 2062  ains the same, b
-000023f0: 7574 2079 6f75 276c 6c20 6e65 6564 2074  ut you'll need t
-00002400: 6f20 636f 6e66 6967 7572 6520 7468 6573  o configure thes
-00002410: 6520 7477 6f20 7661 7269 6162 6c65 733a  e two variables:
-00002420: 0d0a 605f 4f50 454e 5f41 495f 4d4f 4445  ..`_OPEN_AI_MODE
-00002430: 4c60 2c60 5f4f 5045 4e5f 4149 5f41 5049  L`,`_OPEN_AI_API
-00002440: 600d 0a0d 0a0d 0a0d 0a23 2320 322d 312e  `........## 2-1.
-00002450: 202a 5465 6c65 6772 616d 204e 6f74 6966   *Telegram Notif
-00002460: 6965 722a 0d0a 0d0a 2d20 612e 204f 7065  ier*....- a. Ope
-00002470: 6e20 796f 7572 2074 656c 6567 7261 6d20  n your telegram 
-00002480: 6170 7020 616e 6420 7365 6172 6368 2066  app and search f
-00002490: 6f72 2042 6f74 4661 7468 6572 2e20 2841  or BotFather. (A
-000024a0: 2062 7569 6c74 2d69 6e20 5465 6c65 6772   built-in Telegr
-000024b0: 616d 2062 6f74 2074 6861 7420 6865 6c70  am bot that help
-000024c0: 7320 7573 6572 7320 6372 6561 7465 2063  s users create c
-000024d0: 7573 746f 6d20 5465 6c65 6772 616d 2062  ustom Telegram b
-000024e0: 6f74 7329 203c 6272 3e0d 0a2d 2062 2e20  ots) <br>..- b. 
-000024f0: 5479 7065 202f 6e65 7762 6f74 2074 6f20  Type /newbot to 
-00002500: 6372 6561 7465 2061 206e 6577 2062 6f74  create a new bot
-00002510: 203c 6272 3e0d 0a2d 2063 2e20 4769 7665   <br>..- c. Give
-00002520: 2079 6f75 7220 626f 7420 6120 6e61 6d65   your bot a name
-00002530: 2026 2061 2075 7365 726e 616d 6520 3c62   & a username <b
-00002540: 723e 0d0a 2d20 642e 2043 6f70 7920 796f  r>..- d. Copy yo
-00002550: 7572 206e 6577 2054 656c 6567 7261 6d20  ur new Telegram 
-00002560: 626f 74e2 8099 7320 746f 6b65 6e20 3c62  bot...s token <b
-00002570: 723e 0d0a 0d0a 466f 7220 6d6f 7265 2069  r>....For more i
-00002580: 6e66 6f6d 6174 696f 6e2c 2076 6973 6974  nfomation, visit
-00002590: 205b 5465 6c65 6772 616d 2042 6f74 2046   [Telegram Bot F
-000025a0: 6174 6865 7220 4150 495d 2868 7474 7073  ather API](https
-000025b0: 3a2f 2f63 6f72 652e 7465 6c65 6772 616d  ://core.telegram
-000025c0: 2e6f 7267 2f62 6f74 732f 6170 6929 0d0a  .org/bots/api)..
-000025d0: 3c62 723e 3c62 723e 0d0a 200d 0a23 2323  <br><br>.. ..###
-000025e0: 2061 2e20 5769 7468 6f75 7420 4f70 656e   a. Without Open
-000025f0: 4149 2041 5049 0d0a 0d0a 6060 6070 7974  AI API....```pyt
-00002600: 686f 6e0d 0a66 726f 6d20 4578 6365 7074  hon..from Except
-00002610: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
-00002620: 4578 6365 7074 5465 6c65 6772 616d 2c20  ExceptTelegram, 
-00002630: 5375 6363 6573 7354 656c 6567 7261 6d2c  SuccessTelegram,
-00002640: 2053 656e 6454 656c 6567 7261 6d0d 0a69   SendTelegram..i
-00002650: 6d70 6f72 7420 7379 730d 0a73 7973 2e65  mport sys..sys.e
-00002660: 7863 6570 7468 6f6f 6b20 3d20 4578 6365  xcepthook = Exce
-00002670: 7074 5465 6c65 6772 616d 2e5f 5f63 616c  ptTelegram.__cal
-00002680: 6c5f 5f0d 0a0d 0a5f 5445 4c45 4752 414d  l__...._TELEGRAM
-00002690: 5f54 4f4b 454e 203d 2022 7878 7878 220d  _TOKEN = "xxxx".
-000026a0: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
-000026b0: 6e74 2831 2f30 2920 200d 0a20 2020 2053  nt(1/0)  ..    S
-000026c0: 7563 6365 7373 5465 6c65 6772 616d 2829  uccessTelegram()
-000026d0: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2e20  .__call__() #1. 
-000026e0: 7375 6363 6573 7320 7365 6e64 6572 2020  success sender  
-000026f0: 2020 2020 2020 2020 0d0a 0d0a 6578 6365          ....exce
-00002700: 7074 2045 7863 6570 7454 656c 6567 7261  pt ExceptTelegra
-00002710: 6d20 6173 2065 3a20 2020 2020 2023 322e  m as e:      #2.
-00002720: 2065 7863 6570 7420 7365 6e64 6572 2020   except sender  
-00002730: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002740: 7379 732e 6578 6974 2829 0d0a 0d0a 5365  sys.exit()....Se
-00002750: 6e64 5465 6c65 6772 616d 2829 2e5f 5f63  ndTelegram().__c
-00002760: 616c 6c5f 5f28 2920 2020 2020 2020 2023  all__()        #
-00002770: 332e 2063 7573 746f 6d69 7a65 6420 7365  3. customized se
-00002780: 6e64 6572 2020 2020 200d 0a60 6060 0d0a  nder     ..```..
-00002790: 0d0a 0d0a 215b 5d28 6874 7470 733a 2f2f  ....![](https://
-000027a0: 6769 7468 7562 2e63 6f6d 2f64 7364 616e  github.com/dsdan
-000027b0: 6965 6c70 6172 6b2f 4578 6365 7074 4e6f  ielpark/ExceptNo
-000027c0: 7469 6669 6572 2f62 6c6f 622f 6d61 696e  tifier/blob/main
-000027d0: 2f61 7373 6574 732f 696d 6773 2f66 6967  /assets/imgs/fig
-000027e0: 3434 2e70 6e67 290d 0a0d 0a0d 0a23 2323  44.png)......###
-000027f0: 2062 2e20 5769 7468 204f 7065 6e41 4920   b. With OpenAI 
-00002800: 4150 490d 0a60 6060 7079 7468 6f6e 0d0a  API..```python..
-00002810: 6672 6f6d 2045 7863 6570 744e 6f74 6966  from ExceptNotif
-00002820: 6965 7220 696d 706f 7274 2045 7863 6570  ier import Excep
-00002830: 7454 656c 6567 7261 6d2c 2053 7563 6365  tTelegram, Succe
-00002840: 7373 5465 6c65 6772 616d 2c20 5365 6e64  ssTelegram, Send
-00002850: 5465 6c65 6772 616d 0d0a 696d 706f 7274  Telegram..import
-00002860: 2073 7973 0d0a 7379 732e 6578 6365 7074   sys..sys.except
-00002870: 686f 6f6b 203d 2045 7863 6570 7454 656c  hook = ExceptTel
-00002880: 6567 7261 6d2e 5f5f 6361 6c6c 5f5f 0d0a  egram.__call__..
-00002890: 0d0a 5f54 454c 4547 5241 4d5f 544f 4b45  .._TELEGRAM_TOKE
-000028a0: 4e20 3d20 2278 7878 7822 0d0a 5f4f 5045  N = "xxxx".._OPE
-000028b0: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-000028c0: 332e 352d 7475 7262 6f22 0d0a 5f4f 5045  3.5-turbo".._OPE
-000028d0: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
-000028e0: 7878 7822 0d0a 0d0a 7472 793a 0d0a 2020  xxx"....try:..  
-000028f0: 2020 7072 696e 7428 312f 3029 2020 0d0a    print(1/0)  ..
-00002900: 2020 2020 5375 6363 6573 7354 656c 6567      SuccessTeleg
-00002910: 7261 6d28 292e 5f5f 6361 6c6c 5f5f 2829  ram().__call__()
-00002920: 2023 312e 2073 7563 6365 7373 2073 656e   #1. success sen
-00002930: 6465 7220 2020 2020 2020 2020 200d 0a0d  der          ...
-00002940: 0a65 7863 6570 7420 4578 6365 7074 5465  .except ExceptTe
-00002950: 6c65 6772 616d 2061 7320 653a 2020 2020  legram as e:    
-00002960: 2020 2332 2e20 6578 6365 7074 2073 656e    #2. except sen
-00002970: 6465 7220 2020 2020 2020 2020 2020 200d  der            .
-00002980: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
-00002990: 0a0d 0a53 656e 6454 656c 6567 7261 6d28  ...SendTelegram(
-000029a0: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
-000029b0: 2020 2020 2333 2e20 6375 7374 6f6d 697a      #3. customiz
-000029c0: 6564 2073 656e 6465 7220 2020 2020 0d0a  ed sender     ..
-000029d0: 0d0a 6060 600d 0a3c 6272 3e0d 0a0d 0a23  ..```..<br>....#
-000029e0: 2320 322d 322e 202a 4d61 696c 204e 6f74  # 2-2. *Mail Not
-000029f0: 6966 6965 722a 0d0a 496e 2074 6865 2065  ifier*..In the e
-00002a00: 7863 6570 7420 7374 6174 656d 656e 742c  xcept statement,
-00002a10: 2061 6e20 656d 6169 6c20 6973 2073 656e   an email is sen
-00002a20: 7420 616c 6f6e 6720 7769 7468 2074 6865  t along with the
-00002a30: 2065 7272 6f72 206d 6573 7361 6765 2e20   error message. 
-00002a40: 4164 6469 7469 6f6e 616c 6c79 2c20 796f  Additionally, yo
-00002a50: 7520 6361 6e20 7365 6e64 2065 6d61 696c  u can send email
-00002a60: 7320 6672 6f6d 2061 6e79 2064 6573 6972  s from any desir
-00002a70: 6564 206c 696e 652e 203c 6272 3e0d 0a2d  ed line. <br>..-
-00002a80: 2061 2e20 4c6f 6720 696e 2077 6974 6820   a. Log in with 
-00002a90: 7468 6520 7365 6e64 6572 2773 2065 6d61  the sender's ema
-00002aa0: 696c 2049 442e 203c 6272 3e0d 0a2d 2062  il ID. <br>..- b
-00002ab0: 2e20 4f62 7461 696e 2061 6e20 6170 7020  . Obtain an app 
-00002ac0: 7061 7373 776f 7264 2066 6f72 2073 656e  password for sen
-00002ad0: 6469 6e67 2047 6f6f 676c 6520 4d61 696c  ding Google Mail
-00002ae0: 2061 7420 7468 6520 666f 6c6c 6f77 696e   at the followin
-00002af0: 6720 5b6c 696e 6b5d 2868 7474 7073 3a2f  g [link](https:/
-00002b00: 2f6d 7961 6363 6f75 6e74 2e67 6f6f 676c  /myaccount.googl
-00002b10: 652e 636f 6d2f 752f 332f 6170 7070 6173  e.com/u/3/apppas
-00002b20: 7377 6f72 6473 3f75 746d 5f73 6f75 7263  swords?utm_sourc
-00002b30: 653d 676f 6f67 6c65 2d61 6363 6f75 6e74  e=google-account
-00002b40: 2675 746d 5f6d 6564 6975 6d3d 6d79 6163  &utm_medium=myac
-00002b50: 636f 756e 7473 6563 7572 6974 7926 7574  countsecurity&ut
-00002b60: 6d5f 6361 6d70 6169 676e 3d74 7376 2d73  m_campaign=tsv-s
-00002b70: 6574 7469 6e67 7326 7261 7074 3d41 456a  ettings&rapt=AEj
-00002b80: 484c 344e 3262 4d52 574f 3436 5661 4d70  HL4N2bMRWO46VaMp
-00002b90: 5f6a 5030 367a 514b 3134 4257 4e50 7636  _jP06zQK14BWNPv6
-00002ba0: 366c 326f 3539 694a 3939 436b 4f38 426a  6l2o59iJ99CkO8Bj
-00002bb0: 596e 6d6f 5255 6539 6474 5363 686b 6b62  YnmoRUe9dtSchkkb
-00002bc0: 7562 485a 4d55 6865 766b 416e 7756 4a52  ubHZMUhevkAnwVJR
-00002bd0: 4862 3979 674f 3361 6669 7370 4e6c 7729  Hb9ygO3afispNlw)
-00002be0: 206f 7220 5b67 6f6f 676c 6520 646f 6375   or [google docu
-00002bf0: 6d65 6e74 5d28 6874 7470 733a 2f2f 7375  ment](https://su
-00002c00: 7070 6f72 742e 676f 6f67 6c65 2e63 6f6d  pport.google.com
-00002c10: 2f61 6363 6f75 6e74 732f 616e 7377 6572  /accounts/answer
-00002c20: 2f31 3835 3833 333f 686c 3d65 6e29 2e20  /185833?hl=en). 
-00002c30: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00002c40: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00002c50: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00002c60: 6d70 6f72 7420 4578 6365 7074 4d61 696c  mport ExceptMail
-00002c70: 2c20 5375 6363 6573 734d 6169 6c2c 2053  , SuccessMail, S
-00002c80: 656e 644d 6169 6c0d 0a73 7973 2e65 7863  endMail..sys.exc
-00002c90: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
-00002ca0: 4d61 696c 2e5f 5f63 616c 6c5f 5f0d 0a0d  Mail.__call__...
-00002cb0: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
-00002cc0: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
-00002cd0: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
-00002ce0: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
-00002cf0: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
-00002d00: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
-00002d10: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
-00002d20: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
-00002d30: 7878 7878 7822 0d0a 5f47 414d 494c 5f52  xxxxx".._GAMIL_R
-00002d40: 4543 4950 4945 4e54 5f41 4444 5220 3d20  ECIPIENT_ADDR = 
-00002d50: 2778 7878 7878 7878 4067 6d61 696c 2e63  'xxxxxxx@gmail.c
-00002d60: 6f6d 270d 0a5f 474d 4149 4c5f 5345 4e44  om'.._GMAIL_SEND
-00002d70: 4552 5f41 4444 5220 3d20 2779 7979 7979  ER_ADDR = 'yyyyy
-00002d80: 7940 676d 6169 6c2e 636f 6d27 0d0a 5f47  y@gmail.com'.._G
-00002d90: 4d41 494c 5f41 5050 5f50 4153 5357 4f52  MAIL_APP_PASSWOR
-00002da0: 445f 4f46 5f53 454e 4445 5220 3d20 277a  D_OF_SENDER = 'z
-00002db0: 7a7a 7a7a 7a27 0d0a 0d0a 7472 793a 0d0a  zzzzz'....try:..
-00002dc0: 2020 2020 6d61 696e 2829 2020 2020 2020      main()      
-00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2320 596f 7572 2043 6f64 6520 4865 7265  # Your Code Here
-00002df0: 0d0a 2020 2020 5375 6363 6573 734d 6169  ..    SuccessMai
-00002e00: 6c28 292e 5f5f 6361 6c6c 5f5f 2829 2020  l().__call__()  
-00002e10: 2020 2320 4e6f 2045 7863 6570 7469 6f6e    # No Exception
-00002e20: 202d 3e20 5365 6e64 2053 7563 6365 7373   -> Send Success
-00002e30: 206d 6169 6c2e 0d0a 6578 6365 7074 2045   mail...except E
-00002e40: 7863 6570 744d 6169 6c3a 2020 2020 2020  xceptMail:      
-00002e50: 2020 2020 2020 2020 2320 4578 6365 7074          # Except
-00002e60: 696f 6e20 2d3e 2053 656e 6420 4661 696c  ion -> Send Fail
-00002e70: 206d 6169 6c2e 0d0a 2020 2020 7061 7373   mail...    pass
-00002e80: 0d0a 0d0a 5365 6e64 4d61 696c 2829 2e5f  ....SendMail()._
-00002e90: 5f63 616c 6c5f 5f28 2920 2020 2020 2020  _call__()       
-00002ea0: 2020 2020 2320 5768 656e 2050 726f 6365      # When Proce
-00002eb0: 7373 2045 6e64 6564 202d 3e20 416e 7920  ss Ended -> Any 
-00002ec0: 4c69 6e65 206d 6169 6c2e 0d0a 6060 600d  Line mail...```.
-00002ed0: 0a0d 0a3c 6465 7461 696c 733e 0d0a 3c73  ...<details>..<s
-00002ee0: 756d 6d61 7279 3e20 5365 6520 4578 616d  ummary> See Exam
-00002ef0: 706c 652e 2e2e 3c2f 7375 6d6d 6172 793e  ple...</summary>
-00002f00: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00002f10: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00002f20: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00002f30: 6d70 6f72 7420 4578 6365 7074 4d61 696c  mport ExceptMail
-00002f40: 2c20 5375 6363 6573 734d 6169 6c2c 2053  , SuccessMail, S
-00002f50: 656e 644d 6169 6c0d 0a0d 0a23 2044 6566  endMail....# Def
-00002f60: 696e 6520 7468 6520 6e65 7874 2074 776f  ine the next two
-00002f70: 2076 6172 6961 626c 6573 206f 7074 696f   variables optio
-00002f80: 6e61 6c6c 7920 7768 656e 2075 7369 6e67  nally when using
-00002f90: 204f 7065 6e41 4927 7320 4150 492e 0d0a   OpenAI's API...
-00002fa0: 2320 5f4f 5045 4e5f 4149 5f4d 4f44 454c  # _OPEN_AI_MODEL
-00002fb0: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
-00002fc0: 2020 2020 0d0a 2320 5f4f 5045 4e5f 4149      ..# _OPEN_AI
-00002fd0: 5f41 5049 3d22 736b 2d78 7878 7878 7822  _API="sk-xxxxxx"
-00002fe0: 0d0a 5f47 414d 494c 5f52 4543 4950 4945  .._GAMIL_RECIPIE
-00002ff0: 4e54 5f41 4444 5220 3d20 2778 7878 7878  NT_ADDR = 'xxxxx
-00003000: 7878 4067 6d61 696c 2e63 6f6d 270d 0a5f  xx@gmail.com'.._
-00003010: 474d 4149 4c5f 5345 4e44 4552 5f41 4444  GMAIL_SENDER_ADD
-00003020: 5220 3d20 2779 7979 7979 7940 676d 6169  R = 'yyyyyy@gmai
-00003030: 6c2e 636f 6d27 0d0a 5f47 4d41 494c 5f41  l.com'.._GMAIL_A
-00003040: 5050 5f50 4153 5357 4f52 445f 4f46 5f53  PP_PASSWORD_OF_S
-00003050: 454e 4445 5220 3d20 277a 7a7a 7a7a 7a27  ENDER = 'zzzzzz'
-00003060: 0d0a 0d0a 7379 732e 6578 6365 7074 686f  ....sys.exceptho
-00003070: 6f6b 203d 2045 7863 6570 744d 6169 6c2e  ok = ExceptMail.
-00003080: 5f5f 6361 6c6c 5f5f 0d0a 0d0a 7472 793a  __call__....try:
-00003090: 0d0a 2020 2020 2320 3032 2e4c 6f63 6174  ..    # 02.Locat
-000030a0: 6520 796f 7572 2063 6f64 650d 0a20 2020  e your code..   
-000030b0: 2070 7269 6e74 2831 2f30 2920 2020 0d0a   print(1/0)   ..
-000030c0: 2020 2020 5375 6363 6573 734d 6169 6c28      SuccessMail(
-000030d0: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2023  ).__call__()   #
-000030e0: 2053 7563 6365 7373 204d 6169 6c0d 0a0d   Success Mail...
-000030f0: 0a65 7863 6570 7420 4578 6365 7074 4d61  .except ExceptMa
-00003100: 696c 2061 7320 653a 2020 2020 2020 2020  il as e:        
-00003110: 2320 4578 6365 7074 696f 6e20 4d61 696c  # Exception Mail
-00003120: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-00003130: 2e65 7869 7428 290d 0a20 2020 2070 7269  .exit()..    pri
-00003140: 6e74 2865 290d 0a0d 0a53 656e 644d 6169  nt(e)....SendMai
-00003150: 6c28 292e 5f5f 6361 6c6c 5f5f 2829 2020  l().__call__()  
-00003160: 2020 2020 2020 2020 2320 5075 7420 416e          # Put An
-00003170: 7920 4c69 6e65 3a20 5365 6e64 696e 6720  y Line: Sending 
-00003180: 6d61 696c 0d0a 6060 600d 0a3c 2f64 6574  mail..```..</det
-00003190: 6169 6c73 3e0d 0a0d 0a3c 6465 7461 696c  ails>....<detail
-000031a0: 733e 0d0a 3c73 756d 6d61 7279 3e20 536e  s>..<summary> Sn
-000031b0: 6970 7065 7420 666f 7220 5079 7468 6f6e  ippet for Python
-000031c0: 2064 6576 656c 6f70 6572 732e 2e2e 3c2f   developers...</
-000031d0: 7375 6d6d 6172 793e 0d0a 0d0a 6060 6070  summary>....```p
-000031e0: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
-000031f0: 730d 0a66 726f 6d20 4578 6365 7074 4e6f  s..from ExceptNo
-00003200: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
-00003210: 6365 7074 4d61 696c 2c20 5375 6363 6573  ceptMail, Succes
-00003220: 734d 6169 6c2c 2053 656e 644d 6169 6c0d  sMail, SendMail.
-00003230: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
-00003240: 3d20 4578 6365 7074 4d61 696c 2e5f 5f63  = ExceptMail.__c
-00003250: 616c 6c5f 5f0d 0a0d 0a23 2044 6566 696e  all__....# Defin
-00003260: 6520 7468 6520 6e65 7874 2074 776f 2076  e the next two v
-00003270: 6172 6961 626c 6573 206f 7074 696f 6e61  ariables optiona
-00003280: 6c6c 7920 7768 656e 2075 7369 6e67 204f  lly when using O
-00003290: 7065 6e41 4927 7320 4150 492e 0d0a 2320  penAI's API...# 
-000032a0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 3d22  _OPEN_AI_MODEL="
-000032b0: 6770 742d 332e 352d 7475 7262 6f22 2020  gpt-3.5-turbo"  
-000032c0: 2020 0d0a 2320 5f4f 5045 4e5f 4149 5f41    ..# _OPEN_AI_A
-000032d0: 5049 3d22 736b 2d78 7878 7878 7822 0d0a  PI="sk-xxxxxx"..
-000032e0: 5f47 414d 494c 5f52 4543 4950 4945 4e54  _GAMIL_RECIPIENT
-000032f0: 5f41 4444 5220 3d20 2778 7878 7878 7878  _ADDR = 'xxxxxxx
-00003300: 4067 6d61 696c 2e63 6f6d 270d 0a5f 474d  @gmail.com'.._GM
-00003310: 4149 4c5f 5345 4e44 4552 5f41 4444 5220  AIL_SENDER_ADDR 
-00003320: 3d20 2779 7979 7979 7940 676d 6169 6c2e  = 'yyyyyy@gmail.
-00003330: 636f 6d27 0d0a 5f47 4d41 494c 5f41 5050  com'.._GMAIL_APP
-00003340: 5f50 4153 5357 4f52 445f 4f46 5f53 454e  _PASSWORD_OF_SEN
-00003350: 4445 5220 3d20 277a 7a7a 7a7a 7a27 0d0a  DER = 'zzzzzz'..
-00003360: 0d0a 7472 793a 0d0a 2020 2020 2779 6f75  ..try:..    'you
-00003370: 7220 636f 6465 270d 0a20 2020 2053 7563  r code'..    Suc
-00003380: 6365 7373 4d61 696c 2829 2e5f 5f63 616c  cessMail().__cal
-00003390: 6c5f 5f28 290d 0a65 7863 6570 7420 4578  l__()..except Ex
-000033a0: 6365 7074 4d61 696c 3a0d 0a20 2020 2070  ceptMail:..    p
-000033b0: 6173 730d 0a0d 0a53 656e 644d 6169 6c28  ass....SendMail(
-000033c0: 292e 5f5f 6361 6c6c 5f5f 2829 200d 0a60  ).__call__() ..`
-000033d0: 6060 0d0a 3c2f 6465 7461 696c 733e 0d0a  ``..</details>..
-000033e0: 0d0a 3c62 723e 0d0a 0d0a 2323 2032 2d33  ..<br>....## 2-3
-000033f0: 2e20 2a44 6973 636f 7264 204e 6f74 6966  . *Discord Notif
-00003400: 6965 722a 0d0a 2d20 612e 2053 656c 6563  ier*..- a. Selec
-00003410: 7420 7468 6520 6368 616e 6e65 6c20 746f  t the channel to
-00003420: 2072 6563 6569 7665 206e 6f74 6966 6963   receive notific
-00003430: 6174 696f 6e73 2e0d 0a2d 2062 2e20 436c  ations...- b. Cl
-00003440: 6963 6b20 2245 6469 7420 4368 616e 6e65  ick "Edit Channe
-00003450: 6c22 2069 6e20 7468 6520 7570 7065 7220  l" in the upper 
-00003460: 7269 6768 7420 636f 726e 6572 206f 6620  right corner of 
-00003470: 7468 6520 6368 6174 2077 696e 646f 772e  the chat window.
-00003480: 0d0a 2d20 632e 2043 6c69 636b 2049 6e74  ..- c. Click Int
-00003490: 6567 7261 7469 6f6e 7320 2d20 5765 6268  egrations - Webh
-000034a0: 6f6f 6b20 2d20 4e65 7720 5765 6268 6f6f  ook - New Webhoo
-000034b0: 6b2e 0d0a 2d20 642e 2054 6865 6e20 636c  k...- d. Then cl
-000034c0: 6963 6b20 436f 7079 2057 6562 686f 6f6b  ick Copy Webhook
-000034d0: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
-000034e0: 696d 706f 7274 2073 7973 0d0a 6672 6f6d  import sys..from
-000034f0: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
-00003500: 696d 706f 7274 2045 7863 6570 7444 6973  import ExceptDis
-00003510: 636f 7264 2c20 5375 6363 6573 7344 6973  cord, SuccessDis
-00003520: 636f 7264 2c20 5365 6e64 4469 7363 6f72  cord, SendDiscor
-00003530: 640d 0a73 7973 2e65 7863 6570 7468 6f6f  d..sys.excepthoo
-00003540: 6b20 3d20 4578 6365 7074 4469 7363 6f72  k = ExceptDiscor
-00003550: 642e 5f5f 6361 6c6c 5f5f 0d0a 0d0a 2320  d.__call__....# 
-00003560: 4465 6669 6e65 2074 6865 206e 6578 7420  Define the next 
-00003570: 7477 6f20 7661 7269 6162 6c65 7320 6f70  two variables op
-00003580: 7469 6f6e 616c 6c79 2077 6865 6e20 7573  tionally when us
-00003590: 696e 6720 4f70 656e 4149 2773 2041 5049  ing OpenAI's API
-000035a0: 2e0d 0a23 205f 4f50 454e 5f41 495f 4d4f  ...# _OPEN_AI_MO
-000035b0: 4445 4c3d 2267 7074 2d33 2e35 2d74 7572  DEL="gpt-3.5-tur
-000035c0: 626f 2220 2020 200d 0a23 205f 4f50 454e  bo"    ..# _OPEN
-000035d0: 5f41 495f 4150 493d 2273 6b2d 7878 7878  _AI_API="sk-xxxx
-000035e0: 7878 220d 0a5f 4449 5343 4f52 445f 5745  xx".._DISCORD_WE
-000035f0: 4248 4f4f 4b5f 5552 4c20 3d20 2278 7878  BHOOK_URL = "xxx
-00003600: 7878 7878 7878 7878 7878 7878 7878 220d  xxxxxxxxxxxxxx".
-00003610: 0a0d 0a0d 0a74 7279 3a0d 0a20 2020 2070  .....try:..    p
-00003620: 7269 6e74 2831 2f32 3029 2020 0d0a 2020  rint(1/20)  ..  
-00003630: 2020 5375 6363 6573 7344 6973 636f 7264    SuccessDiscord
-00003640: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2331  ().__call__() #1
-00003650: 2073 7563 6365 7373 2073 656e 6465 7220   success sender 
-00003660: 2020 2020 2020 2020 200d 0a65 7863 6570           ..excep
-00003670: 7420 4578 6365 7074 4469 7363 6f72 6420  t ExceptDiscord 
-00003680: 6173 2065 3a20 2020 2020 2023 3220 6578  as e:      #2 ex
-00003690: 6365 7074 2073 656e 6465 7220 2020 2020  cept sender     
-000036a0: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-000036b0: 2e65 7869 7428 290d 0a0d 0a53 656e 6444  .exit()....SendD
-000036c0: 6973 636f 7264 2829 2e5f 5f63 616c 6c5f  iscord().__call_
-000036d0: 5f28 2920 2020 2020 2020 2023 3320 6375  _()        #3 cu
-000036e0: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
-000036f0: 2020 2020 2020 0d0a 6060 600d 0a0d 0a3c        ..```....<
-00003700: 6272 3e0d 0a0d 0a23 2320 322d 342e 202a  br>....## 2-4. *
-00003710: 4368 696d 6520 4e6f 7469 6669 6572 2a0d  Chime Notifier*.
-00003720: 0a2d 2061 2e20 5365 6c65 6374 2074 6865  .- a. Select the
-00003730: 2043 6861 7420 726f 6f6d 2074 6f20 7265   Chat room to re
-00003740: 6365 6976 6520 6e6f 7469 6669 6361 7469  ceive notificati
-00003750: 6f6e 732e 0d0a 2d20 622e 2043 6c69 636b  ons...- b. Click
-00003760: 2022 526f 6f6d 2053 6574 7469 6e67 2220   "Room Setting" 
-00003770: 696e 2074 6865 2075 7070 6572 2072 6967  in the upper rig
-00003780: 6874 2063 6f72 6e65 722e 0d0a 2d20 632e  ht corner...- c.
-00003790: 2043 6c69 636b 2022 4d61 6e61 6765 2057   Click "Manage W
-000037a0: 6562 686f 6f6b 2061 6e64 2062 6f74 2e22  ebhook and bot."
-000037b0: 0d0a 2d20 642e 2043 7265 6174 6520 4164  ..- d. Create Ad
-000037c0: 6420 5765 6268 6f6f 6b2c 2073 6574 2069  d Webhook, set i
-000037d0: 7420 7570 2c20 7468 656e 2063 6c69 636b  t up, then click
-000037e0: 2043 6f70 7920 5765 6268 6f6f 6b2e 0d0a   Copy Webhook...
-000037f0: 6060 6070 7974 686f 6e0d 0a69 6d70 6f72  ```python..impor
-00003800: 7420 7379 730d 0a66 726f 6d20 4578 6365  t sys..from Exce
-00003810: 7074 4e6f 7469 6669 6572 2069 6d70 6f72  ptNotifier impor
-00003820: 7420 5375 6363 6573 7343 6869 6d65 2c20  t SuccessChime, 
-00003830: 4578 6365 7074 4368 696d 652c 2053 656e  ExceptChime, Sen
-00003840: 6443 6869 6d65 0d0a 7379 732e 6578 6365  dChime..sys.exce
-00003850: 7074 686f 6f6b 203d 2045 7863 6570 7443  pthook = ExceptC
-00003860: 6869 6d65 2e5f 5f63 616c 6c5f 5f0d 0a0d  hime.__call__...
-00003870: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
-00003880: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
-00003890: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
-000038a0: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
-000038b0: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
-000038c0: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
-000038d0: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
-000038e0: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
-000038f0: 7878 7878 7822 0d0a 5f43 4849 4d45 5f57  xxxxx".._CHIME_W
-00003900: 4542 484f 4f4b 5f55 524c 203d 2022 7878  EBHOOK_URL = "xx
-00003910: 7878 7878 7878 7878 7878 7878 7878 7878  xxxxxxxxxxxxxxxx
-00003920: 220d 0a0d 0a0d 0a74 7279 3a0d 0a20 2020  "......try:..   
-00003930: 2070 7269 6e74 2831 2f30 2920 200d 0a20   print(1/0)  .. 
-00003940: 2020 2053 7563 6365 7373 4368 696d 6528     SuccessChime(
-00003950: 292e 5f5f 6361 6c6c 5f5f 2829 2023 3120  ).__call__() #1 
-00003960: 7375 6363 6573 7320 7365 6e64 6572 2020  success sender  
-00003970: 2020 2020 2020 2020 0d0a 6578 6365 7074          ..except
-00003980: 2045 7863 6570 7443 6869 6d65 2061 7320   ExceptChime as 
-00003990: 653a 2020 2020 2020 2332 2065 7863 6570  e:      #2 excep
-000039a0: 7420 7365 6e64 6572 2020 2020 2020 2020  t sender        
-000039b0: 2020 2020 0d0a 2020 2020 7379 732e 6578      ..    sys.ex
-000039c0: 6974 2829 0d0a 0d0a 5365 6e64 4368 696d  it()....SendChim
-000039d0: 6528 292e 5f5f 6361 6c6c 5f5f 2829 2020  e().__call__()  
-000039e0: 2020 2020 2020 2333 2063 7573 746f 6d69        #3 customi
-000039f0: 7a65 6420 7365 6e64 6572 2020 2020 2020  zed sender      
-00003a00: 200d 0a60 6060 0d0a 3c62 723e 0d0a 0d0a   ..```..<br>....
-00003a10: 2323 2032 2d35 2e20 2a53 6c61 636b 204e  ## 2-5. *Slack N
-00003a20: 6f74 6966 6965 722a 0d0a 2d20 612e 2076  otifier*..- a. v
-00003a30: 6973 6974 2068 7474 7073 3a2f 2f61 7069  isit https://api
-00003a40: 2e73 6c61 636b 2e63 6f6d 2f0d 0a2d 2062  .slack.com/..- b
-00003a50: 2e20 6043 7265 6174 6520 616e 2061 7070  . `Create an app
-00003a60: 6020 2d20 6046 726f 6d20 7363 7261 7463  ` - `From scratc
-00003a70: 6860 202d 2060 4372 6561 7465 2041 7070  h` - `Create App
-00003a80: 600d 0a2d 2063 2e20 4164 6420 7765 6268  `..- c. Add webh
-00003a90: 6f6f 6b3a 2043 6c69 636b 2060 496e 636f  ook: Click `Inco
-00003aa0: 6d69 6e67 2057 6562 686f 6f6b 7360 202d  ming Webhooks` -
-00003ab0: 2041 6374 6976 6174 6520 496e 636f 6d6d   Activate Incomm
-00003ac0: 696e 6720 604f 6e60 202d 2041 6464 204e  ing `On` - Add N
-00003ad0: 6577 2057 6562 686f 6f6b 2074 6f20 576f  ew Webhook to Wo
-00003ae0: 726b 7370 6163 650d 0a2d 2064 2e20 436f  rkspace..- d. Co
-00003af0: 7079 2060 5765 6268 6f6f 6b20 5552 4c60  py `Webhook URL`
-00003b00: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00003b10: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00003b20: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00003b30: 6d70 6f72 7420 4578 6365 7074 536c 6163  mport ExceptSlac
-00003b40: 6b2c 2053 7563 6365 7373 536c 6361 6b2c  k, SuccessSlcak,
-00003b50: 2053 656e 6453 6c61 636b 0d0a 7379 732e   SendSlack..sys.
-00003b60: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-00003b70: 6570 7453 6c61 636b 2e5f 5f63 616c 6c5f  eptSlack.__call_
-00003b80: 5f0d 0a0d 0a23 2044 6566 696e 6520 7468  _....# Define th
-00003b90: 6520 6e65 7874 2074 776f 2076 6172 6961  e next two varia
-00003ba0: 626c 6573 206f 7074 696f 6e61 6c6c 7920  bles optionally 
-00003bb0: 7768 656e 2075 7369 6e67 204f 7065 6e41  when using OpenA
-00003bc0: 4927 7320 4150 492e 0d0a 2320 5f4f 5045  I's API...# _OPE
-00003bd0: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-00003be0: 332e 352d 7475 7262 6f22 2020 2020 0d0a  3.5-turbo"    ..
-00003bf0: 2320 5f4f 5045 4e5f 4149 5f41 5049 3d22  # _OPEN_AI_API="
-00003c00: 736b 2d78 7878 7878 7822 0d0a 5f53 4c41  sk-xxxxxx".._SLA
-00003c10: 434b 5f57 4542 484f 4f4b 5f55 524c 203d  CK_WEBHOOK_URL =
-00003c20: 2027 6874 7470 733a 2f2f 686f 6f6b 732e   'https://hooks.
-00003c30: 736c 6163 6b2e 636f 6d2f 7365 7276 6963  slack.com/servic
-00003c40: 6573 2f78 7878 7878 7878 7878 7878 7878  es/xxxxxxxxxxxxx
-00003c50: 7878 7878 7878 270d 0a0d 0a74 7279 3a0d  xxxxxx'....try:.
-00003c60: 0a20 2020 2070 7269 6e74 2831 2f30 2920  .    print(1/0) 
-00003c70: 200d 0a20 2020 2053 7563 6365 7373 536c   ..    SuccessSl
-00003c80: 6361 6b28 292e 5f5f 6361 6c6c 5f5f 2829  cak().__call__()
-00003c90: 2023 3120 7375 6363 6573 7320 7365 6e64   #1 success send
-00003ca0: 6572 2020 2020 2020 2020 2020 0d0a 6578  er          ..ex
-00003cb0: 6365 7074 2045 7863 6570 7453 6c61 636b  cept ExceptSlack
-00003cc0: 2061 7320 653a 2020 2020 2020 2332 2065   as e:      #2 e
-00003cd0: 7863 6570 7420 7365 6e64 6572 2020 2020  xcept sender    
-00003ce0: 2020 2020 2020 2020 0d0a 2020 2020 7379          ..    sy
-00003cf0: 732e 6578 6974 2829 0d0a 0d0a 5365 6e64  s.exit()....Send
-00003d00: 536c 6163 6b28 292e 5f5f 6361 6c6c 5f5f  Slack().__call__
-00003d10: 2829 2020 2020 2020 2020 2333 2063 7573  ()        #3 cus
-00003d20: 746f 6d69 7a65 6420 7365 6e64 6572 2020  tomized sender  
-00003d30: 2020 200d 0a60 6060 0d0a 3c42 723e 0d0a     ..```..<Br>..
-00003d40: 0d0a 2323 2032 2d36 2e20 2a4c 696e 6520  ..## 2-6. *Line 
-00003d50: 4e6f 7469 6669 6572 2a0d 0a2d 2061 2e20  Notifier*..- a. 
-00003d60: 5265 6769 7374 6572 205b 6874 7470 733a  Register [https:
-00003d70: 2f2f 6e6f 7469 6679 2d62 6f74 2e6c 696e  //notify-bot.lin
-00003d80: 652e 6d65 2f5d 2868 7474 7073 3a2f 2f6e  e.me/](https://n
-00003d90: 6f74 6966 792d 626f 742e 6c69 6e65 2e6d  otify-bot.line.m
-00003da0: 652f 292e 0d0a 2d20 622e 2047 6f20 746f  e/)...- b. Go to
-00003db0: 206d 7970 6167 6520 5b68 7474 7073 3a2f   mypage [https:/
-00003dc0: 2f6e 6f74 6966 792d 626f 742e 6c69 6e65  /notify-bot.line
-00003dd0: 2e6d 652f 6d79 2f5d 2868 7474 7073 3a2f  .me/my/](https:/
-00003de0: 2f6e 6f74 6966 792d 626f 742e 6c69 6e65  /notify-bot.line
-00003df0: 2e6d 652f 6d79 2f29 2e0d 0a2d 2063 2e20  .me/my/)...- c. 
-00003e00: 436c 6963 6b20 6047 656e 6572 6174 6520  Click `Generate 
-00003e10: 546f 6b65 6e60 2c20 656e 7465 7220 5365  Token`, enter Se
-00003e20: 7276 6963 6520 4e61 6d65 2061 6e64 2063  rvice Name and c
-00003e30: 6c69 636b 2060 312d 6f6e 2d31 2063 6861  lick `1-on-1 cha
-00003e40: 7420 7769 7468 204c 494e 4560 2028 616e  t with LINE` (an
-00003e50: 7974 6869 6e67 2079 6f75 206c 696b 6529  ything you like)
-00003e60: 2e0d 0a2d 2064 2e20 436f 7079 2054 6f6b  ...- d. Copy Tok
-00003e70: 656e 2e0d 0a0d 0a60 6060 7079 7468 6f6e  en.....```python
-00003e80: 0d0a 696d 706f 7274 2073 7973 0d0a 6672  ..import sys..fr
-00003e90: 6f6d 2045 7863 6570 744e 6f74 6966 6965  om ExceptNotifie
-00003ea0: 7220 696d 706f 7274 2045 7863 6570 744c  r import ExceptL
-00003eb0: 696e 652c 2053 7563 6365 7373 4c69 6e65  ine, SuccessLine
-00003ec0: 2c20 5365 6e64 4c69 6e65 0d0a 7379 732e  , SendLine..sys.
-00003ed0: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-00003ee0: 6570 744c 696e 652e 5f5f 6361 6c6c 5f5f  eptLine.__call__
-00003ef0: 0d0a 0d0a 2320 4465 6669 6e65 2074 6865  ....# Define the
-00003f00: 206e 6578 7420 7477 6f20 7661 7269 6162   next two variab
-00003f10: 6c65 7320 6f70 7469 6f6e 616c 6c79 2077  les optionally w
-00003f20: 6865 6e20 7573 696e 6720 4f70 656e 4149  hen using OpenAI
-00003f30: 2773 2041 5049 2e0d 0a23 205f 4f50 454e  's API...# _OPEN
-00003f40: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
-00003f50: 2e35 2d74 7572 626f 2220 2020 200d 0a23  .5-turbo"    ..#
-00003f60: 205f 4f50 454e 5f41 495f 4150 493d 2273   _OPEN_AI_API="s
-00003f70: 6b2d 7878 7878 7878 220d 0a5f 4c49 4e45  k-xxxxxx".._LINE
-00003f80: 5f4e 4f54 4946 595f 4150 495f 544f 4b45  _NOTIFY_API_TOKE
-00003f90: 4e20 3d20 2778 7878 7878 7878 7878 7878  N = 'xxxxxxxxxxx
-00003fa0: 270d 0a0d 0a74 7279 3a0d 0a20 2020 2070  '....try:..    p
-00003fb0: 7269 6e74 2831 2f32 3029 2020 0d0a 2020  rint(1/20)  ..  
-00003fc0: 2020 5375 6363 6573 734c 696e 6528 292e    SuccessLine().
-00003fd0: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
-00003fe0: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
-00003ff0: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
-00004000: 7863 6570 744c 696e 6520 6173 2065 3a20  xceptLine as e: 
-00004010: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
-00004020: 656e 6465 7220 2020 2020 2020 2020 2020  ender           
-00004030: 200d 0a20 2020 2073 7973 2e65 7869 7428   ..    sys.exit(
-00004040: 290d 0a0d 0a53 656e 644c 696e 6528 292e  )....SendLine().
-00004050: 5f5f 6361 6c6c 5f5f 2829 2020 2020 2020  __call__()      
-00004060: 2020 2333 2063 7573 746f 6d69 7a65 6420    #3 customized 
-00004070: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00004080: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
-00004090: 0a23 2320 322d 372e 202a 534d 5320 4e6f  .## 2-7. *SMS No
-000040a0: 7469 6669 6572 2a0d 0a2d 2061 2e20 5369  tifier*..- a. Si
-000040b0: 676e 2075 7020 666f 7220 5477 696c 696f  gn up for Twilio
-000040c0: 2e20 5b68 7474 7073 3a2f 2f77 7777 2e74  . [https://www.t
-000040d0: 7769 6c69 6f2e 636f 6d2f 656e 2d75 735d  wilio.com/en-us]
-000040e0: 2868 7474 7073 3a2f 2f77 7777 2e74 7769  (https://www.twi
-000040f0: 6c69 6f2e 636f 6d2f 656e 2d75 7329 2e0d  lio.com/en-us)..
-00004100: 0a2d 2062 2e20 436c 6963 6b20 436f 6e73  .- b. Click Cons
-00004110: 6f6c 6520 696e 2074 6865 2075 7070 6572  ole in the upper
-00004120: 2072 6967 6874 2063 6f72 6e65 722e 0d0a   right corner...
-00004130: 2d20 632e 2043 6f70 7920 7468 6520 7661  - c. Copy the va
-00004140: 7269 6162 6c65 7320 7072 6f76 6964 6564  riables provided
-00004150: 2069 6e20 7468 6520 636f 6e73 6f6c 652e   in the console.
-00004160: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00004170: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00004180: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00004190: 6d70 6f72 7420 4578 6365 7074 534d 532c  mport ExceptSMS,
-000041a0: 2053 7563 6365 7373 534d 532c 2053 656e   SuccessSMS, Sen
-000041b0: 6453 4d53 0d0a 7379 732e 6578 6365 7074  dSMS..sys.except
-000041c0: 686f 6f6b 203d 2045 7863 6570 7453 4d53  hook = ExceptSMS
-000041d0: 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23 2044  .__call__....# D
-000041e0: 6566 696e 6520 7468 6520 6e65 7874 2074  efine the next t
-000041f0: 776f 2076 6172 6961 626c 6573 206f 7074  wo variables opt
-00004200: 696f 6e61 6c6c 7920 7768 656e 2075 7369  ionally when usi
-00004210: 6e67 204f 7065 6e41 4927 7320 4150 492e  ng OpenAI's API.
-00004220: 0d0a 2320 5f4f 5045 4e5f 4149 5f4d 4f44  ..# _OPEN_AI_MOD
-00004230: 454c 3d22 6770 742d 332e 352d 7475 7262  EL="gpt-3.5-turb
-00004240: 6f22 2020 2020 0d0a 2320 5f4f 5045 4e5f  o"    ..# _OPEN_
-00004250: 4149 5f41 5049 3d22 736b 2d78 7878 7878  AI_API="sk-xxxxx
-00004260: 7822 0d0a 5f54 5749 4c49 4f5f 5349 4420  x".._TWILIO_SID 
-00004270: 3d20 2778 7878 7827 0d0a 5f54 5749 4c49  = 'xxxx'.._TWILI
-00004280: 4f5f 544f 4b45 4e20 3d20 2779 7979 7979  O_TOKEN = 'yyyyy
-00004290: 7927 0d0a 5f52 4543 4950 4945 4e54 5f50  y'.._RECIPIENT_P
-000042a0: 484f 4e45 5f4e 554d 4245 523d 222b 6161  HONE_NUMBER="+aa
-000042b0: 6161 6161 222c 0d0a 5f53 454e 4445 525f  aaaa",.._SENDER_
-000042c0: 5048 4f4e 455f 4e55 4d42 4552 3d22 2b62  PHONE_NUMBER="+b
-000042d0: 6262 6262 6222 2c20 200d 0a0d 0a74 7279  bbbbb",  ....try
-000042e0: 3a0d 0a20 2020 2070 7269 6e74 2831 2f31  :..    print(1/1
-000042f0: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
-00004300: 7353 4d53 2829 2e5f 5f63 616c 6c5f 5f28  sSMS().__call__(
-00004310: 2920 2331 2073 7563 6365 7373 2073 656e  ) #1 success sen
-00004320: 6465 7220 2020 2020 2020 2020 200d 0a65  der          ..e
-00004330: 7863 6570 7420 4578 6365 7074 534d 5320  xcept ExceptSMS 
-00004340: 6173 2065 3a20 2020 2020 2023 3220 6578  as e:      #2 ex
-00004350: 6365 7074 2073 656e 6465 720d 0a20 2020  cept sender..   
-00004360: 2073 7973 2e65 7869 7428 290d 0a0d 0a53   sys.exit()....S
-00004370: 656e 6453 4d53 2829 2e5f 5f63 616c 6c5f  endSMS().__call_
-00004380: 5f28 2920 2020 2020 2020 2023 3320 6375  _()        #3 cu
-00004390: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
-000043a0: 2020 2020 2020 200d 0a60 6060 0d0a 3c42         ..```..<B
-000043b0: 723e 0d0a 0d0a 2323 2032 2d38 2e20 2a54  r>....## 2-8. *T
-000043c0: 6561 6d73 204e 6f74 6966 6965 722a 0d0a  eams Notifier*..
-000043d0: 2d20 612e 2043 7265 6174 6520 7468 6520  - a. Create the 
-000043e0: 6368 616e 6e65 6c20 7468 6174 2079 6f75  channel that you
-000043f0: 2077 616e 7420 746f 206e 6f74 6966 792e   want to notify.
-00004400: 0d0a 2d20 622e 2041 7070 202d 2053 6561  ..- b. App - Sea
-00004410: 7263 683a 2077 6562 686f 6f6b 202d 2049  rch: webhook - I
-00004420: 6e63 6f6d 696e 6720 5765 6268 6f6f 6b20  ncoming Webhook 
-00004430: 5b68 7474 7073 3a2f 2f74 6561 6d73 2e6d  [https://teams.m
-00004440: 6963 726f 736f 6674 2e63 6f6d 2f6c 2f61  icrosoft.com/l/a
-00004450: 7070 2f32 3033 6131 6532 632d 3236 6363  pp/203a1e2c-26cc
-00004460: 2d34 3763 612d 3833 6165 2d62 6539 3866  -47ca-83ae-be98f
-00004470: 3936 3062 3662 323f 736f 7572 6365 3d61  960b6b2?source=a
-00004480: 7070 2d64 6574 6169 6c73 2d64 6961 6c6f  pp-details-dialo
-00004490: 675d 2868 7474 7073 3a2f 2f74 6561 6d73  g](https://teams
-000044a0: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6c  .microsoft.com/l
-000044b0: 2f61 7070 2f32 3033 6131 6532 632d 3236  /app/203a1e2c-26
-000044c0: 6363 2d34 3763 612d 3833 6165 2d62 6539  cc-47ca-83ae-be9
-000044d0: 3866 3936 3062 3662 323f 736f 7572 6365  8f960b6b2?source
-000044e0: 3d61 7070 2d64 6574 6169 6c73 2d64 6961  =app-details-dia
-000044f0: 6c6f 6729 2e0d 0a2d 2063 2e20 436c 6963  log)...- c. Clic
-00004500: 6b20 6052 6571 7565 7374 2041 7070 726f  k `Request Appro
-00004510: 7661 6c60 203c 6272 3e0d 0a41 6674 6572  val` <br>..After
-00004520: 2079 6f75 2063 616e 2075 7365 2077 6562   you can use web
-00004530: 686f 6f6b 2069 6e63 6f6d 6d69 6e67 2e20  hook incomming. 
-00004540: 5072 6f63 6565 6420 746f 206e 6578 7420  Proceed to next 
-00004550: 7374 6570 732e 0d0a 4d69 6372 6f73 6f66  steps...Microsof
-00004560: 7420 5465 616d 7320 616c 6c6f 7773 206c  t Teams allows l
-00004570: 696d 6974 6564 2061 7070 6c69 6361 7469  imited applicati
-00004580: 6f6e 2061 6363 6573 7320 7065 7220 6f72  on access per or
-00004590: 6761 6e69 7a61 7469 6f6e 2c20 736f 2069  ganization, so i
-000045a0: 7420 6361 6e20 6f6e 6c79 2062 6520 7573  t can only be us
-000045b0: 6564 2069 6620 7468 6520 7765 6268 6f6f  ed if the webhoo
-000045c0: 6b20 696e 636f 6d69 6e67 2061 7070 6c69  k incoming appli
-000045d0: 6361 7469 6f6e 2069 7320 6176 6169 6c61  cation is availa
-000045e0: 626c 652e 0d0a 2d20 632e 2047 6f20 746f  ble...- c. Go to
-000045f0: 2074 6865 2074 6561 6d20 6368 616e 6e65   the team channe
-00004600: 6c20 746f 2072 6563 6569 7665 206e 6f74  l to receive not
-00004610: 6966 6963 6174 696f 6e73 2c20 616e 6420  ifications, and 
-00004620: 636c 6963 6b20 6043 6f6e 6e65 6374 6f72  click `Connector
-00004630: 7360 2069 6e20 5365 7474 696e 6773 2e0d  s` in Settings..
-00004640: 0a2d 2064 2e20 6043 6f6e 6e65 6374 6f72  .- d. `Connector
-00004650: 7360 2041 6674 6572 2063 6f6e 6669 6775  s` After configu
-00004660: 7269 6e67 2077 6562 686f 6f6b 2069 6e63  ring webhook inc
-00004670: 6f6d 696e 6720 696e 2043 6f6e 6e65 6374  oming in Connect
-00004680: 6f72 2c20 636f 7079 2074 6865 2077 6562  or, copy the web
-00004690: 686f 6f6b 2055 524c 2e0d 0a0d 0a60 6060  hook URL.....```
-000046a0: 7079 7468 6f6e 0d0a 696d 706f 7274 2073  python..import s
-000046b0: 7973 0d0a 6672 6f6d 2045 7863 6570 744e  ys..from ExceptN
-000046c0: 6f74 6966 6965 7220 696d 706f 7274 2045  otifier import E
-000046d0: 7863 6570 7454 6561 6d73 2c20 5375 6363  xceptTeams, Succ
-000046e0: 6573 7354 6561 6d73 2c20 5365 6e64 5465  essTeams, SendTe
-000046f0: 616d 730d 0a73 7973 2e65 7863 6570 7468  ams..sys.excepth
-00004700: 6f6f 6b20 3d20 4578 6365 7074 5465 616d  ook = ExceptTeam
-00004710: 732e 5f5f 6361 6c6c 5f5f 0d0a 0d0a 2320  s.__call__....# 
-00004720: 4465 6669 6e65 2074 6865 206e 6578 7420  Define the next 
-00004730: 7477 6f20 7661 7269 6162 6c65 7320 6f70  two variables op
-00004740: 7469 6f6e 616c 6c79 2077 6865 6e20 7573  tionally when us
-00004750: 696e 6720 4f70 656e 4149 2773 2041 5049  ing OpenAI's API
-00004760: 2e0d 0a23 205f 4f50 454e 5f41 495f 4d4f  ...# _OPEN_AI_MO
-00004770: 4445 4c3d 2267 7074 2d33 2e35 2d74 7572  DEL="gpt-3.5-tur
-00004780: 626f 2220 2020 200d 0a23 205f 4f50 454e  bo"    ..# _OPEN
-00004790: 5f41 495f 4150 493d 2273 6b2d 7878 7878  _AI_API="sk-xxxx
-000047a0: 7878 220d 0a5f 5445 414d 535f 5745 4248  xx".._TEAMS_WEBH
-000047b0: 4f4f 4b5f 5552 4c20 3d20 276d 6963 726f  OOK_URL = 'micro
-000047c0: 736f 6674 2077 6562 686f 6f6b 205f 5445  soft webhook _TE
-000047d0: 414d 535f 5745 4248 4f4f 4b5f 5552 4c27  AMS_WEBHOOK_URL'
-000047e0: 0d0a 0d0a 7472 793a 0d0a 2020 2020 7072  ....try:..    pr
-000047f0: 696e 7428 312f 3230 2920 200d 0a20 2020  int(1/20)  ..   
-00004800: 2053 7563 6365 7373 5465 616d 7328 292e   SuccessTeams().
-00004810: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
-00004820: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
-00004830: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
-00004840: 7863 6570 7454 6561 6d73 2061 7320 653a  xceptTeams as e:
-00004850: 2020 2020 2020 2332 2065 7863 6570 7420        #2 except 
-00004860: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00004870: 2020 0d0a 2020 2020 7379 732e 6578 6974    ..    sys.exit
-00004880: 2829 0d0a 0d0a 5365 6e64 5465 616d 7328  ()....SendTeams(
-00004890: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
-000048a0: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
-000048b0: 6420 7365 6e64 6572 2020 2020 2020 2020  d sender        
-000048c0: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
-000048d0: 0a23 2320 322d 392e 202a 4b61 6b61 6f74  .## 2-9. *Kakaot
-000048e0: 616c 6b20 4e6f 7469 6669 6572 2a0d 0a2d  alk Notifier*..-
-000048f0: 2061 2e20 5369 676e 2075 7020 6174 2074   a. Sign up at t
-00004900: 6865 2066 6f6c 6c6f 7769 6e67 2073 6974  he following sit
-00004910: 653a 205b 6874 7470 733a 2f2f 6465 7665  e: [https://deve
-00004920: 6c6f 7065 7273 2e6b 616b 616f 2e63 6f6d  lopers.kakao.com
-00004930: 2f5d 2868 7474 7073 3a2f 2f64 6576 656c  /](https://devel
-00004940: 6f70 6572 732e 6b61 6b61 6f2e 636f 6d2f  opers.kakao.com/
-00004950: 292e 0d0a 2d20 622e 2043 6c69 636b 2022  )...- b. Click "
-00004960: 4d79 2041 7070 6c69 6361 7469 6f6e 2220  My Application" 
-00004970: 6f6e 2074 6865 2074 6f70 2062 6172 2e0d  on the top bar..
-00004980: 0a2d 2063 2e20 436c 6963 6b20 2241 6464  .- c. Click "Add
-00004990: 2061 6e20 6170 706c 6963 6174 696f 6e2c   an application,
-000049a0: 2220 7365 7420 6120 6e61 6d65 2c20 616e  " set a name, an
-000049b0: 6420 6372 6561 7465 2069 742e 0d0a 2d20  d create it...- 
-000049c0: 642e 2043 6c69 636b 2022 4b61 6b61 6f20  d. Click "Kakao 
-000049d0: 4c6f 6769 6e22 2069 6e20 7468 6520 6c65  Login" in the le
-000049e0: 6674 206d 656e 752c 2074 6865 6e20 6368  ft menu, then ch
-000049f0: 616e 6765 2074 6865 2053 7461 7465 206f  ange the State o
-00004a00: 6620 224b 616b 616f 204c 6f67 696e 2041  f "Kakao Login A
-00004a10: 6374 6976 6174 696f 6e22 2074 6f20 4f4e  ctivation" to ON
-00004a20: 206f 6e20 7468 6520 7265 7375 6c74 696e   on the resultin
-00004a30: 6720 7061 6765 2e0d 0a2d 2065 2e20 496e  g page...- e. In
-00004a40: 204d 7920 4170 706c 6963 6174 696f 6e20   My Application 
-00004a50: 3e20 5072 6f64 7563 7420 5365 7474 696e  > Product Settin
-00004a60: 6773 203e 204b 616b 616f 204c 6f67 696e  gs > Kakao Login
-00004a70: 2c20 6265 2073 7572 6520 746f 2073 6574  , be sure to set
-00004a80: 2052 6564 6972 6563 7420 5552 4920 6173   Redirect URI as
-00004a90: 2066 6f6c 6c6f 7773 3a20 5b68 7474 7073   follows: [https
-00004aa0: 3a2f 2f65 7861 6d70 6c65 2e63 6f6d 2f6f  ://example.com/o
-00004ab0: 6175 7468 5d28 6874 7470 733a 2f2f 6578  auth](https://ex
-00004ac0: 616d 706c 652e 636f 6d2f 6f61 7574 6829  ample.com/oauth)
-00004ad0: 2e0d 0a2d 2066 2e20 496e 2074 6865 206c  ...- f. In the l
-00004ae0: 6566 7420 436f 6e73 656e 7420 4974 656d  eft Consent Item
-00004af0: 7320 6d65 6e75 2c20 7365 7420 2253 656e  s menu, set "Sen
-00004b00: 6420 6d65 7373 6167 6520 696e 204b 616b  d message in Kak
-00004b10: 616f 5461 6c6b 2220 746f 2073 656c 6563  aoTalk" to selec
-00004b20: 7469 7665 2061 6772 6565 6d65 6e74 2e0d  tive agreement..
-00004b30: 0a2d 2067 2e20 436f 7079 2074 6865 2052  .- g. Copy the R
-00004b40: 4553 5420 4150 4920 4b65 7920 696e 204d  EST API Key in M
-00004b50: 7920 4170 706c 6963 6174 696f 6e20 3e20  y Application > 
-00004b60: 4170 7020 5365 7474 696e 6773 203e 2053  App Settings > S
-00004b70: 756d 6d61 7279 2c20 616e 6420 676f 2074  ummary, and go t
-00004b80: 6f20 7468 6520 666f 6c6c 6f77 696e 6720  o the following 
-00004b90: 646f 6375 6d65 6e74 2e0d 0a2d 2068 2e20  document...- h. 
-00004ba0: 4966 2079 6f75 2068 6176 6520 7375 6363  If you have succ
-00004bb0: 6573 7366 756c 6c79 2063 6f6d 706c 6574  essfully complet
-00004bc0: 6564 2061 6c6c 206f 6620 7468 6520 6162  ed all of the ab
-00004bd0: 6f76 6520 7374 6570 732c 2067 6f20 746f  ove steps, go to
-00004be0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00004bf0: 6f63 756d 656e 7420 616e 6420 666f 6c6c  ocument and foll
-00004c00: 6f77 2074 6865 2069 6e73 7472 7563 7469  ow the instructi
-00004c10: 6f6e 733a 0d0a 2068 7474 7073 3a2f 2f67  ons:.. https://g
-00004c20: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00004c30: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00004c40: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00004c50: 7475 746f 7269 616c 732f 6b61 6b61 6f5f  tutorials/kakao_
-00004c60: 746f 6b65 6e5f 6765 6e65 7261 746f 722e  token_generator.
-00004c70: 6970 796e 620d 0a20 2a2a 496e 2074 6869  ipynb.. **In thi
-00004c80: 7320 6578 616d 706c 652c 2073 6f6d 6520  s example, some 
-00004c90: 4150 4920 6b65 7973 2077 6572 6520 6578  API keys were ex
-00004ca0: 706f 7365 6420 6279 2063 7265 6174 696e  posed by creatin
-00004cb0: 6720 616e 6420 7265 6d6f 7669 6e67 2061  g and removing a
-00004cc0: 2074 6573 7420 6170 706c 6963 6174 696f   test applicatio
-00004cd0: 6e2c 2062 7574 2066 6f72 2073 6563 7572  n, but for secur
-00004ce0: 6974 7920 7265 6173 6f6e 732c 2079 6f75  ity reasons, you
-00004cf0: 7220 4150 4920 6b65 7920 7368 6f75 6c64  r API key should
-00004d00: 206e 6f74 2062 6520 6578 706f 7365 6420   not be exposed 
-00004d10: 746f 2074 6865 206f 7574 7369 6465 2077  to the outside w
-00004d20: 6f72 6c64 2e2a 2a0d 0a3c 4272 3e0d 0a0d  orld.**..<Br>...
-00004d30: 0a60 6060 7079 7468 6f6e 0d0a 696d 706f  .```python..impo
-00004d40: 7274 2073 7973 0d0a 6672 6f6d 2045 7863  rt sys..from Exc
-00004d50: 6570 744e 6f74 6966 6965 7220 696d 706f  eptNotifier impo
-00004d60: 7274 2045 7863 6570 744b 616b 616f 2c20  rt ExceptKakao, 
-00004d70: 5375 6363 6573 734b 616b 616f 2c20 5365  SuccessKakao, Se
-00004d80: 6e64 4b61 6b61 6f0d 0a73 7973 2e65 7863  ndKakao..sys.exc
-00004d90: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
-00004da0: 4b61 6b61 6f2e 5f5f 6361 6c6c 5f5f 0d0a  Kakao.__call__..
-00004db0: 0d0a 2320 4465 6669 6e65 2074 6865 206e  ..# Define the n
-00004dc0: 6578 7420 7477 6f20 7661 7269 6162 6c65  ext two variable
-00004dd0: 7320 6f70 7469 6f6e 616c 6c79 2077 6865  s optionally whe
-00004de0: 6e20 7573 696e 6720 4f70 656e 4149 2773  n using OpenAI's
-00004df0: 2041 5049 2e0d 0a23 205f 4f50 454e 5f41   API...# _OPEN_A
-00004e00: 495f 4d4f 4445 4c3d 2267 7074 2d33 2e35  I_MODEL="gpt-3.5
-00004e10: 2d74 7572 626f 2220 2020 200d 0a23 205f  -turbo"    ..# _
-00004e20: 4f50 454e 5f41 495f 4150 493d 2273 6b2d  OPEN_AI_API="sk-
-00004e30: 7878 7878 7878 220d 0a5f 4b41 4b41 4f5f  xxxxxx".._KAKAO_
-00004e40: 544f 4b45 4e5f 5041 5448 203d 2027 7878  TOKEN_PATH = 'xx
-00004e50: 7878 2f78 7878 2f78 7878 2e6a 736f 6e27  xx/xxx/xxx.json'
-00004e60: 270d 0a0d 0a74 7279 3a0d 0a20 2020 2070  '....try:..    p
-00004e70: 7269 6e74 2831 2f30 2920 200d 0a20 2020  rint(1/0)  ..   
-00004e80: 2053 7563 6365 7373 4b61 6b61 6f28 292e   SuccessKakao().
-00004e90: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
-00004ea0: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
-00004eb0: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
-00004ec0: 7863 6570 744b 616b 616f 2061 7320 653a  xceptKakao as e:
-00004ed0: 2020 2020 2020 2332 2065 7863 6570 7420        #2 except 
-00004ee0: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00004ef0: 2020 0d0a 2020 2020 7379 732e 6578 6974    ..    sys.exit
-00004f00: 2829 0d0a 0d0a 5365 6e64 4b61 6b61 6f28  ()....SendKakao(
-00004f10: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
-00004f20: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
-00004f30: 6420 7365 6e64 6572 2020 2020 2020 2020  d sender        
-00004f40: 200d 0a60 6060 0d0a 0d0a 3c42 723e 0d0a   ..```....<Br>..
-00004f50: 0d0a 2323 2032 2d31 302e 202a 4265 6570  ..## 2-10. *Beep
-00004f60: 204e 6f74 6966 6965 722a 0d0a 4e6f 2073   Notifier*..No s
-00004f70: 6574 7570 2069 7320 7265 7175 6972 6564  etup is required
-00004f80: 2e20 5573 6520 6173 2066 6f6c 6c6f 7773  . Use as follows
-00004f90: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
-00004fa0: 6672 6f6d 2045 7863 6570 746e 6f74 6966  from Exceptnotif
-00004fb0: 6965 7220 696d 706f 7274 2045 7863 6570  ier import Excep
-00004fc0: 7442 6565 702c 2053 7563 6365 7373 4265  tBeep, SuccessBe
-00004fd0: 6570 2c20 5365 6e64 4265 6570 2829 2c20  ep, SendBeep(), 
-00004fe0: 6265 6570 2829 0d0a 4245 4550 5f54 494d  beep()..BEEP_TIM
-00004ff0: 4520 3d20 310d 0a73 7973 2e65 7863 6570  E = 1..sys.excep
-00005000: 7468 6f6f 6b20 3d20 4578 6365 7074 4265  thook = ExceptBe
-00005010: 6570 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a74  ep.__call__....t
-00005020: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
-00005030: 2f32 3029 2020 0d0a 2020 2020 5375 6363  /20)  ..    Succ
-00005040: 6573 7342 6565 7028 292e 5f5f 6361 6c6c  essBeep().__call
-00005050: 5f5f 2829 2023 3120 7375 6363 6573 7320  __() #1 success 
-00005060: 6265 6570 2d62 6565 7020 2020 2020 2020  beep-beep       
-00005070: 2020 200d 0a0d 0a65 7863 6570 7420 4578     ....except Ex
-00005080: 6365 7074 4265 6570 2061 7320 653a 2020  ceptBeep as e:  
-00005090: 2020 2020 2332 2065 7863 6570 7420 6265      #2 except be
-000050a0: 6570 2d62 6565 7020 2020 2020 2020 2020  ep-beep         
-000050b0: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-000050c0: 2e65 7869 7428 290d 0a0d 0a53 656e 6442  .exit()....SendB
-000050d0: 6565 7028 292e 5f5f 6361 6c6c 5f5f 2829  eep().__call__()
-000050e0: 2020 2020 2020 2020 2333 2063 7573 746f          #3 custo
-000050f0: 6d69 7a65 6420 6265 6570 2d62 6565 7020  mized beep-beep 
-00005100: 2020 2020 200d 0a0d 0a62 6565 7028 290d       ....beep().
-00005110: 0a0d 0a60 6060 0d0a 0d0a 3c42 723e 0d0a  ...```....<Br>..
-00005120: 0d0a 0d0a 2323 2032 2d31 312e 202a 4465  ....## 2-11. *De
-00005130: 736b 746f 7020 4e6f 7469 6669 6572 2a0d  sktop Notifier*.
-00005140: 0a4e 6f20 7365 7475 7020 6973 2072 6571  .No setup is req
-00005150: 7569 7265 642e 2055 7365 2061 7320 666f  uired. Use as fo
-00005160: 6c6c 6f77 732e 0d0a 0d0a 6060 6070 7974  llows.....```pyt
-00005170: 686f 6e0d 0a66 726f 6d20 4578 6365 7074  hon..from Except
-00005180: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
-00005190: 4578 6365 7074 4465 736b 746f 702c 2053  ExceptDesktop, S
-000051a0: 7563 6365 7373 4465 736b 746f 702c 2053  uccessDesktop, S
-000051b0: 656e 6444 6573 6b74 6f70 0d0a 7379 732e  endDesktop..sys.
-000051c0: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-000051d0: 6570 7444 6573 6b74 6f70 2e5f 5f63 616c  eptDesktop.__cal
-000051e0: 6c5f 5f0d 0a23 2044 6566 696e 6520 7468  l__..# Define th
-000051f0: 6520 6e65 7874 2074 776f 2076 6172 6961  e next two varia
-00005200: 626c 6573 206f 7074 696f 6e61 6c6c 7920  bles optionally 
-00005210: 7768 656e 2075 7369 6e67 204f 7065 6e41  when using OpenA
-00005220: 4927 7320 4150 492e 0d0a 2320 5f4f 5045  I's API...# _OPE
-00005230: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-00005240: 332e 352d 7475 7262 6f22 2020 2020 0d0a  3.5-turbo"    ..
-00005250: 2320 5f4f 5045 4e5f 4149 5f41 5049 3d22  # _OPEN_AI_API="
-00005260: 736b 2d78 7878 7878 7822 0d0a 0d0a 7472  sk-xxxxxx"....tr
-00005270: 793a 0d0a 2020 2020 7072 696e 7428 312f  y:..    print(1/
-00005280: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
-00005290: 7344 6573 6b74 6f70 2829 2e5f 5f63 616c  sDesktop().__cal
-000052a0: 6c5f 5f28 2920 2331 2073 7563 6365 7373  l__() #1 success
-000052b0: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
-000052c0: 200d 0a0d 0a65 7863 6570 7420 4578 6365   ....except Exce
-000052d0: 7074 4465 736b 746f 7020 6173 2065 3a20  ptDesktop as e: 
-000052e0: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
-000052f0: 656e 6465 7220 2020 2020 2020 2020 2020  ender           
-00005300: 200d 0a20 2020 2073 7973 2e65 7869 7428   ..    sys.exit(
-00005310: 290d 0a0d 0a53 656e 6444 6573 6b74 6f70  )....SendDesktop
-00005320: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
-00005330: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
-00005340: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
-00005350: 2020 0d0a 6060 600d 0a0d 0a3c 4272 3e3c    ..```....<Br><
-00005360: 6272 3e3c 6272 3e0d 0a0d 0a23 2323 2049  br><br>....### I
-00005370: 6e73 7069 7269 6e67 0d0a 2d20 5468 616e  nspiring..- Than
-00005380: 6b73 2074 6f20 5b4d 7975 6e67 6861 6b20  ks to [Myunghak 
-00005390: 4c65 655d 2868 7474 7073 3a2f 2f67 6974  Lee](https://git
-000053a0: 6875 622e 636f 6d2f 6d79 656f 6e67 6861  hub.com/myeongha
-000053b0: 6b29 2066 6f72 2070 726f 7669 6469 6e67  k) for providing
-000053c0: 2067 7265 6174 2069 6465 6173 206f 6e20   great ideas on 
-000053d0: 7072 6f76 6964 696e 6720 6465 6275 6767  providing debugg
-000053e0: 696e 6720 696e 666f 726d 6174 696f 6e20  ing information 
-000053f0: 7468 726f 7567 6820 6f70 656e 2061 6920  through open ai 
-00005400: 4150 492e 0d0a 0d0a 2323 2320 436f 6e74  API.....### Cont
-00005410: 6163 7473 0d0a 2d20 4d61 696e 7461 696e  acts..- Maintain
-00005420: 6572 205b 4461 6e69 656c 2050 6172 6b2c  er [Daniel Park,
-00005430: 2053 6f75 7468 204b 6f72 6561 5d28 6874   South Korea](ht
-00005440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00005450: 2f44 5344 616e 6965 6c50 6172 6b29 203c  /DSDanielPark) <
-00005460: 6272 3e0d 0a2d 2045 6d61 696c 2070 6172  br>..- Email par
-00005470: 6b6d 696e 776f 6f31 3939 3140 676d 6169  kminwoo1991@gmai
-00005480: 6c2e 636f 6d0d 0a0d 0a23 2323 2323 2054  l.com....##### T
-00005490: 6865 2070 6163 6b61 6765 2069 7320 6375  he package is cu
-000054a0: 7272 656e 746c 7920 696e 2074 6865 2064  rrently in the d
-000054b0: 6576 656c 6f70 6d65 6e74 2061 6e64 2051  evelopment and Q
-000054c0: 4120 7374 6167 6573 2c20 616e 6420 7468  A stages, and th
-000054d0: 6520 6465 7665 6c6f 706d 656e 7420 7374  e development st
-000054e0: 6167 6520 7769 6c6c 2062 6520 7570 6461  age will be upda
-000054f0: 7465 6420 6174 2074 6865 2074 6f70 206f  ted at the top o
-00005500: 6620 7468 6973 2070 6167 652e 2049 6620  f this page. If 
-00005510: 6974 2069 7320 6465 7465 726d 696e 6564  it is determined
-00005520: 2074 6861 7420 7468 6520 7072 6f64 7563   that the produc
-00005530: 7420 6973 2073 7461 626c 6520 7468 726f  t is stable thro
-00005540: 7567 6820 6665 6174 7572 6520 696d 7072  ugh feature impr
-00005550: 6f76 656d 656e 742c 2061 6464 6974 696f  ovement, additio
-00005560: 6e2c 2061 6e64 2069 7373 7565 2072 6573  n, and issue res
-00005570: 6f6c 7574 696f 6e2c 2074 6865 2064 6576  olution, the dev
-00005580: 656c 6f70 6d65 6e74 2073 7461 6765 2077  elopment stage w
-00005590: 696c 6c20 7265 6163 6820 7374 6167 6520  ill reach stage 
-000055a0: 352e 2049 6620 6e6f 206e 6577 2075 7064  5. If no new upd
-000055b0: 6174 6573 206f 7220 6973 7375 6573 2061  ates or issues a
-000055c0: 7269 7365 2c20 6974 2077 696c 6c20 6265  rise, it will be
-000055d0: 2061 646a 7573 7465 6420 7570 7761 7264   adjusted upward
-000055e0: 2074 6f20 7374 6167 6520 3620 6f72 2068   to stage 6 or h
-000055f0: 6967 6865 722e 0d0a 0d0a 2323 2323 2043  igher.....#### C
-00005600: 6f75 6c64 2079 6f75 206b 696e 646c 7920  ould you kindly 
-00005610: 6164 6420 7468 6973 2062 6164 6765 2074  add this badge t
-00005620: 6f20 796f 7572 2072 6570 6f73 6974 6f72  o your repositor
-00005630: 793f 0d0a 0d0a 6060 600d 0a21 5b45 7863  y?....```..![Exc
-00005640: 6570 742d 4e6f 7469 6669 6572 5d28 6874  ept-Notifier](ht
-00005650: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00005660: 732e 696f 2f62 6164 6765 2f70 7970 692d  s.io/badge/pypi-
-00005670: 4578 6365 7074 4e6f 7469 6669 6572 2d6f  ExceptNotifier-o
-00005680: 7261 6e67 6529 0d0a 6060 600d 0a0d 0a0d  range)..```.....
-00005690: 0a                                       .
+00000470: 3e0d 0a21 5b5d 2868 7474 7073 3a2f 2f67  >..![](https://g
+00000480: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
+00000490: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
+000004a0: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
+000004b0: 6173 7365 7473 2f69 6d67 732f 4578 6365  assets/imgs/Exce
+000004c0: 7074 4e6f 7469 6669 6572 5f6c 6f67 6f2e  ptNotifier_logo.
+000004d0: 706e 6729 0d0a 0d0a 3c68 3320 616c 6967  png)....<h3 alig
+000004e0: 6e3d 2263 656e 7465 7222 3e49 6e74 6567  n="center">Integ
+000004f0: 7261 7465 7320 4149 2d61 7373 6973 7465  rates AI-assiste
+00000500: 6420 6465 6275 6767 696e 6720 6e6f 7469  d debugging noti
+00000510: 6669 6361 7469 6f6e 7320 696e 746f 2050  fications into P
+00000520: 7974 686f 6e20 7472 792d 6578 6365 7074  ython try-except
+00000530: 2073 7461 7465 6d65 6e74 7320 666f 7220   statements for 
+00000540: 7661 7269 6f75 7320 6d65 7373 6167 696e  various messagin
+00000550: 6720 6170 706c 6963 6174 696f 6e73 2e20  g applications. 
+00000560: 3c2f 6833 3e0d 0a0d 0a3c 7020 616c 6967  </h3>....<p alig
+00000570: 6e3d 2263 656e 7465 7222 3e0d 0a3c 6120  n="center">..<a 
+00000580: 6872 6566 3d22 2868 7474 7073 3a2f 2f69  href="(https://i
+00000590: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000005a0: 6467 652f 7079 7069 2d45 7863 6570 744e  dge/pypi-ExceptN
+000005b0: 6f74 6966 6965 722d 6f72 616e 6765 223e  otifier-orange">
+000005c0: 3c2f 613e 0d0a 3c61 2068 7265 663d 2268  </a>..<a href="h
+000005d0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000005e0: 7072 6f6a 6563 742f 6578 6365 7074 6e6f  project/exceptno
+000005f0: 7469 6669 6572 2f22 3e3c 696d 6720 616c  tifier/"><img al
+00000600: 743d 2250 7950 4922 2073 7263 3d22 6874  t="PyPI" src="ht
+00000610: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000620: 732e 696f 2f70 7970 692f 762f 6578 6365  s.io/pypi/v/exce
+00000630: 7074 6e6f 7469 6669 6572 223e 3c2f 613e  ptnotifier"></a>
+00000640: 0d0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000650: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
+00000660: 6a65 6374 2f65 7863 6570 746e 6f74 6966  ject/exceptnotif
+00000670: 6965 7222 3e3c 696d 6720 616c 743d 2244  ier"><img alt="D
+00000680: 6f77 6e6c 6f61 6473 2220 7372 633d 2268  ownloads" src="h
+00000690: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+000006a0: 2f62 6164 6765 2f65 7863 6570 746e 6f74  /badge/exceptnot
+000006b0: 6966 6965 7222 3e3c 2f61 3e0d 0a3c 6120  ifier"></a>..<a 
+000006c0: 6872 6566 3d22 6874 7470 733a 2f2f 616e  href="https://an
+000006d0: 6163 6f6e 6461 2e6f 7267 2f63 6f6e 6461  aconda.org/conda
+000006e0: 2d66 6f72 6765 2f65 7863 6570 746e 6f74  -forge/exceptnot
+000006f0: 6966 6965 722f 223e 3c69 6d67 2061 6c74  ifier/"><img alt
+00000700: 3d22 636f 6e64 612d 666f 7267 6522 2073  ="conda-forge" s
+00000710: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000720: 7368 6965 6c64 732e 696f 2f63 6f6e 6461  shields.io/conda
+00000730: 2f64 6e2f 636f 6e64 612d 666f 7267 652f  /dn/conda-forge/
+00000740: 6578 6365 7074 6e6f 7469 6669 6572 2e73  exceptnotifier.s
+00000750: 7667 3f6c 6162 656c 3d63 6f6e 6461 2d66  vg?label=conda-f
+00000760: 6f72 6765 223e 3c2f 613e 0d0a 3c61 2068  orge"></a>..<a h
+00000770: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00000780: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
+00000790: 6b22 3e3c 696d 6720 616c 743d 2243 6f64  k"><img alt="Cod
+000007a0: 6520 7374 796c 653a 2062 6c61 636b 2220  e style: black" 
+000007b0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000007c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000007d0: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
+000007e0: 6c61 636b 2d30 3030 3030 302e 7376 6722  lack-000000.svg"
+000007f0: 3e3c 2f61 3e0d 0a3c 2f70 3e0d 0a0d 0a21  ></a>..</p>....!
+00000800: 5b5d 2868 7474 7073 3a2f 2f67 6974 6875  [](https://githu
+00000810: 622e 636f 6d2f 6473 6461 6e69 656c 7061  b.com/dsdanielpa
+00000820: 726b 2f45 7863 6570 744e 6f74 6966 6965  rk/ExceptNotifie
+00000830: 722f 626c 6f62 2f6d 6169 6e2f 6173 7365  r/blob/main/asse
+00000840: 7473 2f69 6d67 732f 6d61 696e 322e 706e  ts/imgs/main2.pn
+00000850: 6729 0d0a 0d0a 2320 5079 7468 6f6e 2050  g)....# Python P
+00000860: 6163 6b61 6765 3a20 4578 6365 7074 4e6f  ackage: ExceptNo
+00000870: 7469 6669 6572 0d0a 2323 2323 2320 5072  tifier..##### Pr
+00000880: 6f76 6964 6573 2061 206e 6f74 6966 6963  ovides a notific
+00000890: 6174 696f 6e20 6672 6f6d 2074 6865 2061  ation from the a
+000008a0: 7070 6c69 6361 7469 6f6e 2073 686f 776e  pplication shown
+000008b0: 2069 6e20 7468 6520 6361 7074 7572 6564   in the captured
+000008c0: 2073 6372 6565 6e2e 0d0a 2054 6865 2060   screen... The `
+000008d0: 4578 6365 7074 4e6f 7469 6669 6572 6020  ExceptNotifier` 
+000008e0: 5079 7468 6f6e 2070 6163 6b61 6765 206f  Python package o
+000008f0: 6666 6572 7320 6120 666c 6578 6962 6c65  ffers a flexible
+00000900: 2061 7070 726f 6163 6820 746f 2072 6563   approach to rec
+00000910: 6569 7669 6e67 206e 6f74 6966 6963 6174  eiving notificat
+00000920: 696f 6e73 2062 7920 656e 6861 6e63 696e  ions by enhancin
+00000930: 6720 5079 7468 6f6e 2773 2074 7279 2d65  g Python's try-e
+00000940: 7863 6570 7420 7374 6174 656d 656e 742e  xcept statement.
+00000950: 2054 6869 7320 7061 636b 6167 6520 656e   This package en
+00000960: 6162 6c65 7320 796f 7520 746f 2072 6563  ables you to rec
+00000970: 6569 7665 2061 6c65 7274 7320 7468 726f  eive alerts thro
+00000980: 7567 6820 7661 7269 6f75 7320 6d65 7373  ugh various mess
+00000990: 6167 696e 6720 6170 706c 6963 6174 696f  aging applicatio
+000009a0: 6e73 206f 7220 656d 6169 6c73 2e0d 0a3c  ns or emails...<
+000009b0: 4272 3e3c 6272 3e0d 0a57 6974 6820 6045  Br><br>..With `E
+000009c0: 7863 6570 744e 6f74 6966 6965 7260 2c20  xceptNotifier`, 
+000009d0: 796f 7520 6361 6e20 6f62 7461 696e 2064  you can obtain d
+000009e0: 6574 6169 6c65 6420 636f 6d70 696c 6174  etailed compilat
+000009f0: 696f 6e20 6572 726f 7273 2c20 696e 636c  ion errors, incl
+00000a00: 7564 696e 6720 6465 6275 6720 696e 666f  uding debug info
+00000a10: 726d 6174 696f 6e2c 2073 656e 7420 6469  rmation, sent di
+00000a20: 7265 6374 6c79 2074 6f20 796f 7572 2070  rectly to your p
+00000a30: 7265 6665 7272 6564 206d 6573 7361 6769  referred messagi
+00000a40: 6e67 2070 6c61 7466 6f72 6d20 6f72 2065  ng platform or e
+00000a50: 6d61 696c 2e20 4279 2069 6e74 6567 7261  mail. By integra
+00000a60: 7469 6e67 204f 7065 6e41 4927 7320 4368  ting OpenAI's Ch
+00000a70: 6174 4750 542c 2079 6f75 2063 616e 2072  atGPT, you can r
+00000a80: 6563 6569 7665 2061 6464 6974 696f 6e61  eceive additiona
+00000a90: 6c20 6572 726f 7220 636f 6465 2069 6e66  l error code inf
+00000aa0: 6f72 6d61 7469 6f6e 2061 7320 6c6f 6e67  ormation as long
+00000ab0: 2061 7320 796f 7520 7072 6f76 6964 6520   as you provide 
+00000ac0: 7468 6520 7265 7175 6972 6564 2041 5049  the required API
+00000ad0: 206d 6f64 656c 206e 616d 6520 616e 6420   model name and 
+00000ae0: 6b65 792e 2054 6869 7320 6665 6174 7572  key. This featur
+00000af0: 6520 656e 7375 7265 7320 7468 6174 2065  e ensures that e
+00000b00: 7272 6f72 2068 616e 646c 696e 6720 616e  rror handling an
+00000b10: 6420 6e6f 7469 6669 6361 7469 6f6e 7320  d notifications 
+00000b20: 6172 6520 6d6f 7265 2069 6e66 6f72 6d61  are more informa
+00000b30: 7469 7665 2061 6e64 2061 6363 6573 7369  tive and accessi
+00000b40: 626c 652c 2073 7472 6561 6d6c 696e 696e  ble, streamlinin
+00000b50: 6720 796f 7572 2064 6562 7567 6769 6e67  g your debugging
+00000b60: 2070 726f 6365 7373 2e0d 0a0d 0a3c 4272   process.....<Br
+00000b70: 3e0d 0a0d 0a23 2323 2320 436f 756c 6420  >....#### Could 
+00000b80: 796f 7520 6b69 6e64 6c79 2061 6464 2074  you kindly add t
+00000b90: 6869 7320 6261 6467 6520 746f 2079 6f75  his badge to you
+00000ba0: 7220 7265 706f 7369 746f 7279 3f0d 0a0d  r repository?...
+00000bb0: 0a60 6060 0d0a 215b 4578 6365 7074 2d4e  .```..![Except-N
+00000bc0: 6f74 6966 6965 725d 2868 7474 7073 3a2f  otifier](https:/
+00000bd0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000be0: 6261 6467 652f 7079 7069 2d45 7863 6570  badge/pypi-Excep
+00000bf0: 744e 6f74 6966 6965 722d 6f72 616e 6765  tNotifier-orange
+00000c00: 290d 0a60 6060 0d0a 0d0a 0d0a 3c62 723e  )..```......<br>
+00000c10: 3c62 723e 0d0a 0d0a 2323 2320 5375 7070  <br>....### Supp
+00000c20: 6f72 7469 6e67 2041 7070 6c69 6361 7469  orting Applicati
+00000c30: 6f6e 730d 0a0d 0a2d 205b 5465 6c65 6772  ons....- [Telegr
+00000c40: 616d 5d28 6874 7470 733a 2f2f 7465 6c65  am](https://tele
+00000c50: 6772 616d 2e6f 7267 2f29 0d0a 2d20 5b44  gram.org/)..- [D
+00000c60: 6973 636f 7264 5d28 6874 7470 733a 2f2f  iscord](https://
+00000c70: 6469 7363 6f72 642e 636f 6d2f 290d 0a2d  discord.com/)..-
+00000c80: 205b 536c 6163 6b5d 2868 7474 7073 3a2f   [Slack](https:/
+00000c90: 2f73 6c61 636b 2e63 6f6d 2f29 0d0a 2d20  /slack.com/)..- 
+00000ca0: 5b47 6f6f 676c 6520 4d61 696c 5d28 6874  [Google Mail](ht
+00000cb0: 7470 733a 2f2f 6d61 696c 2e67 6f6f 676c  tps://mail.googl
+00000cc0: 652e 636f 6d2f 290d 0a2d 205b 4c69 6e65  e.com/)..- [Line
+00000cd0: 5d28 6874 7470 733a 2f2f 6c69 6e65 2e6d  ](https://line.m
+00000ce0: 652f 656e 2f29 0d0a 2d20 5b41 5753 2043  e/en/)..- [AWS C
+00000cf0: 6869 6d65 5d28 6874 7470 733a 2f2f 6177  hime](https://aw
+00000d00: 732e 616d 617a 6f6e 2e63 6f6d 2f6b 6f2f  s.amazon.com/ko/
+00000d10: 6368 696d 652f 646f 776e 6c6f 6164 2d63  chime/download-c
+00000d20: 6869 6d65 2f29 0d0a 2d20 5b4d 6963 726f  hime/)..- [Micro
+00000d30: 736f 6674 2054 6561 6d73 5d28 6874 7470  soft Teams](http
+00000d40: 733a 2f2f 7777 772e 6d69 6372 6f73 6f66  s://www.microsof
+00000d50: 742e 636f 6d2f 656e 2f6d 6963 726f 736f  t.com/en/microso
+00000d60: 6674 2d74 6561 6d73 2f64 6f77 6e6c 6f61  ft-teams/downloa
+00000d70: 642d 6170 7029 0d0a 2d20 5b4b 616b 616f  d-app)..- [Kakao
+00000d80: 2054 616c 6b5d 2868 7474 7073 3a2f 2f77   Talk](https://w
+00000d90: 7777 2e6b 616b 616f 636f 7270 2e63 6f6d  ww.kakaocorp.com
+00000da0: 2f70 6167 652f 7365 7276 6963 652f 7365  /page/service/se
+00000db0: 7276 6963 652f 4b61 6b61 6f54 616c 6b3f  rvice/KakaoTalk?
+00000dc0: 6c61 6e67 3d65 6e29 0d0a 2d20 534d 5320  lang=en)..- SMS 
+00000dd0: 5365 6e64 696e 6720 7573 696e 6720 5b54  Sending using [T
+00000de0: 7769 6c69 6f5d 2868 7474 7073 3a2f 2f77  wilio](https://w
+00000df0: 7777 2e74 7769 6c69 6f2e 636f 6d2f 656e  ww.twilio.com/en
+00000e00: 2d75 7329 0d0a 2d20 4465 736b 746f 7020  -us)..- Desktop 
+00000e10: 4e6f 7469 6669 6361 7469 6f6e 2075 7369  Notification usi
+00000e20: 6e67 205b 506c 7965 725d 2868 7474 7073  ng [Plyer](https
+00000e30: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b69  ://github.com/ki
+00000e40: 7679 2f70 6c79 6572 290d 0a2d 2042 6565  vy/plyer)..- Bee
+00000e50: 7020 536f 756e 6420 6672 6f6d 205b 7379  p Sound from [sy
+00000e60: 7374 656d 5d28 6874 7470 733a 2f2f 646f  stem](https://do
+00000e70: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
+00000e80: 6c69 6272 6172 792f 7769 6e73 6f75 6e64  library/winsound
+00000e90: 2e68 746d 6c29 0d0a 0d0a 3c42 723e 0d0a  .html)....<Br>..
+00000ea0: 0d0a 2323 2320 4149 2044 6562 7567 6769  ..### AI Debuggi
+00000eb0: 6e67 2075 7369 6e67 204f 7065 6e41 4920  ng using OpenAI 
+00000ec0: 4150 490d 0a49 6620 796f 7520 6861 7665  API..If you have
+00000ed0: 204f 7065 6e41 4920 4150 4920 4b65 7920   OpenAI API Key 
+00000ee0: 616e 6420 6d6f 6465 6c20 6e61 6d65 2c20  and model name, 
+00000ef0: 796f 7520 6361 6e20 6765 7420 696e 666f  you can get info
+00000f00: 726d 6174 696f 6e20 616e 6420 636f 6465  rmation and code
+00000f10: 2065 7861 6d70 6c65 7320 666f 7220 6465   examples for de
+00000f20: 6275 6767 696e 6720 696e 2061 6e79 2061  bugging in any a
+00000f30: 7070 6c69 6361 7469 6f6e 2e0d 0a2d 205b  pplication...- [
+00000f40: 4f50 454e 2041 4920 4150 495d 2868 7474  OPEN AI API](htt
+00000f50: 7073 3a2f 2f70 6c61 7466 6f72 6d2e 6f70  ps://platform.op
+00000f60: 656e 6169 2e63 6f6d 2f64 6f63 732f 696e  enai.com/docs/in
+00000f70: 7472 6f64 7563 7469 6f6e 290d 0a0d 0a0d  troduction).....
+00000f80: 0a3c 6272 3e3c 6272 3e0d 0a0d 0a23 2051  .<br><br>....# Q
+00000f90: 7569 636b 2053 7461 7274 0d0a 6060 6062  uick Start..```b
+00000fa0: 6173 680d 0a70 6970 2069 6e73 7461 6c6c  ash..pip install
+00000fb0: 2045 7863 6570 744e 6f74 6966 6965 720d   ExceptNotifier.
+00000fc0: 0a70 6970 2069 6e73 7461 6c6c 2065 7863  .pip install exc
+00000fd0: 6570 746e 6f74 6966 6965 720d 0a0d 0a63  eptnotifier....c
+00000fe0: 6f6e 6461 2069 6e73 7461 6c6c 2045 7863  onda install Exc
+00000ff0: 6570 744e 6f74 6966 6965 720d 0a63 6f6e  eptNotifier..con
+00001000: 6461 2069 6e73 7461 6c6c 2065 7863 6570  da install excep
+00001010: 746e 6f74 6966 6965 720d 0a60 6060 0d0a  tnotifier..```..
+00001020: 0d0a 3c62 723e 0d0a 0d0a 0d0a 2320 4170  ..<br>......# Ap
+00001030: 7020 5365 7475 7020 4f76 6572 7669 6577  p Setup Overview
+00001040: 0d0a 0d0a 2d20 5468 6520 7661 7269 6162  ....- The variab
+00001050: 6c65 7320 696e 2074 6865 2066 6f6c 6c6f  les in the follo
+00001060: 7769 6e67 2074 6162 6c65 206d 7573 7420  wing table must 
+00001070: 6e6f 7420 6265 2063 6f6e 7461 6d69 6e61  not be contamina
+00001080: 7465 642e 0d0a 2d20 4465 7065 6e64 696e  ted...- Dependin
+00001090: 6720 6f6e 2074 6865 2073 6974 7561 7469  g on the situati
+000010a0: 6f6e 2c20 636f 6e73 6964 6572 2064 6573  on, consider des
+000010b0: 6967 6e61 7469 6e67 2074 6865 6d20 6173  ignating them as
+000010c0: 2067 6c6f 6261 6c20 7661 7269 6162 6c65   global variable
+000010d0: 7320 666f 7220 7573 652e 0d0a 2d20 4966  s for use...- If
+000010e0: 2079 6f75 2061 7265 2075 7369 6e67 2054   you are using T
+000010f0: 656c 6567 7261 6d2c 2061 6e20 6578 616d  elegram, an exam
+00001100: 706c 6520 6973 2061 7474 6163 6865 6420  ple is attached 
+00001110: 6173 2061 6e20 696d 6167 652e 0d0a 2d20  as an image...- 
+00001120: 4173 2079 6f75 2061 6c72 6561 6479 206b  As you already k
+00001130: 6e6f 772c 2041 5049 204b 6579 7320 6f72  now, API Keys or
+00001140: 2073 6563 7572 6974 7920 746f 6b65 6e73   security tokens
+00001150: 206d 7573 7420 6265 2073 6563 7572 6564   must be secured
+00001160: 2e20 4e6f 7465 2074 6861 7420 7468 6520  . Note that the 
+00001170: 6b65 7920 7661 6c75 6573 2077 6869 6368  key values which
+00001180: 2065 7870 6f73 7572 6564 2069 6e20 6769   exposured in gi
+00001190: 7468 7562 2077 696c 6c20 6265 2065 7870  thub will be exp
+000011a0: 6972 6564 2061 6674 6572 2069 6e73 6563  ired after insec
+000011b0: 7572 6564 2e0d 0a0d 0a7c 2041 7070 207c  ured.....| App |
+000011c0: 2052 6571 7569 7265 6420 5661 7269 6162   Required Variab
+000011d0: 6c65 7320 7c20 4672 6565 206f 7220 5061  les | Free or Pa
+000011e0: 6964 207c 2045 6173 6520 6f66 2053 6574  id | Ease of Set
+000011f0: 7570 207c 2054 696d 6520 5265 7175 6972  up | Time Requir
+00001200: 6564 2066 6f72 2053 6574 7570 7c47 7569  ed for Setup|Gui
+00001210: 6465 2054 7574 6f72 6961 6c20 4c69 6e6b  de Tutorial Link
+00001220: 7c0d 0a7c 3a2d 2d3a 7c3a 2d2d 7c3a 2d2d  |..|:--:|:--|:--
+00001230: 3a7c 3a2d 2d3a 7c3a 2d2d 3a7c 3a2d 2d2d  :|:--:|:--:|:---
+00001240: 3a7c 0d0a 7c42 6565 707c 4e2f 417c 4672  :|..|Beep|N/A|Fr
+00001250: 6565 7c4e 2f41 7c30 206d 696e 7c5b 4578  ee|N/A|0 min|[Ex
+00001260: 6365 7074 4265 6570 5d28 6874 7470 733a  ceptBeep](https:
+00001270: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7364  //github.com/dsd
+00001280: 616e 6965 6c70 6172 6b2f 4578 6365 7074  anielpark/Except
+00001290: 4e6f 7469 6669 6572 2f62 6c6f 622f 6d61  Notifier/blob/ma
+000012a0: 696e 2f64 6f63 756d 656e 7473 2f45 7863  in/documents/Exc
+000012b0: 6570 7442 6565 702f 4755 4944 452e 6d64  eptBeep/GUIDE.md
+000012c0: 297c 0d0a 7c44 6573 6b74 6f70 7c4e 2f41  )|..|Desktop|N/A
+000012d0: 7c46 7265 657c 4e2f 417c 3020 6d69 6e7c  |Free|N/A|0 min|
+000012e0: 5b45 7863 6570 7444 6573 6b74 6f70 5d28  [ExceptDesktop](
+000012f0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001300: 6f6d 2f64 7364 616e 6965 6c70 6172 6b2f  om/dsdanielpark/
+00001310: 4578 6365 7074 4e6f 7469 6669 6572 2f62  ExceptNotifier/b
+00001320: 6c6f 622f 6d61 696e 2f64 6f63 756d 656e  lob/main/documen
+00001330: 7473 2f45 7863 6570 7444 6573 6b74 6f70  ts/ExceptDesktop
+00001340: 2f47 5549 4445 2e6d 6429 7c0d 0a7c 5465  /GUIDE.md)|..|Te
+00001350: 6c65 6772 616d 7c60 5f54 454c 4547 5241  legram|`_TELEGRA
+00001360: 4d5f 544f 4b45 4e60 7c46 7265 656d 6975  M_TOKEN`|Freemiu
+00001370: 6d7c 4561 7379 7c32 6d69 6e7c 5b45 7863  m|Easy|2min|[Exc
+00001380: 6570 7454 656c 6567 7261 6d5d 2868 7474  eptTelegram](htt
+00001390: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000013a0: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+000013b0: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+000013c0: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+000013d0: 4578 6365 7074 5465 6c65 6772 616d 2f47  ExceptTelegram/G
+000013e0: 5549 4445 2e6d 6429 7c0d 0a7c 4469 7363  UIDE.md)|..|Disc
+000013f0: 6f72 647c 605f 4449 5343 4f52 445f 5745  ord|`_DISCORD_WE
+00001400: 4248 4f4f 4b5f 5552 4c60 7c46 7265 656d  BHOOK_URL`|Freem
+00001410: 6975 6d7c 4561 7379 7c31 6d69 6e7c 5b45  ium|Easy|1min|[E
+00001420: 7863 6570 7444 6973 636f 7264 5d28 6874  xceptDiscord](ht
+00001430: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001440: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+00001450: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+00001460: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
+00001470: 2f45 7863 6570 7454 656c 6567 7261 6d2f  /ExceptTelegram/
+00001480: 4755 4944 452e 6d64 297c 0d0a 7c41 5753  GUIDE.md)|..|AWS
+00001490: 2043 6869 6d65 7c60 5f43 4849 4d45 5f57   Chime|`_CHIME_W
+000014a0: 4542 484f 4f4b 5f55 524c 607c 4672 6565  EBHOOK_URL`|Free
+000014b0: 6d69 756d 7c45 6173 797c 316d 696e 7c5b  mium|Easy|1min|[
+000014c0: 4578 6365 7074 4368 696d 655d 2868 7474  ExceptChime](htt
+000014d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000014e0: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+000014f0: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00001500: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+00001510: 4578 6365 7074 4368 696d 652f 4755 4944  ExceptChime/GUID
+00001520: 452e 6d64 297c 0d0a 7c53 6c61 636b 7c60  E.md)|..|Slack|`
+00001530: 5f53 4c41 434b 5f57 4542 484f 4f4b 5f55  _SLACK_WEBHOOK_U
+00001540: 524c 607c 4672 6565 6d69 756d 7c45 6173  RL`|Freemium|Eas
+00001550: 797c 336d 696e 7c5b 4578 6365 7074 536c  y|3min|[ExceptSl
+00001560: 6163 6b5d 2868 7474 7073 3a2f 2f67 6974  ack](https://git
+00001570: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00001580: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00001590: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+000015a0: 6375 6d65 6e74 732f 4578 6365 7074 536c  cuments/ExceptSl
+000015b0: 6163 6b2f 4755 4944 452e 6d64 297c 0d0a  ack/GUIDE.md)|..
+000015c0: 7c47 2d4d 6169 6c7c 605f 4741 4d49 4c5f  |G-Mail|`_GAMIL_
+000015d0: 5245 4349 5049 454e 545f 4144 4452 602c  RECIPIENT_ADDR`,
+000015e0: 2060 5f47 4d41 494c 5f53 454e 4445 525f   `_GMAIL_SENDER_
+000015f0: 4144 4452 602c 2060 5f47 4d41 494c 5f41  ADDR`, `_GMAIL_A
+00001600: 5050 5f50 4153 5357 4f52 445f 4f46 5f53  PP_PASSWORD_OF_S
+00001610: 454e 4445 5260 207c 5265 7374 7269 6374  ENDER` |Restrict
+00001620: 6564 2066 7265 657c 4d65 6469 756d 7c33  ed free|Medium|3
+00001630: 6d69 6e7c 5b45 7863 6570 744d 6169 6c5d  min|[ExceptMail]
+00001640: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001650: 636f 6d2f 6473 6461 6e69 656c 7061 726b  com/dsdanielpark
+00001660: 2f45 7863 6570 744e 6f74 6966 6965 722f  /ExceptNotifier/
+00001670: 626c 6f62 2f6d 6169 6e2f 646f 6375 6d65  blob/main/docume
+00001680: 6e74 732f 4578 6365 7074 4d61 696c 2f47  nts/ExceptMail/G
+00001690: 5549 4445 2e6d 6429 7c0d 0a7c 4c69 6e65  UIDE.md)|..|Line
+000016a0: 7c60 5f4c 494e 455f 4e4f 5449 4659 5f41  |`_LINE_NOTIFY_A
+000016b0: 5049 5f54 4f4b 454e 607c 4672 6565 6d69  PI_TOKEN`|Freemi
+000016c0: 756d 7c4d 6564 6975 6d7c 346d 696e 7c5b  um|Medium|4min|[
+000016d0: 4578 6365 7074 4c69 6e65 5d28 6874 7470  ExceptLine](http
+000016e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+000016f0: 7364 616e 6965 6c70 6172 6b2f 4578 6365  sdanielpark/Exce
+00001700: 7074 4e6f 7469 6669 6572 2f62 6c6f 622f  ptNotifier/blob/
+00001710: 6d61 696e 2f64 6f63 756d 656e 7473 2f45  main/documents/E
+00001720: 7863 6570 744c 696e 652f 4755 4944 452e  xceptLine/GUIDE.
+00001730: 6d64 297c 0d0a 7c53 4d53 7c60 5f54 5749  md)|..|SMS|`_TWI
+00001740: 4c49 4f5f 5349 4460 2c20 605f 5457 494c  LIO_SID`, `_TWIL
+00001750: 494f 5f54 4f4b 454e 602c 2060 5f52 4543  IO_TOKEN`, `_REC
+00001760: 4950 4945 4e54 5f50 484f 4e45 5f4e 554d  IPIENT_PHONE_NUM
+00001770: 4245 5260 2c20 605f 5345 4e44 4552 5f50  BER`, `_SENDER_P
+00001780: 484f 4e45 5f4e 554d 4245 5260 7c4e 6f74  HONE_NUMBER`|Not
+00001790: 2066 7265 657c 4d65 6469 756d 7c35 6d69   free|Medium|5mi
+000017a0: 6e7c 5b45 7863 6570 7453 4d53 5d28 6874  n|[ExceptSMS](ht
+000017b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000017c0: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+000017d0: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+000017e0: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
+000017f0: 2f45 7863 6570 7453 4d53 2f47 5549 4445  /ExceptSMS/GUIDE
+00001800: 2e6d 6429 7c0d 0a7c 4d69 6372 6f73 6f66  .md)|..|Microsof
+00001810: 7420 5465 616d 737c 605f 5445 414d 535f  t Teams|`_TEAMS_
+00001820: 5745 4248 4f4f 4b5f 5552 4c60 7c4e 6f74  WEBHOOK_URL`|Not
+00001830: 2046 7265 657c 4d65 6469 756d 7c35 6d69   Free|Medium|5mi
+00001840: 6e7c 5b45 7863 6570 7454 6561 6d73 5d28  n|[ExceptTeams](
+00001850: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001860: 6f6d 2f64 7364 616e 6965 6c70 6172 6b2f  om/dsdanielpark/
+00001870: 4578 6365 7074 4e6f 7469 6669 6572 2f62  ExceptNotifier/b
+00001880: 6c6f 622f 6d61 696e 2f64 6f63 756d 656e  lob/main/documen
+00001890: 7473 2f45 7863 6570 7454 6561 6d73 2f47  ts/ExceptTeams/G
+000018a0: 5549 4445 2e6d 6429 7c0d 0a7c 4b61 6b61  UIDE.md)|..|Kaka
+000018b0: 6f54 616c 6b7c 605f 4b41 4b41 4f5f 544f  oTalk|`_KAKAO_TO
+000018c0: 4b45 4e5f 5041 5448 607c 4672 6565 6d69  KEN_PATH`|Freemi
+000018d0: 756d 7c48 656c 6c7c 3e3d 3130 6d69 6e28  um|Hell|>=10min(
+000018e0: 546f 6b65 6e20 7265 6672 6573 6865 7320  Token refreshes 
+000018f0: 6461 696c 7929 7c5b 4578 6365 7074 4b61  daily)|[ExceptKa
+00001900: 6b61 6f5d 2868 7474 7073 3a2f 2f67 6974  kao](https://git
+00001910: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00001920: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00001930: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+00001940: 6375 6d65 6e74 732f 4578 6365 7074 4b61  cuments/ExceptKa
+00001950: 6b61 6f2f 4755 4944 452e 6d64 297c 0d0a  kao/GUIDE.md)|..
+00001960: 0d0a 0d0a 4966 2079 6f75 2061 6464 2074  ....If you add t
+00001970: 6865 2066 6f6c 6c6f 7769 6e67 2074 776f  he following two
+00001980: 2076 6172 6961 626c 6573 2074 6f20 7468   variables to th
+00001990: 6520 7265 7175 6972 6564 2076 6172 6961  e required varia
+000019a0: 626c 6573 2066 6f72 2065 6163 6820 6170  bles for each ap
+000019b0: 706c 6963 6174 696f 6e20 696e 2074 6865  plication in the
+000019c0: 2074 6162 6c65 2061 626f 7665 2c20 796f   table above, yo
+000019d0: 7520 6361 6e20 7265 6365 6976 6520 6572  u can receive er
+000019e0: 726f 7220 6c6f 6361 7469 6f6e 2061 6e64  ror location and
+000019f0: 2065 7870 6c61 6e61 7469 6f6e 2c20 6173   explanation, as
+00001a00: 2077 656c 6c20 6173 2065 7861 6d70 6c65   well as example
+00001a10: 732c 2066 726f 6d20 4f70 656e 4149 2773  s, from OpenAI's
+00001a20: 206d 6f64 656c 0d0a 0d0a 7c20 4150 4920   model....| API 
+00001a30: 7c20 5265 7175 6972 6564 2056 6172 6961  | Required Varia
+00001a40: 626c 6573 207c 2046 7265 6520 6f72 2050  bles | Free or P
+00001a50: 6169 6420 7c20 4561 7365 206f 6620 5365  aid | Ease of Se
+00001a60: 7475 7020 7c20 5469 6d65 2052 6571 7569  tup | Time Requi
+00001a70: 7265 6420 666f 7220 5365 7475 707c 4775  red for Setup|Gu
+00001a80: 6964 6520 5475 746f 7269 616c 204c 696e  ide Tutorial Lin
+00001a90: 6b7c 0d0a 7c3a 2d2d 3a7c 3a2d 2d7c 3a2d  k|..|:--:|:--|:-
+00001aa0: 2d3a 7c3a 2d2d 3a7c 3a2d 2d3a 7c3a 2d2d  -:|:--:|:--:|:--
+00001ab0: 2d3a 7c0d 0a7c 204f 7065 6e41 4920 4150  -:|..| OpenAI AP
+00001ac0: 4920 7c60 5265 7175 6972 6564 2076 6172  I |`Required var
+00001ad0: 6961 626c 6573 2066 6f72 2065 6163 6820  iables for each 
+00001ae0: 6170 706c 6963 6174 696f 6e60 2b20 605f  application`+ `_
+00001af0: 4f50 454e 5f41 495f 4d4f 4445 4c60 2c60  OPEN_AI_MODEL`,`
+00001b00: 5f4f 5045 4e5f 4149 5f41 5049 607c 4e6f  _OPEN_AI_API`|No
+00001b10: 7420 6672 6565 7c45 6173 797c 326d 696e  t free|Easy|2min
+00001b20: 7c5b 4150 494f 7065 6e41 495d 2868 7474  |[APIOpenAI](htt
+00001b30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001b40: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+00001b50: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00001b60: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+00001b70: 4150 494f 7065 6e41 492f 4755 4944 452e  APIOpenAI/GUIDE.
+00001b80: 6d64 297c 0d0a 0d0a 0d0a 3c62 723e 3c62  md)|......<br><b
+00001b90: 723e 0d0a 0d0a 2320 312e 204b 6579 2046  r>....# 1. Key F
+00001ba0: 6561 7475 7265 730d 0a54 6f20 7573 6520  eatures..To use 
+00001bb0: 7468 6520 6465 7369 7265 6420 6170 706c  the desired appl
+00001bc0: 6963 6174 696f 6e2c 2079 6f75 206d 7573  ication, you mus
+00001bd0: 7420 6465 6669 6e65 2074 6865 206e 6563  t define the nec
+00001be0: 6573 7361 7279 2076 6172 6961 626c 6573  essary variables
+00001bf0: 2e20 456e 7375 7265 2074 6861 7420 7468  . Ensure that th
+00001c00: 6520 7661 7269 6162 6c65 206e 616d 6573  e variable names
+00001c10: 2072 656d 6169 6e20 756e 6368 616e 6765   remain unchange
+00001c20: 642c 2061 6e64 2079 6f75 2063 616e 2075  d, and you can u
+00001c30: 7365 2065 6974 6865 7220 6c6f 6361 6c20  se either local 
+00001c40: 6f72 2067 6c6f 6261 6c20 7661 7269 6162  or global variab
+00001c50: 6c65 732e 2049 6620 796f 7520 6172 6520  les. If you are 
+00001c60: 7573 696e 6720 6054 656c 6567 7261 6d60  using `Telegram`
+00001c70: 2c20 616e 2065 7861 6d70 6c65 2069 7320  , an example is 
+00001c80: 6174 7461 6368 6564 2061 7320 616e 2069  attached as an i
+00001c90: 6d61 6765 2e0d 0a0d 0a23 2320 312d 312e  mage.....## 1-1.
+00001ca0: 2045 7863 6570 7460 5b61 7070 4e61 6d65   Except`[appName
+00001cb0: 5d60 0d0a 4966 2079 6f75 2075 7365 2050  ]`..If you use P
+00001cc0: 7974 686f 6e27 7320 7472 7920 6578 6365  ython's try exce
+00001cd0: 7074 2073 7461 7465 6d65 6e74 2061 7320  pt statement as 
+00001ce0: 6974 2069 732c 2062 7574 2063 6861 6e67  it is, but chang
+00001cf0: 6520 6578 6365 7074 2061 7320 666f 6c6c  e except as foll
+00001d00: 6f77 732c 2079 6f75 2063 616e 2072 6563  ows, you can rec
+00001d10: 6569 7665 206e 6f74 6966 6963 6174 696f  eive notificatio
+00001d20: 6e73 2074 6872 6f75 6768 2079 6f75 7220  ns through your 
+00001d30: 6170 706c 6963 6174 696f 6e2e 0d0a 6060  application...``
+00001d40: 600d 0a45 7863 6570 7443 6869 6d65 2c20  `..ExceptChime, 
+00001d50: 4578 6365 7074 5465 6c65 6772 616d 2c20  ExceptTelegram, 
+00001d60: 4578 6365 7074 4469 7363 6f72 642c 2045  ExceptDiscord, E
+00001d70: 7863 6570 7453 4d53 2c20 4578 6365 7074  xceptSMS, Except
+00001d80: 4d61 696c 2c20 4578 6365 7074 4b61 6b61  Mail, ExceptKaka
+00001d90: 6f2c 2045 7863 6570 744c 696e 652c 2045  o, ExceptLine, E
+00001da0: 7863 6570 7453 6c61 636b 2c20 4578 6365  xceptSlack, Exce
+00001db0: 7074 5465 616d 732c 2045 7863 6570 7444  ptTeams, ExceptD
+00001dc0: 6573 6b74 6f70 652c 2045 7863 6570 7442  esktope, ExceptB
+00001dd0: 6565 700d 0a60 6060 0d0a 0d0a 2a45 7861  eep..```....*Exa
+00001de0: 6d70 6c65 2a0d 0a60 6060 7079 7468 6f6e  mple*..```python
+00001df0: 0d0a 6672 6f6d 2045 7863 6570 744e 6f74  ..from ExceptNot
+00001e00: 6966 6965 7220 696d 706f 7274 2045 7863  ifier import Exc
+00001e10: 6570 7454 656c 6765 7261 6d0d 0a5f 5445  eptTelgeram.._TE
+00001e20: 4c45 4752 414d 5f54 4f4b 454e 203d 2022  LEGRAM_TOKEN = "
+00001e30: 7878 7878 220d 0a0d 0a74 7279 3a0d 0a20  xxxx"....try:.. 
+00001e40: 2020 2070 7269 6e74 2831 2f30 290d 0a65     print(1/0)..e
+00001e50: 7863 6570 7420 4578 6365 7074 5465 6c65  xcept ExceptTele
+00001e60: 6772 616d 3a20 2020 2023 2073 656e 6469  gram:    # sendi
+00001e70: 6e67 2065 7863 6570 7420 6d65 7373 6167  ng except messag
+00001e80: 6520 746f 2074 656c 6567 7261 6d0d 0a20  e to telegram.. 
+00001e90: 2020 2073 7973 2e65 7869 7428 290d 0a60     sys.exit()..`
+00001ea0: 6060 0d0a 215b 5d28 6874 7470 733a 2f2f  ``..![](https://
+00001eb0: 6769 7468 7562 2e63 6f6d 2f64 7364 616e  github.com/dsdan
+00001ec0: 6965 6c70 6172 6b2f 4578 6365 7074 4e6f  ielpark/ExceptNo
+00001ed0: 7469 6669 6572 2f62 6c6f 622f 6d61 696e  tifier/blob/main
+00001ee0: 2f61 7373 6574 732f 696d 6773 2f65 7831  /assets/imgs/ex1
+00001ef0: 2e70 6e67 290d 0a0d 0a3c 6272 3e0d 0a0d  .png)....<br>...
+00001f00: 0a23 2320 312d 322e 2041 4920 4465 6262  .## 1-2. AI Debb
+00001f10: 7567 6769 6e67 2049 6e66 6f6d 6174 696f  ugging Infomatio
+00001f20: 6e20 4e6f 7469 6669 6361 7469 6f6e 0d0a  n Notification..
+00001f30: 596f 7520 6361 6e20 7265 6365 6976 6520  You can receive 
+00001f40: 6465 6275 6767 696e 6720 696e 666f 726d  debugging inform
+00001f50: 6174 696f 6e20 6672 6f6d 2043 6861 7447  ation from ChatG
+00001f60: 5054 2076 6961 204f 7065 6e41 4927 7320  PT via OpenAI's 
+00001f70: 4150 4920 7768 656e 2075 7369 6e67 2074  API when using t
+00001f80: 6865 2045 7863 6570 7420 7374 6174 656d  he Except statem
+00001f90: 656e 742e 2054 6865 2073 796e 7461 7820  ent. The syntax 
+00001fa0: 7265 6d61 696e 7320 7468 6520 7361 6d65  remains the same
+00001fb0: 2c20 6275 7420 796f 7527 6c6c 206e 6565  , but you'll nee
+00001fc0: 6420 746f 2063 6f6e 6669 6775 7265 2074  d to configure t
+00001fd0: 6865 7365 2074 776f 2076 6172 6961 626c  hese two variabl
+00001fe0: 6573 3a0d 0a60 5f4f 5045 4e5f 4149 5f4d  es:..`_OPEN_AI_M
+00001ff0: 4f44 454c 602c 605f 4f50 454e 5f41 495f  ODEL`,`_OPEN_AI_
+00002000: 4150 4960 0d0a 0d0a 2a45 7861 6d70 6c65  API`....*Example
+00002010: 2a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  *..```python..fr
+00002020: 6f6d 2045 7863 6570 744e 6f74 6966 6965  om ExceptNotifie
+00002030: 7220 696d 706f 7274 2045 7863 6570 7454  r import ExceptT
+00002040: 656c 6765 7261 6d0d 0a5f 5445 4c45 4752  elgeram.._TELEGR
+00002050: 414d 5f54 4f4b 454e 203d 2022 7878 7878  AM_TOKEN = "xxxx
+00002060: 220d 0a5f 4f50 454e 5f41 495f 4d4f 4445  ".._OPEN_AI_MODE
+00002070: 4c3d 2267 7074 2d33 2e35 2d74 7572 626f  L="gpt-3.5-turbo
+00002080: 220d 0a5f 4f50 454e 5f41 495f 4150 493d  ".._OPEN_AI_API=
+00002090: 2273 6b2d 7878 7878 7878 220d 0a0d 0a74  "sk-xxxxxx"....t
+000020a0: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
+000020b0: 2f30 290d 0a65 7863 6570 7420 4578 6365  /0)..except Exce
+000020c0: 7074 5465 6c65 6772 616d 3a20 2320 7365  ptTelegram: # se
+000020d0: 6e64 696e 6720 6d73 6720 5749 5448 2041  nding msg WITH A
+000020e0: 4920 4445 4255 4747 494e 4720 746f 2074  I DEBUGGING to t
+000020f0: 656c 6567 7261 6d0d 0a20 2020 2073 7973  elegram..    sys
+00002100: 2e65 7869 7428 290d 0a60 6060 0d0a 0d0a  .exit()..```....
+00002110: 215b 5d28 6874 7470 733a 2f2f 6769 7468  ![](https://gith
+00002120: 7562 2e63 6f6d 2f64 7364 616e 6965 6c70  ub.com/dsdanielp
+00002130: 6172 6b2f 4578 6365 7074 4e6f 7469 6669  ark/ExceptNotifi
+00002140: 6572 2f62 6c6f 622f 6d61 696e 2f61 7373  er/blob/main/ass
+00002150: 6574 732f 696d 6773 2f65 7832 2e70 6e67  ets/imgs/ex2.png
+00002160: 290d 0a0d 0a3c 6272 3e0d 0a0d 0a23 2320  )....<br>....## 
+00002170: 312d 332e 2053 7563 6365 7373 605b 6170  1-3. Success`[ap
+00002180: 704e 616d 655d 600d 0a42 7920 706c 6163  pName]`..By plac
+00002190: 696e 6720 7468 6520 7472 7920 6578 6365  ing the try exce
+000021a0: 7074 2069 6e20 7079 7468 6f6e 2061 7420  pt in python at 
+000021b0: 7468 6520 656e 6420 6f66 2074 6865 2074  the end of the t
+000021c0: 7279 2073 7461 7465 6d65 6e74 2c20 6170  ry statement, ap
+000021d0: 706c 6963 6174 696f 6e73 2063 616e 2062  plications can b
+000021e0: 6520 6e6f 7469 6669 6564 2074 6861 7420  e notified that 
+000021f0: 7468 6520 7472 7920 7374 6174 656d 656e  the try statemen
+00002200: 7420 776f 726b 6564 206e 6f72 6d61 6c6c  t worked normall
+00002210: 792e 0d0a 6060 600d 0a53 7563 6365 7373  y...```..Success
+00002220: 4368 696d 652c 2053 7563 6365 7373 5465  Chime, SuccessTe
+00002230: 6c65 6772 616d 2c20 5375 6363 6573 7344  legram, SuccessD
+00002240: 6973 636f 7264 2c20 5375 6363 6573 7353  iscord, SuccessS
+00002250: 4d53 2c20 5375 6363 6573 734d 6169 6c2c  MS, SuccessMail,
+00002260: 2053 7563 6365 7373 4b61 6b61 6f2c 2053   SuccessKakao, S
+00002270: 7563 6365 7373 4c69 6e65 2c20 5375 6363  uccessLine, Succ
+00002280: 6573 7353 6c61 636b 2c20 5375 6363 6573  essSlack, Succes
+00002290: 7354 6561 6d73 2c20 5375 6363 6573 7344  sTeams, SuccessD
+000022a0: 6573 6b74 6f70 652c 2053 7563 6365 7373  esktope, Success
+000022b0: 4265 6570 0d0a 6060 600d 0a2a 4578 616d  Beep..```..*Exam
+000022c0: 706c 652a 0d0a 0d0a 6060 6070 7974 686f  ple*....```pytho
+000022d0: 6e0d 0a66 726f 6d20 4578 6365 7074 4e6f  n..from ExceptNo
+000022e0: 7469 6669 6572 2069 6d70 6f72 7420 5375  tifier import Su
+000022f0: 6363 6573 7354 656c 6765 7261 6d0d 0a5f  ccessTelgeram.._
+00002300: 5445 4c45 4752 414d 5f54 4f4b 454e 203d  TELEGRAM_TOKEN =
+00002310: 2022 7878 7878 220d 0a0d 0a74 7279 3a0d   "xxxx"....try:.
+00002320: 0a20 2020 2070 7269 6e74 2831 2f32 3029  .    print(1/20)
+00002330: 0d0a 2020 2020 5375 6363 6573 7354 656c  ..    SuccessTel
+00002340: 6765 7261 6d28 292e 5f5f 6361 6c6c 5f5f  geram().__call__
+00002350: 2829 2020 2320 7365 6e64 696e 6720 7375  ()  # sending su
+00002360: 6363 6573 7320 6d65 7373 6167 6520 746f  ccess message to
+00002370: 2074 656c 6567 7261 6d0d 0a65 7863 6570   telegram..excep
+00002380: 743a 0d0a 2020 2020 7379 732e 6578 6974  t:..    sys.exit
+00002390: 2829 0d0a 6060 600d 0a0d 0a21 5b5d 2868  ()..```....![](h
+000023a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000023b0: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
+000023c0: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
+000023d0: 6f62 2f6d 6169 6e2f 6173 7365 7473 2f69  ob/main/assets/i
+000023e0: 6d67 732f 6578 332e 706e 6729 0d0a 0d0a  mgs/ex3.png)....
+000023f0: 3c42 723e 0d0a 0d0a 2323 2031 2d34 2e20  <Br>....## 1-4. 
+00002400: 5365 6e64 605b 6170 704e 616d 655d 600d  Send`[appName]`.
+00002410: 0a50 6c61 6365 2069 7420 616e 7977 6865  .Place it anywhe
+00002420: 7265 206f 6e20 7468 6520 6c69 6e65 206f  re on the line o
+00002430: 6620 636f 6465 2079 6f75 2077 616e 742c  f code you want,
+00002440: 2061 6e64 2079 6f75 276c 6c20 6265 206e   and you'll be n
+00002450: 6f74 6966 6965 6420 7768 656e 2074 6861  otified when tha
+00002460: 7420 6c69 6e65 206f 6620 636f 6465 2069  t line of code i
+00002470: 7320 7265 6163 6865 642e 0d0a 6060 600d  s reached...```.
+00002480: 0a53 656e 6443 6869 6d65 2c20 5365 6e64  .SendChime, Send
+00002490: 5465 6c65 6772 616d 2c20 5365 6e64 4469  Telegram, SendDi
+000024a0: 7363 6f72 642c 2053 656e 6453 4d53 2c20  scord, SendSMS, 
+000024b0: 5365 6e64 4d61 696c 2c20 5365 6e64 4b61  SendMail, SendKa
+000024c0: 6b61 6f2c 2053 656e 644c 696e 652c 2053  kao, SendLine, S
+000024d0: 656e 6453 6c61 636b 2c20 5365 6e64 5465  endSlack, SendTe
+000024e0: 616d 732c 2053 656e 6444 6573 6b74 6f70  ams, SendDesktop
+000024f0: 652c 2053 656e 6442 6565 700d 0a60 6060  e, SendBeep..```
+00002500: 0d0a 2a45 7861 6d70 6c65 2a0d 0a0d 0a60  ..*Example*....`
+00002510: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2045  ``python..from E
+00002520: 7863 6570 744e 6f74 6966 6965 7220 696d  xceptNotifier im
+00002530: 706f 7274 2053 656e 6454 656c 6765 7261  port SendTelgera
+00002540: 6d0d 0a5f 5445 4c45 4752 414d 5f54 4f4b  m.._TELEGRAM_TOK
+00002550: 454e 203d 2022 7878 7878 220d 0a0d 0a53  EN = "xxxx"....S
+00002560: 656e 6454 656c 6567 7261 6d28 292e 5f5f  endTelegram().__
+00002570: 6361 6c6c 5f5f 2829 2023 2073 656e 6469  call__() # sendi
+00002580: 6e67 206d 6573 7361 6765 2074 6f20 7465  ng message to te
+00002590: 6c65 6772 616d 0d0a 0d0a 6e6f 7469 203d  legram....noti =
+000025a0: 2053 656e 6454 656c 6567 7261 6d28 290d   SendTelegram().
+000025b0: 0a6e 6f74 6928 2920 2020 2020 2020 2020  .noti()         
+000025c0: 2020 2020 2020 2020 2020 2023 2073 656e             # sen
+000025d0: 6469 6e67 206d 6573 7361 6765 2074 6f20  ding message to 
+000025e0: 7465 6c65 6772 616d 0d0a 6060 600d 0a0d  telegram..```...
+000025f0: 0a21 5b5d 2868 7474 7073 3a2f 2f67 6974  .![](https://git
+00002600: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00002610: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00002620: 6965 722f 626c 6f62 2f6d 6169 6e2f 6173  ier/blob/main/as
+00002630: 7365 7473 2f69 6d67 732f 6578 342e 706e  sets/imgs/ex4.pn
+00002640: 6729 0d0a 0d0a 0d0a 3c62 723e 3c62 723e  g)......<br><br>
+00002650: 0d0a 0d0a 2320 322e 2046 6561 7475 7265  ....# 2. Feature
+00002660: 730d 0a59 6f75 2063 616e 2072 6563 6569  s..You can recei
+00002670: 7665 2064 6562 7567 6769 6e67 2069 6e66  ve debugging inf
+00002680: 6f72 6d61 7469 6f6e 2066 726f 6d20 4368  ormation from Ch
+00002690: 6174 4750 5420 7669 6120 4f70 656e 4149  atGPT via OpenAI
+000026a0: 2773 2041 5049 2077 6865 6e20 7573 696e  's API when usin
+000026b0: 6720 7468 6520 4578 6365 7074 2073 7461  g the Except sta
+000026c0: 7465 6d65 6e74 2e20 5468 6520 7379 6e74  tement. The synt
+000026d0: 6178 2072 656d 6169 6e73 2074 6865 2073  ax remains the s
+000026e0: 616d 652c 2062 7574 2079 6f75 276c 6c20  ame, but you'll 
+000026f0: 6e65 6564 2074 6f20 636f 6e66 6967 7572  need to configur
+00002700: 6520 7468 6573 6520 7477 6f20 7661 7269  e these two vari
+00002710: 6162 6c65 733a 0d0a 605f 4f50 454e 5f41  ables:..`_OPEN_A
+00002720: 495f 4d4f 4445 4c60 2c60 5f4f 5045 4e5f  I_MODEL`,`_OPEN_
+00002730: 4149 5f41 5049 600d 0a0d 0a0d 0a0d 0a23  AI_API`........#
+00002740: 2320 322d 312e 202a 5465 6c65 6772 616d  # 2-1. *Telegram
+00002750: 204e 6f74 6966 6965 722a 0d0a 0d0a 2d20   Notifier*....- 
+00002760: 612e 204f 7065 6e20 796f 7572 2074 656c  a. Open your tel
+00002770: 6567 7261 6d20 6170 7020 616e 6420 7365  egram app and se
+00002780: 6172 6368 2066 6f72 2042 6f74 4661 7468  arch for BotFath
+00002790: 6572 2e20 2841 2062 7569 6c74 2d69 6e20  er. (A built-in 
+000027a0: 5465 6c65 6772 616d 2062 6f74 2074 6861  Telegram bot tha
+000027b0: 7420 6865 6c70 7320 7573 6572 7320 6372  t helps users cr
+000027c0: 6561 7465 2063 7573 746f 6d20 5465 6c65  eate custom Tele
+000027d0: 6772 616d 2062 6f74 7329 203c 6272 3e0d  gram bots) <br>.
+000027e0: 0a2d 2062 2e20 5479 7065 202f 6e65 7762  .- b. Type /newb
+000027f0: 6f74 2074 6f20 6372 6561 7465 2061 206e  ot to create a n
+00002800: 6577 2062 6f74 203c 6272 3e0d 0a2d 2063  ew bot <br>..- c
+00002810: 2e20 4769 7665 2079 6f75 7220 626f 7420  . Give your bot 
+00002820: 6120 6e61 6d65 2026 2061 2075 7365 726e  a name & a usern
+00002830: 616d 6520 3c62 723e 0d0a 2d20 642e 2043  ame <br>..- d. C
+00002840: 6f70 7920 796f 7572 206e 6577 2054 656c  opy your new Tel
+00002850: 6567 7261 6d20 626f 74e2 8099 7320 746f  egram bot...s to
+00002860: 6b65 6e20 3c62 723e 0d0a 0d0a 466f 7220  ken <br>....For 
+00002870: 6d6f 7265 2069 6e66 6f6d 6174 696f 6e2c  more infomation,
+00002880: 2076 6973 6974 205b 5465 6c65 6772 616d   visit [Telegram
+00002890: 2042 6f74 2046 6174 6865 7220 4150 495d   Bot Father API]
+000028a0: 2868 7474 7073 3a2f 2f63 6f72 652e 7465  (https://core.te
+000028b0: 6c65 6772 616d 2e6f 7267 2f62 6f74 732f  legram.org/bots/
+000028c0: 6170 6929 0d0a 3c62 723e 3c62 723e 0d0a  api)..<br><br>..
+000028d0: 200d 0a23 2323 2061 2e20 5769 7468 6f75   ..### a. Withou
+000028e0: 7420 4f70 656e 4149 2041 5049 0d0a 0d0a  t OpenAI API....
+000028f0: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00002900: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
+00002910: 6d70 6f72 7420 4578 6365 7074 5465 6c65  mport ExceptTele
+00002920: 6772 616d 2c20 5375 6363 6573 7354 656c  gram, SuccessTel
+00002930: 6567 7261 6d2c 2053 656e 6454 656c 6567  egram, SendTeleg
+00002940: 7261 6d0d 0a69 6d70 6f72 7420 7379 730d  ram..import sys.
+00002950: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
+00002960: 3d20 4578 6365 7074 5465 6c65 6772 616d  = ExceptTelegram
+00002970: 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a5f 5445  .__call__...._TE
+00002980: 4c45 4752 414d 5f54 4f4b 454e 203d 2022  LEGRAM_TOKEN = "
+00002990: 7878 7878 220d 0a0d 0a74 7279 3a0d 0a20  xxxx"....try:.. 
+000029a0: 2020 2070 7269 6e74 2831 2f30 2920 200d     print(1/0)  .
+000029b0: 0a20 2020 2053 7563 6365 7373 5465 6c65  .    SuccessTele
+000029c0: 6772 616d 2829 2e5f 5f63 616c 6c5f 5f28  gram().__call__(
+000029d0: 2920 2331 2e20 7375 6363 6573 7320 7365  ) #1. success se
+000029e0: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
+000029f0: 0d0a 6578 6365 7074 2045 7863 6570 7454  ..except ExceptT
+00002a00: 656c 6567 7261 6d20 6173 2065 3a20 2020  elegram as e:   
+00002a10: 2020 2023 322e 2065 7863 6570 7420 7365     #2. except se
+00002a20: 6e64 6572 2020 2020 2020 2020 2020 2020  nder            
+00002a30: 0d0a 2020 2020 7379 732e 6578 6974 2829  ..    sys.exit()
+00002a40: 0d0a 0d0a 5365 6e64 5465 6c65 6772 616d  ....SendTelegram
+00002a50: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00002a60: 2020 2020 2023 332e 2063 7573 746f 6d69       #3. customi
+00002a70: 7a65 6420 7365 6e64 6572 2020 2020 200d  zed sender     .
+00002a80: 0a60 6060 0d0a 0d0a 0d0a 215b 5d28 6874  .```......![](ht
+00002a90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002aa0: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+00002ab0: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+00002ac0: 622f 6d61 696e 2f61 7373 6574 732f 696d  b/main/assets/im
+00002ad0: 6773 2f66 6967 3434 2e70 6e67 290d 0a0d  gs/fig44.png)...
+00002ae0: 0a0d 0a23 2323 2062 2e20 5769 7468 204f  ...### b. With O
+00002af0: 7065 6e41 4920 4150 490d 0a60 6060 7079  penAI API..```py
+00002b00: 7468 6f6e 0d0a 6672 6f6d 2045 7863 6570  thon..from Excep
+00002b10: 744e 6f74 6966 6965 7220 696d 706f 7274  tNotifier import
+00002b20: 2045 7863 6570 7454 656c 6567 7261 6d2c   ExceptTelegram,
+00002b30: 2053 7563 6365 7373 5465 6c65 6772 616d   SuccessTelegram
+00002b40: 2c20 5365 6e64 5465 6c65 6772 616d 0d0a  , SendTelegram..
+00002b50: 696d 706f 7274 2073 7973 0d0a 7379 732e  import sys..sys.
+00002b60: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
+00002b70: 6570 7454 656c 6567 7261 6d2e 5f5f 6361  eptTelegram.__ca
+00002b80: 6c6c 5f5f 0d0a 0d0a 5f54 454c 4547 5241  ll__...._TELEGRA
+00002b90: 4d5f 544f 4b45 4e20 3d20 2278 7878 7822  M_TOKEN = "xxxx"
+00002ba0: 0d0a 5f4f 5045 4e5f 4149 5f4d 4f44 454c  .._OPEN_AI_MODEL
+00002bb0: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
+00002bc0: 0d0a 5f4f 5045 4e5f 4149 5f41 5049 3d22  .._OPEN_AI_API="
+00002bd0: 736b 2d78 7878 7878 7822 0d0a 0d0a 7472  sk-xxxxxx"....tr
+00002be0: 793a 0d0a 2020 2020 7072 696e 7428 312f  y:..    print(1/
+00002bf0: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
+00002c00: 7354 656c 6567 7261 6d28 292e 5f5f 6361  sTelegram().__ca
+00002c10: 6c6c 5f5f 2829 2023 312e 2073 7563 6365  ll__() #1. succe
+00002c20: 7373 2073 656e 6465 7220 2020 2020 2020  ss sender       
+00002c30: 2020 200d 0a0d 0a65 7863 6570 7420 4578     ....except Ex
+00002c40: 6365 7074 5465 6c65 6772 616d 2061 7320  ceptTelegram as 
+00002c50: 653a 2020 2020 2020 2332 2e20 6578 6365  e:      #2. exce
+00002c60: 7074 2073 656e 6465 7220 2020 2020 2020  pt sender       
+00002c70: 2020 2020 200d 0a20 2020 2073 7973 2e65       ..    sys.e
+00002c80: 7869 7428 290d 0a0d 0a53 656e 6454 656c  xit()....SendTel
+00002c90: 6567 7261 6d28 292e 5f5f 6361 6c6c 5f5f  egram().__call__
+00002ca0: 2829 2020 2020 2020 2020 2333 2e20 6375  ()        #3. cu
+00002cb0: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
+00002cc0: 2020 2020 0d0a 0d0a 6060 600d 0a3c 6272      ....```..<br
+00002cd0: 3e0d 0a0d 0a23 2320 322d 322e 202a 4d61  >....## 2-2. *Ma
+00002ce0: 696c 204e 6f74 6966 6965 722a 0d0a 496e  il Notifier*..In
+00002cf0: 2074 6865 2065 7863 6570 7420 7374 6174   the except stat
+00002d00: 656d 656e 742c 2061 6e20 656d 6169 6c20  ement, an email 
+00002d10: 6973 2073 656e 7420 616c 6f6e 6720 7769  is sent along wi
+00002d20: 7468 2074 6865 2065 7272 6f72 206d 6573  th the error mes
+00002d30: 7361 6765 2e20 4164 6469 7469 6f6e 616c  sage. Additional
+00002d40: 6c79 2c20 796f 7520 6361 6e20 7365 6e64  ly, you can send
+00002d50: 2065 6d61 696c 7320 6672 6f6d 2061 6e79   emails from any
+00002d60: 2064 6573 6972 6564 206c 696e 652e 203c   desired line. <
+00002d70: 6272 3e0d 0a2d 2061 2e20 4c6f 6720 696e  br>..- a. Log in
+00002d80: 2077 6974 6820 7468 6520 7365 6e64 6572   with the sender
+00002d90: 2773 2065 6d61 696c 2049 442e 203c 6272  's email ID. <br
+00002da0: 3e0d 0a2d 2062 2e20 4f62 7461 696e 2061  >..- b. Obtain a
+00002db0: 6e20 6170 7020 7061 7373 776f 7264 2066  n app password f
+00002dc0: 6f72 2073 656e 6469 6e67 2047 6f6f 676c  or sending Googl
+00002dd0: 6520 4d61 696c 2061 7420 7468 6520 666f  e Mail at the fo
+00002de0: 6c6c 6f77 696e 6720 5b6c 696e 6b5d 2868  llowing [link](h
+00002df0: 7474 7073 3a2f 2f6d 7961 6363 6f75 6e74  ttps://myaccount
+00002e00: 2e67 6f6f 676c 652e 636f 6d2f 752f 332f  .google.com/u/3/
+00002e10: 6170 7070 6173 7377 6f72 6473 3f75 746d  apppasswords?utm
+00002e20: 5f73 6f75 7263 653d 676f 6f67 6c65 2d61  _source=google-a
+00002e30: 6363 6f75 6e74 2675 746d 5f6d 6564 6975  ccount&utm_mediu
+00002e40: 6d3d 6d79 6163 636f 756e 7473 6563 7572  m=myaccountsecur
+00002e50: 6974 7926 7574 6d5f 6361 6d70 6169 676e  ity&utm_campaign
+00002e60: 3d74 7376 2d73 6574 7469 6e67 7326 7261  =tsv-settings&ra
+00002e70: 7074 3d41 456a 484c 344e 3262 4d52 574f  pt=AEjHL4N2bMRWO
+00002e80: 3436 5661 4d70 5f6a 5030 367a 514b 3134  46VaMp_jP06zQK14
+00002e90: 4257 4e50 7636 366c 326f 3539 694a 3939  BWNPv66l2o59iJ99
+00002ea0: 436b 4f38 426a 596e 6d6f 5255 6539 6474  CkO8BjYnmoRUe9dt
+00002eb0: 5363 686b 6b62 7562 485a 4d55 6865 766b  SchkkbubHZMUhevk
+00002ec0: 416e 7756 4a52 4862 3979 674f 3361 6669  AnwVJRHb9ygO3afi
+00002ed0: 7370 4e6c 7729 206f 7220 5b67 6f6f 676c  spNlw) or [googl
+00002ee0: 6520 646f 6375 6d65 6e74 5d28 6874 7470  e document](http
+00002ef0: 733a 2f2f 7375 7070 6f72 742e 676f 6f67  s://support.goog
+00002f00: 6c65 2e63 6f6d 2f61 6363 6f75 6e74 732f  le.com/accounts/
+00002f10: 616e 7377 6572 2f31 3835 3833 333f 686c  answer/185833?hl
+00002f20: 3d65 6e29 2e20 0d0a 0d0a 6060 6070 7974  =en). ....```pyt
+00002f30: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00002f40: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00002f50: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+00002f60: 7074 4d61 696c 2c20 5375 6363 6573 734d  ptMail, SuccessM
+00002f70: 6169 6c2c 2053 656e 644d 6169 6c0d 0a73  ail, SendMail..s
+00002f80: 7973 2e65 7863 6570 7468 6f6f 6b20 3d20  ys.excepthook = 
+00002f90: 4578 6365 7074 4d61 696c 2e5f 5f63 616c  ExceptMail.__cal
+00002fa0: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+00002fb0: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00002fc0: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00002fd0: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00002fe0: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00002ff0: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00003000: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00003010: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00003020: 3d22 736b 2d78 7878 7878 7822 0d0a 5f47  ="sk-xxxxxx".._G
+00003030: 414d 494c 5f52 4543 4950 4945 4e54 5f41  AMIL_RECIPIENT_A
+00003040: 4444 5220 3d20 2778 7878 7878 7878 4067  DDR = 'xxxxxxx@g
+00003050: 6d61 696c 2e63 6f6d 270d 0a5f 474d 4149  mail.com'.._GMAI
+00003060: 4c5f 5345 4e44 4552 5f41 4444 5220 3d20  L_SENDER_ADDR = 
+00003070: 2779 7979 7979 7940 676d 6169 6c2e 636f  'yyyyyy@gmail.co
+00003080: 6d27 0d0a 5f47 4d41 494c 5f41 5050 5f50  m'.._GMAIL_APP_P
+00003090: 4153 5357 4f52 445f 4f46 5f53 454e 4445  ASSWORD_OF_SENDE
+000030a0: 5220 3d20 277a 7a7a 7a7a 7a27 0d0a 0d0a  R = 'zzzzzz'....
+000030b0: 7472 793a 0d0a 2020 2020 6d61 696e 2829  try:..    main()
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 2020 2020 2320 596f 7572 2043 6f64        # Your Cod
+000030e0: 6520 4865 7265 0d0a 2020 2020 5375 6363  e Here..    Succ
+000030f0: 6573 734d 6169 6c28 292e 5f5f 6361 6c6c  essMail().__call
+00003100: 5f5f 2829 2020 2020 2320 4e6f 2045 7863  __()    # No Exc
+00003110: 6570 7469 6f6e 202d 3e20 5365 6e64 2053  eption -> Send S
+00003120: 7563 6365 7373 206d 6169 6c2e 0d0a 6578  uccess mail...ex
+00003130: 6365 7074 2045 7863 6570 744d 6169 6c3a  cept ExceptMail:
+00003140: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003150: 4578 6365 7074 696f 6e20 2d3e 2053 656e  Exception -> Sen
+00003160: 6420 4661 696c 206d 6169 6c2e 0d0a 2020  d Fail mail...  
+00003170: 2020 7061 7373 0d0a 0d0a 5365 6e64 4d61    pass....SendMa
+00003180: 696c 2829 2e5f 5f63 616c 6c5f 5f28 2920  il().__call__() 
+00003190: 2020 2020 2020 2020 2020 2320 5768 656e            # When
+000031a0: 2050 726f 6365 7373 2045 6e64 6564 202d   Process Ended -
+000031b0: 3e20 416e 7920 4c69 6e65 206d 6169 6c2e  > Any Line mail.
+000031c0: 0d0a 6060 600d 0a0d 0a3c 6465 7461 696c  ..```....<detail
+000031d0: 733e 0d0a 3c73 756d 6d61 7279 3e20 5365  s>..<summary> Se
+000031e0: 6520 4578 616d 706c 652e 2e2e 3c2f 7375  e Example...</su
+000031f0: 6d6d 6172 793e 0d0a 0d0a 6060 6070 7974  mmary>....```pyt
+00003200: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00003210: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00003220: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+00003230: 7074 4d61 696c 2c20 5375 6363 6573 734d  ptMail, SuccessM
+00003240: 6169 6c2c 2053 656e 644d 6169 6c0d 0a0d  ail, SendMail...
+00003250: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
+00003260: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
+00003270: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
+00003280: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
+00003290: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
+000032a0: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
+000032b0: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
+000032c0: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
+000032d0: 7878 7878 7822 0d0a 5f47 414d 494c 5f52  xxxxx".._GAMIL_R
+000032e0: 4543 4950 4945 4e54 5f41 4444 5220 3d20  ECIPIENT_ADDR = 
+000032f0: 2778 7878 7878 7878 4067 6d61 696c 2e63  'xxxxxxx@gmail.c
+00003300: 6f6d 270d 0a5f 474d 4149 4c5f 5345 4e44  om'.._GMAIL_SEND
+00003310: 4552 5f41 4444 5220 3d20 2779 7979 7979  ER_ADDR = 'yyyyy
+00003320: 7940 676d 6169 6c2e 636f 6d27 0d0a 5f47  y@gmail.com'.._G
+00003330: 4d41 494c 5f41 5050 5f50 4153 5357 4f52  MAIL_APP_PASSWOR
+00003340: 445f 4f46 5f53 454e 4445 5220 3d20 277a  D_OF_SENDER = 'z
+00003350: 7a7a 7a7a 7a27 0d0a 0d0a 7379 732e 6578  zzzzz'....sys.ex
+00003360: 6365 7074 686f 6f6b 203d 2045 7863 6570  cepthook = Excep
+00003370: 744d 6169 6c2e 5f5f 6361 6c6c 5f5f 0d0a  tMail.__call__..
+00003380: 0d0a 7472 793a 0d0a 2020 2020 2320 3032  ..try:..    # 02
+00003390: 2e4c 6f63 6174 6520 796f 7572 2063 6f64  .Locate your cod
+000033a0: 650d 0a20 2020 2070 7269 6e74 2831 2f30  e..    print(1/0
+000033b0: 2920 2020 0d0a 2020 2020 5375 6363 6573  )   ..    Succes
+000033c0: 734d 6169 6c28 292e 5f5f 6361 6c6c 5f5f  sMail().__call__
+000033d0: 2829 2020 2023 2053 7563 6365 7373 204d  ()   # Success M
+000033e0: 6169 6c0d 0a0d 0a65 7863 6570 7420 4578  ail....except Ex
+000033f0: 6365 7074 4d61 696c 2061 7320 653a 2020  ceptMail as e:  
+00003400: 2020 2020 2020 2320 4578 6365 7074 696f        # Exceptio
+00003410: 6e20 4d61 696c 2020 2020 2020 200d 0a20  n Mail       .. 
+00003420: 2020 2073 7973 2e65 7869 7428 290d 0a20     sys.exit().. 
+00003430: 2020 2070 7269 6e74 2865 290d 0a0d 0a53     print(e)....S
+00003440: 656e 644d 6169 6c28 292e 5f5f 6361 6c6c  endMail().__call
+00003450: 5f5f 2829 2020 2020 2020 2020 2020 2320  __()          # 
+00003460: 5075 7420 416e 7920 4c69 6e65 3a20 5365  Put Any Line: Se
+00003470: 6e64 696e 6720 6d61 696c 0d0a 6060 600d  nding mail..```.
+00003480: 0a3c 2f64 6574 6169 6c73 3e0d 0a0d 0a3c  .</details>....<
+00003490: 6465 7461 696c 733e 0d0a 3c73 756d 6d61  details>..<summa
+000034a0: 7279 3e20 536e 6970 7065 7420 666f 7220  ry> Snippet for 
+000034b0: 5079 7468 6f6e 2064 6576 656c 6f70 6572  Python developer
+000034c0: 732e 2e2e 3c2f 7375 6d6d 6172 793e 0d0a  s...</summary>..
+000034d0: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
+000034e0: 6f72 7420 7379 730d 0a66 726f 6d20 4578  ort sys..from Ex
+000034f0: 6365 7074 4e6f 7469 6669 6572 2069 6d70  ceptNotifier imp
+00003500: 6f72 7420 4578 6365 7074 4d61 696c 2c20  ort ExceptMail, 
+00003510: 5375 6363 6573 734d 6169 6c2c 2053 656e  SuccessMail, Sen
+00003520: 644d 6169 6c0d 0a73 7973 2e65 7863 6570  dMail..sys.excep
+00003530: 7468 6f6f 6b20 3d20 4578 6365 7074 4d61  thook = ExceptMa
+00003540: 696c 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  il.__call__....#
+00003550: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00003560: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00003570: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00003580: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00003590: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+000035a0: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+000035b0: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+000035c0: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+000035d0: 7878 7822 0d0a 5f47 414d 494c 5f52 4543  xxx".._GAMIL_REC
+000035e0: 4950 4945 4e54 5f41 4444 5220 3d20 2778  IPIENT_ADDR = 'x
+000035f0: 7878 7878 7878 4067 6d61 696c 2e63 6f6d  xxxxxx@gmail.com
+00003600: 270d 0a5f 474d 4149 4c5f 5345 4e44 4552  '.._GMAIL_SENDER
+00003610: 5f41 4444 5220 3d20 2779 7979 7979 7940  _ADDR = 'yyyyyy@
+00003620: 676d 6169 6c2e 636f 6d27 0d0a 5f47 4d41  gmail.com'.._GMA
+00003630: 494c 5f41 5050 5f50 4153 5357 4f52 445f  IL_APP_PASSWORD_
+00003640: 4f46 5f53 454e 4445 5220 3d20 277a 7a7a  OF_SENDER = 'zzz
+00003650: 7a7a 7a27 0d0a 0d0a 7472 793a 0d0a 2020  zzz'....try:..  
+00003660: 2020 2779 6f75 7220 636f 6465 270d 0a20    'your code'.. 
+00003670: 2020 2053 7563 6365 7373 4d61 696c 2829     SuccessMail()
+00003680: 2e5f 5f63 616c 6c5f 5f28 290d 0a65 7863  .__call__()..exc
+00003690: 6570 7420 4578 6365 7074 4d61 696c 3a0d  ept ExceptMail:.
+000036a0: 0a20 2020 2070 6173 730d 0a0d 0a53 656e  .    pass....Sen
+000036b0: 644d 6169 6c28 292e 5f5f 6361 6c6c 5f5f  dMail().__call__
+000036c0: 2829 200d 0a60 6060 0d0a 3c2f 6465 7461  () ..```..</deta
+000036d0: 696c 733e 0d0a 0d0a 3c62 723e 0d0a 0d0a  ils>....<br>....
+000036e0: 2323 2032 2d33 2e20 2a44 6973 636f 7264  ## 2-3. *Discord
+000036f0: 204e 6f74 6966 6965 722a 0d0a 2d20 612e   Notifier*..- a.
+00003700: 2053 656c 6563 7420 7468 6520 6368 616e   Select the chan
+00003710: 6e65 6c20 746f 2072 6563 6569 7665 206e  nel to receive n
+00003720: 6f74 6966 6963 6174 696f 6e73 2e0d 0a2d  otifications...-
+00003730: 2062 2e20 436c 6963 6b20 2245 6469 7420   b. Click "Edit 
+00003740: 4368 616e 6e65 6c22 2069 6e20 7468 6520  Channel" in the 
+00003750: 7570 7065 7220 7269 6768 7420 636f 726e  upper right corn
+00003760: 6572 206f 6620 7468 6520 6368 6174 2077  er of the chat w
+00003770: 696e 646f 772e 0d0a 2d20 632e 2043 6c69  indow...- c. Cli
+00003780: 636b 2049 6e74 6567 7261 7469 6f6e 7320  ck Integrations 
+00003790: 2d20 5765 6268 6f6f 6b20 2d20 4e65 7720  - Webhook - New 
+000037a0: 5765 6268 6f6f 6b2e 0d0a 2d20 642e 2054  Webhook...- d. T
+000037b0: 6865 6e20 636c 6963 6b20 436f 7079 2057  hen click Copy W
+000037c0: 6562 686f 6f6b 2e0d 0a0d 0a60 6060 7079  ebhook.....```py
+000037d0: 7468 6f6e 0d0a 696d 706f 7274 2073 7973  thon..import sys
+000037e0: 0d0a 6672 6f6d 2045 7863 6570 744e 6f74  ..from ExceptNot
+000037f0: 6966 6965 7220 696d 706f 7274 2045 7863  ifier import Exc
+00003800: 6570 7444 6973 636f 7264 2c20 5375 6363  eptDiscord, Succ
+00003810: 6573 7344 6973 636f 7264 2c20 5365 6e64  essDiscord, Send
+00003820: 4469 7363 6f72 640d 0a73 7973 2e65 7863  Discord..sys.exc
+00003830: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
+00003840: 4469 7363 6f72 642e 5f5f 6361 6c6c 5f5f  Discord.__call__
+00003850: 0d0a 0d0a 2320 4465 6669 6e65 2074 6865  ....# Define the
+00003860: 206e 6578 7420 7477 6f20 7661 7269 6162   next two variab
+00003870: 6c65 7320 6f70 7469 6f6e 616c 6c79 2077  les optionally w
+00003880: 6865 6e20 7573 696e 6720 4f70 656e 4149  hen using OpenAI
+00003890: 2773 2041 5049 2e0d 0a23 205f 4f50 454e  's API...# _OPEN
+000038a0: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
+000038b0: 2e35 2d74 7572 626f 2220 2020 200d 0a23  .5-turbo"    ..#
+000038c0: 205f 4f50 454e 5f41 495f 4150 493d 2273   _OPEN_AI_API="s
+000038d0: 6b2d 7878 7878 7878 220d 0a5f 4449 5343  k-xxxxxx".._DISC
+000038e0: 4f52 445f 5745 4248 4f4f 4b5f 5552 4c20  ORD_WEBHOOK_URL 
+000038f0: 3d20 2278 7878 7878 7878 7878 7878 7878  = "xxxxxxxxxxxxx
+00003900: 7878 7878 220d 0a0d 0a0d 0a74 7279 3a0d  xxxx"......try:.
+00003910: 0a20 2020 2070 7269 6e74 2831 2f32 3029  .    print(1/20)
+00003920: 2020 0d0a 2020 2020 5375 6363 6573 7344    ..    SuccessD
+00003930: 6973 636f 7264 2829 2e5f 5f63 616c 6c5f  iscord().__call_
+00003940: 5f28 2920 2331 2073 7563 6365 7373 2073  _() #1 success s
+00003950: 656e 6465 7220 2020 2020 2020 2020 200d  ender          .
+00003960: 0a65 7863 6570 7420 4578 6365 7074 4469  .except ExceptDi
+00003970: 7363 6f72 6420 6173 2065 3a20 2020 2020  scord as e:     
+00003980: 2023 3220 6578 6365 7074 2073 656e 6465   #2 except sende
+00003990: 7220 2020 2020 2020 2020 2020 200d 0a20  r            .. 
+000039a0: 2020 2073 7973 2e65 7869 7428 290d 0a0d     sys.exit()...
+000039b0: 0a53 656e 6444 6973 636f 7264 2829 2e5f  .SendDiscord()._
+000039c0: 5f63 616c 6c5f 5f28 2920 2020 2020 2020  _call__()       
+000039d0: 2023 3320 6375 7374 6f6d 697a 6564 2073   #3 customized s
+000039e0: 656e 6465 7220 2020 2020 2020 0d0a 6060  ender       ..``
+000039f0: 600d 0a0d 0a3c 6272 3e0d 0a0d 0a23 2320  `....<br>....## 
+00003a00: 322d 342e 202a 4368 696d 6520 4e6f 7469  2-4. *Chime Noti
+00003a10: 6669 6572 2a0d 0a2d 2061 2e20 5365 6c65  fier*..- a. Sele
+00003a20: 6374 2074 6865 2043 6861 7420 726f 6f6d  ct the Chat room
+00003a30: 2074 6f20 7265 6365 6976 6520 6e6f 7469   to receive noti
+00003a40: 6669 6361 7469 6f6e 732e 0d0a 2d20 622e  fications...- b.
+00003a50: 2043 6c69 636b 2022 526f 6f6d 2053 6574   Click "Room Set
+00003a60: 7469 6e67 2220 696e 2074 6865 2075 7070  ting" in the upp
+00003a70: 6572 2072 6967 6874 2063 6f72 6e65 722e  er right corner.
+00003a80: 0d0a 2d20 632e 2043 6c69 636b 2022 4d61  ..- c. Click "Ma
+00003a90: 6e61 6765 2057 6562 686f 6f6b 2061 6e64  nage Webhook and
+00003aa0: 2062 6f74 2e22 0d0a 2d20 642e 2043 7265   bot."..- d. Cre
+00003ab0: 6174 6520 4164 6420 5765 6268 6f6f 6b2c  ate Add Webhook,
+00003ac0: 2073 6574 2069 7420 7570 2c20 7468 656e   set it up, then
+00003ad0: 2063 6c69 636b 2043 6f70 7920 5765 6268   click Copy Webh
+00003ae0: 6f6f 6b2e 0d0a 6060 6070 7974 686f 6e0d  ook...```python.
+00003af0: 0a69 6d70 6f72 7420 7379 730d 0a66 726f  .import sys..fro
+00003b00: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
+00003b10: 2069 6d70 6f72 7420 5375 6363 6573 7343   import SuccessC
+00003b20: 6869 6d65 2c20 4578 6365 7074 4368 696d  hime, ExceptChim
+00003b30: 652c 2053 656e 6443 6869 6d65 0d0a 7379  e, SendChime..sy
+00003b40: 732e 6578 6365 7074 686f 6f6b 203d 2045  s.excepthook = E
+00003b50: 7863 6570 7443 6869 6d65 2e5f 5f63 616c  xceptChime.__cal
+00003b60: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+00003b70: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00003b80: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00003b90: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00003ba0: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00003bb0: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00003bc0: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00003bd0: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00003be0: 3d22 736b 2d78 7878 7878 7822 0d0a 5f43  ="sk-xxxxxx".._C
+00003bf0: 4849 4d45 5f57 4542 484f 4f4b 5f55 524c  HIME_WEBHOOK_URL
+00003c00: 203d 2022 7878 7878 7878 7878 7878 7878   = "xxxxxxxxxxxx
+00003c10: 7878 7878 7878 220d 0a0d 0a0d 0a74 7279  xxxxxx"......try
+00003c20: 3a0d 0a20 2020 2070 7269 6e74 2831 2f30  :..    print(1/0
+00003c30: 2920 200d 0a20 2020 2053 7563 6365 7373  )  ..    Success
+00003c40: 4368 696d 6528 292e 5f5f 6361 6c6c 5f5f  Chime().__call__
+00003c50: 2829 2023 3120 7375 6363 6573 7320 7365  () #1 success se
+00003c60: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
+00003c70: 6578 6365 7074 2045 7863 6570 7443 6869  except ExceptChi
+00003c80: 6d65 2061 7320 653a 2020 2020 2020 2332  me as e:      #2
+00003c90: 2065 7863 6570 7420 7365 6e64 6572 2020   except sender  
+00003ca0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+00003cb0: 7379 732e 6578 6974 2829 0d0a 0d0a 5365  sys.exit()....Se
+00003cc0: 6e64 4368 696d 6528 292e 5f5f 6361 6c6c  ndChime().__call
+00003cd0: 5f5f 2829 2020 2020 2020 2020 2333 2063  __()        #3 c
+00003ce0: 7573 746f 6d69 7a65 6420 7365 6e64 6572  ustomized sender
+00003cf0: 2020 2020 2020 200d 0a60 6060 0d0a 3c62         ..```..<b
+00003d00: 723e 0d0a 0d0a 2323 2032 2d35 2e20 2a53  r>....## 2-5. *S
+00003d10: 6c61 636b 204e 6f74 6966 6965 722a 0d0a  lack Notifier*..
+00003d20: 2d20 612e 2076 6973 6974 2068 7474 7073  - a. visit https
+00003d30: 3a2f 2f61 7069 2e73 6c61 636b 2e63 6f6d  ://api.slack.com
+00003d40: 2f0d 0a2d 2062 2e20 6043 7265 6174 6520  /..- b. `Create 
+00003d50: 616e 2061 7070 6020 2d20 6046 726f 6d20  an app` - `From 
+00003d60: 7363 7261 7463 6860 202d 2060 4372 6561  scratch` - `Crea
+00003d70: 7465 2041 7070 600d 0a2d 2063 2e20 4164  te App`..- c. Ad
+00003d80: 6420 7765 6268 6f6f 6b3a 2043 6c69 636b  d webhook: Click
+00003d90: 2060 496e 636f 6d69 6e67 2057 6562 686f   `Incoming Webho
+00003da0: 6f6b 7360 202d 2041 6374 6976 6174 6520  oks` - Activate 
+00003db0: 496e 636f 6d6d 696e 6720 604f 6e60 202d  Incomming `On` -
+00003dc0: 2041 6464 204e 6577 2057 6562 686f 6f6b   Add New Webhook
+00003dd0: 2074 6f20 576f 726b 7370 6163 650d 0a2d   to Workspace..-
+00003de0: 2064 2e20 436f 7079 2060 5765 6268 6f6f   d. Copy `Webhoo
+00003df0: 6b20 5552 4c60 0d0a 0d0a 6060 6070 7974  k URL`....```pyt
+00003e00: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00003e10: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00003e20: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+00003e30: 7074 536c 6163 6b2c 2053 7563 6365 7373  ptSlack, Success
+00003e40: 536c 6361 6b2c 2053 656e 6453 6c61 636b  Slcak, SendSlack
+00003e50: 0d0a 7379 732e 6578 6365 7074 686f 6f6b  ..sys.excepthook
+00003e60: 203d 2045 7863 6570 7453 6c61 636b 2e5f   = ExceptSlack._
+00003e70: 5f63 616c 6c5f 5f0d 0a0d 0a23 2044 6566  _call__....# Def
+00003e80: 696e 6520 7468 6520 6e65 7874 2074 776f  ine the next two
+00003e90: 2076 6172 6961 626c 6573 206f 7074 696f   variables optio
+00003ea0: 6e61 6c6c 7920 7768 656e 2075 7369 6e67  nally when using
+00003eb0: 204f 7065 6e41 4927 7320 4150 492e 0d0a   OpenAI's API...
+00003ec0: 2320 5f4f 5045 4e5f 4149 5f4d 4f44 454c  # _OPEN_AI_MODEL
+00003ed0: 3d22 6770 742d 332e 352d 7475 7262 6f22  ="gpt-3.5-turbo"
+00003ee0: 2020 2020 0d0a 2320 5f4f 5045 4e5f 4149      ..# _OPEN_AI
+00003ef0: 5f41 5049 3d22 736b 2d78 7878 7878 7822  _API="sk-xxxxxx"
+00003f00: 0d0a 5f53 4c41 434b 5f57 4542 484f 4f4b  .._SLACK_WEBHOOK
+00003f10: 5f55 524c 203d 2027 6874 7470 733a 2f2f  _URL = 'https://
+00003f20: 686f 6f6b 732e 736c 6163 6b2e 636f 6d2f  hooks.slack.com/
+00003f30: 7365 7276 6963 6573 2f78 7878 7878 7878  services/xxxxxxx
+00003f40: 7878 7878 7878 7878 7878 7878 270d 0a0d  xxxxxxxxxxxx'...
+00003f50: 0a74 7279 3a0d 0a20 2020 2070 7269 6e74  .try:..    print
+00003f60: 2831 2f30 2920 200d 0a20 2020 2053 7563  (1/0)  ..    Suc
+00003f70: 6365 7373 536c 6361 6b28 292e 5f5f 6361  cessSlcak().__ca
+00003f80: 6c6c 5f5f 2829 2023 3120 7375 6363 6573  ll__() #1 succes
+00003f90: 7320 7365 6e64 6572 2020 2020 2020 2020  s sender        
+00003fa0: 2020 0d0a 6578 6365 7074 2045 7863 6570    ..except Excep
+00003fb0: 7453 6c61 636b 2061 7320 653a 2020 2020  tSlack as e:    
+00003fc0: 2020 2332 2065 7863 6570 7420 7365 6e64    #2 except send
+00003fd0: 6572 2020 2020 2020 2020 2020 2020 0d0a  er            ..
+00003fe0: 2020 2020 7379 732e 6578 6974 2829 0d0a      sys.exit()..
+00003ff0: 0d0a 5365 6e64 536c 6163 6b28 292e 5f5f  ..SendSlack().__
+00004000: 6361 6c6c 5f5f 2829 2020 2020 2020 2020  call__()        
+00004010: 2333 2063 7573 746f 6d69 7a65 6420 7365  #3 customized se
+00004020: 6e64 6572 2020 2020 200d 0a60 6060 0d0a  nder     ..```..
+00004030: 3c42 723e 0d0a 0d0a 2323 2032 2d36 2e20  <Br>....## 2-6. 
+00004040: 2a4c 696e 6520 4e6f 7469 6669 6572 2a0d  *Line Notifier*.
+00004050: 0a2d 2061 2e20 5265 6769 7374 6572 205b  .- a. Register [
+00004060: 6874 7470 733a 2f2f 6e6f 7469 6679 2d62  https://notify-b
+00004070: 6f74 2e6c 696e 652e 6d65 2f5d 2868 7474  ot.line.me/](htt
+00004080: 7073 3a2f 2f6e 6f74 6966 792d 626f 742e  ps://notify-bot.
+00004090: 6c69 6e65 2e6d 652f 290d 0a2d 2062 2e20  line.me/)..- b. 
+000040a0: 476f 2074 6f20 6d79 7061 6765 205b 6874  Go to mypage [ht
+000040b0: 7470 733a 2f2f 6e6f 7469 6679 2d62 6f74  tps://notify-bot
+000040c0: 2e6c 696e 652e 6d65 2f6d 792f 5d28 6874  .line.me/my/](ht
+000040d0: 7470 733a 2f2f 6e6f 7469 6679 2d62 6f74  tps://notify-bot
+000040e0: 2e6c 696e 652e 6d65 2f6d 792f 290d 0a2d  .line.me/my/)..-
+000040f0: 2063 2e20 436c 6963 6b20 6047 656e 6572   c. Click `Gener
+00004100: 6174 6520 546f 6b65 6e60 2c20 656e 7465  ate Token`, ente
+00004110: 7220 5365 7276 6963 6520 4e61 6d65 2061  r Service Name a
+00004120: 6e64 2063 6c69 636b 2060 312d 6f6e 2d31  nd click `1-on-1
+00004130: 2063 6861 7420 7769 7468 204c 494e 4560   chat with LINE`
+00004140: 2028 616e 7974 6869 6e67 2079 6f75 206c   (anything you l
+00004150: 696b 6529 0d0a 2d20 642e 2043 6f70 7920  ike)..- d. Copy 
+00004160: 546f 6b65 6e2e 0d0a 0d0a 6060 6070 7974  Token.....```pyt
+00004170: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+00004180: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+00004190: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+000041a0: 7074 4c69 6e65 2c20 5375 6363 6573 734c  ptLine, SuccessL
+000041b0: 696e 652c 2053 656e 644c 696e 650d 0a73  ine, SendLine..s
+000041c0: 7973 2e65 7863 6570 7468 6f6f 6b20 3d20  ys.excepthook = 
+000041d0: 4578 6365 7074 4c69 6e65 2e5f 5f63 616c  ExceptLine.__cal
+000041e0: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+000041f0: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00004200: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00004210: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00004220: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00004230: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00004240: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00004250: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00004260: 3d22 736b 2d78 7878 7878 7822 0d0a 5f4c  ="sk-xxxxxx".._L
+00004270: 494e 455f 4e4f 5449 4659 5f41 5049 5f54  INE_NOTIFY_API_T
+00004280: 4f4b 454e 203d 2027 7878 7878 7878 7878  OKEN = 'xxxxxxxx
+00004290: 7878 7827 0d0a 0d0a 7472 793a 0d0a 2020  xxx'....try:..  
+000042a0: 2020 7072 696e 7428 312f 3230 2920 200d    print(1/20)  .
+000042b0: 0a20 2020 2053 7563 6365 7373 4c69 6e65  .    SuccessLine
+000042c0: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2331  ().__call__() #1
+000042d0: 2073 7563 6365 7373 2073 656e 6465 7220   success sender 
+000042e0: 2020 2020 2020 2020 200d 0a65 7863 6570           ..excep
+000042f0: 7420 4578 6365 7074 4c69 6e65 2061 7320  t ExceptLine as 
+00004300: 653a 2020 2020 2020 2332 2065 7863 6570  e:      #2 excep
+00004310: 7420 7365 6e64 6572 2020 2020 2020 2020  t sender        
+00004320: 2020 2020 0d0a 2020 2020 7379 732e 6578      ..    sys.ex
+00004330: 6974 2829 0d0a 0d0a 5365 6e64 4c69 6e65  it()....SendLine
+00004340: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00004350: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
+00004360: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
+00004370: 2020 200d 0a60 6060 0d0a 0d0a 3c42 723e     ..```....<Br>
+00004380: 0d0a 0d0a 2323 2032 2d37 2e20 2a53 4d53  ....## 2-7. *SMS
+00004390: 204e 6f74 6966 6965 722a 0d0a 2d20 612e   Notifier*..- a.
+000043a0: 2053 6967 6e20 7570 2066 6f72 2054 7769   Sign up for Twi
+000043b0: 6c69 6f2e 205b 6874 7470 733a 2f2f 7777  lio. [https://ww
+000043c0: 772e 7477 696c 696f 2e63 6f6d 2f65 6e2d  w.twilio.com/en-
+000043d0: 7573 5d28 6874 7470 733a 2f2f 7777 772e  us](https://www.
+000043e0: 7477 696c 696f 2e63 6f6d 2f65 6e2d 7573  twilio.com/en-us
+000043f0: 290d 0a2d 2062 2e20 436c 6963 6b20 436f  )..- b. Click Co
+00004400: 6e73 6f6c 6520 696e 2074 6865 2075 7070  nsole in the upp
+00004410: 6572 2072 6967 6874 2063 6f72 6e65 722e  er right corner.
+00004420: 0d0a 2d20 632e 2043 6f70 7920 7468 6520  ..- c. Copy the 
+00004430: 7661 7269 6162 6c65 7320 7072 6f76 6964  variables provid
+00004440: 6564 2069 6e20 7468 6520 636f 6e73 6f6c  ed in the consol
+00004450: 652e 0d0a 0d0a 6060 6070 7974 686f 6e0d  e.....```python.
+00004460: 0a69 6d70 6f72 7420 7379 730d 0a66 726f  .import sys..fro
+00004470: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
+00004480: 2069 6d70 6f72 7420 4578 6365 7074 534d   import ExceptSM
+00004490: 532c 2053 7563 6365 7373 534d 532c 2053  S, SuccessSMS, S
+000044a0: 656e 6453 4d53 0d0a 7379 732e 6578 6365  endSMS..sys.exce
+000044b0: 7074 686f 6f6b 203d 2045 7863 6570 7453  pthook = ExceptS
+000044c0: 4d53 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  MS.__call__....#
+000044d0: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+000044e0: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+000044f0: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00004500: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00004510: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+00004520: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+00004530: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+00004540: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+00004550: 7878 7822 0d0a 5f54 5749 4c49 4f5f 5349  xxx".._TWILIO_SI
+00004560: 4420 3d20 2778 7878 7827 0d0a 5f54 5749  D = 'xxxx'.._TWI
+00004570: 4c49 4f5f 544f 4b45 4e20 3d20 2779 7979  LIO_TOKEN = 'yyy
+00004580: 7979 7927 0d0a 5f52 4543 4950 4945 4e54  yyy'.._RECIPIENT
+00004590: 5f50 484f 4e45 5f4e 554d 4245 523d 222b  _PHONE_NUMBER="+
+000045a0: 6161 6161 6161 222c 0d0a 5f53 454e 4445  aaaaaa",.._SENDE
+000045b0: 525f 5048 4f4e 455f 4e55 4d42 4552 3d22  R_PHONE_NUMBER="
+000045c0: 2b62 6262 6262 6222 2c20 200d 0a0d 0a74  +bbbbbb",  ....t
+000045d0: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
+000045e0: 2f31 3029 2020 0d0a 2020 2020 5375 6363  /10)  ..    Succ
+000045f0: 6573 7353 4d53 2829 2e5f 5f63 616c 6c5f  essSMS().__call_
+00004600: 5f28 2920 2331 2073 7563 6365 7373 2073  _() #1 success s
+00004610: 656e 6465 7220 2020 2020 2020 2020 200d  ender          .
+00004620: 0a65 7863 6570 7420 4578 6365 7074 534d  .except ExceptSM
+00004630: 5320 6173 2065 3a20 2020 2020 2023 3220  S as e:      #2 
+00004640: 6578 6365 7074 2073 656e 6465 720d 0a20  except sender.. 
+00004650: 2020 2073 7973 2e65 7869 7428 290d 0a0d     sys.exit()...
+00004660: 0a53 656e 6453 4d53 2829 2e5f 5f63 616c  .SendSMS().__cal
+00004670: 6c5f 5f28 2920 2020 2020 2020 2023 3320  l__()        #3 
+00004680: 6375 7374 6f6d 697a 6564 2073 656e 6465  customized sende
+00004690: 7220 2020 2020 2020 200d 0a60 6060 0d0a  r        ..```..
+000046a0: 3c42 723e 0d0a 0d0a 2323 2032 2d38 2e20  <Br>....## 2-8. 
+000046b0: 2a54 6561 6d73 204e 6f74 6966 6965 722a  *Teams Notifier*
+000046c0: 0d0a 2d20 612e 2043 7265 6174 6520 7468  ..- a. Create th
+000046d0: 6520 6368 616e 6e65 6c20 7468 6174 2079  e channel that y
+000046e0: 6f75 2077 616e 7420 746f 206e 6f74 6966  ou want to notif
+000046f0: 792e 0d0a 2d20 622e 2041 7070 202d 2053  y...- b. App - S
+00004700: 6561 7263 683a 2077 6562 686f 6f6b 202d  earch: webhook -
+00004710: 2049 6e63 6f6d 696e 6720 5765 6268 6f6f   Incoming Webhoo
+00004720: 6b20 5b68 7474 7073 3a2f 2f74 6561 6d73  k [https://teams
+00004730: 2e6d 6963 726f 736f 6674 2e63 6f6d 2f6c  .microsoft.com/l
+00004740: 2f61 7070 2f32 3033 6131 6532 632d 3236  /app/203a1e2c-26
+00004750: 6363 2d34 3763 612d 3833 6165 2d62 6539  cc-47ca-83ae-be9
+00004760: 3866 3936 3062 3662 323f 736f 7572 6365  8f960b6b2?source
+00004770: 3d61 7070 2d64 6574 6169 6c73 2d64 6961  =app-details-dia
+00004780: 6c6f 675d 2868 7474 7073 3a2f 2f74 6561  log](https://tea
+00004790: 6d73 2e6d 6963 726f 736f 6674 2e63 6f6d  ms.microsoft.com
+000047a0: 2f6c 2f61 7070 2f32 3033 6131 6532 632d  /l/app/203a1e2c-
+000047b0: 3236 6363 2d34 3763 612d 3833 6165 2d62  26cc-47ca-83ae-b
+000047c0: 6539 3866 3936 3062 3662 323f 736f 7572  e98f960b6b2?sour
+000047d0: 6365 3d61 7070 2d64 6574 6169 6c73 2d64  ce=app-details-d
+000047e0: 6961 6c6f 6729 0d0a 2d20 632e 2043 6c69  ialog)..- c. Cli
+000047f0: 636b 2060 5265 7175 6573 7420 4170 7072  ck `Request Appr
+00004800: 6f76 616c 6020 3c62 723e 0d0a 4166 7465  oval` <br>..Afte
+00004810: 7220 796f 7520 6361 6e20 7573 6520 7765  r you can use we
+00004820: 6268 6f6f 6b20 696e 636f 6d6d 696e 672e  bhook incomming.
+00004830: 2050 726f 6365 6564 2074 6f20 6e65 7874   Proceed to next
+00004840: 2073 7465 7073 2e0d 0a4d 6963 726f 736f   steps...Microso
+00004850: 6674 2054 6561 6d73 2061 6c6c 6f77 7320  ft Teams allows 
+00004860: 6c69 6d69 7465 6420 6170 706c 6963 6174  limited applicat
+00004870: 696f 6e20 6163 6365 7373 2070 6572 206f  ion access per o
+00004880: 7267 616e 697a 6174 696f 6e2c 2073 6f20  rganization, so 
+00004890: 6974 2063 616e 206f 6e6c 7920 6265 2075  it can only be u
+000048a0: 7365 6420 6966 2074 6865 2077 6562 686f  sed if the webho
+000048b0: 6f6b 2069 6e63 6f6d 696e 6720 6170 706c  ok incoming appl
+000048c0: 6963 6174 696f 6e20 6973 2061 7661 696c  ication is avail
+000048d0: 6162 6c65 2e0d 0a2d 2063 2e20 476f 2074  able...- c. Go t
+000048e0: 6f20 7468 6520 7465 616d 2063 6861 6e6e  o the team chann
+000048f0: 656c 2074 6f20 7265 6365 6976 6520 6e6f  el to receive no
+00004900: 7469 6669 6361 7469 6f6e 732c 2061 6e64  tifications, and
+00004910: 2063 6c69 636b 2060 436f 6e6e 6563 746f   click `Connecto
+00004920: 7273 6020 696e 2053 6574 7469 6e67 732e  rs` in Settings.
+00004930: 0d0a 2d20 642e 2060 436f 6e6e 6563 746f  ..- d. `Connecto
+00004940: 7273 6020 4166 7465 7220 636f 6e66 6967  rs` After config
+00004950: 7572 696e 6720 7765 6268 6f6f 6b20 696e  uring webhook in
+00004960: 636f 6d69 6e67 2069 6e20 436f 6e6e 6563  coming in Connec
+00004970: 746f 722c 2063 6f70 7920 7468 6520 7765  tor, copy the we
+00004980: 6268 6f6f 6b20 5552 4c2e 0d0a 0d0a 6060  bhook URL.....``
+00004990: 6070 7974 686f 6e0d 0a69 6d70 6f72 7420  `python..import 
+000049a0: 7379 730d 0a66 726f 6d20 4578 6365 7074  sys..from Except
+000049b0: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
+000049c0: 4578 6365 7074 5465 616d 732c 2053 7563  ExceptTeams, Suc
+000049d0: 6365 7373 5465 616d 732c 2053 656e 6454  cessTeams, SendT
+000049e0: 6561 6d73 0d0a 7379 732e 6578 6365 7074  eams..sys.except
+000049f0: 686f 6f6b 203d 2045 7863 6570 7454 6561  hook = ExceptTea
+00004a00: 6d73 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  ms.__call__....#
+00004a10: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00004a20: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00004a30: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00004a40: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00004a50: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+00004a60: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+00004a70: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+00004a80: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+00004a90: 7878 7822 0d0a 5f54 4541 4d53 5f57 4542  xxx".._TEAMS_WEB
+00004aa0: 484f 4f4b 5f55 524c 203d 2027 6d69 6372  HOOK_URL = 'micr
+00004ab0: 6f73 6f66 7420 7765 6268 6f6f 6b20 5f54  osoft webhook _T
+00004ac0: 4541 4d53 5f57 4542 484f 4f4b 5f55 524c  EAMS_WEBHOOK_URL
+00004ad0: 270d 0a0d 0a74 7279 3a0d 0a20 2020 2070  '....try:..    p
+00004ae0: 7269 6e74 2831 2f32 3029 2020 0d0a 2020  rint(1/20)  ..  
+00004af0: 2020 5375 6363 6573 7354 6561 6d73 2829    SuccessTeams()
+00004b00: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2073  .__call__() #1 s
+00004b10: 7563 6365 7373 2073 656e 6465 7220 2020  uccess sender   
+00004b20: 2020 2020 2020 200d 0a65 7863 6570 7420         ..except 
+00004b30: 4578 6365 7074 5465 616d 7320 6173 2065  ExceptTeams as e
+00004b40: 3a20 2020 2020 2023 3220 6578 6365 7074  :      #2 except
+00004b50: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
+00004b60: 2020 200d 0a20 2020 2073 7973 2e65 7869     ..    sys.exi
+00004b70: 7428 290d 0a0d 0a53 656e 6454 6561 6d73  t()....SendTeams
+00004b80: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00004b90: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
+00004ba0: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
+00004bb0: 200d 0a60 6060 0d0a 0d0a 3c42 723e 0d0a   ..```....<Br>..
+00004bc0: 0d0a 2323 2032 2d39 2e20 2a4b 616b 616f  ..## 2-9. *Kakao
+00004bd0: 7461 6c6b 204e 6f74 6966 6965 722a 0d0a  talk Notifier*..
+00004be0: 2d20 612e 2053 6967 6e20 7570 2061 7420  - a. Sign up at 
+00004bf0: 7468 6520 666f 6c6c 6f77 696e 6720 7369  the following si
+00004c00: 7465 3a20 5b68 7474 7073 3a2f 2f64 6576  te: [https://dev
+00004c10: 656c 6f70 6572 732e 6b61 6b61 6f2e 636f  elopers.kakao.co
+00004c20: 6d2f 5d28 6874 7470 733a 2f2f 6465 7665  m/](https://deve
+00004c30: 6c6f 7065 7273 2e6b 616b 616f 2e63 6f6d  lopers.kakao.com
+00004c40: 2f29 0d0a 2d20 622e 2043 6c69 636b 2022  /)..- b. Click "
+00004c50: 4d79 2041 7070 6c69 6361 7469 6f6e 2220  My Application" 
+00004c60: 6f6e 2074 6865 2074 6f70 2062 6172 2e0d  on the top bar..
+00004c70: 0a2d 2063 2e20 436c 6963 6b20 2241 6464  .- c. Click "Add
+00004c80: 2061 6e20 6170 706c 6963 6174 696f 6e2c   an application,
+00004c90: 2220 7365 7420 6120 6e61 6d65 2c20 616e  " set a name, an
+00004ca0: 6420 6372 6561 7465 2069 742e 0d0a 2d20  d create it...- 
+00004cb0: 642e 2043 6c69 636b 2022 4b61 6b61 6f20  d. Click "Kakao 
+00004cc0: 4c6f 6769 6e22 2069 6e20 7468 6520 6c65  Login" in the le
+00004cd0: 6674 206d 656e 752c 2074 6865 6e20 6368  ft menu, then ch
+00004ce0: 616e 6765 2074 6865 2053 7461 7465 206f  ange the State o
+00004cf0: 6620 224b 616b 616f 204c 6f67 696e 2041  f "Kakao Login A
+00004d00: 6374 6976 6174 696f 6e22 2074 6f20 4f4e  ctivation" to ON
+00004d10: 206f 6e20 7468 6520 7265 7375 6c74 696e   on the resultin
+00004d20: 6720 7061 6765 2e0d 0a2d 2065 2e20 496e  g page...- e. In
+00004d30: 204d 7920 4170 706c 6963 6174 696f 6e20   My Application 
+00004d40: 3e20 5072 6f64 7563 7420 5365 7474 696e  > Product Settin
+00004d50: 6773 203e 204b 616b 616f 204c 6f67 696e  gs > Kakao Login
+00004d60: 2c20 6265 2073 7572 6520 746f 2073 6574  , be sure to set
+00004d70: 2052 6564 6972 6563 7420 5552 4920 6173   Redirect URI as
+00004d80: 2066 6f6c 6c6f 7773 3a20 5b68 7474 7073   follows: [https
+00004d90: 3a2f 2f65 7861 6d70 6c65 2e63 6f6d 2f6f  ://example.com/o
+00004da0: 6175 7468 5d28 6874 7470 733a 2f2f 6578  auth](https://ex
+00004db0: 616d 706c 652e 636f 6d2f 6f61 7574 6829  ample.com/oauth)
+00004dc0: 0d0a 2d20 662e 2049 6e20 7468 6520 6c65  ..- f. In the le
+00004dd0: 6674 2043 6f6e 7365 6e74 2049 7465 6d73  ft Consent Items
+00004de0: 206d 656e 752c 2073 6574 2022 5365 6e64   menu, set "Send
+00004df0: 206d 6573 7361 6765 2069 6e20 4b61 6b61   message in Kaka
+00004e00: 6f54 616c 6b22 2074 6f20 7365 6c65 6374  oTalk" to select
+00004e10: 6976 6520 6167 7265 656d 656e 742e 0d0a  ive agreement...
+00004e20: 2d20 672e 2043 6f70 7920 7468 6520 5245  - g. Copy the RE
+00004e30: 5354 2041 5049 204b 6579 2069 6e20 4d79  ST API Key in My
+00004e40: 2041 7070 6c69 6361 7469 6f6e 203e 2041   Application > A
+00004e50: 7070 2053 6574 7469 6e67 7320 3e20 5375  pp Settings > Su
+00004e60: 6d6d 6172 792c 2061 6e64 2067 6f20 746f  mmary, and go to
+00004e70: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
+00004e80: 6f63 756d 656e 742e 0d0a 2d20 682e 2049  ocument...- h. I
+00004e90: 6620 796f 7520 6861 7665 2073 7563 6365  f you have succe
+00004ea0: 7373 6675 6c6c 7920 636f 6d70 6c65 7465  ssfully complete
+00004eb0: 6420 616c 6c20 6f66 2074 6865 2061 626f  d all of the abo
+00004ec0: 7665 2073 7465 7073 2c20 676f 2074 6f20  ve steps, go to 
+00004ed0: 7468 6520 666f 6c6c 6f77 696e 6720 646f  the following do
+00004ee0: 6375 6d65 6e74 2061 6e64 2066 6f6c 6c6f  cument and follo
+00004ef0: 7720 7468 6520 696e 7374 7275 6374 696f  w the instructio
+00004f00: 6e73 3a0d 0a20 6874 7470 733a 2f2f 6769  ns:.. https://gi
+00004f10: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
+00004f20: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
+00004f30: 6669 6572 2f62 6c6f 622f 6d61 696e 2f74  fier/blob/main/t
+00004f40: 7574 6f72 6961 6c73 2f6b 616b 616f 5f74  utorials/kakao_t
+00004f50: 6f6b 656e 5f67 656e 6572 6174 6f72 2e69  oken_generator.i
+00004f60: 7079 6e62 0d0a 202a 2a49 6e20 7468 6973  pynb.. **In this
+00004f70: 2065 7861 6d70 6c65 2c20 736f 6d65 2041   example, some A
+00004f80: 5049 206b 6579 7320 7765 7265 2065 7870  PI keys were exp
+00004f90: 6f73 6564 2062 7920 6372 6561 7469 6e67  osed by creating
+00004fa0: 2061 6e64 2072 656d 6f76 696e 6720 6120   and removing a 
+00004fb0: 7465 7374 2061 7070 6c69 6361 7469 6f6e  test application
+00004fc0: 2c20 6275 7420 666f 7220 7365 6375 7269  , but for securi
+00004fd0: 7479 2072 6561 736f 6e73 2c20 796f 7572  ty reasons, your
+00004fe0: 2041 5049 206b 6579 2073 686f 756c 6420   API key should 
+00004ff0: 6e6f 7420 6265 2065 7870 6f73 6564 2074  not be exposed t
+00005000: 6f20 7468 6520 6f75 7473 6964 6520 776f  o the outside wo
+00005010: 726c 642e 2a2a 0d0a 3c42 723e 0d0a 0d0a  rld.**..<Br>....
+00005020: 6060 6070 7974 686f 6e0d 0a69 6d70 6f72  ```python..impor
+00005030: 7420 7379 730d 0a66 726f 6d20 4578 6365  t sys..from Exce
+00005040: 7074 4e6f 7469 6669 6572 2069 6d70 6f72  ptNotifier impor
+00005050: 7420 4578 6365 7074 4b61 6b61 6f2c 2053  t ExceptKakao, S
+00005060: 7563 6365 7373 4b61 6b61 6f2c 2053 656e  uccessKakao, Sen
+00005070: 644b 616b 616f 0d0a 7379 732e 6578 6365  dKakao..sys.exce
+00005080: 7074 686f 6f6b 203d 2045 7863 6570 744b  pthook = ExceptK
+00005090: 616b 616f 2e5f 5f63 616c 6c5f 5f0d 0a0d  akao.__call__...
+000050a0: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
+000050b0: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
+000050c0: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
+000050d0: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
+000050e0: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
+000050f0: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
+00005100: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
+00005110: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
+00005120: 7878 7878 7822 0d0a 5f4b 414b 414f 5f54  xxxxx".._KAKAO_T
+00005130: 4f4b 454e 5f50 4154 4820 3d20 2778 7878  OKEN_PATH = 'xxx
+00005140: 782f 7878 782f 7878 782e 6a73 6f6e 2727  x/xxx/xxx.json''
+00005150: 0d0a 0d0a 7472 793a 0d0a 2020 2020 7072  ....try:..    pr
+00005160: 696e 7428 312f 3029 2020 0d0a 2020 2020  int(1/0)  ..    
+00005170: 5375 6363 6573 734b 616b 616f 2829 2e5f  SuccessKakao()._
+00005180: 5f63 616c 6c5f 5f28 2920 2331 2073 7563  _call__() #1 suc
+00005190: 6365 7373 2073 656e 6465 7220 2020 2020  cess sender     
+000051a0: 2020 2020 200d 0a65 7863 6570 7420 4578       ..except Ex
+000051b0: 6365 7074 4b61 6b61 6f20 6173 2065 3a20  ceptKakao as e: 
+000051c0: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
+000051d0: 656e 6465 7220 2020 2020 2020 2020 2020  ender           
+000051e0: 200d 0a20 2020 2073 7973 2e65 7869 7428   ..    sys.exit(
+000051f0: 290d 0a0d 0a53 656e 644b 616b 616f 2829  )....SendKakao()
+00005200: 2e5f 5f63 616c 6c5f 5f28 2920 2020 2020  .__call__()     
+00005210: 2020 2023 3320 6375 7374 6f6d 697a 6564     #3 customized
+00005220: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
+00005230: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
+00005240: 0a23 2320 322d 3130 2e20 2a42 6565 7020  .## 2-10. *Beep 
+00005250: 4e6f 7469 6669 6572 2a0d 0a4e 6f20 7365  Notifier*..No se
+00005260: 7475 7020 6973 2072 6571 7569 7265 642e  tup is required.
+00005270: 2055 7365 2061 7320 666f 6c6c 6f77 732e   Use as follows.
+00005280: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a66  ....```python..f
+00005290: 726f 6d20 4578 6365 7074 6e6f 7469 6669  rom Exceptnotifi
+000052a0: 6572 2069 6d70 6f72 7420 4578 6365 7074  er import Except
+000052b0: 4265 6570 2c20 5375 6363 6573 7342 6565  Beep, SuccessBee
+000052c0: 702c 2053 656e 6442 6565 7028 292c 2062  p, SendBeep(), b
+000052d0: 6565 7028 290d 0a42 4545 505f 5449 4d45  eep()..BEEP_TIME
+000052e0: 203d 2031 0d0a 7379 732e 6578 6365 7074   = 1..sys.except
+000052f0: 686f 6f6b 203d 2045 7863 6570 7442 6565  hook = ExceptBee
+00005300: 702e 5f5f 6361 6c6c 5f5f 0d0a 0d0a 7472  p.__call__....tr
+00005310: 793a 0d0a 2020 2020 7072 696e 7428 312f  y:..    print(1/
+00005320: 3230 2920 200d 0a20 2020 2053 7563 6365  20)  ..    Succe
+00005330: 7373 4265 6570 2829 2e5f 5f63 616c 6c5f  ssBeep().__call_
+00005340: 5f28 2920 2331 2073 7563 6365 7373 2062  _() #1 success b
+00005350: 6565 702d 6265 6570 2020 2020 2020 2020  eep-beep        
+00005360: 2020 0d0a 0d0a 6578 6365 7074 2045 7863    ....except Exc
+00005370: 6570 7442 6565 7020 6173 2065 3a20 2020  eptBeep as e:   
+00005380: 2020 2023 3220 6578 6365 7074 2062 6565     #2 except bee
+00005390: 702d 6265 6570 2020 2020 2020 2020 2020  p-beep          
+000053a0: 2020 2020 2020 0d0a 2020 2020 7379 732e        ..    sys.
+000053b0: 6578 6974 2829 0d0a 0d0a 5365 6e64 4265  exit()....SendBe
+000053c0: 6570 2829 2e5f 5f63 616c 6c5f 5f28 2920  ep().__call__() 
+000053d0: 2020 2020 2020 2023 3320 6375 7374 6f6d         #3 custom
+000053e0: 697a 6564 2062 6565 702d 6265 6570 2020  ized beep-beep  
+000053f0: 2020 2020 0d0a 0d0a 6265 6570 2829 0d0a      ....beep()..
+00005400: 0d0a 6060 600d 0a0d 0a3c 4272 3e0d 0a0d  ..```....<Br>...
+00005410: 0a0d 0a23 2320 322d 3131 2e20 2a44 6573  ...## 2-11. *Des
+00005420: 6b74 6f70 204e 6f74 6966 6965 722a 0d0a  ktop Notifier*..
+00005430: 4e6f 2073 6574 7570 2069 7320 7265 7175  No setup is requ
+00005440: 6972 6564 2e20 5573 6520 6173 2066 6f6c  ired. Use as fol
+00005450: 6c6f 7773 2e0d 0a0d 0a60 6060 7079 7468  lows.....```pyth
+00005460: 6f6e 0d0a 6672 6f6d 2045 7863 6570 744e  on..from ExceptN
+00005470: 6f74 6966 6965 7220 696d 706f 7274 2045  otifier import E
+00005480: 7863 6570 7444 6573 6b74 6f70 2c20 5375  xceptDesktop, Su
+00005490: 6363 6573 7344 6573 6b74 6f70 2c20 5365  ccessDesktop, Se
+000054a0: 6e64 4465 736b 746f 700d 0a73 7973 2e65  ndDesktop..sys.e
+000054b0: 7863 6570 7468 6f6f 6b20 3d20 4578 6365  xcepthook = Exce
+000054c0: 7074 4465 736b 746f 702e 5f5f 6361 6c6c  ptDesktop.__call
+000054d0: 5f5f 0d0a 2320 4465 6669 6e65 2074 6865  __..# Define the
+000054e0: 206e 6578 7420 7477 6f20 7661 7269 6162   next two variab
+000054f0: 6c65 7320 6f70 7469 6f6e 616c 6c79 2077  les optionally w
+00005500: 6865 6e20 7573 696e 6720 4f70 656e 4149  hen using OpenAI
+00005510: 2773 2041 5049 2e0d 0a23 205f 4f50 454e  's API...# _OPEN
+00005520: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
+00005530: 2e35 2d74 7572 626f 2220 2020 200d 0a23  .5-turbo"    ..#
+00005540: 205f 4f50 454e 5f41 495f 4150 493d 2273   _OPEN_AI_API="s
+00005550: 6b2d 7878 7878 7878 220d 0a0d 0a74 7279  k-xxxxxx"....try
+00005560: 3a0d 0a20 2020 2070 7269 6e74 2831 2f30  :..    print(1/0
+00005570: 2920 200d 0a20 2020 2053 7563 6365 7373  )  ..    Success
+00005580: 4465 736b 746f 7028 292e 5f5f 6361 6c6c  Desktop().__call
+00005590: 5f5f 2829 2023 3120 7375 6363 6573 7320  __() #1 success 
+000055a0: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
+000055b0: 0d0a 0d0a 6578 6365 7074 2045 7863 6570  ....except Excep
+000055c0: 7444 6573 6b74 6f70 2061 7320 653a 2020  tDesktop as e:  
+000055d0: 2020 2020 2332 2065 7863 6570 7420 7365      #2 except se
+000055e0: 6e64 6572 2020 2020 2020 2020 2020 2020  nder            
+000055f0: 0d0a 2020 2020 7379 732e 6578 6974 2829  ..    sys.exit()
+00005600: 0d0a 0d0a 5365 6e64 4465 736b 746f 7028  ....SendDesktop(
+00005610: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
+00005620: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
+00005630: 6420 7365 6e64 6572 2020 2020 2020 2020  d sender        
+00005640: 200d 0a60 6060 0d0a 0d0a 3c42 723e 3c62   ..```....<Br><b
+00005650: 723e 3c62 723e 0d0a 0d0a 2320 4c69 6365  r><br>....# Lice
+00005660: 6e73 650d 0a4d 4954 0d0a 0d0a 2320 436f  nse..MIT....# Co
+00005670: 6465 206f 6620 436f 6e64 7563 740d 0a45  de of Conduct..E
+00005680: 7665 7279 6f6e 6520 7061 7274 6963 6970  veryone particip
+00005690: 6174 696e 6720 696e 2074 6865 2060 4578  ating in the `Ex
+000056a0: 6365 7074 4e6f 7469 6669 6572 6020 7072  ceptNotifier` pr
+000056b0: 6f6a 6563 742c 2061 6e64 2069 6e20 7061  oject, and in pa
+000056c0: 7274 6963 756c 6172 2069 6e20 7468 6520  rticular in the 
+000056d0: 6973 7375 6520 7472 6163 6b65 722c 2070  issue tracker, p
+000056e0: 756c 6c20 7265 7175 6573 7473 2c20 616e  ull requests, an
+000056f0: 6420 736f 6369 616c 206d 6564 6961 2061  d social media a
+00005700: 6374 6976 6974 792c 2069 7320 6578 7065  ctivity, is expe
+00005710: 6374 6564 2074 6f20 7472 6561 7420 6f74  cted to treat ot
+00005720: 6865 7220 7065 6f70 6c65 2077 6974 6820  her people with 
+00005730: 7265 7370 6563 7420 616e 6420 6d6f 7265  respect and more
+00005740: 2067 656e 6572 616c 6c79 2074 6f20 666f   generally to fo
+00005750: 6c6c 6f77 2074 6865 2067 7569 6465 6c69  llow the guideli
+00005760: 6e65 7320 6172 7469 6375 6c61 7465 6420  nes articulated 
+00005770: 696e 205b 7468 6520 5079 7468 6f6e 2043  in [the Python C
+00005780: 6f6d 6d75 6e69 7479 2043 6f64 6520 6f66  ommunity Code of
+00005790: 2043 6f6e 6475 6374 5d28 6874 7470 733a   Conduct](https:
+000057a0: 2f2f 7777 772e 7079 7468 6f6e 2e6f 7267  //www.python.org
+000057b0: 2f70 7366 2f63 6f6e 6475 6374 2f29 2e0d  /psf/conduct/)..
+000057c0: 0a0d 0a23 2323 2323 2054 6865 2070 6163  ...##### The pac
+000057d0: 6b61 6765 2069 7320 6375 7272 656e 746c  kage is currentl
+000057e0: 7920 696e 2074 6865 2064 6576 656c 6f70  y in the develop
+000057f0: 6d65 6e74 2061 6e64 2051 4120 7374 6167  ment and QA stag
+00005800: 6573 2c20 616e 6420 7468 6520 6465 7665  es, and the deve
+00005810: 6c6f 706d 656e 7420 7374 6167 6520 7769  lopment stage wi
+00005820: 6c6c 2062 6520 7570 6461 7465 6420 6174  ll be updated at
+00005830: 2074 6865 2074 6f70 206f 6620 7468 6973   the top of this
+00005840: 2070 6167 652e 2049 6620 6974 2069 7320   page. If it is 
+00005850: 6465 7465 726d 696e 6564 2074 6861 7420  determined that 
+00005860: 7468 6520 7072 6f64 7563 7420 6973 2073  the product is s
+00005870: 7461 626c 6520 7468 726f 7567 6820 6665  table through fe
+00005880: 6174 7572 6520 696d 7072 6f76 656d 656e  ature improvemen
+00005890: 742c 2061 6464 6974 696f 6e2c 2061 6e64  t, addition, and
+000058a0: 2069 7373 7565 2072 6573 6f6c 7574 696f   issue resolutio
+000058b0: 6e2c 2074 6865 2064 6576 656c 6f70 6d65  n, the developme
+000058c0: 6e74 2073 7461 6765 2077 696c 6c20 7265  nt stage will re
+000058d0: 6163 6820 7374 6167 6520 352e 2049 6620  ach stage 5. If 
+000058e0: 6e6f 206e 6577 2075 7064 6174 6573 206f  no new updates o
+000058f0: 7220 6973 7375 6573 2061 7269 7365 2c20  r issues arise, 
+00005900: 6974 2077 696c 6c20 6265 2061 646a 7573  it will be adjus
+00005910: 7465 6420 7570 7761 7264 2074 6f20 7374  ted upward to st
+00005920: 6167 6520 3620 6f72 2068 6967 6865 722e  age 6 or higher.
+00005930: 0d0a 0d0a 0d0a                           ......
```

### Comparing `ExceptNotifier-0.1.6/README.md` & `ExceptNotifier-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,1320 +1,1362 @@
 00000000: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
 00000010: 7573 203a 3a20 3320 2d20 416c 7068 6120  us :: 3 - Alpha 
 00000020: 3c62 723e 0d0a 2a43 6f70 7972 6967 6874  <br>..*Copyright
 00000030: 2028 6329 2032 3032 3320 4d69 6e57 6f6f   (c) 2023 MinWoo
 00000040: 2050 6172 6b2c 2053 6f75 7468 204b 6f72   Park, South Kor
-00000050: 6561 2a0d 0a3c 6272 3e0d 0a0d 0a23 2050  ea*..<br>....# P
-00000060: 7974 686f 6e20 5061 636b 6167 653a 2045  ython Package: E
-00000070: 7863 6570 744e 6f74 6966 6965 720d 0a21  xceptNotifier..!
-00000080: 5b45 7863 6570 742d 4e6f 7469 6669 6572  [Except-Notifier
-00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-000000b0: 7970 692d 4578 6365 7074 4e6f 7469 6669  ypi-ExceptNotifi
-000000c0: 6572 2d6f 7261 6e67 6529 0d0a 215b 5079  er-orange)..![Py
-000000d0: 7069 2056 6572 7369 6f6e 5d28 6874 7470  pi Version](http
-000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-000000f0: 696f 2f70 7970 692f 762f 4578 6365 7074  io/pypi/v/Except
-00000100: 4e6f 7469 6669 6572 2e73 7667 290d 0a5b  Notifier.svg)..[
-00000110: 215b 5079 7468 6f6e 2056 6572 7369 6f6e  ![Python Version
-00000120: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000130: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
-00000140: 7974 686f 6e2d 332e 3625 3230 746f 2532  ython-3.6%20to%2
-00000150: 3033 2e37 2d62 6c61 636b 295d 2863 6f64  03.7-black)](cod
-00000160: 655f 6f66 5f63 6f6e 6475 6374 2e6d 6429  e_of_conduct.md)
-00000170: 0d0a 215b 436f 6465 2063 6f6e 7665 6e74  ..![Code convent
-00000180: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00000190: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000001a0: 652f 636f 6465 2532 3063 6f6e 7665 6e74  e/code%20convent
-000001b0: 696f 6e2d 7065 7038 2d62 6c61 636b 290d  ion-pep8-black).
-000001c0: 0a23 2323 2323 2050 726f 7669 6465 7320  .##### Provides 
-000001d0: 6120 6e6f 7469 6669 6361 7469 6f6e 2066  a notification f
-000001e0: 726f 6d20 7468 6520 6170 706c 6963 6174  rom the applicat
-000001f0: 696f 6e20 7368 6f77 6e20 696e 2074 6865  ion shown in the
-00000200: 2066 6f6c 6c6f 7769 6e67 2073 6372 6565   following scree
-00000210: 6e2c 0d0a 0d0a 215b 5d28 6874 7470 733a  n,....![](https:
-00000220: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7364  //github.com/dsd
-00000230: 616e 6965 6c70 6172 6b2f 4578 6365 7074  anielpark/Except
-00000240: 4e6f 7469 6669 6572 2f62 6c6f 622f 6d61  Notifier/blob/ma
-00000250: 696e 2f61 7373 6574 732f 696d 6773 2f6d  in/assets/imgs/m
-00000260: 6169 6e32 2e70 6e67 290d 0a20 5468 6520  ain2.png).. The 
-00000270: 6045 7863 6570 744e 6f74 6966 6965 7260  `ExceptNotifier`
-00000280: 2050 7974 686f 6e20 7061 636b 6167 6520   Python package 
-00000290: 6f66 6665 7273 2061 2066 6c65 7869 626c  offers a flexibl
-000002a0: 6520 6170 7072 6f61 6368 2074 6f20 7265  e approach to re
-000002b0: 6365 6976 696e 6720 6e6f 7469 6669 6361  ceiving notifica
-000002c0: 7469 6f6e 7320 6279 2065 6e68 616e 6369  tions by enhanci
-000002d0: 6e67 2050 7974 686f 6e27 7320 7472 792d  ng Python's try-
-000002e0: 6578 6365 7074 2073 7461 7465 6d65 6e74  except statement
-000002f0: 2e20 5468 6973 2070 6163 6b61 6765 2065  . This package e
-00000300: 6e61 626c 6573 2079 6f75 2074 6f20 7265  nables you to re
-00000310: 6365 6976 6520 616c 6572 7473 2074 6872  ceive alerts thr
-00000320: 6f75 6768 2076 6172 696f 7573 206d 6573  ough various mes
-00000330: 7361 6769 6e67 2061 7070 6c69 6361 7469  saging applicati
-00000340: 6f6e 7320 6f72 2065 6d61 696c 732e 0d0a  ons or emails...
-00000350: 3c42 723e 3c62 723e 0d0a 5769 7468 2060  <Br><br>..With `
-00000360: 4578 6365 7074 4e6f 7469 6669 6572 602c  ExceptNotifier`,
-00000370: 2079 6f75 2063 616e 206f 6274 6169 6e20   you can obtain 
-00000380: 6465 7461 696c 6564 2063 6f6d 7069 6c61  detailed compila
-00000390: 7469 6f6e 2065 7272 6f72 732c 2069 6e63  tion errors, inc
-000003a0: 6c75 6469 6e67 2064 6562 7567 2069 6e66  luding debug inf
-000003b0: 6f72 6d61 7469 6f6e 2c20 7365 6e74 2064  ormation, sent d
-000003c0: 6972 6563 746c 7920 746f 2079 6f75 7220  irectly to your 
-000003d0: 7072 6566 6572 7265 6420 6d65 7373 6167  preferred messag
-000003e0: 696e 6720 706c 6174 666f 726d 206f 7220  ing platform or 
-000003f0: 656d 6169 6c2e 2042 7920 696e 7465 6772  email. By integr
-00000400: 6174 696e 6720 4f70 656e 4149 2773 2043  ating OpenAI's C
-00000410: 6861 7447 5054 2c20 796f 7520 6361 6e20  hatGPT, you can 
-00000420: 7265 6365 6976 6520 6164 6469 7469 6f6e  receive addition
-00000430: 616c 2065 7272 6f72 2063 6f64 6520 696e  al error code in
-00000440: 666f 726d 6174 696f 6e20 6173 206c 6f6e  formation as lon
-00000450: 6720 6173 2079 6f75 2070 726f 7669 6465  g as you provide
-00000460: 2074 6865 2072 6571 7569 7265 6420 4150   the required AP
-00000470: 4920 6d6f 6465 6c20 6e61 6d65 2061 6e64  I model name and
-00000480: 206b 6579 2e20 5468 6973 2066 6561 7475   key. This featu
-00000490: 7265 2065 6e73 7572 6573 2074 6861 7420  re ensures that 
-000004a0: 6572 726f 7220 6861 6e64 6c69 6e67 2061  error handling a
-000004b0: 6e64 206e 6f74 6966 6963 6174 696f 6e73  nd notifications
-000004c0: 2061 7265 206d 6f72 6520 696e 666f 726d   are more inform
-000004d0: 6174 6976 6520 616e 6420 6163 6365 7373  ative and access
-000004e0: 6962 6c65 2c20 7374 7265 616d 6c69 6e69  ible, streamlini
-000004f0: 6e67 2079 6f75 7220 6465 6275 6767 696e  ng your debuggin
-00000500: 6720 7072 6f63 6573 732e 0d0a 0d0a 3c62  g process.....<b
-00000510: 723e 3c62 723e 0d0a 0d0a 2323 2320 5375  r><br>....### Su
-00000520: 7070 6f72 7469 6e67 2041 7070 6c69 6361  pporting Applica
-00000530: 7469 6f6e 730d 0a0d 0a2d 205b 5465 6c65  tions....- [Tele
-00000540: 6772 616d 5d28 6874 7470 733a 2f2f 7465  gram](https://te
-00000550: 6c65 6772 616d 2e6f 7267 2f29 0d0a 2d20  legram.org/)..- 
-00000560: 5b44 6973 636f 7264 5d28 6874 7470 733a  [Discord](https:
-00000570: 2f2f 6469 7363 6f72 642e 636f 6d2f 290d  //discord.com/).
-00000580: 0a2d 205b 536c 6163 6b5d 2868 7474 7073  .- [Slack](https
-00000590: 3a2f 2f73 6c61 636b 2e63 6f6d 2f29 0d0a  ://slack.com/)..
-000005a0: 2d20 5b47 6f6f 676c 6520 4d61 696c 5d28  - [Google Mail](
-000005b0: 6874 7470 733a 2f2f 6d61 696c 2e67 6f6f  https://mail.goo
-000005c0: 676c 652e 636f 6d2f 290d 0a2d 2053 4d53  gle.com/)..- SMS
-000005d0: 2053 656e 6469 6e67 2075 7369 6e67 205b   Sending using [
-000005e0: 5477 696c 696f 5d28 6874 7470 733a 2f2f  Twilio](https://
-000005f0: 7777 772e 7477 696c 696f 2e63 6f6d 2f65  www.twilio.com/e
-00000600: 6e2d 7573 290d 0a2d 2044 6573 6b74 6f70  n-us)..- Desktop
-00000610: 204e 6f74 6966 6963 6174 696f 6e20 7573   Notification us
-00000620: 696e 6720 5b50 6c79 6572 5d28 6874 7470  ing [Plyer](http
-00000630: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-00000640: 6976 792f 706c 7965 7229 0d0a 2d20 5b4c  ivy/plyer)..- [L
-00000650: 696e 655d 2868 7474 7073 3a2f 2f6c 696e  ine](https://lin
-00000660: 652e 6d65 2f65 6e2f 290d 0a2d 205b 4157  e.me/en/)..- [AW
-00000670: 5320 4368 696d 655d 2868 7474 7073 3a2f  S Chime](https:/
-00000680: 2f61 7773 2e61 6d61 7a6f 6e2e 636f 6d2f  /aws.amazon.com/
-00000690: 6b6f 2f63 6869 6d65 2f64 6f77 6e6c 6f61  ko/chime/downloa
-000006a0: 642d 6368 696d 652f 290d 0a2d 205b 4d69  d-chime/)..- [Mi
-000006b0: 6372 6f73 6f66 7420 5465 616d 735d 2868  crosoft Teams](h
-000006c0: 7474 7073 3a2f 2f77 7777 2e6d 6963 726f  ttps://www.micro
-000006d0: 736f 6674 2e63 6f6d 2f65 6e2f 6d69 6372  soft.com/en/micr
-000006e0: 6f73 6f66 742d 7465 616d 732f 646f 776e  osoft-teams/down
-000006f0: 6c6f 6164 2d61 7070 290d 0a2d 205b 4b61  load-app)..- [Ka
-00000700: 6b61 6f20 5461 6c6b 5d28 6874 7470 733a  kao Talk](https:
-00000710: 2f2f 7777 772e 6b61 6b61 6f63 6f72 702e  //www.kakaocorp.
-00000720: 636f 6d2f 7061 6765 2f73 6572 7669 6365  com/page/service
-00000730: 2f73 6572 7669 6365 2f4b 616b 616f 5461  /service/KakaoTa
-00000740: 6c6b 3f6c 616e 673d 656e 290d 0a2d 2042  lk?lang=en)..- B
-00000750: 6565 7020 536f 756e 6420 6672 6f6d 205b  eep Sound from [
-00000760: 7379 7374 656d 5d28 6874 7470 733a 2f2f  system](https://
-00000770: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
-00000780: 332f 6c69 6272 6172 792f 7769 6e73 6f75  3/library/winsou
-00000790: 6e64 2e68 746d 6c29 0d0a 0d0a 3c42 723e  nd.html)....<Br>
-000007a0: 0d0a 0d0a 2323 2320 4149 2044 6562 7567  ....### AI Debug
-000007b0: 6769 6e67 0d0a 4966 2079 6f75 2068 6176  ging..If you hav
-000007c0: 6520 4f70 656e 4149 2041 5049 204b 6579  e OpenAI API Key
-000007d0: 2061 6e64 206d 6f64 656c 206e 616d 652c   and model name,
-000007e0: 2079 6f75 2063 616e 2067 6574 2069 6e66   you can get inf
-000007f0: 6f72 6d61 7469 6f6e 2061 6e64 2063 6f64  ormation and cod
-00000800: 6520 6578 616d 706c 6573 2066 6f72 2064  e examples for d
-00000810: 6562 7567 6769 6e67 2069 6e20 616e 7920  ebugging in any 
-00000820: 6170 706c 6963 6174 696f 6e2e 0d0a 2d20  application...- 
-00000830: 5b4f 5045 4e20 4149 2041 5049 5d28 6874  [OPEN AI API](ht
-00000840: 7470 733a 2f2f 706c 6174 666f 726d 2e6f  tps://platform.o
-00000850: 7065 6e61 692e 636f 6d2f 646f 6373 2f69  penai.com/docs/i
-00000860: 6e74 726f 6475 6374 696f 6e29 0d0a 0d0a  ntroduction)....
-00000870: 0d0a 3c62 723e 3c62 723e 0d0a 0d0a 2320  ..<br><br>....# 
-00000880: 5175 6963 6b20 5374 6172 740d 0a60 6060  Quick Start..```
-00000890: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
-000008a0: 6c20 4578 6365 7074 4e6f 7469 6669 6572  l ExceptNotifier
-000008b0: 0d0a 7069 7020 696e 7374 616c 6c20 6578  ..pip install ex
-000008c0: 6365 7074 6e6f 7469 6669 6572 0d0a 0d0a  ceptnotifier....
-000008d0: 636f 6e64 6120 696e 7374 616c 6c20 4578  conda install Ex
-000008e0: 6365 7074 4e6f 7469 6669 6572 0d0a 636f  ceptNotifier..co
-000008f0: 6e64 6120 696e 7374 616c 6c20 6578 6365  nda install exce
-00000900: 7074 6e6f 7469 6669 6572 0d0a 6060 600d  ptnotifier..```.
-00000910: 0a0d 0a3c 6272 3e0d 0a0d 0a0d 0a23 2041  ...<br>......# A
-00000920: 7070 2053 6574 7570 204f 7665 7276 6965  pp Setup Overvie
-00000930: 770d 0a0d 0a2d 2054 6865 2076 6172 6961  w....- The varia
-00000940: 626c 6573 2069 6e20 7468 6520 666f 6c6c  bles in the foll
-00000950: 6f77 696e 6720 7461 626c 6520 6d75 7374  owing table must
-00000960: 206e 6f74 2062 6520 636f 6e74 616d 696e   not be contamin
-00000970: 6174 6564 2e0d 0a2d 2044 6570 656e 6469  ated...- Dependi
-00000980: 6e67 206f 6e20 7468 6520 7369 7475 6174  ng on the situat
-00000990: 696f 6e2c 2063 6f6e 7369 6465 7220 6465  ion, consider de
-000009a0: 7369 676e 6174 696e 6720 7468 656d 2061  signating them a
-000009b0: 7320 676c 6f62 616c 2076 6172 6961 626c  s global variabl
-000009c0: 6573 2066 6f72 2075 7365 2e0d 0a2d 2049  es for use...- I
-000009d0: 6620 796f 7520 6172 6520 7573 696e 6720  f you are using 
-000009e0: 5465 6c65 6772 616d 2c20 616e 2065 7861  Telegram, an exa
-000009f0: 6d70 6c65 2069 7320 6174 7461 6368 6564  mple is attached
-00000a00: 2061 7320 616e 2069 6d61 6765 2e0d 0a2d   as an image...-
-00000a10: 2041 7320 796f 7520 616c 7265 6164 7920   As you already 
-00000a20: 6b6e 6f77 2c20 4150 4920 4b65 7973 206f  know, API Keys o
-00000a30: 7220 7365 6375 7269 7479 2074 6f6b 656e  r security token
-00000a40: 7320 6d75 7374 2062 6520 7365 6375 7265  s must be secure
-00000a50: 642e 204e 6f74 6520 7468 6174 2074 6865  d. Note that the
-00000a60: 206b 6579 2076 616c 7565 7320 7768 6963   key values whic
-00000a70: 6820 6578 706f 7375 7265 6420 696e 2067  h exposured in g
-00000a80: 6974 6875 6220 7769 6c6c 2062 6520 6578  ithub will be ex
-00000a90: 7069 7265 6420 6166 7465 7220 696e 7365  pired after inse
-00000aa0: 6375 7265 642e 0d0a 0d0a 7c20 4170 7020  cured.....| App 
-00000ab0: 7c20 5265 7175 6972 6564 2056 6172 6961  | Required Varia
-00000ac0: 626c 6573 207c 2046 7265 6520 6f72 2050  bles | Free or P
-00000ad0: 6169 6420 7c20 4561 7365 206f 6620 5365  aid | Ease of Se
-00000ae0: 7475 7020 7c20 5469 6d65 2052 6571 7569  tup | Time Requi
-00000af0: 7265 6420 666f 7220 5365 7475 707c 4775  red for Setup|Gu
-00000b00: 6964 6520 5475 746f 7269 616c 204c 696e  ide Tutorial Lin
-00000b10: 6b7c 0d0a 7c3a 2d2d 3a7c 3a2d 2d7c 3a2d  k|..|:--:|:--|:-
-00000b20: 2d3a 7c3a 2d2d 3a7c 3a2d 2d3a 7c3a 2d2d  -:|:--:|:--:|:--
-00000b30: 2d3a 7c0d 0a7c 4265 6570 7c4e 2f41 7c46  -:|..|Beep|N/A|F
-00000b40: 7265 657c 4e2f 417c 3020 6d69 6e7c 5b45  ree|N/A|0 min|[E
-00000b50: 7863 6570 7442 6565 705d 2868 7474 7073  xceptBeep](https
-00000b60: 3a2f 2f67 6974 6875 622e 636f 6d2f 6473  ://github.com/ds
-00000b70: 6461 6e69 656c 7061 726b 2f45 7863 6570  danielpark/Excep
-00000b80: 744e 6f74 6966 6965 722f 626c 6f62 2f6d  tNotifier/blob/m
-00000b90: 6169 6e2f 646f 6375 6d65 6e74 732f 4578  ain/documents/Ex
-00000ba0: 6365 7074 4265 6570 2f47 5549 4445 2e6d  ceptBeep/GUIDE.m
-00000bb0: 6429 7c0d 0a7c 4465 736b 746f 707c 4e2f  d)|..|Desktop|N/
-00000bc0: 417c 4672 6565 7c4e 2f41 7c30 206d 696e  A|Free|N/A|0 min
-00000bd0: 7c5b 4578 6365 7074 4465 736b 746f 705d  |[ExceptDesktop]
-00000be0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000bf0: 636f 6d2f 6473 6461 6e69 656c 7061 726b  com/dsdanielpark
-00000c00: 2f45 7863 6570 744e 6f74 6966 6965 722f  /ExceptNotifier/
-00000c10: 626c 6f62 2f6d 6169 6e2f 646f 6375 6d65  blob/main/docume
-00000c20: 6e74 732f 4578 6365 7074 4465 736b 746f  nts/ExceptDeskto
-00000c30: 702f 4755 4944 452e 6d64 297c 0d0a 7c54  p/GUIDE.md)|..|T
-00000c40: 656c 6567 7261 6d7c 605f 5445 4c45 4752  elegram|`_TELEGR
-00000c50: 414d 5f54 4f4b 454e 607c 4672 6565 6d69  AM_TOKEN`|Freemi
-00000c60: 756d 7c45 6173 797c 326d 696e 7c5b 4578  um|Easy|2min|[Ex
-00000c70: 6365 7074 5465 6c65 6772 616d 5d28 6874  ceptTelegram](ht
-00000c80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000c90: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
-00000ca0: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
-00000cb0: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
-00000cc0: 2f45 7863 6570 7454 656c 6567 7261 6d2f  /ExceptTelegram/
-00000cd0: 4755 4944 452e 6d64 297c 0d0a 7c44 6973  GUIDE.md)|..|Dis
-00000ce0: 636f 7264 7c60 5f44 4953 434f 5244 5f57  cord|`_DISCORD_W
-00000cf0: 4542 484f 4f4b 5f55 524c 607c 4672 6565  EBHOOK_URL`|Free
-00000d00: 6d69 756d 7c45 6173 797c 316d 696e 7c5b  mium|Easy|1min|[
-00000d10: 4578 6365 7074 4469 7363 6f72 645d 2868  ExceptDiscord](h
-00000d20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000d30: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00000d40: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00000d50: 6f62 2f6d 6169 6e2f 646f 6375 6d65 6e74  ob/main/document
-00000d60: 732f 4578 6365 7074 5465 6c65 6772 616d  s/ExceptTelegram
-00000d70: 2f47 5549 4445 2e6d 6429 7c0d 0a7c 4157  /GUIDE.md)|..|AW
-00000d80: 5320 4368 696d 657c 605f 4348 494d 455f  S Chime|`_CHIME_
-00000d90: 5745 4248 4f4f 4b5f 5552 4c60 7c46 7265  WEBHOOK_URL`|Fre
-00000da0: 656d 6975 6d7c 4561 7379 7c31 6d69 6e7c  emium|Easy|1min|
-00000db0: 5b45 7863 6570 7443 6869 6d65 5d28 6874  [ExceptChime](ht
-00000dc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000dd0: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
-00000de0: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
-00000df0: 622f 6d61 696e 2f64 6f63 756d 656e 7473  b/main/documents
-00000e00: 2f45 7863 6570 7443 6869 6d65 2f47 5549  /ExceptChime/GUI
-00000e10: 4445 2e6d 6429 7c0d 0a7c 536c 6163 6b7c  DE.md)|..|Slack|
-00000e20: 605f 534c 4143 4b5f 5745 4248 4f4f 4b5f  `_SLACK_WEBHOOK_
-00000e30: 5552 4c60 7c46 7265 656d 6975 6d7c 4561  URL`|Freemium|Ea
-00000e40: 7379 7c33 6d69 6e7c 5b45 7863 6570 7453  sy|3min|[ExceptS
-00000e50: 6c61 636b 5d28 6874 7470 733a 2f2f 6769  lack](https://gi
-00000e60: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
-00000e70: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
-00000e80: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
-00000e90: 6f63 756d 656e 7473 2f45 7863 6570 7453  ocuments/ExceptS
-00000ea0: 6c61 636b 2f47 5549 4445 2e6d 6429 7c0d  lack/GUIDE.md)|.
-00000eb0: 0a7c 472d 4d61 696c 7c60 5f47 414d 494c  .|G-Mail|`_GAMIL
-00000ec0: 5f52 4543 4950 4945 4e54 5f41 4444 5260  _RECIPIENT_ADDR`
-00000ed0: 2c20 605f 474d 4149 4c5f 5345 4e44 4552  , `_GMAIL_SENDER
-00000ee0: 5f41 4444 5260 2c20 605f 474d 4149 4c5f  _ADDR`, `_GMAIL_
-00000ef0: 4150 505f 5041 5353 574f 5244 5f4f 465f  APP_PASSWORD_OF_
-00000f00: 5345 4e44 4552 6020 7c52 6573 7472 6963  SENDER` |Restric
-00000f10: 7465 6420 6672 6565 7c4d 6564 6975 6d7c  ted free|Medium|
-00000f20: 336d 696e 7c5b 4578 6365 7074 4d61 696c  3min|[ExceptMail
-00000f30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000f40: 2e63 6f6d 2f64 7364 616e 6965 6c70 6172  .com/dsdanielpar
-00000f50: 6b2f 4578 6365 7074 4e6f 7469 6669 6572  k/ExceptNotifier
-00000f60: 2f62 6c6f 622f 6d61 696e 2f64 6f63 756d  /blob/main/docum
-00000f70: 656e 7473 2f45 7863 6570 744d 6169 6c2f  ents/ExceptMail/
-00000f80: 4755 4944 452e 6d64 297c 0d0a 7c4c 696e  GUIDE.md)|..|Lin
-00000f90: 657c 605f 4c49 4e45 5f4e 4f54 4946 595f  e|`_LINE_NOTIFY_
-00000fa0: 4150 495f 544f 4b45 4e60 7c46 7265 656d  API_TOKEN`|Freem
-00000fb0: 6975 6d7c 4d65 6469 756d 7c34 6d69 6e7c  ium|Medium|4min|
-00000fc0: 5b45 7863 6570 744c 696e 655d 2868 7474  [ExceptLine](htt
-00000fd0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000fe0: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
-00000ff0: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
-00001000: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
-00001010: 4578 6365 7074 4c69 6e65 2f47 5549 4445  ExceptLine/GUIDE
-00001020: 2e6d 6429 7c0d 0a7c 534d 537c 605f 5457  .md)|..|SMS|`_TW
-00001030: 494c 494f 5f53 4944 602c 2060 5f54 5749  ILIO_SID`, `_TWI
-00001040: 4c49 4f5f 544f 4b45 4e60 2c20 605f 5245  LIO_TOKEN`, `_RE
-00001050: 4349 5049 454e 545f 5048 4f4e 455f 4e55  CIPIENT_PHONE_NU
-00001060: 4d42 4552 602c 2060 5f53 454e 4445 525f  MBER`, `_SENDER_
-00001070: 5048 4f4e 455f 4e55 4d42 4552 607c 4e6f  PHONE_NUMBER`|No
-00001080: 7420 6672 6565 7c4d 6564 6975 6d7c 356d  t free|Medium|5m
-00001090: 696e 7c5b 4578 6365 7074 534d 535d 2868  in|[ExceptSMS](h
-000010a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000010b0: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-000010c0: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-000010d0: 6f62 2f6d 6169 6e2f 646f 6375 6d65 6e74  ob/main/document
-000010e0: 732f 4578 6365 7074 534d 532f 4755 4944  s/ExceptSMS/GUID
-000010f0: 452e 6d64 297c 0d0a 7c4d 6963 726f 736f  E.md)|..|Microso
-00001100: 6674 2054 6561 6d73 7c60 5f54 4541 4d53  ft Teams|`_TEAMS
-00001110: 5f57 4542 484f 4f4b 5f55 524c 607c 4e6f  _WEBHOOK_URL`|No
-00001120: 7420 4672 6565 7c4d 6564 6975 6d7c 356d  t Free|Medium|5m
-00001130: 696e 7c5b 4578 6365 7074 5465 616d 735d  in|[ExceptTeams]
-00001140: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001150: 636f 6d2f 6473 6461 6e69 656c 7061 726b  com/dsdanielpark
-00001160: 2f45 7863 6570 744e 6f74 6966 6965 722f  /ExceptNotifier/
-00001170: 626c 6f62 2f6d 6169 6e2f 646f 6375 6d65  blob/main/docume
-00001180: 6e74 732f 4578 6365 7074 5465 616d 732f  nts/ExceptTeams/
-00001190: 4755 4944 452e 6d64 297c 0d0a 7c4b 616b  GUIDE.md)|..|Kak
-000011a0: 616f 5461 6c6b 7c60 5f4b 414b 414f 5f54  aoTalk|`_KAKAO_T
-000011b0: 4f4b 454e 5f50 4154 4860 7c46 7265 656d  OKEN_PATH`|Freem
-000011c0: 6975 6d7c 4865 6c6c 7c3e 3d31 306d 696e  ium|Hell|>=10min
-000011d0: 2854 6f6b 656e 2072 6566 7265 7368 6573  (Token refreshes
-000011e0: 2064 6169 6c79 2e29 7c5b 4578 6365 7074   daily.)|[Except
-000011f0: 4b61 6b61 6f5d 2868 7474 7073 3a2f 2f67  Kakao](https://g
-00001200: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00001210: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00001220: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00001230: 646f 6375 6d65 6e74 732f 4578 6365 7074  documents/Except
-00001240: 4b61 6b61 6f2f 4755 4944 452e 6d64 297c  Kakao/GUIDE.md)|
-00001250: 0d0a 0d0a 0d0a 4966 2079 6f75 2061 6464  ......If you add
-00001260: 2074 6865 2066 6f6c 6c6f 7769 6e67 2074   the following t
-00001270: 776f 2076 6172 6961 626c 6573 2074 6f20  wo variables to 
-00001280: 7468 6520 7265 7175 6972 6564 2076 6172  the required var
-00001290: 6961 626c 6573 2066 6f72 2065 6163 6820  iables for each 
-000012a0: 6170 706c 6963 6174 696f 6e20 696e 2074  application in t
-000012b0: 6865 2074 6162 6c65 2061 626f 7665 2c20  he table above, 
-000012c0: 796f 7520 6361 6e20 7265 6365 6976 6520  you can receive 
-000012d0: 6572 726f 7220 6c6f 6361 7469 6f6e 2061  error location a
-000012e0: 6e64 2065 7870 6c61 6e61 7469 6f6e 2c20  nd explanation, 
-000012f0: 6173 2077 656c 6c20 6173 2065 7861 6d70  as well as examp
-00001300: 6c65 732c 2066 726f 6d20 4f70 656e 4149  les, from OpenAI
-00001310: 2773 206d 6f64 656c 0d0a 0d0a 7c20 4150  's model....| AP
-00001320: 4920 7c20 5265 7175 6972 6564 2056 6172  I | Required Var
-00001330: 6961 626c 6573 207c 2046 7265 6520 6f72  iables | Free or
-00001340: 2050 6169 6420 7c20 4561 7365 206f 6620   Paid | Ease of 
-00001350: 5365 7475 7020 7c20 5469 6d65 2052 6571  Setup | Time Req
-00001360: 7569 7265 6420 666f 7220 5365 7475 707c  uired for Setup|
-00001370: 4775 6964 6520 5475 746f 7269 616c 204c  Guide Tutorial L
-00001380: 696e 6b7c 0d0a 7c3a 2d2d 3a7c 3a2d 2d7c  ink|..|:--:|:--|
-00001390: 3a2d 2d3a 7c3a 2d2d 3a7c 3a2d 2d3a 7c3a  :--:|:--:|:--:|:
-000013a0: 2d2d 2d3a 7c0d 0a7c 204f 7065 6e41 4920  ---:|..| OpenAI 
-000013b0: 4150 4920 7c60 5265 7175 6972 6564 2076  API |`Required v
-000013c0: 6172 6961 626c 6573 2066 6f72 2065 6163  ariables for eac
-000013d0: 6820 6170 706c 6963 6174 696f 6e60 2b20  h application`+ 
-000013e0: 605f 4f50 454e 5f41 495f 4d4f 4445 4c60  `_OPEN_AI_MODEL`
-000013f0: 2c60 5f4f 5045 4e5f 4149 5f41 5049 607c  ,`_OPEN_AI_API`|
-00001400: 4e6f 7420 6672 6565 7c45 6173 797c 326d  Not free|Easy|2m
-00001410: 696e 7c5b 4150 494f 7065 6e41 495d 2868  in|[APIOpenAI](h
-00001420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001430: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00001440: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00001450: 6f62 2f6d 6169 6e2f 646f 6375 6d65 6e74  ob/main/document
-00001460: 732f 4150 494f 7065 6e41 492f 4755 4944  s/APIOpenAI/GUID
-00001470: 452e 6d64 297c 0d0a 0d0a 0d0a 3c62 723e  E.md)|......<br>
-00001480: 3c62 723e 0d0a 0d0a 2320 312e 204b 6579  <br>....# 1. Key
-00001490: 2046 6561 7475 7265 730d 0a54 6f20 7573   Features..To us
-000014a0: 6520 7468 6520 6465 7369 7265 6420 6170  e the desired ap
-000014b0: 706c 6963 6174 696f 6e2c 2079 6f75 206d  plication, you m
-000014c0: 7573 7420 6465 6669 6e65 2074 6865 206e  ust define the n
-000014d0: 6563 6573 7361 7279 2076 6172 6961 626c  ecessary variabl
-000014e0: 6573 2e20 456e 7375 7265 2074 6861 7420  es. Ensure that 
-000014f0: 7468 6520 7661 7269 6162 6c65 206e 616d  the variable nam
-00001500: 6573 2072 656d 6169 6e20 756e 6368 616e  es remain unchan
-00001510: 6765 642c 2061 6e64 2079 6f75 2063 616e  ged, and you can
-00001520: 2075 7365 2065 6974 6865 7220 6c6f 6361   use either loca
-00001530: 6c20 6f72 2067 6c6f 6261 6c20 7661 7269  l or global vari
-00001540: 6162 6c65 732e 2049 6620 796f 7520 6172  ables. If you ar
-00001550: 6520 7573 696e 6720 6054 656c 6567 7261  e using `Telegra
-00001560: 6d60 2c20 616e 2065 7861 6d70 6c65 2069  m`, an example i
-00001570: 7320 6174 7461 6368 6564 2061 7320 616e  s attached as an
-00001580: 2069 6d61 6765 2e0d 0a0d 0a23 2320 312d   image.....## 1-
-00001590: 312e 2045 7863 6570 7460 5b61 7070 4e61  1. Except`[appNa
-000015a0: 6d65 5d60 0d0a 4966 2079 6f75 2075 7365  me]`..If you use
-000015b0: 2050 7974 686f 6e27 7320 7472 7920 6578   Python's try ex
-000015c0: 6365 7074 2073 7461 7465 6d65 6e74 2061  cept statement a
-000015d0: 7320 6974 2069 732c 2062 7574 2063 6861  s it is, but cha
-000015e0: 6e67 6520 6578 6365 7074 2061 7320 666f  nge except as fo
-000015f0: 6c6c 6f77 732c 2079 6f75 2063 616e 2072  llows, you can r
-00001600: 6563 6569 7665 206e 6f74 6966 6963 6174  eceive notificat
-00001610: 696f 6e73 2074 6872 6f75 6768 2079 6f75  ions through you
-00001620: 7220 6170 706c 6963 6174 696f 6e2e 0d0a  r application...
-00001630: 6060 600d 0a45 7863 6570 7443 6869 6d65  ```..ExceptChime
-00001640: 2c20 4578 6365 7074 5465 6c65 6772 616d  , ExceptTelegram
-00001650: 2c20 4578 6365 7074 4469 7363 6f72 642c  , ExceptDiscord,
-00001660: 2045 7863 6570 7453 4d53 2c20 4578 6365   ExceptSMS, Exce
-00001670: 7074 4d61 696c 2c20 4578 6365 7074 4b61  ptMail, ExceptKa
-00001680: 6b61 6f2c 2045 7863 6570 744c 696e 652c  kao, ExceptLine,
-00001690: 2045 7863 6570 7453 6c61 636b 2c20 4578   ExceptSlack, Ex
-000016a0: 6365 7074 5465 616d 732c 2045 7863 6570  ceptTeams, Excep
-000016b0: 7444 6573 6b74 6f70 652c 2045 7863 6570  tDesktope, Excep
-000016c0: 7442 6565 700d 0a60 6060 0d0a 0d0a 2a45  tBeep..```....*E
-000016d0: 7861 6d70 6c65 2a0d 0a60 6060 7079 7468  xample*..```pyth
-000016e0: 6f6e 0d0a 6672 6f6d 2045 7863 6570 744e  on..from ExceptN
-000016f0: 6f74 6966 6965 7220 696d 706f 7274 2045  otifier import E
-00001700: 7863 6570 7454 656c 6765 7261 6d0d 0a5f  xceptTelgeram.._
-00001710: 5445 4c45 4752 414d 5f54 4f4b 454e 203d  TELEGRAM_TOKEN =
-00001720: 2022 7878 7878 220d 0a0d 0a74 7279 3a0d   "xxxx"....try:.
-00001730: 0a20 2020 2070 7269 6e74 2831 2f30 290d  .    print(1/0).
-00001740: 0a65 7863 6570 7420 4578 6365 7074 5465  .except ExceptTe
-00001750: 6c65 6772 616d 3a20 2020 2023 2073 656e  legram:    # sen
-00001760: 6469 6e67 2065 7863 6570 7420 6d65 7373  ding except mess
-00001770: 6167 6520 746f 2074 656c 6567 7261 6d0d  age to telegram.
-00001780: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
-00001790: 0a60 6060 0d0a 215b 5d28 6874 7470 733a  .```..![](https:
-000017a0: 2f2f 6769 7468 7562 2e63 6f6d 2f64 7364  //github.com/dsd
-000017b0: 616e 6965 6c70 6172 6b2f 4578 6365 7074  anielpark/Except
-000017c0: 4e6f 7469 6669 6572 2f62 6c6f 622f 6d61  Notifier/blob/ma
-000017d0: 696e 2f61 7373 6574 732f 696d 6773 2f65  in/assets/imgs/e
-000017e0: 7831 2e70 6e67 290d 0a0d 0a3c 6272 3e0d  x1.png)....<br>.
-000017f0: 0a0d 0a23 2320 312d 322e 2041 4920 4465  ...## 1-2. AI De
-00001800: 6262 7567 6769 6e67 2049 6e66 6f6d 6174  bbugging Infomat
-00001810: 696f 6e20 4e6f 7469 6669 6361 7469 6f6e  ion Notification
-00001820: 0d0a 596f 7520 6361 6e20 7265 6365 6976  ..You can receiv
-00001830: 6520 6465 6275 6767 696e 6720 696e 666f  e debugging info
-00001840: 726d 6174 696f 6e20 6672 6f6d 2043 6861  rmation from Cha
-00001850: 7447 5054 2076 6961 204f 7065 6e41 4927  tGPT via OpenAI'
-00001860: 7320 4150 4920 7768 656e 2075 7369 6e67  s API when using
-00001870: 2074 6865 2045 7863 6570 7420 7374 6174   the Except stat
-00001880: 656d 656e 742e 2054 6865 2073 796e 7461  ement. The synta
-00001890: 7820 7265 6d61 696e 7320 7468 6520 7361  x remains the sa
-000018a0: 6d65 2c20 6275 7420 796f 7527 6c6c 206e  me, but you'll n
-000018b0: 6565 6420 746f 2063 6f6e 6669 6775 7265  eed to configure
-000018c0: 2074 6865 7365 2074 776f 2076 6172 6961   these two varia
-000018d0: 626c 6573 3a0d 0a60 5f4f 5045 4e5f 4149  bles:..`_OPEN_AI
-000018e0: 5f4d 4f44 454c 602c 605f 4f50 454e 5f41  _MODEL`,`_OPEN_A
-000018f0: 495f 4150 4960 0d0a 0d0a 2a45 7861 6d70  I_API`....*Examp
-00001900: 6c65 2a0d 0a60 6060 7079 7468 6f6e 0d0a  le*..```python..
-00001910: 6672 6f6d 2045 7863 6570 744e 6f74 6966  from ExceptNotif
-00001920: 6965 7220 696d 706f 7274 2045 7863 6570  ier import Excep
-00001930: 7454 656c 6765 7261 6d0d 0a5f 5445 4c45  tTelgeram.._TELE
-00001940: 4752 414d 5f54 4f4b 454e 203d 2022 7878  GRAM_TOKEN = "xx
-00001950: 7878 220d 0a5f 4f50 454e 5f41 495f 4d4f  xx".._OPEN_AI_MO
-00001960: 4445 4c3d 2267 7074 2d33 2e35 2d74 7572  DEL="gpt-3.5-tur
-00001970: 626f 220d 0a5f 4f50 454e 5f41 495f 4150  bo".._OPEN_AI_AP
-00001980: 493d 2273 6b2d 7878 7878 7878 220d 0a0d  I="sk-xxxxxx"...
-00001990: 0a74 7279 3a0d 0a20 2020 2070 7269 6e74  .try:..    print
-000019a0: 2831 2f30 290d 0a65 7863 6570 7420 4578  (1/0)..except Ex
-000019b0: 6365 7074 5465 6c65 6772 616d 3a20 2320  ceptTelegram: # 
-000019c0: 7365 6e64 696e 6720 6d73 6720 5749 5448  sending msg WITH
-000019d0: 2041 4920 4445 4255 4747 494e 4720 746f   AI DEBUGGING to
-000019e0: 2074 656c 6567 7261 6d0d 0a20 2020 2073   telegram..    s
-000019f0: 7973 2e65 7869 7428 290d 0a60 6060 0d0a  ys.exit()..```..
-00001a00: 0d0a 215b 5d28 6874 7470 733a 2f2f 6769  ..![](https://gi
-00001a10: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
-00001a20: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
-00001a30: 6669 6572 2f62 6c6f 622f 6d61 696e 2f61  fier/blob/main/a
-00001a40: 7373 6574 732f 696d 6773 2f65 7832 2e70  ssets/imgs/ex2.p
-00001a50: 6e67 290d 0a0d 0a3c 6272 3e0d 0a0d 0a23  ng)....<br>....#
-00001a60: 2320 312d 332e 2053 7563 6365 7373 605b  # 1-3. Success`[
-00001a70: 6170 704e 616d 655d 600d 0a42 7920 706c  appName]`..By pl
-00001a80: 6163 696e 6720 7468 6520 7472 7920 6578  acing the try ex
-00001a90: 6365 7074 2069 6e20 7079 7468 6f6e 2061  cept in python a
-00001aa0: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
-00001ab0: 2074 7279 2073 7461 7465 6d65 6e74 2c20   try statement, 
-00001ac0: 6170 706c 6963 6174 696f 6e73 2063 616e  applications can
-00001ad0: 2062 6520 6e6f 7469 6669 6564 2074 6861   be notified tha
-00001ae0: 7420 7468 6520 7472 7920 7374 6174 656d  t the try statem
-00001af0: 656e 7420 776f 726b 6564 206e 6f72 6d61  ent worked norma
-00001b00: 6c6c 792e 0d0a 6060 600d 0a53 7563 6365  lly...```..Succe
-00001b10: 7373 4368 696d 652c 2053 7563 6365 7373  ssChime, Success
-00001b20: 5465 6c65 6772 616d 2c20 5375 6363 6573  Telegram, Succes
-00001b30: 7344 6973 636f 7264 2c20 5375 6363 6573  sDiscord, Succes
-00001b40: 7353 4d53 2c20 5375 6363 6573 734d 6169  sSMS, SuccessMai
-00001b50: 6c2c 2053 7563 6365 7373 4b61 6b61 6f2c  l, SuccessKakao,
-00001b60: 2053 7563 6365 7373 4c69 6e65 2c20 5375   SuccessLine, Su
-00001b70: 6363 6573 7353 6c61 636b 2c20 5375 6363  ccessSlack, Succ
-00001b80: 6573 7354 6561 6d73 2c20 5375 6363 6573  essTeams, Succes
-00001b90: 7344 6573 6b74 6f70 652c 2053 7563 6365  sDesktope, Succe
-00001ba0: 7373 4265 6570 0d0a 6060 600d 0a2a 4578  ssBeep..```..*Ex
-00001bb0: 616d 706c 652a 0d0a 0d0a 6060 6070 7974  ample*....```pyt
-00001bc0: 686f 6e0d 0a66 726f 6d20 4578 6365 7074  hon..from Except
-00001bd0: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
-00001be0: 5375 6363 6573 7354 656c 6765 7261 6d0d  SuccessTelgeram.
-00001bf0: 0a5f 5445 4c45 4752 414d 5f54 4f4b 454e  ._TELEGRAM_TOKEN
-00001c00: 203d 2022 7878 7878 220d 0a0d 0a74 7279   = "xxxx"....try
-00001c10: 3a0d 0a20 2020 2070 7269 6e74 2831 2f32  :..    print(1/2
-00001c20: 3029 0d0a 2020 2020 5375 6363 6573 7354  0)..    SuccessT
-00001c30: 656c 6765 7261 6d28 292e 5f5f 6361 6c6c  elgeram().__call
-00001c40: 5f5f 2829 2020 2320 7365 6e64 696e 6720  __()  # sending 
-00001c50: 7375 6363 6573 7320 6d65 7373 6167 6520  success message 
-00001c60: 746f 2074 656c 6567 7261 6d0d 0a65 7863  to telegram..exc
-00001c70: 6570 743a 0d0a 2020 2020 7379 732e 6578  ept:..    sys.ex
-00001c80: 6974 2829 0d0a 6060 600d 0a0d 0a21 5b5d  it()..```....![]
-00001c90: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001ca0: 636f 6d2f 6473 6461 6e69 656c 7061 726b  com/dsdanielpark
-00001cb0: 2f45 7863 6570 744e 6f74 6966 6965 722f  /ExceptNotifier/
-00001cc0: 626c 6f62 2f6d 6169 6e2f 6173 7365 7473  blob/main/assets
-00001cd0: 2f69 6d67 732f 6578 332e 706e 6729 0d0a  /imgs/ex3.png)..
-00001ce0: 0d0a 3c42 723e 0d0a 0d0a 2323 2031 2d34  ..<Br>....## 1-4
-00001cf0: 2e20 5365 6e64 605b 6170 704e 616d 655d  . Send`[appName]
-00001d00: 600d 0a50 6c61 6365 2069 7420 616e 7977  `..Place it anyw
-00001d10: 6865 7265 206f 6e20 7468 6520 6c69 6e65  here on the line
-00001d20: 206f 6620 636f 6465 2079 6f75 2077 616e   of code you wan
-00001d30: 742c 2061 6e64 2079 6f75 276c 6c20 6265  t, and you'll be
-00001d40: 206e 6f74 6966 6965 6420 7768 656e 2074   notified when t
-00001d50: 6861 7420 6c69 6e65 206f 6620 636f 6465  hat line of code
-00001d60: 2069 7320 7265 6163 6865 642e 0d0a 6060   is reached...``
-00001d70: 600d 0a53 656e 6443 6869 6d65 2c20 5365  `..SendChime, Se
-00001d80: 6e64 5465 6c65 6772 616d 2c20 5365 6e64  ndTelegram, Send
-00001d90: 4469 7363 6f72 642c 2053 656e 6453 4d53  Discord, SendSMS
-00001da0: 2c20 5365 6e64 4d61 696c 2c20 5365 6e64  , SendMail, Send
-00001db0: 4b61 6b61 6f2c 2053 656e 644c 696e 652c  Kakao, SendLine,
-00001dc0: 2053 656e 6453 6c61 636b 2c20 5365 6e64   SendSlack, Send
-00001dd0: 5465 616d 732c 2053 656e 6444 6573 6b74  Teams, SendDeskt
-00001de0: 6f70 652c 2053 656e 6442 6565 700d 0a60  ope, SendBeep..`
-00001df0: 6060 0d0a 2a45 7861 6d70 6c65 2a0d 0a0d  ``..*Example*...
-00001e00: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
-00001e10: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
-00001e20: 696d 706f 7274 2053 656e 6454 656c 6765  import SendTelge
-00001e30: 7261 6d0d 0a5f 5445 4c45 4752 414d 5f54  ram.._TELEGRAM_T
-00001e40: 4f4b 454e 203d 2022 7878 7878 220d 0a0d  OKEN = "xxxx"...
-00001e50: 0a53 656e 6454 656c 6567 7261 6d28 292e  .SendTelegram().
-00001e60: 5f5f 6361 6c6c 5f5f 2829 2023 2073 656e  __call__() # sen
-00001e70: 6469 6e67 206d 6573 7361 6765 2074 6f20  ding message to 
-00001e80: 7465 6c65 6772 616d 0d0a 0d0a 6e6f 7469  telegram....noti
-00001e90: 203d 2053 656e 6454 656c 6567 7261 6d28   = SendTelegram(
-00001ea0: 290d 0a6e 6f74 6928 2920 2020 2020 2020  )..noti()       
-00001eb0: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00001ec0: 656e 6469 6e67 206d 6573 7361 6765 2074  ending message t
-00001ed0: 6f20 7465 6c65 6772 616d 0d0a 6060 600d  o telegram..```.
-00001ee0: 0a0d 0a21 5b5d 2868 7474 7073 3a2f 2f67  ...![](https://g
-00001ef0: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
-00001f00: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
-00001f10: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
-00001f20: 6173 7365 7473 2f69 6d67 732f 6578 342e  assets/imgs/ex4.
-00001f30: 706e 6729 0d0a 0d0a 0d0a 3c62 723e 3c62  png)......<br><b
-00001f40: 723e 0d0a 0d0a 2320 322e 2046 6561 7475  r>....# 2. Featu
-00001f50: 7265 730d 0a59 6f75 2063 616e 2072 6563  res..You can rec
-00001f60: 6569 7665 2064 6562 7567 6769 6e67 2069  eive debugging i
-00001f70: 6e66 6f72 6d61 7469 6f6e 2066 726f 6d20  nformation from 
-00001f80: 4368 6174 4750 5420 7669 6120 4f70 656e  ChatGPT via Open
-00001f90: 4149 2773 2041 5049 2077 6865 6e20 7573  AI's API when us
-00001fa0: 696e 6720 7468 6520 4578 6365 7074 2073  ing the Except s
-00001fb0: 7461 7465 6d65 6e74 2e20 5468 6520 7379  tatement. The sy
-00001fc0: 6e74 6178 2072 656d 6169 6e73 2074 6865  ntax remains the
-00001fd0: 2073 616d 652c 2062 7574 2079 6f75 276c   same, but you'l
-00001fe0: 6c20 6e65 6564 2074 6f20 636f 6e66 6967  l need to config
-00001ff0: 7572 6520 7468 6573 6520 7477 6f20 7661  ure these two va
-00002000: 7269 6162 6c65 733a 0d0a 605f 4f50 454e  riables:..`_OPEN
-00002010: 5f41 495f 4d4f 4445 4c60 2c60 5f4f 5045  _AI_MODEL`,`_OPE
-00002020: 4e5f 4149 5f41 5049 600d 0a0d 0a0d 0a0d  N_AI_API`.......
-00002030: 0a23 2320 322d 312e 202a 5465 6c65 6772  .## 2-1. *Telegr
-00002040: 616d 204e 6f74 6966 6965 722a 0d0a 0d0a  am Notifier*....
-00002050: 2d20 612e 204f 7065 6e20 796f 7572 2074  - a. Open your t
-00002060: 656c 6567 7261 6d20 6170 7020 616e 6420  elegram app and 
-00002070: 7365 6172 6368 2066 6f72 2042 6f74 4661  search for BotFa
-00002080: 7468 6572 2e20 2841 2062 7569 6c74 2d69  ther. (A built-i
-00002090: 6e20 5465 6c65 6772 616d 2062 6f74 2074  n Telegram bot t
-000020a0: 6861 7420 6865 6c70 7320 7573 6572 7320  hat helps users 
-000020b0: 6372 6561 7465 2063 7573 746f 6d20 5465  create custom Te
-000020c0: 6c65 6772 616d 2062 6f74 7329 203c 6272  legram bots) <br
-000020d0: 3e0d 0a2d 2062 2e20 5479 7065 202f 6e65  >..- b. Type /ne
-000020e0: 7762 6f74 2074 6f20 6372 6561 7465 2061  wbot to create a
-000020f0: 206e 6577 2062 6f74 203c 6272 3e0d 0a2d   new bot <br>..-
-00002100: 2063 2e20 4769 7665 2079 6f75 7220 626f   c. Give your bo
-00002110: 7420 6120 6e61 6d65 2026 2061 2075 7365  t a name & a use
-00002120: 726e 616d 6520 3c62 723e 0d0a 2d20 642e  rname <br>..- d.
-00002130: 2043 6f70 7920 796f 7572 206e 6577 2054   Copy your new T
-00002140: 656c 6567 7261 6d20 626f 74e2 8099 7320  elegram bot...s 
-00002150: 746f 6b65 6e20 3c62 723e 0d0a 0d0a 466f  token <br>....Fo
-00002160: 7220 6d6f 7265 2069 6e66 6f6d 6174 696f  r more infomatio
-00002170: 6e2c 2076 6973 6974 205b 5465 6c65 6772  n, visit [Telegr
-00002180: 616d 2042 6f74 2046 6174 6865 7220 4150  am Bot Father AP
-00002190: 495d 2868 7474 7073 3a2f 2f63 6f72 652e  I](https://core.
-000021a0: 7465 6c65 6772 616d 2e6f 7267 2f62 6f74  telegram.org/bot
-000021b0: 732f 6170 6929 0d0a 3c62 723e 3c62 723e  s/api)..<br><br>
-000021c0: 0d0a 200d 0a23 2323 2061 2e20 5769 7468  .. ..### a. With
-000021d0: 6f75 7420 4f70 656e 4149 2041 5049 0d0a  out OpenAI API..
-000021e0: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-000021f0: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
-00002200: 2069 6d70 6f72 7420 4578 6365 7074 5465   import ExceptTe
-00002210: 6c65 6772 616d 2c20 5375 6363 6573 7354  legram, SuccessT
-00002220: 656c 6567 7261 6d2c 2053 656e 6454 656c  elegram, SendTel
-00002230: 6567 7261 6d0d 0a69 6d70 6f72 7420 7379  egram..import sy
-00002240: 730d 0a73 7973 2e65 7863 6570 7468 6f6f  s..sys.excepthoo
-00002250: 6b20 3d20 4578 6365 7074 5465 6c65 6772  k = ExceptTelegr
-00002260: 616d 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a5f  am.__call__...._
-00002270: 5445 4c45 4752 414d 5f54 4f4b 454e 203d  TELEGRAM_TOKEN =
-00002280: 2022 7878 7878 220d 0a0d 0a74 7279 3a0d   "xxxx"....try:.
-00002290: 0a20 2020 2070 7269 6e74 2831 2f30 2920  .    print(1/0) 
-000022a0: 200d 0a20 2020 2053 7563 6365 7373 5465   ..    SuccessTe
-000022b0: 6c65 6772 616d 2829 2e5f 5f63 616c 6c5f  legram().__call_
-000022c0: 5f28 2920 2331 2e20 7375 6363 6573 7320  _() #1. success 
-000022d0: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-000022e0: 0d0a 0d0a 6578 6365 7074 2045 7863 6570  ....except Excep
-000022f0: 7454 656c 6567 7261 6d20 6173 2065 3a20  tTelegram as e: 
-00002300: 2020 2020 2023 322e 2065 7863 6570 7420       #2. except 
-00002310: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00002320: 2020 0d0a 2020 2020 7379 732e 6578 6974    ..    sys.exit
-00002330: 2829 0d0a 0d0a 5365 6e64 5465 6c65 6772  ()....SendTelegr
-00002340: 616d 2829 2e5f 5f63 616c 6c5f 5f28 2920  am().__call__() 
-00002350: 2020 2020 2020 2023 332e 2063 7573 746f         #3. custo
-00002360: 6d69 7a65 6420 7365 6e64 6572 2020 2020  mized sender    
-00002370: 200d 0a60 6060 0d0a 0d0a 0d0a 215b 5d28   ..```......![](
-00002380: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002390: 6f6d 2f64 7364 616e 6965 6c70 6172 6b2f  om/dsdanielpark/
-000023a0: 4578 6365 7074 4e6f 7469 6669 6572 2f62  ExceptNotifier/b
-000023b0: 6c6f 622f 6d61 696e 2f61 7373 6574 732f  lob/main/assets/
-000023c0: 696d 6773 2f66 6967 3434 2e70 6e67 290d  imgs/fig44.png).
-000023d0: 0a0d 0a0d 0a23 2323 2062 2e20 5769 7468  .....### b. With
-000023e0: 204f 7065 6e41 4920 4150 490d 0a60 6060   OpenAI API..```
-000023f0: 7079 7468 6f6e 0d0a 6672 6f6d 2045 7863  python..from Exc
-00002400: 6570 744e 6f74 6966 6965 7220 696d 706f  eptNotifier impo
-00002410: 7274 2045 7863 6570 7454 656c 6567 7261  rt ExceptTelegra
-00002420: 6d2c 2053 7563 6365 7373 5465 6c65 6772  m, SuccessTelegr
-00002430: 616d 2c20 5365 6e64 5465 6c65 6772 616d  am, SendTelegram
-00002440: 0d0a 696d 706f 7274 2073 7973 0d0a 7379  ..import sys..sy
-00002450: 732e 6578 6365 7074 686f 6f6b 203d 2045  s.excepthook = E
-00002460: 7863 6570 7454 656c 6567 7261 6d2e 5f5f  xceptTelegram.__
-00002470: 6361 6c6c 5f5f 0d0a 0d0a 5f54 454c 4547  call__...._TELEG
-00002480: 5241 4d5f 544f 4b45 4e20 3d20 2278 7878  RAM_TOKEN = "xxx
-00002490: 7822 0d0a 5f4f 5045 4e5f 4149 5f4d 4f44  x".._OPEN_AI_MOD
-000024a0: 454c 3d22 6770 742d 332e 352d 7475 7262  EL="gpt-3.5-turb
-000024b0: 6f22 0d0a 5f4f 5045 4e5f 4149 5f41 5049  o".._OPEN_AI_API
-000024c0: 3d22 736b 2d78 7878 7878 7822 0d0a 0d0a  ="sk-xxxxxx"....
-000024d0: 7472 793a 0d0a 2020 2020 7072 696e 7428  try:..    print(
-000024e0: 312f 3029 2020 0d0a 2020 2020 5375 6363  1/0)  ..    Succ
-000024f0: 6573 7354 656c 6567 7261 6d28 292e 5f5f  essTelegram().__
-00002500: 6361 6c6c 5f5f 2829 2023 312e 2073 7563  call__() #1. suc
-00002510: 6365 7373 2073 656e 6465 7220 2020 2020  cess sender     
-00002520: 2020 2020 200d 0a0d 0a65 7863 6570 7420       ....except 
-00002530: 4578 6365 7074 5465 6c65 6772 616d 2061  ExceptTelegram a
-00002540: 7320 653a 2020 2020 2020 2332 2e20 6578  s e:      #2. ex
-00002550: 6365 7074 2073 656e 6465 7220 2020 2020  cept sender     
-00002560: 2020 2020 2020 200d 0a20 2020 2073 7973         ..    sys
-00002570: 2e65 7869 7428 290d 0a0d 0a53 656e 6454  .exit()....SendT
-00002580: 656c 6567 7261 6d28 292e 5f5f 6361 6c6c  elegram().__call
-00002590: 5f5f 2829 2020 2020 2020 2020 2333 2e20  __()        #3. 
-000025a0: 6375 7374 6f6d 697a 6564 2073 656e 6465  customized sende
-000025b0: 7220 2020 2020 0d0a 0d0a 6060 600d 0a3c  r     ....```..<
-000025c0: 6272 3e0d 0a0d 0a23 2320 322d 322e 202a  br>....## 2-2. *
-000025d0: 4d61 696c 204e 6f74 6966 6965 722a 0d0a  Mail Notifier*..
-000025e0: 496e 2074 6865 2065 7863 6570 7420 7374  In the except st
-000025f0: 6174 656d 656e 742c 2061 6e20 656d 6169  atement, an emai
-00002600: 6c20 6973 2073 656e 7420 616c 6f6e 6720  l is sent along 
-00002610: 7769 7468 2074 6865 2065 7272 6f72 206d  with the error m
-00002620: 6573 7361 6765 2e20 4164 6469 7469 6f6e  essage. Addition
-00002630: 616c 6c79 2c20 796f 7520 6361 6e20 7365  ally, you can se
-00002640: 6e64 2065 6d61 696c 7320 6672 6f6d 2061  nd emails from a
-00002650: 6e79 2064 6573 6972 6564 206c 696e 652e  ny desired line.
-00002660: 203c 6272 3e0d 0a2d 2061 2e20 4c6f 6720   <br>..- a. Log 
-00002670: 696e 2077 6974 6820 7468 6520 7365 6e64  in with the send
-00002680: 6572 2773 2065 6d61 696c 2049 442e 203c  er's email ID. <
-00002690: 6272 3e0d 0a2d 2062 2e20 4f62 7461 696e  br>..- b. Obtain
-000026a0: 2061 6e20 6170 7020 7061 7373 776f 7264   an app password
-000026b0: 2066 6f72 2073 656e 6469 6e67 2047 6f6f   for sending Goo
-000026c0: 676c 6520 4d61 696c 2061 7420 7468 6520  gle Mail at the 
-000026d0: 666f 6c6c 6f77 696e 6720 5b6c 696e 6b5d  following [link]
-000026e0: 2868 7474 7073 3a2f 2f6d 7961 6363 6f75  (https://myaccou
-000026f0: 6e74 2e67 6f6f 676c 652e 636f 6d2f 752f  nt.google.com/u/
-00002700: 332f 6170 7070 6173 7377 6f72 6473 3f75  3/apppasswords?u
-00002710: 746d 5f73 6f75 7263 653d 676f 6f67 6c65  tm_source=google
-00002720: 2d61 6363 6f75 6e74 2675 746d 5f6d 6564  -account&utm_med
-00002730: 6975 6d3d 6d79 6163 636f 756e 7473 6563  ium=myaccountsec
-00002740: 7572 6974 7926 7574 6d5f 6361 6d70 6169  urity&utm_campai
-00002750: 676e 3d74 7376 2d73 6574 7469 6e67 7326  gn=tsv-settings&
-00002760: 7261 7074 3d41 456a 484c 344e 3262 4d52  rapt=AEjHL4N2bMR
-00002770: 574f 3436 5661 4d70 5f6a 5030 367a 514b  WO46VaMp_jP06zQK
-00002780: 3134 4257 4e50 7636 366c 326f 3539 694a  14BWNPv66l2o59iJ
-00002790: 3939 436b 4f38 426a 596e 6d6f 5255 6539  99CkO8BjYnmoRUe9
-000027a0: 6474 5363 686b 6b62 7562 485a 4d55 6865  dtSchkkbubHZMUhe
-000027b0: 766b 416e 7756 4a52 4862 3979 674f 3361  vkAnwVJRHb9ygO3a
-000027c0: 6669 7370 4e6c 7729 206f 7220 5b67 6f6f  fispNlw) or [goo
-000027d0: 676c 6520 646f 6375 6d65 6e74 5d28 6874  gle document](ht
-000027e0: 7470 733a 2f2f 7375 7070 6f72 742e 676f  tps://support.go
-000027f0: 6f67 6c65 2e63 6f6d 2f61 6363 6f75 6e74  ogle.com/account
-00002800: 732f 616e 7377 6572 2f31 3835 3833 333f  s/answer/185833?
-00002810: 686c 3d65 6e29 2e20 0d0a 0d0a 6060 6070  hl=en). ....```p
-00002820: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
-00002830: 730d 0a66 726f 6d20 4578 6365 7074 4e6f  s..from ExceptNo
-00002840: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
-00002850: 6365 7074 4d61 696c 2c20 5375 6363 6573  ceptMail, Succes
-00002860: 734d 6169 6c2c 2053 656e 644d 6169 6c0d  sMail, SendMail.
-00002870: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
-00002880: 3d20 4578 6365 7074 4d61 696c 2e5f 5f63  = ExceptMail.__c
-00002890: 616c 6c5f 5f0d 0a0d 0a23 2044 6566 696e  all__....# Defin
-000028a0: 6520 7468 6520 6e65 7874 2074 776f 2076  e the next two v
-000028b0: 6172 6961 626c 6573 206f 7074 696f 6e61  ariables optiona
-000028c0: 6c6c 7920 7768 656e 2075 7369 6e67 204f  lly when using O
-000028d0: 7065 6e41 4927 7320 4150 492e 0d0a 2320  penAI's API...# 
-000028e0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 3d22  _OPEN_AI_MODEL="
-000028f0: 6770 742d 332e 352d 7475 7262 6f22 2020  gpt-3.5-turbo"  
-00002900: 2020 0d0a 2320 5f4f 5045 4e5f 4149 5f41    ..# _OPEN_AI_A
-00002910: 5049 3d22 736b 2d78 7878 7878 7822 0d0a  PI="sk-xxxxxx"..
-00002920: 5f47 414d 494c 5f52 4543 4950 4945 4e54  _GAMIL_RECIPIENT
-00002930: 5f41 4444 5220 3d20 2778 7878 7878 7878  _ADDR = 'xxxxxxx
-00002940: 4067 6d61 696c 2e63 6f6d 270d 0a5f 474d  @gmail.com'.._GM
-00002950: 4149 4c5f 5345 4e44 4552 5f41 4444 5220  AIL_SENDER_ADDR 
-00002960: 3d20 2779 7979 7979 7940 676d 6169 6c2e  = 'yyyyyy@gmail.
-00002970: 636f 6d27 0d0a 5f47 4d41 494c 5f41 5050  com'.._GMAIL_APP
-00002980: 5f50 4153 5357 4f52 445f 4f46 5f53 454e  _PASSWORD_OF_SEN
-00002990: 4445 5220 3d20 277a 7a7a 7a7a 7a27 0d0a  DER = 'zzzzzz'..
-000029a0: 0d0a 7472 793a 0d0a 2020 2020 6d61 696e  ..try:..    main
-000029b0: 2829 2020 2020 2020 2020 2020 2020 2020  ()              
-000029c0: 2020 2020 2020 2020 2320 596f 7572 2043          # Your C
-000029d0: 6f64 6520 4865 7265 0d0a 2020 2020 5375  ode Here..    Su
-000029e0: 6363 6573 734d 6169 6c28 292e 5f5f 6361  ccessMail().__ca
-000029f0: 6c6c 5f5f 2829 2020 2020 2320 4e6f 2045  ll__()    # No E
-00002a00: 7863 6570 7469 6f6e 202d 3e20 5365 6e64  xception -> Send
-00002a10: 2053 7563 6365 7373 206d 6169 6c2e 0d0a   Success mail...
-00002a20: 6578 6365 7074 2045 7863 6570 744d 6169  except ExceptMai
-00002a30: 6c3a 2020 2020 2020 2020 2020 2020 2020  l:              
-00002a40: 2320 4578 6365 7074 696f 6e20 2d3e 2053  # Exception -> S
-00002a50: 656e 6420 4661 696c 206d 6169 6c2e 0d0a  end Fail mail...
-00002a60: 2020 2020 7061 7373 0d0a 0d0a 5365 6e64      pass....Send
-00002a70: 4d61 696c 2829 2e5f 5f63 616c 6c5f 5f28  Mail().__call__(
-00002a80: 2920 2020 2020 2020 2020 2020 2320 5768  )           # Wh
-00002a90: 656e 2050 726f 6365 7373 2045 6e64 6564  en Process Ended
-00002aa0: 202d 3e20 416e 7920 4c69 6e65 206d 6169   -> Any Line mai
-00002ab0: 6c2e 0d0a 6060 600d 0a0d 0a3c 6465 7461  l...```....<deta
-00002ac0: 696c 733e 0d0a 3c73 756d 6d61 7279 3e20  ils>..<summary> 
-00002ad0: 5365 6520 4578 616d 706c 652e 2e2e 3c2f  See Example...</
-00002ae0: 7375 6d6d 6172 793e 0d0a 0d0a 6060 6070  summary>....```p
-00002af0: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
-00002b00: 730d 0a66 726f 6d20 4578 6365 7074 4e6f  s..from ExceptNo
-00002b10: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
-00002b20: 6365 7074 4d61 696c 2c20 5375 6363 6573  ceptMail, Succes
-00002b30: 734d 6169 6c2c 2053 656e 644d 6169 6c0d  sMail, SendMail.
-00002b40: 0a0d 0a23 2044 6566 696e 6520 7468 6520  ...# Define the 
-00002b50: 6e65 7874 2074 776f 2076 6172 6961 626c  next two variabl
-00002b60: 6573 206f 7074 696f 6e61 6c6c 7920 7768  es optionally wh
-00002b70: 656e 2075 7369 6e67 204f 7065 6e41 4927  en using OpenAI'
-00002b80: 7320 4150 492e 0d0a 2320 5f4f 5045 4e5f  s API...# _OPEN_
-00002b90: 4149 5f4d 4f44 454c 3d22 6770 742d 332e  AI_MODEL="gpt-3.
-00002ba0: 352d 7475 7262 6f22 2020 2020 0d0a 2320  5-turbo"    ..# 
-00002bb0: 5f4f 5045 4e5f 4149 5f41 5049 3d22 736b  _OPEN_AI_API="sk
-00002bc0: 2d78 7878 7878 7822 0d0a 5f47 414d 494c  -xxxxxx".._GAMIL
-00002bd0: 5f52 4543 4950 4945 4e54 5f41 4444 5220  _RECIPIENT_ADDR 
-00002be0: 3d20 2778 7878 7878 7878 4067 6d61 696c  = 'xxxxxxx@gmail
-00002bf0: 2e63 6f6d 270d 0a5f 474d 4149 4c5f 5345  .com'.._GMAIL_SE
-00002c00: 4e44 4552 5f41 4444 5220 3d20 2779 7979  NDER_ADDR = 'yyy
-00002c10: 7979 7940 676d 6169 6c2e 636f 6d27 0d0a  yyy@gmail.com'..
-00002c20: 5f47 4d41 494c 5f41 5050 5f50 4153 5357  _GMAIL_APP_PASSW
-00002c30: 4f52 445f 4f46 5f53 454e 4445 5220 3d20  ORD_OF_SENDER = 
-00002c40: 277a 7a7a 7a7a 7a27 0d0a 0d0a 7379 732e  'zzzzzz'....sys.
-00002c50: 6578 6365 7074 686f 6f6b 203d 2045 7863  excepthook = Exc
-00002c60: 6570 744d 6169 6c2e 5f5f 6361 6c6c 5f5f  eptMail.__call__
-00002c70: 0d0a 0d0a 7472 793a 0d0a 2020 2020 2320  ....try:..    # 
-00002c80: 3032 2e4c 6f63 6174 6520 796f 7572 2063  02.Locate your c
-00002c90: 6f64 650d 0a20 2020 2070 7269 6e74 2831  ode..    print(1
-00002ca0: 2f30 2920 2020 0d0a 2020 2020 5375 6363  /0)   ..    Succ
-00002cb0: 6573 734d 6169 6c28 292e 5f5f 6361 6c6c  essMail().__call
-00002cc0: 5f5f 2829 2020 2023 2053 7563 6365 7373  __()   # Success
-00002cd0: 204d 6169 6c0d 0a0d 0a65 7863 6570 7420   Mail....except 
-00002ce0: 4578 6365 7074 4d61 696c 2061 7320 653a  ExceptMail as e:
-00002cf0: 2020 2020 2020 2020 2320 4578 6365 7074          # Except
-00002d00: 696f 6e20 4d61 696c 2020 2020 2020 200d  ion Mail       .
-00002d10: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
-00002d20: 0a20 2020 2070 7269 6e74 2865 290d 0a0d  .    print(e)...
-00002d30: 0a53 656e 644d 6169 6c28 292e 5f5f 6361  .SendMail().__ca
-00002d40: 6c6c 5f5f 2829 2020 2020 2020 2020 2020  ll__()          
-00002d50: 2320 5075 7420 416e 7920 4c69 6e65 3a20  # Put Any Line: 
-00002d60: 5365 6e64 696e 6720 6d61 696c 0d0a 6060  Sending mail..``
-00002d70: 600d 0a3c 2f64 6574 6169 6c73 3e0d 0a0d  `..</details>...
-00002d80: 0a3c 6465 7461 696c 733e 0d0a 3c73 756d  .<details>..<sum
-00002d90: 6d61 7279 3e20 536e 6970 7065 7420 666f  mary> Snippet fo
-00002da0: 7220 5079 7468 6f6e 2064 6576 656c 6f70  r Python develop
-00002db0: 6572 732e 2e2e 3c2f 7375 6d6d 6172 793e  ers...</summary>
-00002dc0: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a69  ....```python..i
-00002dd0: 6d70 6f72 7420 7379 730d 0a66 726f 6d20  mport sys..from 
-00002de0: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
-00002df0: 6d70 6f72 7420 4578 6365 7074 4d61 696c  mport ExceptMail
-00002e00: 2c20 5375 6363 6573 734d 6169 6c2c 2053  , SuccessMail, S
-00002e10: 656e 644d 6169 6c0d 0a73 7973 2e65 7863  endMail..sys.exc
-00002e20: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
-00002e30: 4d61 696c 2e5f 5f63 616c 6c5f 5f0d 0a0d  Mail.__call__...
-00002e40: 0a23 2044 6566 696e 6520 7468 6520 6e65  .# Define the ne
-00002e50: 7874 2074 776f 2076 6172 6961 626c 6573  xt two variables
-00002e60: 206f 7074 696f 6e61 6c6c 7920 7768 656e   optionally when
-00002e70: 2075 7369 6e67 204f 7065 6e41 4927 7320   using OpenAI's 
-00002e80: 4150 492e 0d0a 2320 5f4f 5045 4e5f 4149  API...# _OPEN_AI
-00002e90: 5f4d 4f44 454c 3d22 6770 742d 332e 352d  _MODEL="gpt-3.5-
-00002ea0: 7475 7262 6f22 2020 2020 0d0a 2320 5f4f  turbo"    ..# _O
-00002eb0: 5045 4e5f 4149 5f41 5049 3d22 736b 2d78  PEN_AI_API="sk-x
-00002ec0: 7878 7878 7822 0d0a 5f47 414d 494c 5f52  xxxxx".._GAMIL_R
-00002ed0: 4543 4950 4945 4e54 5f41 4444 5220 3d20  ECIPIENT_ADDR = 
-00002ee0: 2778 7878 7878 7878 4067 6d61 696c 2e63  'xxxxxxx@gmail.c
-00002ef0: 6f6d 270d 0a5f 474d 4149 4c5f 5345 4e44  om'.._GMAIL_SEND
-00002f00: 4552 5f41 4444 5220 3d20 2779 7979 7979  ER_ADDR = 'yyyyy
-00002f10: 7940 676d 6169 6c2e 636f 6d27 0d0a 5f47  y@gmail.com'.._G
-00002f20: 4d41 494c 5f41 5050 5f50 4153 5357 4f52  MAIL_APP_PASSWOR
-00002f30: 445f 4f46 5f53 454e 4445 5220 3d20 277a  D_OF_SENDER = 'z
-00002f40: 7a7a 7a7a 7a27 0d0a 0d0a 7472 793a 0d0a  zzzzz'....try:..
-00002f50: 2020 2020 2779 6f75 7220 636f 6465 270d      'your code'.
-00002f60: 0a20 2020 2053 7563 6365 7373 4d61 696c  .    SuccessMail
-00002f70: 2829 2e5f 5f63 616c 6c5f 5f28 290d 0a65  ().__call__()..e
-00002f80: 7863 6570 7420 4578 6365 7074 4d61 696c  xcept ExceptMail
-00002f90: 3a0d 0a20 2020 2070 6173 730d 0a0d 0a53  :..    pass....S
-00002fa0: 656e 644d 6169 6c28 292e 5f5f 6361 6c6c  endMail().__call
-00002fb0: 5f5f 2829 200d 0a60 6060 0d0a 3c2f 6465  __() ..```..</de
-00002fc0: 7461 696c 733e 0d0a 0d0a 3c62 723e 0d0a  tails>....<br>..
-00002fd0: 0d0a 2323 2032 2d33 2e20 2a44 6973 636f  ..## 2-3. *Disco
-00002fe0: 7264 204e 6f74 6966 6965 722a 0d0a 2d20  rd Notifier*..- 
-00002ff0: 612e 2053 656c 6563 7420 7468 6520 6368  a. Select the ch
-00003000: 616e 6e65 6c20 746f 2072 6563 6569 7665  annel to receive
-00003010: 206e 6f74 6966 6963 6174 696f 6e73 2e0d   notifications..
-00003020: 0a2d 2062 2e20 436c 6963 6b20 2245 6469  .- b. Click "Edi
-00003030: 7420 4368 616e 6e65 6c22 2069 6e20 7468  t Channel" in th
-00003040: 6520 7570 7065 7220 7269 6768 7420 636f  e upper right co
-00003050: 726e 6572 206f 6620 7468 6520 6368 6174  rner of the chat
-00003060: 2077 696e 646f 772e 0d0a 2d20 632e 2043   window...- c. C
-00003070: 6c69 636b 2049 6e74 6567 7261 7469 6f6e  lick Integration
-00003080: 7320 2d20 5765 6268 6f6f 6b20 2d20 4e65  s - Webhook - Ne
-00003090: 7720 5765 6268 6f6f 6b2e 0d0a 2d20 642e  w Webhook...- d.
-000030a0: 2054 6865 6e20 636c 6963 6b20 436f 7079   Then click Copy
-000030b0: 2057 6562 686f 6f6b 2e0d 0a0d 0a60 6060   Webhook.....```
-000030c0: 7079 7468 6f6e 0d0a 696d 706f 7274 2073  python..import s
-000030d0: 7973 0d0a 6672 6f6d 2045 7863 6570 744e  ys..from ExceptN
-000030e0: 6f74 6966 6965 7220 696d 706f 7274 2045  otifier import E
-000030f0: 7863 6570 7444 6973 636f 7264 2c20 5375  xceptDiscord, Su
-00003100: 6363 6573 7344 6973 636f 7264 2c20 5365  ccessDiscord, Se
-00003110: 6e64 4469 7363 6f72 640d 0a73 7973 2e65  ndDiscord..sys.e
-00003120: 7863 6570 7468 6f6f 6b20 3d20 4578 6365  xcepthook = Exce
-00003130: 7074 4469 7363 6f72 642e 5f5f 6361 6c6c  ptDiscord.__call
-00003140: 5f5f 0d0a 0d0a 2320 4465 6669 6e65 2074  __....# Define t
-00003150: 6865 206e 6578 7420 7477 6f20 7661 7269  he next two vari
-00003160: 6162 6c65 7320 6f70 7469 6f6e 616c 6c79  ables optionally
-00003170: 2077 6865 6e20 7573 696e 6720 4f70 656e   when using Open
-00003180: 4149 2773 2041 5049 2e0d 0a23 205f 4f50  AI's API...# _OP
-00003190: 454e 5f41 495f 4d4f 4445 4c3d 2267 7074  EN_AI_MODEL="gpt
-000031a0: 2d33 2e35 2d74 7572 626f 2220 2020 200d  -3.5-turbo"    .
-000031b0: 0a23 205f 4f50 454e 5f41 495f 4150 493d  .# _OPEN_AI_API=
-000031c0: 2273 6b2d 7878 7878 7878 220d 0a5f 4449  "sk-xxxxxx".._DI
-000031d0: 5343 4f52 445f 5745 4248 4f4f 4b5f 5552  SCORD_WEBHOOK_UR
-000031e0: 4c20 3d20 2278 7878 7878 7878 7878 7878  L = "xxxxxxxxxxx
-000031f0: 7878 7878 7878 220d 0a0d 0a0d 0a74 7279  xxxxxx"......try
-00003200: 3a0d 0a20 2020 2070 7269 6e74 2831 2f32  :..    print(1/2
-00003210: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
-00003220: 7344 6973 636f 7264 2829 2e5f 5f63 616c  sDiscord().__cal
-00003230: 6c5f 5f28 2920 2331 2073 7563 6365 7373  l__() #1 success
-00003240: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
-00003250: 200d 0a65 7863 6570 7420 4578 6365 7074   ..except Except
-00003260: 4469 7363 6f72 6420 6173 2065 3a20 2020  Discord as e:   
-00003270: 2020 2023 3220 6578 6365 7074 2073 656e     #2 except sen
-00003280: 6465 7220 2020 2020 2020 2020 2020 200d  der            .
-00003290: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
-000032a0: 0a0d 0a53 656e 6444 6973 636f 7264 2829  ...SendDiscord()
-000032b0: 2e5f 5f63 616c 6c5f 5f28 2920 2020 2020  .__call__()     
-000032c0: 2020 2023 3320 6375 7374 6f6d 697a 6564     #3 customized
-000032d0: 2073 656e 6465 7220 2020 2020 2020 0d0a   sender       ..
-000032e0: 6060 600d 0a0d 0a3c 6272 3e0d 0a0d 0a23  ```....<br>....#
-000032f0: 2320 322d 342e 202a 4368 696d 6520 4e6f  # 2-4. *Chime No
-00003300: 7469 6669 6572 2a0d 0a2d 2061 2e20 5365  tifier*..- a. Se
-00003310: 6c65 6374 2074 6865 2043 6861 7420 726f  lect the Chat ro
-00003320: 6f6d 2074 6f20 7265 6365 6976 6520 6e6f  om to receive no
-00003330: 7469 6669 6361 7469 6f6e 732e 0d0a 2d20  tifications...- 
-00003340: 622e 2043 6c69 636b 2022 526f 6f6d 2053  b. Click "Room S
-00003350: 6574 7469 6e67 2220 696e 2074 6865 2075  etting" in the u
-00003360: 7070 6572 2072 6967 6874 2063 6f72 6e65  pper right corne
-00003370: 722e 0d0a 2d20 632e 2043 6c69 636b 2022  r...- c. Click "
-00003380: 4d61 6e61 6765 2057 6562 686f 6f6b 2061  Manage Webhook a
-00003390: 6e64 2062 6f74 2e22 0d0a 2d20 642e 2043  nd bot."..- d. C
-000033a0: 7265 6174 6520 4164 6420 5765 6268 6f6f  reate Add Webhoo
-000033b0: 6b2c 2073 6574 2069 7420 7570 2c20 7468  k, set it up, th
-000033c0: 656e 2063 6c69 636b 2043 6f70 7920 5765  en click Copy We
-000033d0: 6268 6f6f 6b2e 0d0a 6060 6070 7974 686f  bhook...```pytho
-000033e0: 6e0d 0a69 6d70 6f72 7420 7379 730d 0a66  n..import sys..f
-000033f0: 726f 6d20 4578 6365 7074 4e6f 7469 6669  rom ExceptNotifi
-00003400: 6572 2069 6d70 6f72 7420 5375 6363 6573  er import Succes
-00003410: 7343 6869 6d65 2c20 4578 6365 7074 4368  sChime, ExceptCh
-00003420: 696d 652c 2053 656e 6443 6869 6d65 0d0a  ime, SendChime..
-00003430: 7379 732e 6578 6365 7074 686f 6f6b 203d  sys.excepthook =
-00003440: 2045 7863 6570 7443 6869 6d65 2e5f 5f63   ExceptChime.__c
-00003450: 616c 6c5f 5f0d 0a0d 0a23 2044 6566 696e  all__....# Defin
-00003460: 6520 7468 6520 6e65 7874 2074 776f 2076  e the next two v
-00003470: 6172 6961 626c 6573 206f 7074 696f 6e61  ariables optiona
-00003480: 6c6c 7920 7768 656e 2075 7369 6e67 204f  lly when using O
-00003490: 7065 6e41 4927 7320 4150 492e 0d0a 2320  penAI's API...# 
-000034a0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 3d22  _OPEN_AI_MODEL="
-000034b0: 6770 742d 332e 352d 7475 7262 6f22 2020  gpt-3.5-turbo"  
-000034c0: 2020 0d0a 2320 5f4f 5045 4e5f 4149 5f41    ..# _OPEN_AI_A
-000034d0: 5049 3d22 736b 2d78 7878 7878 7822 0d0a  PI="sk-xxxxxx"..
-000034e0: 5f43 4849 4d45 5f57 4542 484f 4f4b 5f55  _CHIME_WEBHOOK_U
-000034f0: 524c 203d 2022 7878 7878 7878 7878 7878  RL = "xxxxxxxxxx
-00003500: 7878 7878 7878 7878 220d 0a0d 0a0d 0a74  xxxxxxxx"......t
-00003510: 7279 3a0d 0a20 2020 2070 7269 6e74 2831  ry:..    print(1
-00003520: 2f30 2920 200d 0a20 2020 2053 7563 6365  /0)  ..    Succe
-00003530: 7373 4368 696d 6528 292e 5f5f 6361 6c6c  ssChime().__call
-00003540: 5f5f 2829 2023 3120 7375 6363 6573 7320  __() #1 success 
-00003550: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
-00003560: 0d0a 6578 6365 7074 2045 7863 6570 7443  ..except ExceptC
-00003570: 6869 6d65 2061 7320 653a 2020 2020 2020  hime as e:      
-00003580: 2332 2065 7863 6570 7420 7365 6e64 6572  #2 except sender
-00003590: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-000035a0: 2020 7379 732e 6578 6974 2829 0d0a 0d0a    sys.exit()....
-000035b0: 5365 6e64 4368 696d 6528 292e 5f5f 6361  SendChime().__ca
-000035c0: 6c6c 5f5f 2829 2020 2020 2020 2020 2333  ll__()        #3
-000035d0: 2063 7573 746f 6d69 7a65 6420 7365 6e64   customized send
-000035e0: 6572 2020 2020 2020 200d 0a60 6060 0d0a  er       ..```..
-000035f0: 3c62 723e 0d0a 0d0a 2323 2032 2d35 2e20  <br>....## 2-5. 
-00003600: 2a53 6c61 636b 204e 6f74 6966 6965 722a  *Slack Notifier*
-00003610: 0d0a 2d20 612e 2076 6973 6974 2068 7474  ..- a. visit htt
-00003620: 7073 3a2f 2f61 7069 2e73 6c61 636b 2e63  ps://api.slack.c
-00003630: 6f6d 2f0d 0a2d 2062 2e20 6043 7265 6174  om/..- b. `Creat
-00003640: 6520 616e 2061 7070 6020 2d20 6046 726f  e an app` - `Fro
-00003650: 6d20 7363 7261 7463 6860 202d 2060 4372  m scratch` - `Cr
-00003660: 6561 7465 2041 7070 600d 0a2d 2063 2e20  eate App`..- c. 
-00003670: 4164 6420 7765 6268 6f6f 6b3a 2043 6c69  Add webhook: Cli
-00003680: 636b 2060 496e 636f 6d69 6e67 2057 6562  ck `Incoming Web
-00003690: 686f 6f6b 7360 202d 2041 6374 6976 6174  hooks` - Activat
-000036a0: 6520 496e 636f 6d6d 696e 6720 604f 6e60  e Incomming `On`
-000036b0: 202d 2041 6464 204e 6577 2057 6562 686f   - Add New Webho
-000036c0: 6f6b 2074 6f20 576f 726b 7370 6163 650d  ok to Workspace.
-000036d0: 0a2d 2064 2e20 436f 7079 2060 5765 6268  .- d. Copy `Webh
-000036e0: 6f6f 6b20 5552 4c60 0d0a 0d0a 6060 6070  ook URL`....```p
-000036f0: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
-00003700: 730d 0a66 726f 6d20 4578 6365 7074 4e6f  s..from ExceptNo
-00003710: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
-00003720: 6365 7074 536c 6163 6b2c 2053 7563 6365  ceptSlack, Succe
-00003730: 7373 536c 6361 6b2c 2053 656e 6453 6c61  ssSlcak, SendSla
-00003740: 636b 0d0a 7379 732e 6578 6365 7074 686f  ck..sys.exceptho
-00003750: 6f6b 203d 2045 7863 6570 7453 6c61 636b  ok = ExceptSlack
-00003760: 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23 2044  .__call__....# D
-00003770: 6566 696e 6520 7468 6520 6e65 7874 2074  efine the next t
-00003780: 776f 2076 6172 6961 626c 6573 206f 7074  wo variables opt
-00003790: 696f 6e61 6c6c 7920 7768 656e 2075 7369  ionally when usi
-000037a0: 6e67 204f 7065 6e41 4927 7320 4150 492e  ng OpenAI's API.
-000037b0: 0d0a 2320 5f4f 5045 4e5f 4149 5f4d 4f44  ..# _OPEN_AI_MOD
-000037c0: 454c 3d22 6770 742d 332e 352d 7475 7262  EL="gpt-3.5-turb
-000037d0: 6f22 2020 2020 0d0a 2320 5f4f 5045 4e5f  o"    ..# _OPEN_
-000037e0: 4149 5f41 5049 3d22 736b 2d78 7878 7878  AI_API="sk-xxxxx
-000037f0: 7822 0d0a 5f53 4c41 434b 5f57 4542 484f  x".._SLACK_WEBHO
-00003800: 4f4b 5f55 524c 203d 2027 6874 7470 733a  OK_URL = 'https:
-00003810: 2f2f 686f 6f6b 732e 736c 6163 6b2e 636f  //hooks.slack.co
-00003820: 6d2f 7365 7276 6963 6573 2f78 7878 7878  m/services/xxxxx
-00003830: 7878 7878 7878 7878 7878 7878 7878 270d  xxxxxxxxxxxxxx'.
-00003840: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
-00003850: 6e74 2831 2f30 2920 200d 0a20 2020 2053  nt(1/0)  ..    S
-00003860: 7563 6365 7373 536c 6361 6b28 292e 5f5f  uccessSlcak().__
-00003870: 6361 6c6c 5f5f 2829 2023 3120 7375 6363  call__() #1 succ
-00003880: 6573 7320 7365 6e64 6572 2020 2020 2020  ess sender      
-00003890: 2020 2020 0d0a 6578 6365 7074 2045 7863      ..except Exc
-000038a0: 6570 7453 6c61 636b 2061 7320 653a 2020  eptSlack as e:  
-000038b0: 2020 2020 2332 2065 7863 6570 7420 7365      #2 except se
-000038c0: 6e64 6572 2020 2020 2020 2020 2020 2020  nder            
-000038d0: 0d0a 2020 2020 7379 732e 6578 6974 2829  ..    sys.exit()
-000038e0: 0d0a 0d0a 5365 6e64 536c 6163 6b28 292e  ....SendSlack().
-000038f0: 5f5f 6361 6c6c 5f5f 2829 2020 2020 2020  __call__()      
-00003900: 2020 2333 2063 7573 746f 6d69 7a65 6420    #3 customized 
-00003910: 7365 6e64 6572 2020 2020 200d 0a60 6060  sender     ..```
-00003920: 0d0a 3c42 723e 0d0a 0d0a 2323 2032 2d36  ..<Br>....## 2-6
-00003930: 2e20 2a4c 696e 6520 4e6f 7469 6669 6572  . *Line Notifier
-00003940: 2a0d 0a2d 2061 2e20 5265 6769 7374 6572  *..- a. Register
-00003950: 205b 6874 7470 733a 2f2f 6e6f 7469 6679   [https://notify
-00003960: 2d62 6f74 2e6c 696e 652e 6d65 2f5d 2868  -bot.line.me/](h
-00003970: 7474 7073 3a2f 2f6e 6f74 6966 792d 626f  ttps://notify-bo
-00003980: 742e 6c69 6e65 2e6d 652f 292e 0d0a 2d20  t.line.me/)...- 
-00003990: 622e 2047 6f20 746f 206d 7970 6167 6520  b. Go to mypage 
-000039a0: 5b68 7474 7073 3a2f 2f6e 6f74 6966 792d  [https://notify-
-000039b0: 626f 742e 6c69 6e65 2e6d 652f 6d79 2f5d  bot.line.me/my/]
-000039c0: 2868 7474 7073 3a2f 2f6e 6f74 6966 792d  (https://notify-
-000039d0: 626f 742e 6c69 6e65 2e6d 652f 6d79 2f29  bot.line.me/my/)
-000039e0: 2e0d 0a2d 2063 2e20 436c 6963 6b20 6047  ...- c. Click `G
-000039f0: 656e 6572 6174 6520 546f 6b65 6e60 2c20  enerate Token`, 
-00003a00: 656e 7465 7220 5365 7276 6963 6520 4e61  enter Service Na
-00003a10: 6d65 2061 6e64 2063 6c69 636b 2060 312d  me and click `1-
-00003a20: 6f6e 2d31 2063 6861 7420 7769 7468 204c  on-1 chat with L
-00003a30: 494e 4560 2028 616e 7974 6869 6e67 2079  INE` (anything y
-00003a40: 6f75 206c 696b 6529 2e0d 0a2d 2064 2e20  ou like)...- d. 
-00003a50: 436f 7079 2054 6f6b 656e 2e0d 0a0d 0a60  Copy Token.....`
-00003a60: 6060 7079 7468 6f6e 0d0a 696d 706f 7274  ``python..import
-00003a70: 2073 7973 0d0a 6672 6f6d 2045 7863 6570   sys..from Excep
-00003a80: 744e 6f74 6966 6965 7220 696d 706f 7274  tNotifier import
-00003a90: 2045 7863 6570 744c 696e 652c 2053 7563   ExceptLine, Suc
-00003aa0: 6365 7373 4c69 6e65 2c20 5365 6e64 4c69  cessLine, SendLi
-00003ab0: 6e65 0d0a 7379 732e 6578 6365 7074 686f  ne..sys.exceptho
-00003ac0: 6f6b 203d 2045 7863 6570 744c 696e 652e  ok = ExceptLine.
-00003ad0: 5f5f 6361 6c6c 5f5f 0d0a 0d0a 2320 4465  __call__....# De
-00003ae0: 6669 6e65 2074 6865 206e 6578 7420 7477  fine the next tw
-00003af0: 6f20 7661 7269 6162 6c65 7320 6f70 7469  o variables opti
-00003b00: 6f6e 616c 6c79 2077 6865 6e20 7573 696e  onally when usin
-00003b10: 6720 4f70 656e 4149 2773 2041 5049 2e0d  g OpenAI's API..
-00003b20: 0a23 205f 4f50 454e 5f41 495f 4d4f 4445  .# _OPEN_AI_MODE
-00003b30: 4c3d 2267 7074 2d33 2e35 2d74 7572 626f  L="gpt-3.5-turbo
-00003b40: 2220 2020 200d 0a23 205f 4f50 454e 5f41  "    ..# _OPEN_A
-00003b50: 495f 4150 493d 2273 6b2d 7878 7878 7878  I_API="sk-xxxxxx
-00003b60: 220d 0a5f 4c49 4e45 5f4e 4f54 4946 595f  ".._LINE_NOTIFY_
-00003b70: 4150 495f 544f 4b45 4e20 3d20 2778 7878  API_TOKEN = 'xxx
-00003b80: 7878 7878 7878 7878 270d 0a0d 0a74 7279  xxxxxxxx'....try
-00003b90: 3a0d 0a20 2020 2070 7269 6e74 2831 2f32  :..    print(1/2
-00003ba0: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
-00003bb0: 734c 696e 6528 292e 5f5f 6361 6c6c 5f5f  sLine().__call__
-00003bc0: 2829 2023 3120 7375 6363 6573 7320 7365  () #1 success se
-00003bd0: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
-00003be0: 6578 6365 7074 2045 7863 6570 744c 696e  except ExceptLin
-00003bf0: 6520 6173 2065 3a20 2020 2020 2023 3220  e as e:      #2 
-00003c00: 6578 6365 7074 2073 656e 6465 7220 2020  except sender   
-00003c10: 2020 2020 2020 2020 200d 0a20 2020 2073           ..    s
-00003c20: 7973 2e65 7869 7428 290d 0a0d 0a53 656e  ys.exit()....Sen
-00003c30: 644c 696e 6528 292e 5f5f 6361 6c6c 5f5f  dLine().__call__
-00003c40: 2829 2020 2020 2020 2020 2333 2063 7573  ()        #3 cus
-00003c50: 746f 6d69 7a65 6420 7365 6e64 6572 2020  tomized sender  
-00003c60: 2020 2020 2020 2020 0d0a 6060 600d 0a0d          ..```...
-00003c70: 0a3c 4272 3e0d 0a0d 0a23 2320 322d 372e  .<Br>....## 2-7.
-00003c80: 202a 534d 5320 4e6f 7469 6669 6572 2a0d   *SMS Notifier*.
-00003c90: 0a2d 2061 2e20 5369 676e 2075 7020 666f  .- a. Sign up fo
-00003ca0: 7220 5477 696c 696f 2e20 5b68 7474 7073  r Twilio. [https
-00003cb0: 3a2f 2f77 7777 2e74 7769 6c69 6f2e 636f  ://www.twilio.co
-00003cc0: 6d2f 656e 2d75 735d 2868 7474 7073 3a2f  m/en-us](https:/
-00003cd0: 2f77 7777 2e74 7769 6c69 6f2e 636f 6d2f  /www.twilio.com/
-00003ce0: 656e 2d75 7329 2e0d 0a2d 2062 2e20 436c  en-us)...- b. Cl
-00003cf0: 6963 6b20 436f 6e73 6f6c 6520 696e 2074  ick Console in t
-00003d00: 6865 2075 7070 6572 2072 6967 6874 2063  he upper right c
-00003d10: 6f72 6e65 722e 0d0a 2d20 632e 2043 6f70  orner...- c. Cop
-00003d20: 7920 7468 6520 7661 7269 6162 6c65 7320  y the variables 
-00003d30: 7072 6f76 6964 6564 2069 6e20 7468 6520  provided in the 
-00003d40: 636f 6e73 6f6c 652e 0d0a 0d0a 6060 6070  console.....```p
-00003d50: 7974 686f 6e0d 0a69 6d70 6f72 7420 7379  ython..import sy
-00003d60: 730d 0a66 726f 6d20 4578 6365 7074 4e6f  s..from ExceptNo
-00003d70: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
-00003d80: 6365 7074 534d 532c 2053 7563 6365 7373  ceptSMS, Success
-00003d90: 534d 532c 2053 656e 6453 4d53 0d0a 7379  SMS, SendSMS..sy
-00003da0: 732e 6578 6365 7074 686f 6f6b 203d 2045  s.excepthook = E
-00003db0: 7863 6570 7453 4d53 2e5f 5f63 616c 6c5f  xceptSMS.__call_
-00003dc0: 5f0d 0a0d 0a23 2044 6566 696e 6520 7468  _....# Define th
-00003dd0: 6520 6e65 7874 2074 776f 2076 6172 6961  e next two varia
-00003de0: 626c 6573 206f 7074 696f 6e61 6c6c 7920  bles optionally 
-00003df0: 7768 656e 2075 7369 6e67 204f 7065 6e41  when using OpenA
-00003e00: 4927 7320 4150 492e 0d0a 2320 5f4f 5045  I's API...# _OPE
-00003e10: 4e5f 4149 5f4d 4f44 454c 3d22 6770 742d  N_AI_MODEL="gpt-
-00003e20: 332e 352d 7475 7262 6f22 2020 2020 0d0a  3.5-turbo"    ..
-00003e30: 2320 5f4f 5045 4e5f 4149 5f41 5049 3d22  # _OPEN_AI_API="
-00003e40: 736b 2d78 7878 7878 7822 0d0a 5f54 5749  sk-xxxxxx".._TWI
-00003e50: 4c49 4f5f 5349 4420 3d20 2778 7878 7827  LIO_SID = 'xxxx'
-00003e60: 0d0a 5f54 5749 4c49 4f5f 544f 4b45 4e20  .._TWILIO_TOKEN 
-00003e70: 3d20 2779 7979 7979 7927 0d0a 5f52 4543  = 'yyyyyy'.._REC
-00003e80: 4950 4945 4e54 5f50 484f 4e45 5f4e 554d  IPIENT_PHONE_NUM
-00003e90: 4245 523d 222b 6161 6161 6161 222c 0d0a  BER="+aaaaaa",..
-00003ea0: 5f53 454e 4445 525f 5048 4f4e 455f 4e55  _SENDER_PHONE_NU
-00003eb0: 4d42 4552 3d22 2b62 6262 6262 6222 2c20  MBER="+bbbbbb", 
-00003ec0: 200d 0a0d 0a74 7279 3a0d 0a20 2020 2070   ....try:..    p
-00003ed0: 7269 6e74 2831 2f31 3029 2020 0d0a 2020  rint(1/10)  ..  
-00003ee0: 2020 5375 6363 6573 7353 4d53 2829 2e5f    SuccessSMS()._
-00003ef0: 5f63 616c 6c5f 5f28 2920 2331 2073 7563  _call__() #1 suc
-00003f00: 6365 7373 2073 656e 6465 7220 2020 2020  cess sender     
-00003f10: 2020 2020 200d 0a65 7863 6570 7420 4578       ..except Ex
-00003f20: 6365 7074 534d 5320 6173 2065 3a20 2020  ceptSMS as e:   
-00003f30: 2020 2023 3220 6578 6365 7074 2073 656e     #2 except sen
-00003f40: 6465 720d 0a20 2020 2073 7973 2e65 7869  der..    sys.exi
-00003f50: 7428 290d 0a0d 0a53 656e 6453 4d53 2829  t()....SendSMS()
-00003f60: 2e5f 5f63 616c 6c5f 5f28 2920 2020 2020  .__call__()     
-00003f70: 2020 2023 3320 6375 7374 6f6d 697a 6564     #3 customized
-00003f80: 2073 656e 6465 7220 2020 2020 2020 200d   sender        .
-00003f90: 0a60 6060 0d0a 3c42 723e 0d0a 0d0a 2323  .```..<Br>....##
-00003fa0: 2032 2d38 2e20 2a54 6561 6d73 204e 6f74   2-8. *Teams Not
-00003fb0: 6966 6965 722a 0d0a 2d20 612e 2043 7265  ifier*..- a. Cre
-00003fc0: 6174 6520 7468 6520 6368 616e 6e65 6c20  ate the channel 
-00003fd0: 7468 6174 2079 6f75 2077 616e 7420 746f  that you want to
-00003fe0: 206e 6f74 6966 792e 0d0a 2d20 622e 2041   notify...- b. A
-00003ff0: 7070 202d 2053 6561 7263 683a 2077 6562  pp - Search: web
-00004000: 686f 6f6b 202d 2049 6e63 6f6d 696e 6720  hook - Incoming 
-00004010: 5765 6268 6f6f 6b20 5b68 7474 7073 3a2f  Webhook [https:/
-00004020: 2f74 6561 6d73 2e6d 6963 726f 736f 6674  /teams.microsoft
-00004030: 2e63 6f6d 2f6c 2f61 7070 2f32 3033 6131  .com/l/app/203a1
-00004040: 6532 632d 3236 6363 2d34 3763 612d 3833  e2c-26cc-47ca-83
-00004050: 6165 2d62 6539 3866 3936 3062 3662 323f  ae-be98f960b6b2?
-00004060: 736f 7572 6365 3d61 7070 2d64 6574 6169  source=app-detai
-00004070: 6c73 2d64 6961 6c6f 675d 2868 7474 7073  ls-dialog](https
-00004080: 3a2f 2f74 6561 6d73 2e6d 6963 726f 736f  ://teams.microso
-00004090: 6674 2e63 6f6d 2f6c 2f61 7070 2f32 3033  ft.com/l/app/203
-000040a0: 6131 6532 632d 3236 6363 2d34 3763 612d  a1e2c-26cc-47ca-
-000040b0: 3833 6165 2d62 6539 3866 3936 3062 3662  83ae-be98f960b6b
-000040c0: 323f 736f 7572 6365 3d61 7070 2d64 6574  2?source=app-det
-000040d0: 6169 6c73 2d64 6961 6c6f 6729 2e0d 0a2d  ails-dialog)...-
-000040e0: 2063 2e20 436c 6963 6b20 6052 6571 7565   c. Click `Reque
-000040f0: 7374 2041 7070 726f 7661 6c60 203c 6272  st Approval` <br
-00004100: 3e0d 0a41 6674 6572 2079 6f75 2063 616e  >..After you can
-00004110: 2075 7365 2077 6562 686f 6f6b 2069 6e63   use webhook inc
-00004120: 6f6d 6d69 6e67 2e20 5072 6f63 6565 6420  omming. Proceed 
-00004130: 746f 206e 6578 7420 7374 6570 732e 0d0a  to next steps...
-00004140: 4d69 6372 6f73 6f66 7420 5465 616d 7320  Microsoft Teams 
-00004150: 616c 6c6f 7773 206c 696d 6974 6564 2061  allows limited a
-00004160: 7070 6c69 6361 7469 6f6e 2061 6363 6573  pplication acces
-00004170: 7320 7065 7220 6f72 6761 6e69 7a61 7469  s per organizati
-00004180: 6f6e 2c20 736f 2069 7420 6361 6e20 6f6e  on, so it can on
-00004190: 6c79 2062 6520 7573 6564 2069 6620 7468  ly be used if th
-000041a0: 6520 7765 6268 6f6f 6b20 696e 636f 6d69  e webhook incomi
-000041b0: 6e67 2061 7070 6c69 6361 7469 6f6e 2069  ng application i
-000041c0: 7320 6176 6169 6c61 626c 652e 0d0a 2d20  s available...- 
-000041d0: 632e 2047 6f20 746f 2074 6865 2074 6561  c. Go to the tea
-000041e0: 6d20 6368 616e 6e65 6c20 746f 2072 6563  m channel to rec
-000041f0: 6569 7665 206e 6f74 6966 6963 6174 696f  eive notificatio
-00004200: 6e73 2c20 616e 6420 636c 6963 6b20 6043  ns, and click `C
-00004210: 6f6e 6e65 6374 6f72 7360 2069 6e20 5365  onnectors` in Se
-00004220: 7474 696e 6773 2e0d 0a2d 2064 2e20 6043  ttings...- d. `C
-00004230: 6f6e 6e65 6374 6f72 7360 2041 6674 6572  onnectors` After
-00004240: 2063 6f6e 6669 6775 7269 6e67 2077 6562   configuring web
-00004250: 686f 6f6b 2069 6e63 6f6d 696e 6720 696e  hook incoming in
-00004260: 2043 6f6e 6e65 6374 6f72 2c20 636f 7079   Connector, copy
-00004270: 2074 6865 2077 6562 686f 6f6b 2055 524c   the webhook URL
-00004280: 2e0d 0a0d 0a60 6060 7079 7468 6f6e 0d0a  .....```python..
-00004290: 696d 706f 7274 2073 7973 0d0a 6672 6f6d  import sys..from
-000042a0: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
-000042b0: 696d 706f 7274 2045 7863 6570 7454 6561  import ExceptTea
-000042c0: 6d73 2c20 5375 6363 6573 7354 6561 6d73  ms, SuccessTeams
-000042d0: 2c20 5365 6e64 5465 616d 730d 0a73 7973  , SendTeams..sys
-000042e0: 2e65 7863 6570 7468 6f6f 6b20 3d20 4578  .excepthook = Ex
-000042f0: 6365 7074 5465 616d 732e 5f5f 6361 6c6c  ceptTeams.__call
-00004300: 5f5f 0d0a 0d0a 2320 4465 6669 6e65 2074  __....# Define t
-00004310: 6865 206e 6578 7420 7477 6f20 7661 7269  he next two vari
-00004320: 6162 6c65 7320 6f70 7469 6f6e 616c 6c79  ables optionally
-00004330: 2077 6865 6e20 7573 696e 6720 4f70 656e   when using Open
-00004340: 4149 2773 2041 5049 2e0d 0a23 205f 4f50  AI's API...# _OP
-00004350: 454e 5f41 495f 4d4f 4445 4c3d 2267 7074  EN_AI_MODEL="gpt
-00004360: 2d33 2e35 2d74 7572 626f 2220 2020 200d  -3.5-turbo"    .
-00004370: 0a23 205f 4f50 454e 5f41 495f 4150 493d  .# _OPEN_AI_API=
-00004380: 2273 6b2d 7878 7878 7878 220d 0a5f 5445  "sk-xxxxxx".._TE
-00004390: 414d 535f 5745 4248 4f4f 4b5f 5552 4c20  AMS_WEBHOOK_URL 
-000043a0: 3d20 276d 6963 726f 736f 6674 2077 6562  = 'microsoft web
-000043b0: 686f 6f6b 205f 5445 414d 535f 5745 4248  hook _TEAMS_WEBH
-000043c0: 4f4f 4b5f 5552 4c27 0d0a 0d0a 7472 793a  OOK_URL'....try:
-000043d0: 0d0a 2020 2020 7072 696e 7428 312f 3230  ..    print(1/20
-000043e0: 2920 200d 0a20 2020 2053 7563 6365 7373  )  ..    Success
-000043f0: 5465 616d 7328 292e 5f5f 6361 6c6c 5f5f  Teams().__call__
-00004400: 2829 2023 3120 7375 6363 6573 7320 7365  () #1 success se
-00004410: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
-00004420: 6578 6365 7074 2045 7863 6570 7454 6561  except ExceptTea
-00004430: 6d73 2061 7320 653a 2020 2020 2020 2332  ms as e:      #2
-00004440: 2065 7863 6570 7420 7365 6e64 6572 2020   except sender  
-00004450: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00004460: 7379 732e 6578 6974 2829 0d0a 0d0a 5365  sys.exit()....Se
-00004470: 6e64 5465 616d 7328 292e 5f5f 6361 6c6c  ndTeams().__call
-00004480: 5f5f 2829 2020 2020 2020 2020 2333 2063  __()        #3 c
-00004490: 7573 746f 6d69 7a65 6420 7365 6e64 6572  ustomized sender
-000044a0: 2020 2020 2020 2020 0d0a 6060 600d 0a0d          ..```...
-000044b0: 0a3c 4272 3e0d 0a0d 0a23 2320 322d 392e  .<Br>....## 2-9.
-000044c0: 202a 4b61 6b61 6f74 616c 6b20 4e6f 7469   *Kakaotalk Noti
-000044d0: 6669 6572 2a0d 0a2d 2061 2e20 5369 676e  fier*..- a. Sign
-000044e0: 2075 7020 6174 2074 6865 2066 6f6c 6c6f   up at the follo
-000044f0: 7769 6e67 2073 6974 653a 205b 6874 7470  wing site: [http
-00004500: 733a 2f2f 6465 7665 6c6f 7065 7273 2e6b  s://developers.k
-00004510: 616b 616f 2e63 6f6d 2f5d 2868 7474 7073  akao.com/](https
-00004520: 3a2f 2f64 6576 656c 6f70 6572 732e 6b61  ://developers.ka
-00004530: 6b61 6f2e 636f 6d2f 292e 0d0a 2d20 622e  kao.com/)...- b.
-00004540: 2043 6c69 636b 2022 4d79 2041 7070 6c69   Click "My Appli
-00004550: 6361 7469 6f6e 2220 6f6e 2074 6865 2074  cation" on the t
-00004560: 6f70 2062 6172 2e0d 0a2d 2063 2e20 436c  op bar...- c. Cl
-00004570: 6963 6b20 2241 6464 2061 6e20 6170 706c  ick "Add an appl
-00004580: 6963 6174 696f 6e2c 2220 7365 7420 6120  ication," set a 
-00004590: 6e61 6d65 2c20 616e 6420 6372 6561 7465  name, and create
-000045a0: 2069 742e 0d0a 2d20 642e 2043 6c69 636b   it...- d. Click
-000045b0: 2022 4b61 6b61 6f20 4c6f 6769 6e22 2069   "Kakao Login" i
-000045c0: 6e20 7468 6520 6c65 6674 206d 656e 752c  n the left menu,
-000045d0: 2074 6865 6e20 6368 616e 6765 2074 6865   then change the
-000045e0: 2053 7461 7465 206f 6620 224b 616b 616f   State of "Kakao
-000045f0: 204c 6f67 696e 2041 6374 6976 6174 696f   Login Activatio
-00004600: 6e22 2074 6f20 4f4e 206f 6e20 7468 6520  n" to ON on the 
-00004610: 7265 7375 6c74 696e 6720 7061 6765 2e0d  resulting page..
-00004620: 0a2d 2065 2e20 496e 204d 7920 4170 706c  .- e. In My Appl
-00004630: 6963 6174 696f 6e20 3e20 5072 6f64 7563  ication > Produc
-00004640: 7420 5365 7474 696e 6773 203e 204b 616b  t Settings > Kak
-00004650: 616f 204c 6f67 696e 2c20 6265 2073 7572  ao Login, be sur
-00004660: 6520 746f 2073 6574 2052 6564 6972 6563  e to set Redirec
-00004670: 7420 5552 4920 6173 2066 6f6c 6c6f 7773  t URI as follows
-00004680: 3a20 5b68 7474 7073 3a2f 2f65 7861 6d70  : [https://examp
-00004690: 6c65 2e63 6f6d 2f6f 6175 7468 5d28 6874  le.com/oauth](ht
-000046a0: 7470 733a 2f2f 6578 616d 706c 652e 636f  tps://example.co
-000046b0: 6d2f 6f61 7574 6829 2e0d 0a2d 2066 2e20  m/oauth)...- f. 
-000046c0: 496e 2074 6865 206c 6566 7420 436f 6e73  In the left Cons
-000046d0: 656e 7420 4974 656d 7320 6d65 6e75 2c20  ent Items menu, 
-000046e0: 7365 7420 2253 656e 6420 6d65 7373 6167  set "Send messag
-000046f0: 6520 696e 204b 616b 616f 5461 6c6b 2220  e in KakaoTalk" 
-00004700: 746f 2073 656c 6563 7469 7665 2061 6772  to selective agr
-00004710: 6565 6d65 6e74 2e0d 0a2d 2067 2e20 436f  eement...- g. Co
-00004720: 7079 2074 6865 2052 4553 5420 4150 4920  py the REST API 
-00004730: 4b65 7920 696e 204d 7920 4170 706c 6963  Key in My Applic
-00004740: 6174 696f 6e20 3e20 4170 7020 5365 7474  ation > App Sett
-00004750: 696e 6773 203e 2053 756d 6d61 7279 2c20  ings > Summary, 
-00004760: 616e 6420 676f 2074 6f20 7468 6520 666f  and go to the fo
-00004770: 6c6c 6f77 696e 6720 646f 6375 6d65 6e74  llowing document
-00004780: 2e0d 0a2d 2068 2e20 4966 2079 6f75 2068  ...- h. If you h
-00004790: 6176 6520 7375 6363 6573 7366 756c 6c79  ave successfully
-000047a0: 2063 6f6d 706c 6574 6564 2061 6c6c 206f   completed all o
-000047b0: 6620 7468 6520 6162 6f76 6520 7374 6570  f the above step
-000047c0: 732c 2067 6f20 746f 2074 6865 2066 6f6c  s, go to the fol
-000047d0: 6c6f 7769 6e67 2064 6f63 756d 656e 7420  lowing document 
-000047e0: 616e 6420 666f 6c6c 6f77 2074 6865 2069  and follow the i
-000047f0: 6e73 7472 7563 7469 6f6e 733a 0d0a 2068  nstructions:.. h
-00004800: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004810: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
-00004820: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
-00004830: 6f62 2f6d 6169 6e2f 7475 746f 7269 616c  ob/main/tutorial
-00004840: 732f 6b61 6b61 6f5f 746f 6b65 6e5f 6765  s/kakao_token_ge
-00004850: 6e65 7261 746f 722e 6970 796e 620d 0a20  nerator.ipynb.. 
-00004860: 2a2a 496e 2074 6869 7320 6578 616d 706c  **In this exampl
-00004870: 652c 2073 6f6d 6520 4150 4920 6b65 7973  e, some API keys
-00004880: 2077 6572 6520 6578 706f 7365 6420 6279   were exposed by
-00004890: 2063 7265 6174 696e 6720 616e 6420 7265   creating and re
-000048a0: 6d6f 7669 6e67 2061 2074 6573 7420 6170  moving a test ap
-000048b0: 706c 6963 6174 696f 6e2c 2062 7574 2066  plication, but f
-000048c0: 6f72 2073 6563 7572 6974 7920 7265 6173  or security reas
-000048d0: 6f6e 732c 2079 6f75 7220 4150 4920 6b65  ons, your API ke
-000048e0: 7920 7368 6f75 6c64 206e 6f74 2062 6520  y should not be 
-000048f0: 6578 706f 7365 6420 746f 2074 6865 206f  exposed to the o
-00004900: 7574 7369 6465 2077 6f72 6c64 2e2a 2a0d  utside world.**.
-00004910: 0a3c 4272 3e0d 0a0d 0a60 6060 7079 7468  .<Br>....```pyth
-00004920: 6f6e 0d0a 696d 706f 7274 2073 7973 0d0a  on..import sys..
-00004930: 6672 6f6d 2045 7863 6570 744e 6f74 6966  from ExceptNotif
-00004940: 6965 7220 696d 706f 7274 2045 7863 6570  ier import Excep
-00004950: 744b 616b 616f 2c20 5375 6363 6573 734b  tKakao, SuccessK
-00004960: 616b 616f 2c20 5365 6e64 4b61 6b61 6f0d  akao, SendKakao.
-00004970: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
-00004980: 3d20 4578 6365 7074 4b61 6b61 6f2e 5f5f  = ExceptKakao.__
-00004990: 6361 6c6c 5f5f 0d0a 0d0a 2320 4465 6669  call__....# Defi
-000049a0: 6e65 2074 6865 206e 6578 7420 7477 6f20  ne the next two 
-000049b0: 7661 7269 6162 6c65 7320 6f70 7469 6f6e  variables option
-000049c0: 616c 6c79 2077 6865 6e20 7573 696e 6720  ally when using 
-000049d0: 4f70 656e 4149 2773 2041 5049 2e0d 0a23  OpenAI's API...#
-000049e0: 205f 4f50 454e 5f41 495f 4d4f 4445 4c3d   _OPEN_AI_MODEL=
-000049f0: 2267 7074 2d33 2e35 2d74 7572 626f 2220  "gpt-3.5-turbo" 
-00004a00: 2020 200d 0a23 205f 4f50 454e 5f41 495f     ..# _OPEN_AI_
-00004a10: 4150 493d 2273 6b2d 7878 7878 7878 220d  API="sk-xxxxxx".
-00004a20: 0a5f 4b41 4b41 4f5f 544f 4b45 4e5f 5041  ._KAKAO_TOKEN_PA
-00004a30: 5448 203d 2027 7878 7878 2f78 7878 2f78  TH = 'xxxx/xxx/x
-00004a40: 7878 2e6a 736f 6e27 270d 0a0d 0a74 7279  xx.json''....try
-00004a50: 3a0d 0a20 2020 2070 7269 6e74 2831 2f30  :..    print(1/0
-00004a60: 2920 200d 0a20 2020 2053 7563 6365 7373  )  ..    Success
-00004a70: 4b61 6b61 6f28 292e 5f5f 6361 6c6c 5f5f  Kakao().__call__
-00004a80: 2829 2023 3120 7375 6363 6573 7320 7365  () #1 success se
-00004a90: 6e64 6572 2020 2020 2020 2020 2020 0d0a  nder          ..
-00004aa0: 6578 6365 7074 2045 7863 6570 744b 616b  except ExceptKak
-00004ab0: 616f 2061 7320 653a 2020 2020 2020 2332  ao as e:      #2
-00004ac0: 2065 7863 6570 7420 7365 6e64 6572 2020   except sender  
-00004ad0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00004ae0: 7379 732e 6578 6974 2829 0d0a 0d0a 5365  sys.exit()....Se
-00004af0: 6e64 4b61 6b61 6f28 292e 5f5f 6361 6c6c  ndKakao().__call
-00004b00: 5f5f 2829 2020 2020 2020 2020 2333 2063  __()        #3 c
-00004b10: 7573 746f 6d69 7a65 6420 7365 6e64 6572  ustomized sender
-00004b20: 2020 2020 2020 2020 200d 0a60 6060 0d0a           ..```..
-00004b30: 0d0a 3c42 723e 0d0a 0d0a 2323 2032 2d31  ..<Br>....## 2-1
-00004b40: 302e 202a 4265 6570 204e 6f74 6966 6965  0. *Beep Notifie
-00004b50: 722a 0d0a 4e6f 2073 6574 7570 2069 7320  r*..No setup is 
-00004b60: 7265 7175 6972 6564 2e20 5573 6520 6173  required. Use as
-00004b70: 2066 6f6c 6c6f 7773 2e0d 0a0d 0a60 6060   follows.....```
-00004b80: 7079 7468 6f6e 0d0a 6672 6f6d 2045 7863  python..from Exc
-00004b90: 6570 746e 6f74 6966 6965 7220 696d 706f  eptnotifier impo
-00004ba0: 7274 2045 7863 6570 7442 6565 702c 2053  rt ExceptBeep, S
-00004bb0: 7563 6365 7373 4265 6570 2c20 5365 6e64  uccessBeep, Send
-00004bc0: 4265 6570 2829 2c20 6265 6570 2829 0d0a  Beep(), beep()..
-00004bd0: 4245 4550 5f54 494d 4520 3d20 310d 0a73  BEEP_TIME = 1..s
-00004be0: 7973 2e65 7863 6570 7468 6f6f 6b20 3d20  ys.excepthook = 
-00004bf0: 4578 6365 7074 4265 6570 2e5f 5f63 616c  ExceptBeep.__cal
-00004c00: 6c5f 5f0d 0a0d 0a74 7279 3a0d 0a20 2020  l__....try:..   
-00004c10: 2070 7269 6e74 2831 2f32 3029 2020 0d0a   print(1/20)  ..
-00004c20: 2020 2020 5375 6363 6573 7342 6565 7028      SuccessBeep(
-00004c30: 292e 5f5f 6361 6c6c 5f5f 2829 2023 3120  ).__call__() #1 
-00004c40: 7375 6363 6573 7320 6265 6570 2d62 6565  success beep-bee
-00004c50: 7020 2020 2020 2020 2020 200d 0a0d 0a65  p          ....e
-00004c60: 7863 6570 7420 4578 6365 7074 4265 6570  xcept ExceptBeep
-00004c70: 2061 7320 653a 2020 2020 2020 2332 2065   as e:      #2 e
-00004c80: 7863 6570 7420 6265 6570 2d62 6565 7020  xcept beep-beep 
-00004c90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00004ca0: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
-00004cb0: 0a0d 0a53 656e 6442 6565 7028 292e 5f5f  ...SendBeep().__
-00004cc0: 6361 6c6c 5f5f 2829 2020 2020 2020 2020  call__()        
-00004cd0: 2333 2063 7573 746f 6d69 7a65 6420 6265  #3 customized be
-00004ce0: 6570 2d62 6565 7020 2020 2020 200d 0a0d  ep-beep      ...
-00004cf0: 0a62 6565 7028 290d 0a0d 0a60 6060 0d0a  .beep()....```..
-00004d00: 0d0a 3c42 723e 0d0a 0d0a 0d0a 2323 2032  ..<Br>......## 2
-00004d10: 2d31 312e 202a 4465 736b 746f 7020 4e6f  -11. *Desktop No
-00004d20: 7469 6669 6572 2a0d 0a4e 6f20 7365 7475  tifier*..No setu
-00004d30: 7020 6973 2072 6571 7569 7265 642e 2055  p is required. U
-00004d40: 7365 2061 7320 666f 6c6c 6f77 732e 0d0a  se as follows...
-00004d50: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00004d60: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
-00004d70: 2069 6d70 6f72 7420 4578 6365 7074 4465   import ExceptDe
-00004d80: 736b 746f 702c 2053 7563 6365 7373 4465  sktop, SuccessDe
-00004d90: 736b 746f 702c 2053 656e 6444 6573 6b74  sktop, SendDeskt
-00004da0: 6f70 0d0a 7379 732e 6578 6365 7074 686f  op..sys.exceptho
-00004db0: 6f6b 203d 2045 7863 6570 7444 6573 6b74  ok = ExceptDeskt
-00004dc0: 6f70 2e5f 5f63 616c 6c5f 5f0d 0a23 2044  op.__call__..# D
-00004dd0: 6566 696e 6520 7468 6520 6e65 7874 2074  efine the next t
-00004de0: 776f 2076 6172 6961 626c 6573 206f 7074  wo variables opt
-00004df0: 696f 6e61 6c6c 7920 7768 656e 2075 7369  ionally when usi
-00004e00: 6e67 204f 7065 6e41 4927 7320 4150 492e  ng OpenAI's API.
-00004e10: 0d0a 2320 5f4f 5045 4e5f 4149 5f4d 4f44  ..# _OPEN_AI_MOD
-00004e20: 454c 3d22 6770 742d 332e 352d 7475 7262  EL="gpt-3.5-turb
-00004e30: 6f22 2020 2020 0d0a 2320 5f4f 5045 4e5f  o"    ..# _OPEN_
-00004e40: 4149 5f41 5049 3d22 736b 2d78 7878 7878  AI_API="sk-xxxxx
-00004e50: 7822 0d0a 0d0a 7472 793a 0d0a 2020 2020  x"....try:..    
-00004e60: 7072 696e 7428 312f 3029 2020 0d0a 2020  print(1/0)  ..  
-00004e70: 2020 5375 6363 6573 7344 6573 6b74 6f70    SuccessDesktop
-00004e80: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2331  ().__call__() #1
-00004e90: 2073 7563 6365 7373 2073 656e 6465 7220   success sender 
-00004ea0: 2020 2020 2020 2020 200d 0a0d 0a65 7863           ....exc
-00004eb0: 6570 7420 4578 6365 7074 4465 736b 746f  ept ExceptDeskto
-00004ec0: 7020 6173 2065 3a20 2020 2020 2023 3220  p as e:      #2 
-00004ed0: 6578 6365 7074 2073 656e 6465 7220 2020  except sender   
-00004ee0: 2020 2020 2020 2020 200d 0a20 2020 2073           ..    s
-00004ef0: 7973 2e65 7869 7428 290d 0a0d 0a53 656e  ys.exit()....Sen
-00004f00: 6444 6573 6b74 6f70 2829 2e5f 5f63 616c  dDesktop().__cal
-00004f10: 6c5f 5f28 2920 2020 2020 2020 2023 3320  l__()        #3 
-00004f20: 6375 7374 6f6d 697a 6564 2073 656e 6465  customized sende
-00004f30: 7220 2020 2020 2020 2020 0d0a 6060 600d  r         ..```.
-00004f40: 0a0d 0a3c 4272 3e3c 6272 3e3c 6272 3e0d  ...<Br><br><br>.
-00004f50: 0a0d 0a23 2323 2049 6e73 7069 7269 6e67  ...### Inspiring
-00004f60: 0d0a 2d20 5468 616e 6b73 2074 6f20 5b4d  ..- Thanks to [M
-00004f70: 7975 6e67 6861 6b20 4c65 655d 2868 7474  yunghak Lee](htt
-00004f80: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00004f90: 6d79 656f 6e67 6861 6b29 2066 6f72 2070  myeonghak) for p
-00004fa0: 726f 7669 6469 6e67 2067 7265 6174 2069  roviding great i
-00004fb0: 6465 6173 206f 6e20 7072 6f76 6964 696e  deas on providin
-00004fc0: 6720 6465 6275 6767 696e 6720 696e 666f  g debugging info
-00004fd0: 726d 6174 696f 6e20 7468 726f 7567 6820  rmation through 
-00004fe0: 6f70 656e 2061 6920 4150 492e 0d0a 0d0a  open ai API.....
-00004ff0: 2323 2320 436f 6e74 6163 7473 0d0a 2d20  ### Contacts..- 
-00005000: 4d61 696e 7461 696e 6572 205b 4461 6e69  Maintainer [Dani
-00005010: 656c 2050 6172 6b2c 2053 6f75 7468 204b  el Park, South K
-00005020: 6f72 6561 5d28 6874 7470 733a 2f2f 6769  orea](https://gi
-00005030: 7468 7562 2e63 6f6d 2f44 5344 616e 6965  thub.com/DSDanie
-00005040: 6c50 6172 6b29 203c 6272 3e0d 0a2d 2045  lPark) <br>..- E
-00005050: 6d61 696c 2070 6172 6b6d 696e 776f 6f31  mail parkminwoo1
-00005060: 3939 3140 676d 6169 6c2e 636f 6d0d 0a0d  991@gmail.com...
-00005070: 0a23 2323 2323 2054 6865 2070 6163 6b61  .##### The packa
-00005080: 6765 2069 7320 6375 7272 656e 746c 7920  ge is currently 
-00005090: 696e 2074 6865 2064 6576 656c 6f70 6d65  in the developme
-000050a0: 6e74 2061 6e64 2051 4120 7374 6167 6573  nt and QA stages
-000050b0: 2c20 616e 6420 7468 6520 6465 7665 6c6f  , and the develo
-000050c0: 706d 656e 7420 7374 6167 6520 7769 6c6c  pment stage will
-000050d0: 2062 6520 7570 6461 7465 6420 6174 2074   be updated at t
-000050e0: 6865 2074 6f70 206f 6620 7468 6973 2070  he top of this p
-000050f0: 6167 652e 2049 6620 6974 2069 7320 6465  age. If it is de
-00005100: 7465 726d 696e 6564 2074 6861 7420 7468  termined that th
-00005110: 6520 7072 6f64 7563 7420 6973 2073 7461  e product is sta
-00005120: 626c 6520 7468 726f 7567 6820 6665 6174  ble through feat
-00005130: 7572 6520 696d 7072 6f76 656d 656e 742c  ure improvement,
-00005140: 2061 6464 6974 696f 6e2c 2061 6e64 2069   addition, and i
-00005150: 7373 7565 2072 6573 6f6c 7574 696f 6e2c  ssue resolution,
-00005160: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
-00005170: 2073 7461 6765 2077 696c 6c20 7265 6163   stage will reac
-00005180: 6820 7374 6167 6520 352e 2049 6620 6e6f  h stage 5. If no
-00005190: 206e 6577 2075 7064 6174 6573 206f 7220   new updates or 
-000051a0: 6973 7375 6573 2061 7269 7365 2c20 6974  issues arise, it
-000051b0: 2077 696c 6c20 6265 2061 646a 7573 7465   will be adjuste
-000051c0: 6420 7570 7761 7264 2074 6f20 7374 6167  d upward to stag
-000051d0: 6520 3620 6f72 2068 6967 6865 722e 0d0a  e 6 or higher...
-000051e0: 0d0a 2323 2323 2043 6f75 6c64 2079 6f75  ..#### Could you
-000051f0: 206b 696e 646c 7920 6164 6420 7468 6973   kindly add this
-00005200: 2062 6164 6765 2074 6f20 796f 7572 2072   badge to your r
-00005210: 6570 6f73 6974 6f72 793f 0d0a 0d0a 6060  epository?....``
-00005220: 600d 0a21 5b45 7863 6570 742d 4e6f 7469  `..![Except-Noti
-00005230: 6669 6572 5d28 6874 7470 733a 2f2f 696d  fier](https://im
-00005240: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00005250: 6765 2f70 7970 692d 4578 6365 7074 4e6f  ge/pypi-ExceptNo
-00005260: 7469 6669 6572 2d6f 7261 6e67 6529 0d0a  tifier-orange)..
-00005270: 6060 600d 0a0d 0a0d 0a                   ```......
+00000050: 6561 2a0d 0a3c 6272 3e0d 0a21 5b5d 2868  ea*..<br>..![](h
+00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000070: 6d2f 6473 6461 6e69 656c 7061 726b 2f45  m/dsdanielpark/E
+00000080: 7863 6570 744e 6f74 6966 6965 722f 626c  xceptNotifier/bl
+00000090: 6f62 2f6d 6169 6e2f 6173 7365 7473 2f69  ob/main/assets/i
+000000a0: 6d67 732f 4578 6365 7074 4e6f 7469 6669  mgs/ExceptNotifi
+000000b0: 6572 5f6c 6f67 6f2e 706e 6729 0d0a 0d0a  er_logo.png)....
+000000c0: 3c68 3320 616c 6967 6e3d 2263 656e 7465  <h3 align="cente
+000000d0: 7222 3e49 6e74 6567 7261 7465 7320 4149  r">Integrates AI
+000000e0: 2d61 7373 6973 7465 6420 6465 6275 6767  -assisted debugg
+000000f0: 696e 6720 6e6f 7469 6669 6361 7469 6f6e  ing notification
+00000100: 7320 696e 746f 2050 7974 686f 6e20 7472  s into Python tr
+00000110: 792d 6578 6365 7074 2073 7461 7465 6d65  y-except stateme
+00000120: 6e74 7320 666f 7220 7661 7269 6f75 7320  nts for various 
+00000130: 6d65 7373 6167 696e 6720 6170 706c 6963  messaging applic
+00000140: 6174 696f 6e73 2e20 3c2f 6833 3e0d 0a0d  ations. </h3>...
+00000150: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000160: 7222 3e0d 0a3c 6120 6872 6566 3d22 2868  r">..<a href="(h
+00000170: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000180: 6473 2e69 6f2f 6261 6467 652f 7079 7069  ds.io/badge/pypi
+00000190: 2d45 7863 6570 744e 6f74 6966 6965 722d  -ExceptNotifier-
+000001a0: 6f72 616e 6765 223e 3c2f 613e 0d0a 3c61  orange"></a>..<a
+000001b0: 2068 7265 663d 2268 7474 7073 3a2f 2f70   href="https://p
+000001c0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
+000001d0: 6578 6365 7074 6e6f 7469 6669 6572 2f22  exceptnotifier/"
+000001e0: 3e3c 696d 6720 616c 743d 2250 7950 4922  ><img alt="PyPI"
+000001f0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000200: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000210: 692f 762f 6578 6365 7074 6e6f 7469 6669  i/v/exceptnotifi
+00000220: 6572 223e 3c2f 613e 0d0a 3c61 2068 7265  er"></a>..<a hre
+00000230: 663d 2268 7474 7073 3a2f 2f70 6570 792e  f="https://pepy.
+00000240: 7465 6368 2f70 726f 6a65 6374 2f65 7863  tech/project/exc
+00000250: 6570 746e 6f74 6966 6965 7222 3e3c 696d  eptnotifier"><im
+00000260: 6720 616c 743d 2244 6f77 6e6c 6f61 6473  g alt="Downloads
+00000270: 2220 7372 633d 2268 7474 7073 3a2f 2f70  " src="https://p
+00000280: 6570 792e 7465 6368 2f62 6164 6765 2f65  epy.tech/badge/e
+00000290: 7863 6570 746e 6f74 6966 6965 7222 3e3c  xceptnotifier"><
+000002a0: 2f61 3e0d 0a3c 6120 6872 6566 3d22 6874  /a>..<a href="ht
+000002b0: 7470 733a 2f2f 616e 6163 6f6e 6461 2e6f  tps://anaconda.o
+000002c0: 7267 2f63 6f6e 6461 2d66 6f72 6765 2f65  rg/conda-forge/e
+000002d0: 7863 6570 746e 6f74 6966 6965 722f 223e  xceptnotifier/">
+000002e0: 3c69 6d67 2061 6c74 3d22 636f 6e64 612d  <img alt="conda-
+000002f0: 666f 7267 6522 2073 7263 3d22 6874 7470  forge" src="http
+00000300: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000310: 696f 2f63 6f6e 6461 2f64 6e2f 636f 6e64  io/conda/dn/cond
+00000320: 612d 666f 7267 652f 6578 6365 7074 6e6f  a-forge/exceptno
+00000330: 7469 6669 6572 2e73 7667 3f6c 6162 656c  tifier.svg?label
+00000340: 3d63 6f6e 6461 2d66 6f72 6765 223e 3c2f  =conda-forge"></
+00000350: 613e 0d0a 3c61 2068 7265 663d 2268 7474  a>..<a href="htt
+00000360: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000370: 7073 662f 626c 6163 6b22 3e3c 696d 6720  psf/black"><img 
+00000380: 616c 743d 2243 6f64 6520 7374 796c 653a  alt="Code style:
+00000390: 2062 6c61 636b 2220 7372 633d 2268 7474   black" src="htt
+000003a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000003b0: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
+000003c0: 3073 7479 6c65 2d62 6c61 636b 2d30 3030  0style-black-000
+000003d0: 3030 302e 7376 6722 3e3c 2f61 3e0d 0a3c  000.svg"></a>..<
+000003e0: 2f70 3e0d 0a0d 0a21 5b5d 2868 7474 7073  /p>....![](https
+000003f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6473  ://github.com/ds
+00000400: 6461 6e69 656c 7061 726b 2f45 7863 6570  danielpark/Excep
+00000410: 744e 6f74 6966 6965 722f 626c 6f62 2f6d  tNotifier/blob/m
+00000420: 6169 6e2f 6173 7365 7473 2f69 6d67 732f  ain/assets/imgs/
+00000430: 6d61 696e 322e 706e 6729 0d0a 0d0a 2320  main2.png)....# 
+00000440: 5079 7468 6f6e 2050 6163 6b61 6765 3a20  Python Package: 
+00000450: 4578 6365 7074 4e6f 7469 6669 6572 0d0a  ExceptNotifier..
+00000460: 2323 2323 2320 5072 6f76 6964 6573 2061  ##### Provides a
+00000470: 206e 6f74 6966 6963 6174 696f 6e20 6672   notification fr
+00000480: 6f6d 2074 6865 2061 7070 6c69 6361 7469  om the applicati
+00000490: 6f6e 2073 686f 776e 2069 6e20 7468 6520  on shown in the 
+000004a0: 6361 7074 7572 6564 2073 6372 6565 6e2e  captured screen.
+000004b0: 0d0a 2054 6865 2060 4578 6365 7074 4e6f  .. The `ExceptNo
+000004c0: 7469 6669 6572 6020 5079 7468 6f6e 2070  tifier` Python p
+000004d0: 6163 6b61 6765 206f 6666 6572 7320 6120  ackage offers a 
+000004e0: 666c 6578 6962 6c65 2061 7070 726f 6163  flexible approac
+000004f0: 6820 746f 2072 6563 6569 7669 6e67 206e  h to receiving n
+00000500: 6f74 6966 6963 6174 696f 6e73 2062 7920  otifications by 
+00000510: 656e 6861 6e63 696e 6720 5079 7468 6f6e  enhancing Python
+00000520: 2773 2074 7279 2d65 7863 6570 7420 7374  's try-except st
+00000530: 6174 656d 656e 742e 2054 6869 7320 7061  atement. This pa
+00000540: 636b 6167 6520 656e 6162 6c65 7320 796f  ckage enables yo
+00000550: 7520 746f 2072 6563 6569 7665 2061 6c65  u to receive ale
+00000560: 7274 7320 7468 726f 7567 6820 7661 7269  rts through vari
+00000570: 6f75 7320 6d65 7373 6167 696e 6720 6170  ous messaging ap
+00000580: 706c 6963 6174 696f 6e73 206f 7220 656d  plications or em
+00000590: 6169 6c73 2e0d 0a3c 4272 3e3c 6272 3e0d  ails...<Br><br>.
+000005a0: 0a57 6974 6820 6045 7863 6570 744e 6f74  .With `ExceptNot
+000005b0: 6966 6965 7260 2c20 796f 7520 6361 6e20  ifier`, you can 
+000005c0: 6f62 7461 696e 2064 6574 6169 6c65 6420  obtain detailed 
+000005d0: 636f 6d70 696c 6174 696f 6e20 6572 726f  compilation erro
+000005e0: 7273 2c20 696e 636c 7564 696e 6720 6465  rs, including de
+000005f0: 6275 6720 696e 666f 726d 6174 696f 6e2c  bug information,
+00000600: 2073 656e 7420 6469 7265 6374 6c79 2074   sent directly t
+00000610: 6f20 796f 7572 2070 7265 6665 7272 6564  o your preferred
+00000620: 206d 6573 7361 6769 6e67 2070 6c61 7466   messaging platf
+00000630: 6f72 6d20 6f72 2065 6d61 696c 2e20 4279  orm or email. By
+00000640: 2069 6e74 6567 7261 7469 6e67 204f 7065   integrating Ope
+00000650: 6e41 4927 7320 4368 6174 4750 542c 2079  nAI's ChatGPT, y
+00000660: 6f75 2063 616e 2072 6563 6569 7665 2061  ou can receive a
+00000670: 6464 6974 696f 6e61 6c20 6572 726f 7220  dditional error 
+00000680: 636f 6465 2069 6e66 6f72 6d61 7469 6f6e  code information
+00000690: 2061 7320 6c6f 6e67 2061 7320 796f 7520   as long as you 
+000006a0: 7072 6f76 6964 6520 7468 6520 7265 7175  provide the requ
+000006b0: 6972 6564 2041 5049 206d 6f64 656c 206e  ired API model n
+000006c0: 616d 6520 616e 6420 6b65 792e 2054 6869  ame and key. Thi
+000006d0: 7320 6665 6174 7572 6520 656e 7375 7265  s feature ensure
+000006e0: 7320 7468 6174 2065 7272 6f72 2068 616e  s that error han
+000006f0: 646c 696e 6720 616e 6420 6e6f 7469 6669  dling and notifi
+00000700: 6361 7469 6f6e 7320 6172 6520 6d6f 7265  cations are more
+00000710: 2069 6e66 6f72 6d61 7469 7665 2061 6e64   informative and
+00000720: 2061 6363 6573 7369 626c 652c 2073 7472   accessible, str
+00000730: 6561 6d6c 696e 696e 6720 796f 7572 2064  eamlining your d
+00000740: 6562 7567 6769 6e67 2070 726f 6365 7373  ebugging process
+00000750: 2e0d 0a0d 0a3c 4272 3e0d 0a0d 0a23 2323  .....<Br>....###
+00000760: 2320 436f 756c 6420 796f 7520 6b69 6e64  # Could you kind
+00000770: 6c79 2061 6464 2074 6869 7320 6261 6467  ly add this badg
+00000780: 6520 746f 2079 6f75 7220 7265 706f 7369  e to your reposi
+00000790: 746f 7279 3f0d 0a0d 0a60 6060 0d0a 215b  tory?....```..![
+000007a0: 4578 6365 7074 2d4e 6f74 6966 6965 725d  Except-Notifier]
+000007b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000007c0: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+000007d0: 7069 2d45 7863 6570 744e 6f74 6966 6965  pi-ExceptNotifie
+000007e0: 722d 6f72 616e 6765 290d 0a60 6060 0d0a  r-orange)..```..
+000007f0: 0d0a 0d0a 3c62 723e 3c62 723e 0d0a 0d0a  ....<br><br>....
+00000800: 2323 2320 5375 7070 6f72 7469 6e67 2041  ### Supporting A
+00000810: 7070 6c69 6361 7469 6f6e 730d 0a0d 0a2d  pplications....-
+00000820: 205b 5465 6c65 6772 616d 5d28 6874 7470   [Telegram](http
+00000830: 733a 2f2f 7465 6c65 6772 616d 2e6f 7267  s://telegram.org
+00000840: 2f29 0d0a 2d20 5b44 6973 636f 7264 5d28  /)..- [Discord](
+00000850: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
+00000860: 636f 6d2f 290d 0a2d 205b 536c 6163 6b5d  com/)..- [Slack]
+00000870: 2868 7474 7073 3a2f 2f73 6c61 636b 2e63  (https://slack.c
+00000880: 6f6d 2f29 0d0a 2d20 5b47 6f6f 676c 6520  om/)..- [Google 
+00000890: 4d61 696c 5d28 6874 7470 733a 2f2f 6d61  Mail](https://ma
+000008a0: 696c 2e67 6f6f 676c 652e 636f 6d2f 290d  il.google.com/).
+000008b0: 0a2d 205b 4c69 6e65 5d28 6874 7470 733a  .- [Line](https:
+000008c0: 2f2f 6c69 6e65 2e6d 652f 656e 2f29 0d0a  //line.me/en/)..
+000008d0: 2d20 5b41 5753 2043 6869 6d65 5d28 6874  - [AWS Chime](ht
+000008e0: 7470 733a 2f2f 6177 732e 616d 617a 6f6e  tps://aws.amazon
+000008f0: 2e63 6f6d 2f6b 6f2f 6368 696d 652f 646f  .com/ko/chime/do
+00000900: 776e 6c6f 6164 2d63 6869 6d65 2f29 0d0a  wnload-chime/)..
+00000910: 2d20 5b4d 6963 726f 736f 6674 2054 6561  - [Microsoft Tea
+00000920: 6d73 5d28 6874 7470 733a 2f2f 7777 772e  ms](https://www.
+00000930: 6d69 6372 6f73 6f66 742e 636f 6d2f 656e  microsoft.com/en
+00000940: 2f6d 6963 726f 736f 6674 2d74 6561 6d73  /microsoft-teams
+00000950: 2f64 6f77 6e6c 6f61 642d 6170 7029 0d0a  /download-app)..
+00000960: 2d20 5b4b 616b 616f 2054 616c 6b5d 2868  - [Kakao Talk](h
+00000970: 7474 7073 3a2f 2f77 7777 2e6b 616b 616f  ttps://www.kakao
+00000980: 636f 7270 2e63 6f6d 2f70 6167 652f 7365  corp.com/page/se
+00000990: 7276 6963 652f 7365 7276 6963 652f 4b61  rvice/service/Ka
+000009a0: 6b61 6f54 616c 6b3f 6c61 6e67 3d65 6e29  kaoTalk?lang=en)
+000009b0: 0d0a 2d20 534d 5320 5365 6e64 696e 6720  ..- SMS Sending 
+000009c0: 7573 696e 6720 5b54 7769 6c69 6f5d 2868  using [Twilio](h
+000009d0: 7474 7073 3a2f 2f77 7777 2e74 7769 6c69  ttps://www.twili
+000009e0: 6f2e 636f 6d2f 656e 2d75 7329 0d0a 2d20  o.com/en-us)..- 
+000009f0: 4465 736b 746f 7020 4e6f 7469 6669 6361  Desktop Notifica
+00000a00: 7469 6f6e 2075 7369 6e67 205b 506c 7965  tion using [Plye
+00000a10: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
+00000a20: 622e 636f 6d2f 6b69 7679 2f70 6c79 6572  b.com/kivy/plyer
+00000a30: 290d 0a2d 2042 6565 7020 536f 756e 6420  )..- Beep Sound 
+00000a40: 6672 6f6d 205b 7379 7374 656d 5d28 6874  from [system](ht
+00000a50: 7470 733a 2f2f 646f 6373 2e70 7974 686f  tps://docs.pytho
+00000a60: 6e2e 6f72 672f 332f 6c69 6272 6172 792f  n.org/3/library/
+00000a70: 7769 6e73 6f75 6e64 2e68 746d 6c29 0d0a  winsound.html)..
+00000a80: 0d0a 3c42 723e 0d0a 0d0a 2323 2320 4149  ..<Br>....### AI
+00000a90: 2044 6562 7567 6769 6e67 2075 7369 6e67   Debugging using
+00000aa0: 204f 7065 6e41 4920 4150 490d 0a49 6620   OpenAI API..If 
+00000ab0: 796f 7520 6861 7665 204f 7065 6e41 4920  you have OpenAI 
+00000ac0: 4150 4920 4b65 7920 616e 6420 6d6f 6465  API Key and mode
+00000ad0: 6c20 6e61 6d65 2c20 796f 7520 6361 6e20  l name, you can 
+00000ae0: 6765 7420 696e 666f 726d 6174 696f 6e20  get information 
+00000af0: 616e 6420 636f 6465 2065 7861 6d70 6c65  and code example
+00000b00: 7320 666f 7220 6465 6275 6767 696e 6720  s for debugging 
+00000b10: 696e 2061 6e79 2061 7070 6c69 6361 7469  in any applicati
+00000b20: 6f6e 2e0d 0a2d 205b 4f50 454e 2041 4920  on...- [OPEN AI 
+00000b30: 4150 495d 2868 7474 7073 3a2f 2f70 6c61  API](https://pla
+00000b40: 7466 6f72 6d2e 6f70 656e 6169 2e63 6f6d  tform.openai.com
+00000b50: 2f64 6f63 732f 696e 7472 6f64 7563 7469  /docs/introducti
+00000b60: 6f6e 290d 0a0d 0a0d 0a3c 6272 3e3c 6272  on)......<br><br
+00000b70: 3e0d 0a0d 0a23 2051 7569 636b 2053 7461  >....# Quick Sta
+00000b80: 7274 0d0a 6060 6062 6173 680d 0a70 6970  rt..```bash..pip
+00000b90: 2069 6e73 7461 6c6c 2045 7863 6570 744e   install ExceptN
+00000ba0: 6f74 6966 6965 720d 0a70 6970 2069 6e73  otifier..pip ins
+00000bb0: 7461 6c6c 2065 7863 6570 746e 6f74 6966  tall exceptnotif
+00000bc0: 6965 720d 0a0d 0a63 6f6e 6461 2069 6e73  ier....conda ins
+00000bd0: 7461 6c6c 2045 7863 6570 744e 6f74 6966  tall ExceptNotif
+00000be0: 6965 720d 0a63 6f6e 6461 2069 6e73 7461  ier..conda insta
+00000bf0: 6c6c 2065 7863 6570 746e 6f74 6966 6965  ll exceptnotifie
+00000c00: 720d 0a60 6060 0d0a 0d0a 3c62 723e 0d0a  r..```....<br>..
+00000c10: 0d0a 0d0a 2320 4170 7020 5365 7475 7020  ....# App Setup 
+00000c20: 4f76 6572 7669 6577 0d0a 0d0a 2d20 5468  Overview....- Th
+00000c30: 6520 7661 7269 6162 6c65 7320 696e 2074  e variables in t
+00000c40: 6865 2066 6f6c 6c6f 7769 6e67 2074 6162  he following tab
+00000c50: 6c65 206d 7573 7420 6e6f 7420 6265 2063  le must not be c
+00000c60: 6f6e 7461 6d69 6e61 7465 642e 0d0a 2d20  ontaminated...- 
+00000c70: 4465 7065 6e64 696e 6720 6f6e 2074 6865  Depending on the
+00000c80: 2073 6974 7561 7469 6f6e 2c20 636f 6e73   situation, cons
+00000c90: 6964 6572 2064 6573 6967 6e61 7469 6e67  ider designating
+00000ca0: 2074 6865 6d20 6173 2067 6c6f 6261 6c20   them as global 
+00000cb0: 7661 7269 6162 6c65 7320 666f 7220 7573  variables for us
+00000cc0: 652e 0d0a 2d20 4966 2079 6f75 2061 7265  e...- If you are
+00000cd0: 2075 7369 6e67 2054 656c 6567 7261 6d2c   using Telegram,
+00000ce0: 2061 6e20 6578 616d 706c 6520 6973 2061   an example is a
+00000cf0: 7474 6163 6865 6420 6173 2061 6e20 696d  ttached as an im
+00000d00: 6167 652e 0d0a 2d20 4173 2079 6f75 2061  age...- As you a
+00000d10: 6c72 6561 6479 206b 6e6f 772c 2041 5049  lready know, API
+00000d20: 204b 6579 7320 6f72 2073 6563 7572 6974   Keys or securit
+00000d30: 7920 746f 6b65 6e73 206d 7573 7420 6265  y tokens must be
+00000d40: 2073 6563 7572 6564 2e20 4e6f 7465 2074   secured. Note t
+00000d50: 6861 7420 7468 6520 6b65 7920 7661 6c75  hat the key valu
+00000d60: 6573 2077 6869 6368 2065 7870 6f73 7572  es which exposur
+00000d70: 6564 2069 6e20 6769 7468 7562 2077 696c  ed in github wil
+00000d80: 6c20 6265 2065 7870 6972 6564 2061 6674  l be expired aft
+00000d90: 6572 2069 6e73 6563 7572 6564 2e0d 0a0d  er insecured....
+00000da0: 0a7c 2041 7070 207c 2052 6571 7569 7265  .| App | Require
+00000db0: 6420 5661 7269 6162 6c65 7320 7c20 4672  d Variables | Fr
+00000dc0: 6565 206f 7220 5061 6964 207c 2045 6173  ee or Paid | Eas
+00000dd0: 6520 6f66 2053 6574 7570 207c 2054 696d  e of Setup | Tim
+00000de0: 6520 5265 7175 6972 6564 2066 6f72 2053  e Required for S
+00000df0: 6574 7570 7c47 7569 6465 2054 7574 6f72  etup|Guide Tutor
+00000e00: 6961 6c20 4c69 6e6b 7c0d 0a7c 3a2d 2d3a  ial Link|..|:--:
+00000e10: 7c3a 2d2d 7c3a 2d2d 3a7c 3a2d 2d3a 7c3a  |:--|:--:|:--:|:
+00000e20: 2d2d 3a7c 3a2d 2d2d 3a7c 0d0a 7c42 6565  --:|:---:|..|Bee
+00000e30: 707c 4e2f 417c 4672 6565 7c4e 2f41 7c30  p|N/A|Free|N/A|0
+00000e40: 206d 696e 7c5b 4578 6365 7074 4265 6570   min|[ExceptBeep
+00000e50: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000e60: 2e63 6f6d 2f64 7364 616e 6965 6c70 6172  .com/dsdanielpar
+00000e70: 6b2f 4578 6365 7074 4e6f 7469 6669 6572  k/ExceptNotifier
+00000e80: 2f62 6c6f 622f 6d61 696e 2f64 6f63 756d  /blob/main/docum
+00000e90: 656e 7473 2f45 7863 6570 7442 6565 702f  ents/ExceptBeep/
+00000ea0: 4755 4944 452e 6d64 297c 0d0a 7c44 6573  GUIDE.md)|..|Des
+00000eb0: 6b74 6f70 7c4e 2f41 7c46 7265 657c 4e2f  ktop|N/A|Free|N/
+00000ec0: 417c 3020 6d69 6e7c 5b45 7863 6570 7444  A|0 min|[ExceptD
+00000ed0: 6573 6b74 6f70 5d28 6874 7470 733a 2f2f  esktop](https://
+00000ee0: 6769 7468 7562 2e63 6f6d 2f64 7364 616e  github.com/dsdan
+00000ef0: 6965 6c70 6172 6b2f 4578 6365 7074 4e6f  ielpark/ExceptNo
+00000f00: 7469 6669 6572 2f62 6c6f 622f 6d61 696e  tifier/blob/main
+00000f10: 2f64 6f63 756d 656e 7473 2f45 7863 6570  /documents/Excep
+00000f20: 7444 6573 6b74 6f70 2f47 5549 4445 2e6d  tDesktop/GUIDE.m
+00000f30: 6429 7c0d 0a7c 5465 6c65 6772 616d 7c60  d)|..|Telegram|`
+00000f40: 5f54 454c 4547 5241 4d5f 544f 4b45 4e60  _TELEGRAM_TOKEN`
+00000f50: 7c46 7265 656d 6975 6d7c 4561 7379 7c32  |Freemium|Easy|2
+00000f60: 6d69 6e7c 5b45 7863 6570 7454 656c 6567  min|[ExceptTeleg
+00000f70: 7261 6d5d 2868 7474 7073 3a2f 2f67 6974  ram](https://git
+00000f80: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00000f90: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00000fa0: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+00000fb0: 6375 6d65 6e74 732f 4578 6365 7074 5465  cuments/ExceptTe
+00000fc0: 6c65 6772 616d 2f47 5549 4445 2e6d 6429  legram/GUIDE.md)
+00000fd0: 7c0d 0a7c 4469 7363 6f72 647c 605f 4449  |..|Discord|`_DI
+00000fe0: 5343 4f52 445f 5745 4248 4f4f 4b5f 5552  SCORD_WEBHOOK_UR
+00000ff0: 4c60 7c46 7265 656d 6975 6d7c 4561 7379  L`|Freemium|Easy
+00001000: 7c31 6d69 6e7c 5b45 7863 6570 7444 6973  |1min|[ExceptDis
+00001010: 636f 7264 5d28 6874 7470 733a 2f2f 6769  cord](https://gi
+00001020: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
+00001030: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
+00001040: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
+00001050: 6f63 756d 656e 7473 2f45 7863 6570 7454  ocuments/ExceptT
+00001060: 656c 6567 7261 6d2f 4755 4944 452e 6d64  elegram/GUIDE.md
+00001070: 297c 0d0a 7c41 5753 2043 6869 6d65 7c60  )|..|AWS Chime|`
+00001080: 5f43 4849 4d45 5f57 4542 484f 4f4b 5f55  _CHIME_WEBHOOK_U
+00001090: 524c 607c 4672 6565 6d69 756d 7c45 6173  RL`|Freemium|Eas
+000010a0: 797c 316d 696e 7c5b 4578 6365 7074 4368  y|1min|[ExceptCh
+000010b0: 696d 655d 2868 7474 7073 3a2f 2f67 6974  ime](https://git
+000010c0: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+000010d0: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+000010e0: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+000010f0: 6375 6d65 6e74 732f 4578 6365 7074 4368  cuments/ExceptCh
+00001100: 696d 652f 4755 4944 452e 6d64 297c 0d0a  ime/GUIDE.md)|..
+00001110: 7c53 6c61 636b 7c60 5f53 4c41 434b 5f57  |Slack|`_SLACK_W
+00001120: 4542 484f 4f4b 5f55 524c 607c 4672 6565  EBHOOK_URL`|Free
+00001130: 6d69 756d 7c45 6173 797c 336d 696e 7c5b  mium|Easy|3min|[
+00001140: 4578 6365 7074 536c 6163 6b5d 2868 7474  ExceptSlack](htt
+00001150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001160: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+00001170: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00001180: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+00001190: 4578 6365 7074 536c 6163 6b2f 4755 4944  ExceptSlack/GUID
+000011a0: 452e 6d64 297c 0d0a 7c47 2d4d 6169 6c7c  E.md)|..|G-Mail|
+000011b0: 605f 4741 4d49 4c5f 5245 4349 5049 454e  `_GAMIL_RECIPIEN
+000011c0: 545f 4144 4452 602c 2060 5f47 4d41 494c  T_ADDR`, `_GMAIL
+000011d0: 5f53 454e 4445 525f 4144 4452 602c 2060  _SENDER_ADDR`, `
+000011e0: 5f47 4d41 494c 5f41 5050 5f50 4153 5357  _GMAIL_APP_PASSW
+000011f0: 4f52 445f 4f46 5f53 454e 4445 5260 207c  ORD_OF_SENDER` |
+00001200: 5265 7374 7269 6374 6564 2066 7265 657c  Restricted free|
+00001210: 4d65 6469 756d 7c33 6d69 6e7c 5b45 7863  Medium|3min|[Exc
+00001220: 6570 744d 6169 6c5d 2868 7474 7073 3a2f  eptMail](https:/
+00001230: 2f67 6974 6875 622e 636f 6d2f 6473 6461  /github.com/dsda
+00001240: 6e69 656c 7061 726b 2f45 7863 6570 744e  nielpark/ExceptN
+00001250: 6f74 6966 6965 722f 626c 6f62 2f6d 6169  otifier/blob/mai
+00001260: 6e2f 646f 6375 6d65 6e74 732f 4578 6365  n/documents/Exce
+00001270: 7074 4d61 696c 2f47 5549 4445 2e6d 6429  ptMail/GUIDE.md)
+00001280: 7c0d 0a7c 4c69 6e65 7c60 5f4c 494e 455f  |..|Line|`_LINE_
+00001290: 4e4f 5449 4659 5f41 5049 5f54 4f4b 454e  NOTIFY_API_TOKEN
+000012a0: 607c 4672 6565 6d69 756d 7c4d 6564 6975  `|Freemium|Mediu
+000012b0: 6d7c 346d 696e 7c5b 4578 6365 7074 4c69  m|4min|[ExceptLi
+000012c0: 6e65 5d28 6874 7470 733a 2f2f 6769 7468  ne](https://gith
+000012d0: 7562 2e63 6f6d 2f64 7364 616e 6965 6c70  ub.com/dsdanielp
+000012e0: 6172 6b2f 4578 6365 7074 4e6f 7469 6669  ark/ExceptNotifi
+000012f0: 6572 2f62 6c6f 622f 6d61 696e 2f64 6f63  er/blob/main/doc
+00001300: 756d 656e 7473 2f45 7863 6570 744c 696e  uments/ExceptLin
+00001310: 652f 4755 4944 452e 6d64 297c 0d0a 7c53  e/GUIDE.md)|..|S
+00001320: 4d53 7c60 5f54 5749 4c49 4f5f 5349 4460  MS|`_TWILIO_SID`
+00001330: 2c20 605f 5457 494c 494f 5f54 4f4b 454e  , `_TWILIO_TOKEN
+00001340: 602c 2060 5f52 4543 4950 4945 4e54 5f50  `, `_RECIPIENT_P
+00001350: 484f 4e45 5f4e 554d 4245 5260 2c20 605f  HONE_NUMBER`, `_
+00001360: 5345 4e44 4552 5f50 484f 4e45 5f4e 554d  SENDER_PHONE_NUM
+00001370: 4245 5260 7c4e 6f74 2066 7265 657c 4d65  BER`|Not free|Me
+00001380: 6469 756d 7c35 6d69 6e7c 5b45 7863 6570  dium|5min|[Excep
+00001390: 7453 4d53 5d28 6874 7470 733a 2f2f 6769  tSMS](https://gi
+000013a0: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
+000013b0: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
+000013c0: 6669 6572 2f62 6c6f 622f 6d61 696e 2f64  fier/blob/main/d
+000013d0: 6f63 756d 656e 7473 2f45 7863 6570 7453  ocuments/ExceptS
+000013e0: 4d53 2f47 5549 4445 2e6d 6429 7c0d 0a7c  MS/GUIDE.md)|..|
+000013f0: 4d69 6372 6f73 6f66 7420 5465 616d 737c  Microsoft Teams|
+00001400: 605f 5445 414d 535f 5745 4248 4f4f 4b5f  `_TEAMS_WEBHOOK_
+00001410: 5552 4c60 7c4e 6f74 2046 7265 657c 4d65  URL`|Not Free|Me
+00001420: 6469 756d 7c35 6d69 6e7c 5b45 7863 6570  dium|5min|[Excep
+00001430: 7454 6561 6d73 5d28 6874 7470 733a 2f2f  tTeams](https://
+00001440: 6769 7468 7562 2e63 6f6d 2f64 7364 616e  github.com/dsdan
+00001450: 6965 6c70 6172 6b2f 4578 6365 7074 4e6f  ielpark/ExceptNo
+00001460: 7469 6669 6572 2f62 6c6f 622f 6d61 696e  tifier/blob/main
+00001470: 2f64 6f63 756d 656e 7473 2f45 7863 6570  /documents/Excep
+00001480: 7454 6561 6d73 2f47 5549 4445 2e6d 6429  tTeams/GUIDE.md)
+00001490: 7c0d 0a7c 4b61 6b61 6f54 616c 6b7c 605f  |..|KakaoTalk|`_
+000014a0: 4b41 4b41 4f5f 544f 4b45 4e5f 5041 5448  KAKAO_TOKEN_PATH
+000014b0: 607c 4672 6565 6d69 756d 7c48 656c 6c7c  `|Freemium|Hell|
+000014c0: 3e3d 3130 6d69 6e28 546f 6b65 6e20 7265  >=10min(Token re
+000014d0: 6672 6573 6865 7320 6461 696c 7929 7c5b  freshes daily)|[
+000014e0: 4578 6365 7074 4b61 6b61 6f5d 2868 7474  ExceptKakao](htt
+000014f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001500: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+00001510: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00001520: 2f6d 6169 6e2f 646f 6375 6d65 6e74 732f  /main/documents/
+00001530: 4578 6365 7074 4b61 6b61 6f2f 4755 4944  ExceptKakao/GUID
+00001540: 452e 6d64 297c 0d0a 0d0a 0d0a 4966 2079  E.md)|......If y
+00001550: 6f75 2061 6464 2074 6865 2066 6f6c 6c6f  ou add the follo
+00001560: 7769 6e67 2074 776f 2076 6172 6961 626c  wing two variabl
+00001570: 6573 2074 6f20 7468 6520 7265 7175 6972  es to the requir
+00001580: 6564 2076 6172 6961 626c 6573 2066 6f72  ed variables for
+00001590: 2065 6163 6820 6170 706c 6963 6174 696f   each applicatio
+000015a0: 6e20 696e 2074 6865 2074 6162 6c65 2061  n in the table a
+000015b0: 626f 7665 2c20 796f 7520 6361 6e20 7265  bove, you can re
+000015c0: 6365 6976 6520 6572 726f 7220 6c6f 6361  ceive error loca
+000015d0: 7469 6f6e 2061 6e64 2065 7870 6c61 6e61  tion and explana
+000015e0: 7469 6f6e 2c20 6173 2077 656c 6c20 6173  tion, as well as
+000015f0: 2065 7861 6d70 6c65 732c 2066 726f 6d20   examples, from 
+00001600: 4f70 656e 4149 2773 206d 6f64 656c 0d0a  OpenAI's model..
+00001610: 0d0a 7c20 4150 4920 7c20 5265 7175 6972  ..| API | Requir
+00001620: 6564 2056 6172 6961 626c 6573 207c 2046  ed Variables | F
+00001630: 7265 6520 6f72 2050 6169 6420 7c20 4561  ree or Paid | Ea
+00001640: 7365 206f 6620 5365 7475 7020 7c20 5469  se of Setup | Ti
+00001650: 6d65 2052 6571 7569 7265 6420 666f 7220  me Required for 
+00001660: 5365 7475 707c 4775 6964 6520 5475 746f  Setup|Guide Tuto
+00001670: 7269 616c 204c 696e 6b7c 0d0a 7c3a 2d2d  rial Link|..|:--
+00001680: 3a7c 3a2d 2d7c 3a2d 2d3a 7c3a 2d2d 3a7c  :|:--|:--:|:--:|
+00001690: 3a2d 2d3a 7c3a 2d2d 2d3a 7c0d 0a7c 204f  :--:|:---:|..| O
+000016a0: 7065 6e41 4920 4150 4920 7c60 5265 7175  penAI API |`Requ
+000016b0: 6972 6564 2076 6172 6961 626c 6573 2066  ired variables f
+000016c0: 6f72 2065 6163 6820 6170 706c 6963 6174  or each applicat
+000016d0: 696f 6e60 2b20 605f 4f50 454e 5f41 495f  ion`+ `_OPEN_AI_
+000016e0: 4d4f 4445 4c60 2c60 5f4f 5045 4e5f 4149  MODEL`,`_OPEN_AI
+000016f0: 5f41 5049 607c 4e6f 7420 6672 6565 7c45  _API`|Not free|E
+00001700: 6173 797c 326d 696e 7c5b 4150 494f 7065  asy|2min|[APIOpe
+00001710: 6e41 495d 2868 7474 7073 3a2f 2f67 6974  nAI](https://git
+00001720: 6875 622e 636f 6d2f 6473 6461 6e69 656c  hub.com/dsdaniel
+00001730: 7061 726b 2f45 7863 6570 744e 6f74 6966  park/ExceptNotif
+00001740: 6965 722f 626c 6f62 2f6d 6169 6e2f 646f  ier/blob/main/do
+00001750: 6375 6d65 6e74 732f 4150 494f 7065 6e41  cuments/APIOpenA
+00001760: 492f 4755 4944 452e 6d64 297c 0d0a 0d0a  I/GUIDE.md)|....
+00001770: 0d0a 3c62 723e 3c62 723e 0d0a 0d0a 2320  ..<br><br>....# 
+00001780: 312e 204b 6579 2046 6561 7475 7265 730d  1. Key Features.
+00001790: 0a54 6f20 7573 6520 7468 6520 6465 7369  .To use the desi
+000017a0: 7265 6420 6170 706c 6963 6174 696f 6e2c  red application,
+000017b0: 2079 6f75 206d 7573 7420 6465 6669 6e65   you must define
+000017c0: 2074 6865 206e 6563 6573 7361 7279 2076   the necessary v
+000017d0: 6172 6961 626c 6573 2e20 456e 7375 7265  ariables. Ensure
+000017e0: 2074 6861 7420 7468 6520 7661 7269 6162   that the variab
+000017f0: 6c65 206e 616d 6573 2072 656d 6169 6e20  le names remain 
+00001800: 756e 6368 616e 6765 642c 2061 6e64 2079  unchanged, and y
+00001810: 6f75 2063 616e 2075 7365 2065 6974 6865  ou can use eithe
+00001820: 7220 6c6f 6361 6c20 6f72 2067 6c6f 6261  r local or globa
+00001830: 6c20 7661 7269 6162 6c65 732e 2049 6620  l variables. If 
+00001840: 796f 7520 6172 6520 7573 696e 6720 6054  you are using `T
+00001850: 656c 6567 7261 6d60 2c20 616e 2065 7861  elegram`, an exa
+00001860: 6d70 6c65 2069 7320 6174 7461 6368 6564  mple is attached
+00001870: 2061 7320 616e 2069 6d61 6765 2e0d 0a0d   as an image....
+00001880: 0a23 2320 312d 312e 2045 7863 6570 7460  .## 1-1. Except`
+00001890: 5b61 7070 4e61 6d65 5d60 0d0a 4966 2079  [appName]`..If y
+000018a0: 6f75 2075 7365 2050 7974 686f 6e27 7320  ou use Python's 
+000018b0: 7472 7920 6578 6365 7074 2073 7461 7465  try except state
+000018c0: 6d65 6e74 2061 7320 6974 2069 732c 2062  ment as it is, b
+000018d0: 7574 2063 6861 6e67 6520 6578 6365 7074  ut change except
+000018e0: 2061 7320 666f 6c6c 6f77 732c 2079 6f75   as follows, you
+000018f0: 2063 616e 2072 6563 6569 7665 206e 6f74   can receive not
+00001900: 6966 6963 6174 696f 6e73 2074 6872 6f75  ifications throu
+00001910: 6768 2079 6f75 7220 6170 706c 6963 6174  gh your applicat
+00001920: 696f 6e2e 0d0a 6060 600d 0a45 7863 6570  ion...```..Excep
+00001930: 7443 6869 6d65 2c20 4578 6365 7074 5465  tChime, ExceptTe
+00001940: 6c65 6772 616d 2c20 4578 6365 7074 4469  legram, ExceptDi
+00001950: 7363 6f72 642c 2045 7863 6570 7453 4d53  scord, ExceptSMS
+00001960: 2c20 4578 6365 7074 4d61 696c 2c20 4578  , ExceptMail, Ex
+00001970: 6365 7074 4b61 6b61 6f2c 2045 7863 6570  ceptKakao, Excep
+00001980: 744c 696e 652c 2045 7863 6570 7453 6c61  tLine, ExceptSla
+00001990: 636b 2c20 4578 6365 7074 5465 616d 732c  ck, ExceptTeams,
+000019a0: 2045 7863 6570 7444 6573 6b74 6f70 652c   ExceptDesktope,
+000019b0: 2045 7863 6570 7442 6565 700d 0a60 6060   ExceptBeep..```
+000019c0: 0d0a 0d0a 2a45 7861 6d70 6c65 2a0d 0a60  ....*Example*..`
+000019d0: 6060 7079 7468 6f6e 0d0a 6672 6f6d 2045  ``python..from E
+000019e0: 7863 6570 744e 6f74 6966 6965 7220 696d  xceptNotifier im
+000019f0: 706f 7274 2045 7863 6570 7454 656c 6765  port ExceptTelge
+00001a00: 7261 6d0d 0a5f 5445 4c45 4752 414d 5f54  ram.._TELEGRAM_T
+00001a10: 4f4b 454e 203d 2022 7878 7878 220d 0a0d  OKEN = "xxxx"...
+00001a20: 0a74 7279 3a0d 0a20 2020 2070 7269 6e74  .try:..    print
+00001a30: 2831 2f30 290d 0a65 7863 6570 7420 4578  (1/0)..except Ex
+00001a40: 6365 7074 5465 6c65 6772 616d 3a20 2020  ceptTelegram:   
+00001a50: 2023 2073 656e 6469 6e67 2065 7863 6570   # sending excep
+00001a60: 7420 6d65 7373 6167 6520 746f 2074 656c  t message to tel
+00001a70: 6567 7261 6d0d 0a20 2020 2073 7973 2e65  egram..    sys.e
+00001a80: 7869 7428 290d 0a60 6060 0d0a 215b 5d28  xit()..```..![](
+00001a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001aa0: 6f6d 2f64 7364 616e 6965 6c70 6172 6b2f  om/dsdanielpark/
+00001ab0: 4578 6365 7074 4e6f 7469 6669 6572 2f62  ExceptNotifier/b
+00001ac0: 6c6f 622f 6d61 696e 2f61 7373 6574 732f  lob/main/assets/
+00001ad0: 696d 6773 2f65 7831 2e70 6e67 290d 0a0d  imgs/ex1.png)...
+00001ae0: 0a3c 6272 3e0d 0a0d 0a23 2320 312d 322e  .<br>....## 1-2.
+00001af0: 2041 4920 4465 6262 7567 6769 6e67 2049   AI Debbugging I
+00001b00: 6e66 6f6d 6174 696f 6e20 4e6f 7469 6669  nfomation Notifi
+00001b10: 6361 7469 6f6e 0d0a 596f 7520 6361 6e20  cation..You can 
+00001b20: 7265 6365 6976 6520 6465 6275 6767 696e  receive debuggin
+00001b30: 6720 696e 666f 726d 6174 696f 6e20 6672  g information fr
+00001b40: 6f6d 2043 6861 7447 5054 2076 6961 204f  om ChatGPT via O
+00001b50: 7065 6e41 4927 7320 4150 4920 7768 656e  penAI's API when
+00001b60: 2075 7369 6e67 2074 6865 2045 7863 6570   using the Excep
+00001b70: 7420 7374 6174 656d 656e 742e 2054 6865  t statement. The
+00001b80: 2073 796e 7461 7820 7265 6d61 696e 7320   syntax remains 
+00001b90: 7468 6520 7361 6d65 2c20 6275 7420 796f  the same, but yo
+00001ba0: 7527 6c6c 206e 6565 6420 746f 2063 6f6e  u'll need to con
+00001bb0: 6669 6775 7265 2074 6865 7365 2074 776f  figure these two
+00001bc0: 2076 6172 6961 626c 6573 3a0d 0a60 5f4f   variables:..`_O
+00001bd0: 5045 4e5f 4149 5f4d 4f44 454c 602c 605f  PEN_AI_MODEL`,`_
+00001be0: 4f50 454e 5f41 495f 4150 4960 0d0a 0d0a  OPEN_AI_API`....
+00001bf0: 2a45 7861 6d70 6c65 2a0d 0a60 6060 7079  *Example*..```py
+00001c00: 7468 6f6e 0d0a 6672 6f6d 2045 7863 6570  thon..from Excep
+00001c10: 744e 6f74 6966 6965 7220 696d 706f 7274  tNotifier import
+00001c20: 2045 7863 6570 7454 656c 6765 7261 6d0d   ExceptTelgeram.
+00001c30: 0a5f 5445 4c45 4752 414d 5f54 4f4b 454e  ._TELEGRAM_TOKEN
+00001c40: 203d 2022 7878 7878 220d 0a5f 4f50 454e   = "xxxx".._OPEN
+00001c50: 5f41 495f 4d4f 4445 4c3d 2267 7074 2d33  _AI_MODEL="gpt-3
+00001c60: 2e35 2d74 7572 626f 220d 0a5f 4f50 454e  .5-turbo".._OPEN
+00001c70: 5f41 495f 4150 493d 2273 6b2d 7878 7878  _AI_API="sk-xxxx
+00001c80: 7878 220d 0a0d 0a74 7279 3a0d 0a20 2020  xx"....try:..   
+00001c90: 2070 7269 6e74 2831 2f30 290d 0a65 7863   print(1/0)..exc
+00001ca0: 6570 7420 4578 6365 7074 5465 6c65 6772  ept ExceptTelegr
+00001cb0: 616d 3a20 2320 7365 6e64 696e 6720 6d73  am: # sending ms
+00001cc0: 6720 5749 5448 2041 4920 4445 4255 4747  g WITH AI DEBUGG
+00001cd0: 494e 4720 746f 2074 656c 6567 7261 6d0d  ING to telegram.
+00001ce0: 0a20 2020 2073 7973 2e65 7869 7428 290d  .    sys.exit().
+00001cf0: 0a60 6060 0d0a 0d0a 215b 5d28 6874 7470  .```....![](http
+00001d00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001d10: 7364 616e 6965 6c70 6172 6b2f 4578 6365  sdanielpark/Exce
+00001d20: 7074 4e6f 7469 6669 6572 2f62 6c6f 622f  ptNotifier/blob/
+00001d30: 6d61 696e 2f61 7373 6574 732f 696d 6773  main/assets/imgs
+00001d40: 2f65 7832 2e70 6e67 290d 0a0d 0a3c 6272  /ex2.png)....<br
+00001d50: 3e0d 0a0d 0a23 2320 312d 332e 2053 7563  >....## 1-3. Suc
+00001d60: 6365 7373 605b 6170 704e 616d 655d 600d  cess`[appName]`.
+00001d70: 0a42 7920 706c 6163 696e 6720 7468 6520  .By placing the 
+00001d80: 7472 7920 6578 6365 7074 2069 6e20 7079  try except in py
+00001d90: 7468 6f6e 2061 7420 7468 6520 656e 6420  thon at the end 
+00001da0: 6f66 2074 6865 2074 7279 2073 7461 7465  of the try state
+00001db0: 6d65 6e74 2c20 6170 706c 6963 6174 696f  ment, applicatio
+00001dc0: 6e73 2063 616e 2062 6520 6e6f 7469 6669  ns can be notifi
+00001dd0: 6564 2074 6861 7420 7468 6520 7472 7920  ed that the try 
+00001de0: 7374 6174 656d 656e 7420 776f 726b 6564  statement worked
+00001df0: 206e 6f72 6d61 6c6c 792e 0d0a 6060 600d   normally...```.
+00001e00: 0a53 7563 6365 7373 4368 696d 652c 2053  .SuccessChime, S
+00001e10: 7563 6365 7373 5465 6c65 6772 616d 2c20  uccessTelegram, 
+00001e20: 5375 6363 6573 7344 6973 636f 7264 2c20  SuccessDiscord, 
+00001e30: 5375 6363 6573 7353 4d53 2c20 5375 6363  SuccessSMS, Succ
+00001e40: 6573 734d 6169 6c2c 2053 7563 6365 7373  essMail, Success
+00001e50: 4b61 6b61 6f2c 2053 7563 6365 7373 4c69  Kakao, SuccessLi
+00001e60: 6e65 2c20 5375 6363 6573 7353 6c61 636b  ne, SuccessSlack
+00001e70: 2c20 5375 6363 6573 7354 6561 6d73 2c20  , SuccessTeams, 
+00001e80: 5375 6363 6573 7344 6573 6b74 6f70 652c  SuccessDesktope,
+00001e90: 2053 7563 6365 7373 4265 6570 0d0a 6060   SuccessBeep..``
+00001ea0: 600d 0a2a 4578 616d 706c 652a 0d0a 0d0a  `..*Example*....
+00001eb0: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00001ec0: 4578 6365 7074 4e6f 7469 6669 6572 2069  ExceptNotifier i
+00001ed0: 6d70 6f72 7420 5375 6363 6573 7354 656c  mport SuccessTel
+00001ee0: 6765 7261 6d0d 0a5f 5445 4c45 4752 414d  geram.._TELEGRAM
+00001ef0: 5f54 4f4b 454e 203d 2022 7878 7878 220d  _TOKEN = "xxxx".
+00001f00: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
+00001f10: 6e74 2831 2f32 3029 0d0a 2020 2020 5375  nt(1/20)..    Su
+00001f20: 6363 6573 7354 656c 6765 7261 6d28 292e  ccessTelgeram().
+00001f30: 5f5f 6361 6c6c 5f5f 2829 2020 2320 7365  __call__()  # se
+00001f40: 6e64 696e 6720 7375 6363 6573 7320 6d65  nding success me
+00001f50: 7373 6167 6520 746f 2074 656c 6567 7261  ssage to telegra
+00001f60: 6d0d 0a65 7863 6570 743a 0d0a 2020 2020  m..except:..    
+00001f70: 7379 732e 6578 6974 2829 0d0a 6060 600d  sys.exit()..```.
+00001f80: 0a0d 0a21 5b5d 2868 7474 7073 3a2f 2f67  ...![](https://g
+00001f90: 6974 6875 622e 636f 6d2f 6473 6461 6e69  ithub.com/dsdani
+00001fa0: 656c 7061 726b 2f45 7863 6570 744e 6f74  elpark/ExceptNot
+00001fb0: 6966 6965 722f 626c 6f62 2f6d 6169 6e2f  ifier/blob/main/
+00001fc0: 6173 7365 7473 2f69 6d67 732f 6578 332e  assets/imgs/ex3.
+00001fd0: 706e 6729 0d0a 0d0a 3c42 723e 0d0a 0d0a  png)....<Br>....
+00001fe0: 2323 2031 2d34 2e20 5365 6e64 605b 6170  ## 1-4. Send`[ap
+00001ff0: 704e 616d 655d 600d 0a50 6c61 6365 2069  pName]`..Place i
+00002000: 7420 616e 7977 6865 7265 206f 6e20 7468  t anywhere on th
+00002010: 6520 6c69 6e65 206f 6620 636f 6465 2079  e line of code y
+00002020: 6f75 2077 616e 742c 2061 6e64 2079 6f75  ou want, and you
+00002030: 276c 6c20 6265 206e 6f74 6966 6965 6420  'll be notified 
+00002040: 7768 656e 2074 6861 7420 6c69 6e65 206f  when that line o
+00002050: 6620 636f 6465 2069 7320 7265 6163 6865  f code is reache
+00002060: 642e 0d0a 6060 600d 0a53 656e 6443 6869  d...```..SendChi
+00002070: 6d65 2c20 5365 6e64 5465 6c65 6772 616d  me, SendTelegram
+00002080: 2c20 5365 6e64 4469 7363 6f72 642c 2053  , SendDiscord, S
+00002090: 656e 6453 4d53 2c20 5365 6e64 4d61 696c  endSMS, SendMail
+000020a0: 2c20 5365 6e64 4b61 6b61 6f2c 2053 656e  , SendKakao, Sen
+000020b0: 644c 696e 652c 2053 656e 6453 6c61 636b  dLine, SendSlack
+000020c0: 2c20 5365 6e64 5465 616d 732c 2053 656e  , SendTeams, Sen
+000020d0: 6444 6573 6b74 6f70 652c 2053 656e 6442  dDesktope, SendB
+000020e0: 6565 700d 0a60 6060 0d0a 2a45 7861 6d70  eep..```..*Examp
+000020f0: 6c65 2a0d 0a0d 0a60 6060 7079 7468 6f6e  le*....```python
+00002100: 0d0a 6672 6f6d 2045 7863 6570 744e 6f74  ..from ExceptNot
+00002110: 6966 6965 7220 696d 706f 7274 2053 656e  ifier import Sen
+00002120: 6454 656c 6765 7261 6d0d 0a5f 5445 4c45  dTelgeram.._TELE
+00002130: 4752 414d 5f54 4f4b 454e 203d 2022 7878  GRAM_TOKEN = "xx
+00002140: 7878 220d 0a0d 0a53 656e 6454 656c 6567  xx"....SendTeleg
+00002150: 7261 6d28 292e 5f5f 6361 6c6c 5f5f 2829  ram().__call__()
+00002160: 2023 2073 656e 6469 6e67 206d 6573 7361   # sending messa
+00002170: 6765 2074 6f20 7465 6c65 6772 616d 0d0a  ge to telegram..
+00002180: 0d0a 6e6f 7469 203d 2053 656e 6454 656c  ..noti = SendTel
+00002190: 6567 7261 6d28 290d 0a6e 6f74 6928 2920  egram()..noti() 
+000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021b0: 2020 2023 2073 656e 6469 6e67 206d 6573     # sending mes
+000021c0: 7361 6765 2074 6f20 7465 6c65 6772 616d  sage to telegram
+000021d0: 0d0a 6060 600d 0a0d 0a21 5b5d 2868 7474  ..```....![](htt
+000021e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000021f0: 6473 6461 6e69 656c 7061 726b 2f45 7863  dsdanielpark/Exc
+00002200: 6570 744e 6f74 6966 6965 722f 626c 6f62  eptNotifier/blob
+00002210: 2f6d 6169 6e2f 6173 7365 7473 2f69 6d67  /main/assets/img
+00002220: 732f 6578 342e 706e 6729 0d0a 0d0a 0d0a  s/ex4.png)......
+00002230: 3c62 723e 3c62 723e 0d0a 0d0a 2320 322e  <br><br>....# 2.
+00002240: 2046 6561 7475 7265 730d 0a59 6f75 2063   Features..You c
+00002250: 616e 2072 6563 6569 7665 2064 6562 7567  an receive debug
+00002260: 6769 6e67 2069 6e66 6f72 6d61 7469 6f6e  ging information
+00002270: 2066 726f 6d20 4368 6174 4750 5420 7669   from ChatGPT vi
+00002280: 6120 4f70 656e 4149 2773 2041 5049 2077  a OpenAI's API w
+00002290: 6865 6e20 7573 696e 6720 7468 6520 4578  hen using the Ex
+000022a0: 6365 7074 2073 7461 7465 6d65 6e74 2e20  cept statement. 
+000022b0: 5468 6520 7379 6e74 6178 2072 656d 6169  The syntax remai
+000022c0: 6e73 2074 6865 2073 616d 652c 2062 7574  ns the same, but
+000022d0: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
+000022e0: 636f 6e66 6967 7572 6520 7468 6573 6520  configure these 
+000022f0: 7477 6f20 7661 7269 6162 6c65 733a 0d0a  two variables:..
+00002300: 605f 4f50 454e 5f41 495f 4d4f 4445 4c60  `_OPEN_AI_MODEL`
+00002310: 2c60 5f4f 5045 4e5f 4149 5f41 5049 600d  ,`_OPEN_AI_API`.
+00002320: 0a0d 0a0d 0a0d 0a23 2320 322d 312e 202a  .......## 2-1. *
+00002330: 5465 6c65 6772 616d 204e 6f74 6966 6965  Telegram Notifie
+00002340: 722a 0d0a 0d0a 2d20 612e 204f 7065 6e20  r*....- a. Open 
+00002350: 796f 7572 2074 656c 6567 7261 6d20 6170  your telegram ap
+00002360: 7020 616e 6420 7365 6172 6368 2066 6f72  p and search for
+00002370: 2042 6f74 4661 7468 6572 2e20 2841 2062   BotFather. (A b
+00002380: 7569 6c74 2d69 6e20 5465 6c65 6772 616d  uilt-in Telegram
+00002390: 2062 6f74 2074 6861 7420 6865 6c70 7320   bot that helps 
+000023a0: 7573 6572 7320 6372 6561 7465 2063 7573  users create cus
+000023b0: 746f 6d20 5465 6c65 6772 616d 2062 6f74  tom Telegram bot
+000023c0: 7329 203c 6272 3e0d 0a2d 2062 2e20 5479  s) <br>..- b. Ty
+000023d0: 7065 202f 6e65 7762 6f74 2074 6f20 6372  pe /newbot to cr
+000023e0: 6561 7465 2061 206e 6577 2062 6f74 203c  eate a new bot <
+000023f0: 6272 3e0d 0a2d 2063 2e20 4769 7665 2079  br>..- c. Give y
+00002400: 6f75 7220 626f 7420 6120 6e61 6d65 2026  our bot a name &
+00002410: 2061 2075 7365 726e 616d 6520 3c62 723e   a username <br>
+00002420: 0d0a 2d20 642e 2043 6f70 7920 796f 7572  ..- d. Copy your
+00002430: 206e 6577 2054 656c 6567 7261 6d20 626f   new Telegram bo
+00002440: 74e2 8099 7320 746f 6b65 6e20 3c62 723e  t...s token <br>
+00002450: 0d0a 0d0a 466f 7220 6d6f 7265 2069 6e66  ....For more inf
+00002460: 6f6d 6174 696f 6e2c 2076 6973 6974 205b  omation, visit [
+00002470: 5465 6c65 6772 616d 2042 6f74 2046 6174  Telegram Bot Fat
+00002480: 6865 7220 4150 495d 2868 7474 7073 3a2f  her API](https:/
+00002490: 2f63 6f72 652e 7465 6c65 6772 616d 2e6f  /core.telegram.o
+000024a0: 7267 2f62 6f74 732f 6170 6929 0d0a 3c62  rg/bots/api)..<b
+000024b0: 723e 3c62 723e 0d0a 200d 0a23 2323 2061  r><br>.. ..### a
+000024c0: 2e20 5769 7468 6f75 7420 4f70 656e 4149  . Without OpenAI
+000024d0: 2041 5049 0d0a 0d0a 6060 6070 7974 686f   API....```pytho
+000024e0: 6e0d 0a66 726f 6d20 4578 6365 7074 4e6f  n..from ExceptNo
+000024f0: 7469 6669 6572 2069 6d70 6f72 7420 4578  tifier import Ex
+00002500: 6365 7074 5465 6c65 6772 616d 2c20 5375  ceptTelegram, Su
+00002510: 6363 6573 7354 656c 6567 7261 6d2c 2053  ccessTelegram, S
+00002520: 656e 6454 656c 6567 7261 6d0d 0a69 6d70  endTelegram..imp
+00002530: 6f72 7420 7379 730d 0a73 7973 2e65 7863  ort sys..sys.exc
+00002540: 6570 7468 6f6f 6b20 3d20 4578 6365 7074  epthook = Except
+00002550: 5465 6c65 6772 616d 2e5f 5f63 616c 6c5f  Telegram.__call_
+00002560: 5f0d 0a0d 0a5f 5445 4c45 4752 414d 5f54  _...._TELEGRAM_T
+00002570: 4f4b 454e 203d 2022 7878 7878 220d 0a0d  OKEN = "xxxx"...
+00002580: 0a74 7279 3a0d 0a20 2020 2070 7269 6e74  .try:..    print
+00002590: 2831 2f30 2920 200d 0a20 2020 2053 7563  (1/0)  ..    Suc
+000025a0: 6365 7373 5465 6c65 6772 616d 2829 2e5f  cessTelegram()._
+000025b0: 5f63 616c 6c5f 5f28 2920 2331 2e20 7375  _call__() #1. su
+000025c0: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
+000025d0: 2020 2020 2020 0d0a 0d0a 6578 6365 7074        ....except
+000025e0: 2045 7863 6570 7454 656c 6567 7261 6d20   ExceptTelegram 
+000025f0: 6173 2065 3a20 2020 2020 2023 322e 2065  as e:      #2. e
+00002600: 7863 6570 7420 7365 6e64 6572 2020 2020  xcept sender    
+00002610: 2020 2020 2020 2020 0d0a 2020 2020 7379          ..    sy
+00002620: 732e 6578 6974 2829 0d0a 0d0a 5365 6e64  s.exit()....Send
+00002630: 5465 6c65 6772 616d 2829 2e5f 5f63 616c  Telegram().__cal
+00002640: 6c5f 5f28 2920 2020 2020 2020 2023 332e  l__()        #3.
+00002650: 2063 7573 746f 6d69 7a65 6420 7365 6e64   customized send
+00002660: 6572 2020 2020 200d 0a60 6060 0d0a 0d0a  er     ..```....
+00002670: 0d0a 215b 5d28 6874 7470 733a 2f2f 6769  ..![](https://gi
+00002680: 7468 7562 2e63 6f6d 2f64 7364 616e 6965  thub.com/dsdanie
+00002690: 6c70 6172 6b2f 4578 6365 7074 4e6f 7469  lpark/ExceptNoti
+000026a0: 6669 6572 2f62 6c6f 622f 6d61 696e 2f61  fier/blob/main/a
+000026b0: 7373 6574 732f 696d 6773 2f66 6967 3434  ssets/imgs/fig44
+000026c0: 2e70 6e67 290d 0a0d 0a0d 0a23 2323 2062  .png)......### b
+000026d0: 2e20 5769 7468 204f 7065 6e41 4920 4150  . With OpenAI AP
+000026e0: 490d 0a60 6060 7079 7468 6f6e 0d0a 6672  I..```python..fr
+000026f0: 6f6d 2045 7863 6570 744e 6f74 6966 6965  om ExceptNotifie
+00002700: 7220 696d 706f 7274 2045 7863 6570 7454  r import ExceptT
+00002710: 656c 6567 7261 6d2c 2053 7563 6365 7373  elegram, Success
+00002720: 5465 6c65 6772 616d 2c20 5365 6e64 5465  Telegram, SendTe
+00002730: 6c65 6772 616d 0d0a 696d 706f 7274 2073  legram..import s
+00002740: 7973 0d0a 7379 732e 6578 6365 7074 686f  ys..sys.exceptho
+00002750: 6f6b 203d 2045 7863 6570 7454 656c 6567  ok = ExceptTeleg
+00002760: 7261 6d2e 5f5f 6361 6c6c 5f5f 0d0a 0d0a  ram.__call__....
+00002770: 5f54 454c 4547 5241 4d5f 544f 4b45 4e20  _TELEGRAM_TOKEN 
+00002780: 3d20 2278 7878 7822 0d0a 5f4f 5045 4e5f  = "xxxx".._OPEN_
+00002790: 4149 5f4d 4f44 454c 3d22 6770 742d 332e  AI_MODEL="gpt-3.
+000027a0: 352d 7475 7262 6f22 0d0a 5f4f 5045 4e5f  5-turbo".._OPEN_
+000027b0: 4149 5f41 5049 3d22 736b 2d78 7878 7878  AI_API="sk-xxxxx
+000027c0: 7822 0d0a 0d0a 7472 793a 0d0a 2020 2020  x"....try:..    
+000027d0: 7072 696e 7428 312f 3029 2020 0d0a 2020  print(1/0)  ..  
+000027e0: 2020 5375 6363 6573 7354 656c 6567 7261    SuccessTelegra
+000027f0: 6d28 292e 5f5f 6361 6c6c 5f5f 2829 2023  m().__call__() #
+00002800: 312e 2073 7563 6365 7373 2073 656e 6465  1. success sende
+00002810: 7220 2020 2020 2020 2020 200d 0a0d 0a65  r          ....e
+00002820: 7863 6570 7420 4578 6365 7074 5465 6c65  xcept ExceptTele
+00002830: 6772 616d 2061 7320 653a 2020 2020 2020  gram as e:      
+00002840: 2332 2e20 6578 6365 7074 2073 656e 6465  #2. except sende
+00002850: 7220 2020 2020 2020 2020 2020 200d 0a20  r            .. 
+00002860: 2020 2073 7973 2e65 7869 7428 290d 0a0d     sys.exit()...
+00002870: 0a53 656e 6454 656c 6567 7261 6d28 292e  .SendTelegram().
+00002880: 5f5f 6361 6c6c 5f5f 2829 2020 2020 2020  __call__()      
+00002890: 2020 2333 2e20 6375 7374 6f6d 697a 6564    #3. customized
+000028a0: 2073 656e 6465 7220 2020 2020 0d0a 0d0a   sender     ....
+000028b0: 6060 600d 0a3c 6272 3e0d 0a0d 0a23 2320  ```..<br>....## 
+000028c0: 322d 322e 202a 4d61 696c 204e 6f74 6966  2-2. *Mail Notif
+000028d0: 6965 722a 0d0a 496e 2074 6865 2065 7863  ier*..In the exc
+000028e0: 6570 7420 7374 6174 656d 656e 742c 2061  ept statement, a
+000028f0: 6e20 656d 6169 6c20 6973 2073 656e 7420  n email is sent 
+00002900: 616c 6f6e 6720 7769 7468 2074 6865 2065  along with the e
+00002910: 7272 6f72 206d 6573 7361 6765 2e20 4164  rror message. Ad
+00002920: 6469 7469 6f6e 616c 6c79 2c20 796f 7520  ditionally, you 
+00002930: 6361 6e20 7365 6e64 2065 6d61 696c 7320  can send emails 
+00002940: 6672 6f6d 2061 6e79 2064 6573 6972 6564  from any desired
+00002950: 206c 696e 652e 203c 6272 3e0d 0a2d 2061   line. <br>..- a
+00002960: 2e20 4c6f 6720 696e 2077 6974 6820 7468  . Log in with th
+00002970: 6520 7365 6e64 6572 2773 2065 6d61 696c  e sender's email
+00002980: 2049 442e 203c 6272 3e0d 0a2d 2062 2e20   ID. <br>..- b. 
+00002990: 4f62 7461 696e 2061 6e20 6170 7020 7061  Obtain an app pa
+000029a0: 7373 776f 7264 2066 6f72 2073 656e 6469  ssword for sendi
+000029b0: 6e67 2047 6f6f 676c 6520 4d61 696c 2061  ng Google Mail a
+000029c0: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
+000029d0: 5b6c 696e 6b5d 2868 7474 7073 3a2f 2f6d  [link](https://m
+000029e0: 7961 6363 6f75 6e74 2e67 6f6f 676c 652e  yaccount.google.
+000029f0: 636f 6d2f 752f 332f 6170 7070 6173 7377  com/u/3/apppassw
+00002a00: 6f72 6473 3f75 746d 5f73 6f75 7263 653d  ords?utm_source=
+00002a10: 676f 6f67 6c65 2d61 6363 6f75 6e74 2675  google-account&u
+00002a20: 746d 5f6d 6564 6975 6d3d 6d79 6163 636f  tm_medium=myacco
+00002a30: 756e 7473 6563 7572 6974 7926 7574 6d5f  untsecurity&utm_
+00002a40: 6361 6d70 6169 676e 3d74 7376 2d73 6574  campaign=tsv-set
+00002a50: 7469 6e67 7326 7261 7074 3d41 456a 484c  tings&rapt=AEjHL
+00002a60: 344e 3262 4d52 574f 3436 5661 4d70 5f6a  4N2bMRWO46VaMp_j
+00002a70: 5030 367a 514b 3134 4257 4e50 7636 366c  P06zQK14BWNPv66l
+00002a80: 326f 3539 694a 3939 436b 4f38 426a 596e  2o59iJ99CkO8BjYn
+00002a90: 6d6f 5255 6539 6474 5363 686b 6b62 7562  moRUe9dtSchkkbub
+00002aa0: 485a 4d55 6865 766b 416e 7756 4a52 4862  HZMUhevkAnwVJRHb
+00002ab0: 3979 674f 3361 6669 7370 4e6c 7729 206f  9ygO3afispNlw) o
+00002ac0: 7220 5b67 6f6f 676c 6520 646f 6375 6d65  r [google docume
+00002ad0: 6e74 5d28 6874 7470 733a 2f2f 7375 7070  nt](https://supp
+00002ae0: 6f72 742e 676f 6f67 6c65 2e63 6f6d 2f61  ort.google.com/a
+00002af0: 6363 6f75 6e74 732f 616e 7377 6572 2f31  ccounts/answer/1
+00002b00: 3835 3833 333f 686c 3d65 6e29 2e20 0d0a  85833?hl=en). ..
+00002b10: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
+00002b20: 6f72 7420 7379 730d 0a66 726f 6d20 4578  ort sys..from Ex
+00002b30: 6365 7074 4e6f 7469 6669 6572 2069 6d70  ceptNotifier imp
+00002b40: 6f72 7420 4578 6365 7074 4d61 696c 2c20  ort ExceptMail, 
+00002b50: 5375 6363 6573 734d 6169 6c2c 2053 656e  SuccessMail, Sen
+00002b60: 644d 6169 6c0d 0a73 7973 2e65 7863 6570  dMail..sys.excep
+00002b70: 7468 6f6f 6b20 3d20 4578 6365 7074 4d61  thook = ExceptMa
+00002b80: 696c 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  il.__call__....#
+00002b90: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00002ba0: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00002bb0: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00002bc0: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00002bd0: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+00002be0: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+00002bf0: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+00002c00: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+00002c10: 7878 7822 0d0a 5f47 414d 494c 5f52 4543  xxx".._GAMIL_REC
+00002c20: 4950 4945 4e54 5f41 4444 5220 3d20 2778  IPIENT_ADDR = 'x
+00002c30: 7878 7878 7878 4067 6d61 696c 2e63 6f6d  xxxxxx@gmail.com
+00002c40: 270d 0a5f 474d 4149 4c5f 5345 4e44 4552  '.._GMAIL_SENDER
+00002c50: 5f41 4444 5220 3d20 2779 7979 7979 7940  _ADDR = 'yyyyyy@
+00002c60: 676d 6169 6c2e 636f 6d27 0d0a 5f47 4d41  gmail.com'.._GMA
+00002c70: 494c 5f41 5050 5f50 4153 5357 4f52 445f  IL_APP_PASSWORD_
+00002c80: 4f46 5f53 454e 4445 5220 3d20 277a 7a7a  OF_SENDER = 'zzz
+00002c90: 7a7a 7a27 0d0a 0d0a 7472 793a 0d0a 2020  zzz'....try:..  
+00002ca0: 2020 6d61 696e 2829 2020 2020 2020 2020    main()        
+00002cb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002cc0: 596f 7572 2043 6f64 6520 4865 7265 0d0a  Your Code Here..
+00002cd0: 2020 2020 5375 6363 6573 734d 6169 6c28      SuccessMail(
+00002ce0: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
+00002cf0: 2320 4e6f 2045 7863 6570 7469 6f6e 202d  # No Exception -
+00002d00: 3e20 5365 6e64 2053 7563 6365 7373 206d  > Send Success m
+00002d10: 6169 6c2e 0d0a 6578 6365 7074 2045 7863  ail...except Exc
+00002d20: 6570 744d 6169 6c3a 2020 2020 2020 2020  eptMail:        
+00002d30: 2020 2020 2020 2320 4578 6365 7074 696f        # Exceptio
+00002d40: 6e20 2d3e 2053 656e 6420 4661 696c 206d  n -> Send Fail m
+00002d50: 6169 6c2e 0d0a 2020 2020 7061 7373 0d0a  ail...    pass..
+00002d60: 0d0a 5365 6e64 4d61 696c 2829 2e5f 5f63  ..SendMail().__c
+00002d70: 616c 6c5f 5f28 2920 2020 2020 2020 2020  all__()         
+00002d80: 2020 2320 5768 656e 2050 726f 6365 7373    # When Process
+00002d90: 2045 6e64 6564 202d 3e20 416e 7920 4c69   Ended -> Any Li
+00002da0: 6e65 206d 6169 6c2e 0d0a 6060 600d 0a0d  ne mail...```...
+00002db0: 0a3c 6465 7461 696c 733e 0d0a 3c73 756d  .<details>..<sum
+00002dc0: 6d61 7279 3e20 5365 6520 4578 616d 706c  mary> See Exampl
+00002dd0: 652e 2e2e 3c2f 7375 6d6d 6172 793e 0d0a  e...</summary>..
+00002de0: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
+00002df0: 6f72 7420 7379 730d 0a66 726f 6d20 4578  ort sys..from Ex
+00002e00: 6365 7074 4e6f 7469 6669 6572 2069 6d70  ceptNotifier imp
+00002e10: 6f72 7420 4578 6365 7074 4d61 696c 2c20  ort ExceptMail, 
+00002e20: 5375 6363 6573 734d 6169 6c2c 2053 656e  SuccessMail, Sen
+00002e30: 644d 6169 6c0d 0a0d 0a23 2044 6566 696e  dMail....# Defin
+00002e40: 6520 7468 6520 6e65 7874 2074 776f 2076  e the next two v
+00002e50: 6172 6961 626c 6573 206f 7074 696f 6e61  ariables optiona
+00002e60: 6c6c 7920 7768 656e 2075 7369 6e67 204f  lly when using O
+00002e70: 7065 6e41 4927 7320 4150 492e 0d0a 2320  penAI's API...# 
+00002e80: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 3d22  _OPEN_AI_MODEL="
+00002e90: 6770 742d 332e 352d 7475 7262 6f22 2020  gpt-3.5-turbo"  
+00002ea0: 2020 0d0a 2320 5f4f 5045 4e5f 4149 5f41    ..# _OPEN_AI_A
+00002eb0: 5049 3d22 736b 2d78 7878 7878 7822 0d0a  PI="sk-xxxxxx"..
+00002ec0: 5f47 414d 494c 5f52 4543 4950 4945 4e54  _GAMIL_RECIPIENT
+00002ed0: 5f41 4444 5220 3d20 2778 7878 7878 7878  _ADDR = 'xxxxxxx
+00002ee0: 4067 6d61 696c 2e63 6f6d 270d 0a5f 474d  @gmail.com'.._GM
+00002ef0: 4149 4c5f 5345 4e44 4552 5f41 4444 5220  AIL_SENDER_ADDR 
+00002f00: 3d20 2779 7979 7979 7940 676d 6169 6c2e  = 'yyyyyy@gmail.
+00002f10: 636f 6d27 0d0a 5f47 4d41 494c 5f41 5050  com'.._GMAIL_APP
+00002f20: 5f50 4153 5357 4f52 445f 4f46 5f53 454e  _PASSWORD_OF_SEN
+00002f30: 4445 5220 3d20 277a 7a7a 7a7a 7a27 0d0a  DER = 'zzzzzz'..
+00002f40: 0d0a 7379 732e 6578 6365 7074 686f 6f6b  ..sys.excepthook
+00002f50: 203d 2045 7863 6570 744d 6169 6c2e 5f5f   = ExceptMail.__
+00002f60: 6361 6c6c 5f5f 0d0a 0d0a 7472 793a 0d0a  call__....try:..
+00002f70: 2020 2020 2320 3032 2e4c 6f63 6174 6520      # 02.Locate 
+00002f80: 796f 7572 2063 6f64 650d 0a20 2020 2070  your code..    p
+00002f90: 7269 6e74 2831 2f30 2920 2020 0d0a 2020  rint(1/0)   ..  
+00002fa0: 2020 5375 6363 6573 734d 6169 6c28 292e    SuccessMail().
+00002fb0: 5f5f 6361 6c6c 5f5f 2829 2020 2023 2053  __call__()   # S
+00002fc0: 7563 6365 7373 204d 6169 6c0d 0a0d 0a65  uccess Mail....e
+00002fd0: 7863 6570 7420 4578 6365 7074 4d61 696c  xcept ExceptMail
+00002fe0: 2061 7320 653a 2020 2020 2020 2020 2320   as e:        # 
+00002ff0: 4578 6365 7074 696f 6e20 4d61 696c 2020  Exception Mail  
+00003000: 2020 2020 200d 0a20 2020 2073 7973 2e65       ..    sys.e
+00003010: 7869 7428 290d 0a20 2020 2070 7269 6e74  xit()..    print
+00003020: 2865 290d 0a0d 0a53 656e 644d 6169 6c28  (e)....SendMail(
+00003030: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
+00003040: 2020 2020 2020 2320 5075 7420 416e 7920        # Put Any 
+00003050: 4c69 6e65 3a20 5365 6e64 696e 6720 6d61  Line: Sending ma
+00003060: 696c 0d0a 6060 600d 0a3c 2f64 6574 6169  il..```..</detai
+00003070: 6c73 3e0d 0a0d 0a3c 6465 7461 696c 733e  ls>....<details>
+00003080: 0d0a 3c73 756d 6d61 7279 3e20 536e 6970  ..<summary> Snip
+00003090: 7065 7420 666f 7220 5079 7468 6f6e 2064  pet for Python d
+000030a0: 6576 656c 6f70 6572 732e 2e2e 3c2f 7375  evelopers...</su
+000030b0: 6d6d 6172 793e 0d0a 0d0a 6060 6070 7974  mmary>....```pyt
+000030c0: 686f 6e0d 0a69 6d70 6f72 7420 7379 730d  hon..import sys.
+000030d0: 0a66 726f 6d20 4578 6365 7074 4e6f 7469  .from ExceptNoti
+000030e0: 6669 6572 2069 6d70 6f72 7420 4578 6365  fier import Exce
+000030f0: 7074 4d61 696c 2c20 5375 6363 6573 734d  ptMail, SuccessM
+00003100: 6169 6c2c 2053 656e 644d 6169 6c0d 0a73  ail, SendMail..s
+00003110: 7973 2e65 7863 6570 7468 6f6f 6b20 3d20  ys.excepthook = 
+00003120: 4578 6365 7074 4d61 696c 2e5f 5f63 616c  ExceptMail.__cal
+00003130: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+00003140: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00003150: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00003160: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00003170: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00003180: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00003190: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+000031a0: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+000031b0: 3d22 736b 2d78 7878 7878 7822 0d0a 5f47  ="sk-xxxxxx".._G
+000031c0: 414d 494c 5f52 4543 4950 4945 4e54 5f41  AMIL_RECIPIENT_A
+000031d0: 4444 5220 3d20 2778 7878 7878 7878 4067  DDR = 'xxxxxxx@g
+000031e0: 6d61 696c 2e63 6f6d 270d 0a5f 474d 4149  mail.com'.._GMAI
+000031f0: 4c5f 5345 4e44 4552 5f41 4444 5220 3d20  L_SENDER_ADDR = 
+00003200: 2779 7979 7979 7940 676d 6169 6c2e 636f  'yyyyyy@gmail.co
+00003210: 6d27 0d0a 5f47 4d41 494c 5f41 5050 5f50  m'.._GMAIL_APP_P
+00003220: 4153 5357 4f52 445f 4f46 5f53 454e 4445  ASSWORD_OF_SENDE
+00003230: 5220 3d20 277a 7a7a 7a7a 7a27 0d0a 0d0a  R = 'zzzzzz'....
+00003240: 7472 793a 0d0a 2020 2020 2779 6f75 7220  try:..    'your 
+00003250: 636f 6465 270d 0a20 2020 2053 7563 6365  code'..    Succe
+00003260: 7373 4d61 696c 2829 2e5f 5f63 616c 6c5f  ssMail().__call_
+00003270: 5f28 290d 0a65 7863 6570 7420 4578 6365  _()..except Exce
+00003280: 7074 4d61 696c 3a0d 0a20 2020 2070 6173  ptMail:..    pas
+00003290: 730d 0a0d 0a53 656e 644d 6169 6c28 292e  s....SendMail().
+000032a0: 5f5f 6361 6c6c 5f5f 2829 200d 0a60 6060  __call__() ..```
+000032b0: 0d0a 3c2f 6465 7461 696c 733e 0d0a 0d0a  ..</details>....
+000032c0: 3c62 723e 0d0a 0d0a 2323 2032 2d33 2e20  <br>....## 2-3. 
+000032d0: 2a44 6973 636f 7264 204e 6f74 6966 6965  *Discord Notifie
+000032e0: 722a 0d0a 2d20 612e 2053 656c 6563 7420  r*..- a. Select 
+000032f0: 7468 6520 6368 616e 6e65 6c20 746f 2072  the channel to r
+00003300: 6563 6569 7665 206e 6f74 6966 6963 6174  eceive notificat
+00003310: 696f 6e73 2e0d 0a2d 2062 2e20 436c 6963  ions...- b. Clic
+00003320: 6b20 2245 6469 7420 4368 616e 6e65 6c22  k "Edit Channel"
+00003330: 2069 6e20 7468 6520 7570 7065 7220 7269   in the upper ri
+00003340: 6768 7420 636f 726e 6572 206f 6620 7468  ght corner of th
+00003350: 6520 6368 6174 2077 696e 646f 772e 0d0a  e chat window...
+00003360: 2d20 632e 2043 6c69 636b 2049 6e74 6567  - c. Click Integ
+00003370: 7261 7469 6f6e 7320 2d20 5765 6268 6f6f  rations - Webhoo
+00003380: 6b20 2d20 4e65 7720 5765 6268 6f6f 6b2e  k - New Webhook.
+00003390: 0d0a 2d20 642e 2054 6865 6e20 636c 6963  ..- d. Then clic
+000033a0: 6b20 436f 7079 2057 6562 686f 6f6b 2e0d  k Copy Webhook..
+000033b0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 696d  ...```python..im
+000033c0: 706f 7274 2073 7973 0d0a 6672 6f6d 2045  port sys..from E
+000033d0: 7863 6570 744e 6f74 6966 6965 7220 696d  xceptNotifier im
+000033e0: 706f 7274 2045 7863 6570 7444 6973 636f  port ExceptDisco
+000033f0: 7264 2c20 5375 6363 6573 7344 6973 636f  rd, SuccessDisco
+00003400: 7264 2c20 5365 6e64 4469 7363 6f72 640d  rd, SendDiscord.
+00003410: 0a73 7973 2e65 7863 6570 7468 6f6f 6b20  .sys.excepthook 
+00003420: 3d20 4578 6365 7074 4469 7363 6f72 642e  = ExceptDiscord.
+00003430: 5f5f 6361 6c6c 5f5f 0d0a 0d0a 2320 4465  __call__....# De
+00003440: 6669 6e65 2074 6865 206e 6578 7420 7477  fine the next tw
+00003450: 6f20 7661 7269 6162 6c65 7320 6f70 7469  o variables opti
+00003460: 6f6e 616c 6c79 2077 6865 6e20 7573 696e  onally when usin
+00003470: 6720 4f70 656e 4149 2773 2041 5049 2e0d  g OpenAI's API..
+00003480: 0a23 205f 4f50 454e 5f41 495f 4d4f 4445  .# _OPEN_AI_MODE
+00003490: 4c3d 2267 7074 2d33 2e35 2d74 7572 626f  L="gpt-3.5-turbo
+000034a0: 2220 2020 200d 0a23 205f 4f50 454e 5f41  "    ..# _OPEN_A
+000034b0: 495f 4150 493d 2273 6b2d 7878 7878 7878  I_API="sk-xxxxxx
+000034c0: 220d 0a5f 4449 5343 4f52 445f 5745 4248  ".._DISCORD_WEBH
+000034d0: 4f4f 4b5f 5552 4c20 3d20 2278 7878 7878  OOK_URL = "xxxxx
+000034e0: 7878 7878 7878 7878 7878 7878 220d 0a0d  xxxxxxxxxxxx"...
+000034f0: 0a0d 0a74 7279 3a0d 0a20 2020 2070 7269  ...try:..    pri
+00003500: 6e74 2831 2f32 3029 2020 0d0a 2020 2020  nt(1/20)  ..    
+00003510: 5375 6363 6573 7344 6973 636f 7264 2829  SuccessDiscord()
+00003520: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2073  .__call__() #1 s
+00003530: 7563 6365 7373 2073 656e 6465 7220 2020  uccess sender   
+00003540: 2020 2020 2020 200d 0a65 7863 6570 7420         ..except 
+00003550: 4578 6365 7074 4469 7363 6f72 6420 6173  ExceptDiscord as
+00003560: 2065 3a20 2020 2020 2023 3220 6578 6365   e:      #2 exce
+00003570: 7074 2073 656e 6465 7220 2020 2020 2020  pt sender       
+00003580: 2020 2020 200d 0a20 2020 2073 7973 2e65       ..    sys.e
+00003590: 7869 7428 290d 0a0d 0a53 656e 6444 6973  xit()....SendDis
+000035a0: 636f 7264 2829 2e5f 5f63 616c 6c5f 5f28  cord().__call__(
+000035b0: 2920 2020 2020 2020 2023 3320 6375 7374  )        #3 cust
+000035c0: 6f6d 697a 6564 2073 656e 6465 7220 2020  omized sender   
+000035d0: 2020 2020 0d0a 6060 600d 0a0d 0a3c 6272      ..```....<br
+000035e0: 3e0d 0a0d 0a23 2320 322d 342e 202a 4368  >....## 2-4. *Ch
+000035f0: 696d 6520 4e6f 7469 6669 6572 2a0d 0a2d  ime Notifier*..-
+00003600: 2061 2e20 5365 6c65 6374 2074 6865 2043   a. Select the C
+00003610: 6861 7420 726f 6f6d 2074 6f20 7265 6365  hat room to rece
+00003620: 6976 6520 6e6f 7469 6669 6361 7469 6f6e  ive notification
+00003630: 732e 0d0a 2d20 622e 2043 6c69 636b 2022  s...- b. Click "
+00003640: 526f 6f6d 2053 6574 7469 6e67 2220 696e  Room Setting" in
+00003650: 2074 6865 2075 7070 6572 2072 6967 6874   the upper right
+00003660: 2063 6f72 6e65 722e 0d0a 2d20 632e 2043   corner...- c. C
+00003670: 6c69 636b 2022 4d61 6e61 6765 2057 6562  lick "Manage Web
+00003680: 686f 6f6b 2061 6e64 2062 6f74 2e22 0d0a  hook and bot."..
+00003690: 2d20 642e 2043 7265 6174 6520 4164 6420  - d. Create Add 
+000036a0: 5765 6268 6f6f 6b2c 2073 6574 2069 7420  Webhook, set it 
+000036b0: 7570 2c20 7468 656e 2063 6c69 636b 2043  up, then click C
+000036c0: 6f70 7920 5765 6268 6f6f 6b2e 0d0a 6060  opy Webhook...``
+000036d0: 6070 7974 686f 6e0d 0a69 6d70 6f72 7420  `python..import 
+000036e0: 7379 730d 0a66 726f 6d20 4578 6365 7074  sys..from Except
+000036f0: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
+00003700: 5375 6363 6573 7343 6869 6d65 2c20 4578  SuccessChime, Ex
+00003710: 6365 7074 4368 696d 652c 2053 656e 6443  ceptChime, SendC
+00003720: 6869 6d65 0d0a 7379 732e 6578 6365 7074  hime..sys.except
+00003730: 686f 6f6b 203d 2045 7863 6570 7443 6869  hook = ExceptChi
+00003740: 6d65 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  me.__call__....#
+00003750: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00003760: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00003770: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00003780: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00003790: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+000037a0: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+000037b0: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+000037c0: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+000037d0: 7878 7822 0d0a 5f43 4849 4d45 5f57 4542  xxx".._CHIME_WEB
+000037e0: 484f 4f4b 5f55 524c 203d 2022 7878 7878  HOOK_URL = "xxxx
+000037f0: 7878 7878 7878 7878 7878 7878 7878 220d  xxxxxxxxxxxxxx".
+00003800: 0a0d 0a0d 0a74 7279 3a0d 0a20 2020 2070  .....try:..    p
+00003810: 7269 6e74 2831 2f30 2920 200d 0a20 2020  rint(1/0)  ..   
+00003820: 2053 7563 6365 7373 4368 696d 6528 292e   SuccessChime().
+00003830: 5f5f 6361 6c6c 5f5f 2829 2023 3120 7375  __call__() #1 su
+00003840: 6363 6573 7320 7365 6e64 6572 2020 2020  ccess sender    
+00003850: 2020 2020 2020 0d0a 6578 6365 7074 2045        ..except E
+00003860: 7863 6570 7443 6869 6d65 2061 7320 653a  xceptChime as e:
+00003870: 2020 2020 2020 2332 2065 7863 6570 7420        #2 except 
+00003880: 7365 6e64 6572 2020 2020 2020 2020 2020  sender          
+00003890: 2020 0d0a 2020 2020 7379 732e 6578 6974    ..    sys.exit
+000038a0: 2829 0d0a 0d0a 5365 6e64 4368 696d 6528  ()....SendChime(
+000038b0: 292e 5f5f 6361 6c6c 5f5f 2829 2020 2020  ).__call__()    
+000038c0: 2020 2020 2333 2063 7573 746f 6d69 7a65      #3 customize
+000038d0: 6420 7365 6e64 6572 2020 2020 2020 200d  d sender       .
+000038e0: 0a60 6060 0d0a 3c62 723e 0d0a 0d0a 2323  .```..<br>....##
+000038f0: 2032 2d35 2e20 2a53 6c61 636b 204e 6f74   2-5. *Slack Not
+00003900: 6966 6965 722a 0d0a 2d20 612e 2076 6973  ifier*..- a. vis
+00003910: 6974 2068 7474 7073 3a2f 2f61 7069 2e73  it https://api.s
+00003920: 6c61 636b 2e63 6f6d 2f0d 0a2d 2062 2e20  lack.com/..- b. 
+00003930: 6043 7265 6174 6520 616e 2061 7070 6020  `Create an app` 
+00003940: 2d20 6046 726f 6d20 7363 7261 7463 6860  - `From scratch`
+00003950: 202d 2060 4372 6561 7465 2041 7070 600d   - `Create App`.
+00003960: 0a2d 2063 2e20 4164 6420 7765 6268 6f6f  .- c. Add webhoo
+00003970: 6b3a 2043 6c69 636b 2060 496e 636f 6d69  k: Click `Incomi
+00003980: 6e67 2057 6562 686f 6f6b 7360 202d 2041  ng Webhooks` - A
+00003990: 6374 6976 6174 6520 496e 636f 6d6d 696e  ctivate Incommin
+000039a0: 6720 604f 6e60 202d 2041 6464 204e 6577  g `On` - Add New
+000039b0: 2057 6562 686f 6f6b 2074 6f20 576f 726b   Webhook to Work
+000039c0: 7370 6163 650d 0a2d 2064 2e20 436f 7079  space..- d. Copy
+000039d0: 2060 5765 6268 6f6f 6b20 5552 4c60 0d0a   `Webhook URL`..
+000039e0: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
+000039f0: 6f72 7420 7379 730d 0a66 726f 6d20 4578  ort sys..from Ex
+00003a00: 6365 7074 4e6f 7469 6669 6572 2069 6d70  ceptNotifier imp
+00003a10: 6f72 7420 4578 6365 7074 536c 6163 6b2c  ort ExceptSlack,
+00003a20: 2053 7563 6365 7373 536c 6361 6b2c 2053   SuccessSlcak, S
+00003a30: 656e 6453 6c61 636b 0d0a 7379 732e 6578  endSlack..sys.ex
+00003a40: 6365 7074 686f 6f6b 203d 2045 7863 6570  cepthook = Excep
+00003a50: 7453 6c61 636b 2e5f 5f63 616c 6c5f 5f0d  tSlack.__call__.
+00003a60: 0a0d 0a23 2044 6566 696e 6520 7468 6520  ...# Define the 
+00003a70: 6e65 7874 2074 776f 2076 6172 6961 626c  next two variabl
+00003a80: 6573 206f 7074 696f 6e61 6c6c 7920 7768  es optionally wh
+00003a90: 656e 2075 7369 6e67 204f 7065 6e41 4927  en using OpenAI'
+00003aa0: 7320 4150 492e 0d0a 2320 5f4f 5045 4e5f  s API...# _OPEN_
+00003ab0: 4149 5f4d 4f44 454c 3d22 6770 742d 332e  AI_MODEL="gpt-3.
+00003ac0: 352d 7475 7262 6f22 2020 2020 0d0a 2320  5-turbo"    ..# 
+00003ad0: 5f4f 5045 4e5f 4149 5f41 5049 3d22 736b  _OPEN_AI_API="sk
+00003ae0: 2d78 7878 7878 7822 0d0a 5f53 4c41 434b  -xxxxxx".._SLACK
+00003af0: 5f57 4542 484f 4f4b 5f55 524c 203d 2027  _WEBHOOK_URL = '
+00003b00: 6874 7470 733a 2f2f 686f 6f6b 732e 736c  https://hooks.sl
+00003b10: 6163 6b2e 636f 6d2f 7365 7276 6963 6573  ack.com/services
+00003b20: 2f78 7878 7878 7878 7878 7878 7878 7878  /xxxxxxxxxxxxxxx
+00003b30: 7878 7878 270d 0a0d 0a74 7279 3a0d 0a20  xxxx'....try:.. 
+00003b40: 2020 2070 7269 6e74 2831 2f30 2920 200d     print(1/0)  .
+00003b50: 0a20 2020 2053 7563 6365 7373 536c 6361  .    SuccessSlca
+00003b60: 6b28 292e 5f5f 6361 6c6c 5f5f 2829 2023  k().__call__() #
+00003b70: 3120 7375 6363 6573 7320 7365 6e64 6572  1 success sender
+00003b80: 2020 2020 2020 2020 2020 0d0a 6578 6365            ..exce
+00003b90: 7074 2045 7863 6570 7453 6c61 636b 2061  pt ExceptSlack a
+00003ba0: 7320 653a 2020 2020 2020 2332 2065 7863  s e:      #2 exc
+00003bb0: 6570 7420 7365 6e64 6572 2020 2020 2020  ept sender      
+00003bc0: 2020 2020 2020 0d0a 2020 2020 7379 732e        ..    sys.
+00003bd0: 6578 6974 2829 0d0a 0d0a 5365 6e64 536c  exit()....SendSl
+00003be0: 6163 6b28 292e 5f5f 6361 6c6c 5f5f 2829  ack().__call__()
+00003bf0: 2020 2020 2020 2020 2333 2063 7573 746f          #3 custo
+00003c00: 6d69 7a65 6420 7365 6e64 6572 2020 2020  mized sender    
+00003c10: 200d 0a60 6060 0d0a 3c42 723e 0d0a 0d0a   ..```..<Br>....
+00003c20: 2323 2032 2d36 2e20 2a4c 696e 6520 4e6f  ## 2-6. *Line No
+00003c30: 7469 6669 6572 2a0d 0a2d 2061 2e20 5265  tifier*..- a. Re
+00003c40: 6769 7374 6572 205b 6874 7470 733a 2f2f  gister [https://
+00003c50: 6e6f 7469 6679 2d62 6f74 2e6c 696e 652e  notify-bot.line.
+00003c60: 6d65 2f5d 2868 7474 7073 3a2f 2f6e 6f74  me/](https://not
+00003c70: 6966 792d 626f 742e 6c69 6e65 2e6d 652f  ify-bot.line.me/
+00003c80: 290d 0a2d 2062 2e20 476f 2074 6f20 6d79  )..- b. Go to my
+00003c90: 7061 6765 205b 6874 7470 733a 2f2f 6e6f  page [https://no
+00003ca0: 7469 6679 2d62 6f74 2e6c 696e 652e 6d65  tify-bot.line.me
+00003cb0: 2f6d 792f 5d28 6874 7470 733a 2f2f 6e6f  /my/](https://no
+00003cc0: 7469 6679 2d62 6f74 2e6c 696e 652e 6d65  tify-bot.line.me
+00003cd0: 2f6d 792f 290d 0a2d 2063 2e20 436c 6963  /my/)..- c. Clic
+00003ce0: 6b20 6047 656e 6572 6174 6520 546f 6b65  k `Generate Toke
+00003cf0: 6e60 2c20 656e 7465 7220 5365 7276 6963  n`, enter Servic
+00003d00: 6520 4e61 6d65 2061 6e64 2063 6c69 636b  e Name and click
+00003d10: 2060 312d 6f6e 2d31 2063 6861 7420 7769   `1-on-1 chat wi
+00003d20: 7468 204c 494e 4560 2028 616e 7974 6869  th LINE` (anythi
+00003d30: 6e67 2079 6f75 206c 696b 6529 0d0a 2d20  ng you like)..- 
+00003d40: 642e 2043 6f70 7920 546f 6b65 6e2e 0d0a  d. Copy Token...
+00003d50: 0d0a 6060 6070 7974 686f 6e0d 0a69 6d70  ..```python..imp
+00003d60: 6f72 7420 7379 730d 0a66 726f 6d20 4578  ort sys..from Ex
+00003d70: 6365 7074 4e6f 7469 6669 6572 2069 6d70  ceptNotifier imp
+00003d80: 6f72 7420 4578 6365 7074 4c69 6e65 2c20  ort ExceptLine, 
+00003d90: 5375 6363 6573 734c 696e 652c 2053 656e  SuccessLine, Sen
+00003da0: 644c 696e 650d 0a73 7973 2e65 7863 6570  dLine..sys.excep
+00003db0: 7468 6f6f 6b20 3d20 4578 6365 7074 4c69  thook = ExceptLi
+00003dc0: 6e65 2e5f 5f63 616c 6c5f 5f0d 0a0d 0a23  ne.__call__....#
+00003dd0: 2044 6566 696e 6520 7468 6520 6e65 7874   Define the next
+00003de0: 2074 776f 2076 6172 6961 626c 6573 206f   two variables o
+00003df0: 7074 696f 6e61 6c6c 7920 7768 656e 2075  ptionally when u
+00003e00: 7369 6e67 204f 7065 6e41 4927 7320 4150  sing OpenAI's AP
+00003e10: 492e 0d0a 2320 5f4f 5045 4e5f 4149 5f4d  I...# _OPEN_AI_M
+00003e20: 4f44 454c 3d22 6770 742d 332e 352d 7475  ODEL="gpt-3.5-tu
+00003e30: 7262 6f22 2020 2020 0d0a 2320 5f4f 5045  rbo"    ..# _OPE
+00003e40: 4e5f 4149 5f41 5049 3d22 736b 2d78 7878  N_AI_API="sk-xxx
+00003e50: 7878 7822 0d0a 5f4c 494e 455f 4e4f 5449  xxx".._LINE_NOTI
+00003e60: 4659 5f41 5049 5f54 4f4b 454e 203d 2027  FY_API_TOKEN = '
+00003e70: 7878 7878 7878 7878 7878 7827 0d0a 0d0a  xxxxxxxxxxx'....
+00003e80: 7472 793a 0d0a 2020 2020 7072 696e 7428  try:..    print(
+00003e90: 312f 3230 2920 200d 0a20 2020 2053 7563  1/20)  ..    Suc
+00003ea0: 6365 7373 4c69 6e65 2829 2e5f 5f63 616c  cessLine().__cal
+00003eb0: 6c5f 5f28 2920 2331 2073 7563 6365 7373  l__() #1 success
+00003ec0: 2073 656e 6465 7220 2020 2020 2020 2020   sender         
+00003ed0: 200d 0a65 7863 6570 7420 4578 6365 7074   ..except Except
+00003ee0: 4c69 6e65 2061 7320 653a 2020 2020 2020  Line as e:      
+00003ef0: 2332 2065 7863 6570 7420 7365 6e64 6572  #2 except sender
+00003f00: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00003f10: 2020 7379 732e 6578 6974 2829 0d0a 0d0a    sys.exit()....
+00003f20: 5365 6e64 4c69 6e65 2829 2e5f 5f63 616c  SendLine().__cal
+00003f30: 6c5f 5f28 2920 2020 2020 2020 2023 3320  l__()        #3 
+00003f40: 6375 7374 6f6d 697a 6564 2073 656e 6465  customized sende
+00003f50: 7220 2020 2020 2020 2020 200d 0a60 6060  r          ..```
+00003f60: 0d0a 0d0a 3c42 723e 0d0a 0d0a 2323 2032  ....<Br>....## 2
+00003f70: 2d37 2e20 2a53 4d53 204e 6f74 6966 6965  -7. *SMS Notifie
+00003f80: 722a 0d0a 2d20 612e 2053 6967 6e20 7570  r*..- a. Sign up
+00003f90: 2066 6f72 2054 7769 6c69 6f2e 205b 6874   for Twilio. [ht
+00003fa0: 7470 733a 2f2f 7777 772e 7477 696c 696f  tps://www.twilio
+00003fb0: 2e63 6f6d 2f65 6e2d 7573 5d28 6874 7470  .com/en-us](http
+00003fc0: 733a 2f2f 7777 772e 7477 696c 696f 2e63  s://www.twilio.c
+00003fd0: 6f6d 2f65 6e2d 7573 290d 0a2d 2062 2e20  om/en-us)..- b. 
+00003fe0: 436c 6963 6b20 436f 6e73 6f6c 6520 696e  Click Console in
+00003ff0: 2074 6865 2075 7070 6572 2072 6967 6874   the upper right
+00004000: 2063 6f72 6e65 722e 0d0a 2d20 632e 2043   corner...- c. C
+00004010: 6f70 7920 7468 6520 7661 7269 6162 6c65  opy the variable
+00004020: 7320 7072 6f76 6964 6564 2069 6e20 7468  s provided in th
+00004030: 6520 636f 6e73 6f6c 652e 0d0a 0d0a 6060  e console.....``
+00004040: 6070 7974 686f 6e0d 0a69 6d70 6f72 7420  `python..import 
+00004050: 7379 730d 0a66 726f 6d20 4578 6365 7074  sys..from Except
+00004060: 4e6f 7469 6669 6572 2069 6d70 6f72 7420  Notifier import 
+00004070: 4578 6365 7074 534d 532c 2053 7563 6365  ExceptSMS, Succe
+00004080: 7373 534d 532c 2053 656e 6453 4d53 0d0a  ssSMS, SendSMS..
+00004090: 7379 732e 6578 6365 7074 686f 6f6b 203d  sys.excepthook =
+000040a0: 2045 7863 6570 7453 4d53 2e5f 5f63 616c   ExceptSMS.__cal
+000040b0: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+000040c0: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+000040d0: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+000040e0: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+000040f0: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00004100: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00004110: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00004120: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00004130: 3d22 736b 2d78 7878 7878 7822 0d0a 5f54  ="sk-xxxxxx".._T
+00004140: 5749 4c49 4f5f 5349 4420 3d20 2778 7878  WILIO_SID = 'xxx
+00004150: 7827 0d0a 5f54 5749 4c49 4f5f 544f 4b45  x'.._TWILIO_TOKE
+00004160: 4e20 3d20 2779 7979 7979 7927 0d0a 5f52  N = 'yyyyyy'.._R
+00004170: 4543 4950 4945 4e54 5f50 484f 4e45 5f4e  ECIPIENT_PHONE_N
+00004180: 554d 4245 523d 222b 6161 6161 6161 222c  UMBER="+aaaaaa",
+00004190: 0d0a 5f53 454e 4445 525f 5048 4f4e 455f  .._SENDER_PHONE_
+000041a0: 4e55 4d42 4552 3d22 2b62 6262 6262 6222  NUMBER="+bbbbbb"
+000041b0: 2c20 200d 0a0d 0a74 7279 3a0d 0a20 2020  ,  ....try:..   
+000041c0: 2070 7269 6e74 2831 2f31 3029 2020 0d0a   print(1/10)  ..
+000041d0: 2020 2020 5375 6363 6573 7353 4d53 2829      SuccessSMS()
+000041e0: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2073  .__call__() #1 s
+000041f0: 7563 6365 7373 2073 656e 6465 7220 2020  uccess sender   
+00004200: 2020 2020 2020 200d 0a65 7863 6570 7420         ..except 
+00004210: 4578 6365 7074 534d 5320 6173 2065 3a20  ExceptSMS as e: 
+00004220: 2020 2020 2023 3220 6578 6365 7074 2073       #2 except s
+00004230: 656e 6465 720d 0a20 2020 2073 7973 2e65  ender..    sys.e
+00004240: 7869 7428 290d 0a0d 0a53 656e 6453 4d53  xit()....SendSMS
+00004250: 2829 2e5f 5f63 616c 6c5f 5f28 2920 2020  ().__call__()   
+00004260: 2020 2020 2023 3320 6375 7374 6f6d 697a       #3 customiz
+00004270: 6564 2073 656e 6465 7220 2020 2020 2020  ed sender       
+00004280: 200d 0a60 6060 0d0a 3c42 723e 0d0a 0d0a   ..```..<Br>....
+00004290: 2323 2032 2d38 2e20 2a54 6561 6d73 204e  ## 2-8. *Teams N
+000042a0: 6f74 6966 6965 722a 0d0a 2d20 612e 2043  otifier*..- a. C
+000042b0: 7265 6174 6520 7468 6520 6368 616e 6e65  reate the channe
+000042c0: 6c20 7468 6174 2079 6f75 2077 616e 7420  l that you want 
+000042d0: 746f 206e 6f74 6966 792e 0d0a 2d20 622e  to notify...- b.
+000042e0: 2041 7070 202d 2053 6561 7263 683a 2077   App - Search: w
+000042f0: 6562 686f 6f6b 202d 2049 6e63 6f6d 696e  ebhook - Incomin
+00004300: 6720 5765 6268 6f6f 6b20 5b68 7474 7073  g Webhook [https
+00004310: 3a2f 2f74 6561 6d73 2e6d 6963 726f 736f  ://teams.microso
+00004320: 6674 2e63 6f6d 2f6c 2f61 7070 2f32 3033  ft.com/l/app/203
+00004330: 6131 6532 632d 3236 6363 2d34 3763 612d  a1e2c-26cc-47ca-
+00004340: 3833 6165 2d62 6539 3866 3936 3062 3662  83ae-be98f960b6b
+00004350: 323f 736f 7572 6365 3d61 7070 2d64 6574  2?source=app-det
+00004360: 6169 6c73 2d64 6961 6c6f 675d 2868 7474  ails-dialog](htt
+00004370: 7073 3a2f 2f74 6561 6d73 2e6d 6963 726f  ps://teams.micro
+00004380: 736f 6674 2e63 6f6d 2f6c 2f61 7070 2f32  soft.com/l/app/2
+00004390: 3033 6131 6532 632d 3236 6363 2d34 3763  03a1e2c-26cc-47c
+000043a0: 612d 3833 6165 2d62 6539 3866 3936 3062  a-83ae-be98f960b
+000043b0: 3662 323f 736f 7572 6365 3d61 7070 2d64  6b2?source=app-d
+000043c0: 6574 6169 6c73 2d64 6961 6c6f 6729 0d0a  etails-dialog)..
+000043d0: 2d20 632e 2043 6c69 636b 2060 5265 7175  - c. Click `Requ
+000043e0: 6573 7420 4170 7072 6f76 616c 6020 3c62  est Approval` <b
+000043f0: 723e 0d0a 4166 7465 7220 796f 7520 6361  r>..After you ca
+00004400: 6e20 7573 6520 7765 6268 6f6f 6b20 696e  n use webhook in
+00004410: 636f 6d6d 696e 672e 2050 726f 6365 6564  comming. Proceed
+00004420: 2074 6f20 6e65 7874 2073 7465 7073 2e0d   to next steps..
+00004430: 0a4d 6963 726f 736f 6674 2054 6561 6d73  .Microsoft Teams
+00004440: 2061 6c6c 6f77 7320 6c69 6d69 7465 6420   allows limited 
+00004450: 6170 706c 6963 6174 696f 6e20 6163 6365  application acce
+00004460: 7373 2070 6572 206f 7267 616e 697a 6174  ss per organizat
+00004470: 696f 6e2c 2073 6f20 6974 2063 616e 206f  ion, so it can o
+00004480: 6e6c 7920 6265 2075 7365 6420 6966 2074  nly be used if t
+00004490: 6865 2077 6562 686f 6f6b 2069 6e63 6f6d  he webhook incom
+000044a0: 696e 6720 6170 706c 6963 6174 696f 6e20  ing application 
+000044b0: 6973 2061 7661 696c 6162 6c65 2e0d 0a2d  is available...-
+000044c0: 2063 2e20 476f 2074 6f20 7468 6520 7465   c. Go to the te
+000044d0: 616d 2063 6861 6e6e 656c 2074 6f20 7265  am channel to re
+000044e0: 6365 6976 6520 6e6f 7469 6669 6361 7469  ceive notificati
+000044f0: 6f6e 732c 2061 6e64 2063 6c69 636b 2060  ons, and click `
+00004500: 436f 6e6e 6563 746f 7273 6020 696e 2053  Connectors` in S
+00004510: 6574 7469 6e67 732e 0d0a 2d20 642e 2060  ettings...- d. `
+00004520: 436f 6e6e 6563 746f 7273 6020 4166 7465  Connectors` Afte
+00004530: 7220 636f 6e66 6967 7572 696e 6720 7765  r configuring we
+00004540: 6268 6f6f 6b20 696e 636f 6d69 6e67 2069  bhook incoming i
+00004550: 6e20 436f 6e6e 6563 746f 722c 2063 6f70  n Connector, cop
+00004560: 7920 7468 6520 7765 6268 6f6f 6b20 5552  y the webhook UR
+00004570: 4c2e 0d0a 0d0a 6060 6070 7974 686f 6e0d  L.....```python.
+00004580: 0a69 6d70 6f72 7420 7379 730d 0a66 726f  .import sys..fro
+00004590: 6d20 4578 6365 7074 4e6f 7469 6669 6572  m ExceptNotifier
+000045a0: 2069 6d70 6f72 7420 4578 6365 7074 5465   import ExceptTe
+000045b0: 616d 732c 2053 7563 6365 7373 5465 616d  ams, SuccessTeam
+000045c0: 732c 2053 656e 6454 6561 6d73 0d0a 7379  s, SendTeams..sy
+000045d0: 732e 6578 6365 7074 686f 6f6b 203d 2045  s.excepthook = E
+000045e0: 7863 6570 7454 6561 6d73 2e5f 5f63 616c  xceptTeams.__cal
+000045f0: 6c5f 5f0d 0a0d 0a23 2044 6566 696e 6520  l__....# Define 
+00004600: 7468 6520 6e65 7874 2074 776f 2076 6172  the next two var
+00004610: 6961 626c 6573 206f 7074 696f 6e61 6c6c  iables optionall
+00004620: 7920 7768 656e 2075 7369 6e67 204f 7065  y when using Ope
+00004630: 6e41 4927 7320 4150 492e 0d0a 2320 5f4f  nAI's API...# _O
+00004640: 5045 4e5f 4149 5f4d 4f44 454c 3d22 6770  PEN_AI_MODEL="gp
+00004650: 742d 332e 352d 7475 7262 6f22 2020 2020  t-3.5-turbo"    
+00004660: 0d0a 2320 5f4f 5045 4e5f 4149 5f41 5049  ..# _OPEN_AI_API
+00004670: 3d22 736b 2d78 7878 7878 7822 0d0a 5f54  ="sk-xxxxxx".._T
+00004680: 4541 4d53 5f57 4542 484f 4f4b 5f55 524c  EAMS_WEBHOOK_URL
+00004690: 203d 2027 6d69 6372 6f73 6f66 7420 7765   = 'microsoft we
+000046a0: 6268 6f6f 6b20 5f54 4541 4d53 5f57 4542  bhook _TEAMS_WEB
+000046b0: 484f 4f4b 5f55 524c 270d 0a0d 0a74 7279  HOOK_URL'....try
+000046c0: 3a0d 0a20 2020 2070 7269 6e74 2831 2f32  :..    print(1/2
+000046d0: 3029 2020 0d0a 2020 2020 5375 6363 6573  0)  ..    Succes
+000046e0: 7354 6561 6d73 2829 2e5f 5f63 616c 6c5f  sTeams().__call_
+000046f0: 5f28 2920 2331 2073 7563 6365 7373 2073  _() #1 success s
+00004700: 656e 6465 7220 2020 2020 2020 2020 200d  ender          .
+00004710: 0a65 7863 6570 7420 4578 6365 7074 5465  .except ExceptTe
+00004720: 616d 7320 6173 2065 3a20 2020 2020 2023  ams as e:      #
+00004730: 3220 6578 6365 7074 2073 656e 6465 7220  2 except sender 
+00004740: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00004750: 2073 7973 2e65 7869 7428 290d 0a0d 0a53   sys.exit()....S
+00004760: 656e 6454 6561 6d73 2829 2e5f 5f63 616c  endTeams().__cal
+00004770: 6c5f 5f28 2920 2020 2020 2020 2023 3320  l__()        #3 
+00004780: 6375 7374 6f6d 697a 6564 2073 656e 6465  customized sende
+00004790: 7220 2020 2020 2020 200d 0a60 6060 0d0a  r        ..```..
+000047a0: 0d0a 3c42 723e 0d0a 0d0a 2323 2032 2d39  ..<Br>....## 2-9
+000047b0: 2e20 2a4b 616b 616f 7461 6c6b 204e 6f74  . *Kakaotalk Not
+000047c0: 6966 6965 722a 0d0a 2d20 612e 2053 6967  ifier*..- a. Sig
+000047d0: 6e20 7570 2061 7420 7468 6520 666f 6c6c  n up at the foll
+000047e0: 6f77 696e 6720 7369 7465 3a20 5b68 7474  owing site: [htt
+000047f0: 7073 3a2f 2f64 6576 656c 6f70 6572 732e  ps://developers.
+00004800: 6b61 6b61 6f2e 636f 6d2f 5d28 6874 7470  kakao.com/](http
+00004810: 733a 2f2f 6465 7665 6c6f 7065 7273 2e6b  s://developers.k
+00004820: 616b 616f 2e63 6f6d 2f29 0d0a 2d20 622e  akao.com/)..- b.
+00004830: 2043 6c69 636b 2022 4d79 2041 7070 6c69   Click "My Appli
+00004840: 6361 7469 6f6e 2220 6f6e 2074 6865 2074  cation" on the t
+00004850: 6f70 2062 6172 2e0d 0a2d 2063 2e20 436c  op bar...- c. Cl
+00004860: 6963 6b20 2241 6464 2061 6e20 6170 706c  ick "Add an appl
+00004870: 6963 6174 696f 6e2c 2220 7365 7420 6120  ication," set a 
+00004880: 6e61 6d65 2c20 616e 6420 6372 6561 7465  name, and create
+00004890: 2069 742e 0d0a 2d20 642e 2043 6c69 636b   it...- d. Click
+000048a0: 2022 4b61 6b61 6f20 4c6f 6769 6e22 2069   "Kakao Login" i
+000048b0: 6e20 7468 6520 6c65 6674 206d 656e 752c  n the left menu,
+000048c0: 2074 6865 6e20 6368 616e 6765 2074 6865   then change the
+000048d0: 2053 7461 7465 206f 6620 224b 616b 616f   State of "Kakao
+000048e0: 204c 6f67 696e 2041 6374 6976 6174 696f   Login Activatio
+000048f0: 6e22 2074 6f20 4f4e 206f 6e20 7468 6520  n" to ON on the 
+00004900: 7265 7375 6c74 696e 6720 7061 6765 2e0d  resulting page..
+00004910: 0a2d 2065 2e20 496e 204d 7920 4170 706c  .- e. In My Appl
+00004920: 6963 6174 696f 6e20 3e20 5072 6f64 7563  ication > Produc
+00004930: 7420 5365 7474 696e 6773 203e 204b 616b  t Settings > Kak
+00004940: 616f 204c 6f67 696e 2c20 6265 2073 7572  ao Login, be sur
+00004950: 6520 746f 2073 6574 2052 6564 6972 6563  e to set Redirec
+00004960: 7420 5552 4920 6173 2066 6f6c 6c6f 7773  t URI as follows
+00004970: 3a20 5b68 7474 7073 3a2f 2f65 7861 6d70  : [https://examp
+00004980: 6c65 2e63 6f6d 2f6f 6175 7468 5d28 6874  le.com/oauth](ht
+00004990: 7470 733a 2f2f 6578 616d 706c 652e 636f  tps://example.co
+000049a0: 6d2f 6f61 7574 6829 0d0a 2d20 662e 2049  m/oauth)..- f. I
+000049b0: 6e20 7468 6520 6c65 6674 2043 6f6e 7365  n the left Conse
+000049c0: 6e74 2049 7465 6d73 206d 656e 752c 2073  nt Items menu, s
+000049d0: 6574 2022 5365 6e64 206d 6573 7361 6765  et "Send message
+000049e0: 2069 6e20 4b61 6b61 6f54 616c 6b22 2074   in KakaoTalk" t
+000049f0: 6f20 7365 6c65 6374 6976 6520 6167 7265  o selective agre
+00004a00: 656d 656e 742e 0d0a 2d20 672e 2043 6f70  ement...- g. Cop
+00004a10: 7920 7468 6520 5245 5354 2041 5049 204b  y the REST API K
+00004a20: 6579 2069 6e20 4d79 2041 7070 6c69 6361  ey in My Applica
+00004a30: 7469 6f6e 203e 2041 7070 2053 6574 7469  tion > App Setti
+00004a40: 6e67 7320 3e20 5375 6d6d 6172 792c 2061  ngs > Summary, a
+00004a50: 6e64 2067 6f20 746f 2074 6865 2066 6f6c  nd go to the fol
+00004a60: 6c6f 7769 6e67 2064 6f63 756d 656e 742e  lowing document.
+00004a70: 0d0a 2d20 682e 2049 6620 796f 7520 6861  ..- h. If you ha
+00004a80: 7665 2073 7563 6365 7373 6675 6c6c 7920  ve successfully 
+00004a90: 636f 6d70 6c65 7465 6420 616c 6c20 6f66  completed all of
+00004aa0: 2074 6865 2061 626f 7665 2073 7465 7073   the above steps
+00004ab0: 2c20 676f 2074 6f20 7468 6520 666f 6c6c  , go to the foll
+00004ac0: 6f77 696e 6720 646f 6375 6d65 6e74 2061  owing document a
+00004ad0: 6e64 2066 6f6c 6c6f 7720 7468 6520 696e  nd follow the in
+00004ae0: 7374 7275 6374 696f 6e73 3a0d 0a20 6874  structions:.. ht
+00004af0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004b00: 2f64 7364 616e 6965 6c70 6172 6b2f 4578  /dsdanielpark/Ex
+00004b10: 6365 7074 4e6f 7469 6669 6572 2f62 6c6f  ceptNotifier/blo
+00004b20: 622f 6d61 696e 2f74 7574 6f72 6961 6c73  b/main/tutorials
+00004b30: 2f6b 616b 616f 5f74 6f6b 656e 5f67 656e  /kakao_token_gen
+00004b40: 6572 6174 6f72 2e69 7079 6e62 0d0a 202a  erator.ipynb.. *
+00004b50: 2a49 6e20 7468 6973 2065 7861 6d70 6c65  *In this example
+00004b60: 2c20 736f 6d65 2041 5049 206b 6579 7320  , some API keys 
+00004b70: 7765 7265 2065 7870 6f73 6564 2062 7920  were exposed by 
+00004b80: 6372 6561 7469 6e67 2061 6e64 2072 656d  creating and rem
+00004b90: 6f76 696e 6720 6120 7465 7374 2061 7070  oving a test app
+00004ba0: 6c69 6361 7469 6f6e 2c20 6275 7420 666f  lication, but fo
+00004bb0: 7220 7365 6375 7269 7479 2072 6561 736f  r security reaso
+00004bc0: 6e73 2c20 796f 7572 2041 5049 206b 6579  ns, your API key
+00004bd0: 2073 686f 756c 6420 6e6f 7420 6265 2065   should not be e
+00004be0: 7870 6f73 6564 2074 6f20 7468 6520 6f75  xposed to the ou
+00004bf0: 7473 6964 6520 776f 726c 642e 2a2a 0d0a  tside world.**..
+00004c00: 3c42 723e 0d0a 0d0a 6060 6070 7974 686f  <Br>....```pytho
+00004c10: 6e0d 0a69 6d70 6f72 7420 7379 730d 0a66  n..import sys..f
+00004c20: 726f 6d20 4578 6365 7074 4e6f 7469 6669  rom ExceptNotifi
+00004c30: 6572 2069 6d70 6f72 7420 4578 6365 7074  er import Except
+00004c40: 4b61 6b61 6f2c 2053 7563 6365 7373 4b61  Kakao, SuccessKa
+00004c50: 6b61 6f2c 2053 656e 644b 616b 616f 0d0a  kao, SendKakao..
+00004c60: 7379 732e 6578 6365 7074 686f 6f6b 203d  sys.excepthook =
+00004c70: 2045 7863 6570 744b 616b 616f 2e5f 5f63   ExceptKakao.__c
+00004c80: 616c 6c5f 5f0d 0a0d 0a23 2044 6566 696e  all__....# Defin
+00004c90: 6520 7468 6520 6e65 7874 2074 776f 2076  e the next two v
+00004ca0: 6172 6961 626c 6573 206f 7074 696f 6e61  ariables optiona
+00004cb0: 6c6c 7920 7768 656e 2075 7369 6e67 204f  lly when using O
+00004cc0: 7065 6e41 4927 7320 4150 492e 0d0a 2320  penAI's API...# 
+00004cd0: 5f4f 5045 4e5f 4149 5f4d 4f44 454c 3d22  _OPEN_AI_MODEL="
+00004ce0: 6770 742d 332e 352d 7475 7262 6f22 2020  gpt-3.5-turbo"  
+00004cf0: 2020 0d0a 2320 5f4f 5045 4e5f 4149 5f41    ..# _OPEN_AI_A
+00004d00: 5049 3d22 736b 2d78 7878 7878 7822 0d0a  PI="sk-xxxxxx"..
+00004d10: 5f4b 414b 414f 5f54 4f4b 454e 5f50 4154  _KAKAO_TOKEN_PAT
+00004d20: 4820 3d20 2778 7878 782f 7878 782f 7878  H = 'xxxx/xxx/xx
+00004d30: 782e 6a73 6f6e 2727 0d0a 0d0a 7472 793a  x.json''....try:
+00004d40: 0d0a 2020 2020 7072 696e 7428 312f 3029  ..    print(1/0)
+00004d50: 2020 0d0a 2020 2020 5375 6363 6573 734b    ..    SuccessK
+00004d60: 616b 616f 2829 2e5f 5f63 616c 6c5f 5f28  akao().__call__(
+00004d70: 2920 2331 2073 7563 6365 7373 2073 656e  ) #1 success sen
+00004d80: 6465 7220 2020 2020 2020 2020 200d 0a65  der          ..e
+00004d90: 7863 6570 7420 4578 6365 7074 4b61 6b61  xcept ExceptKaka
+00004da0: 6f20 6173 2065 3a20 2020 2020 2023 3220  o as e:      #2 
+00004db0: 6578 6365 7074 2073 656e 6465 7220 2020  except sender   
+00004dc0: 2020 2020 2020 2020 200d 0a20 2020 2073           ..    s
+00004dd0: 7973 2e65 7869 7428 290d 0a0d 0a53 656e  ys.exit()....Sen
+00004de0: 644b 616b 616f 2829 2e5f 5f63 616c 6c5f  dKakao().__call_
+00004df0: 5f28 2920 2020 2020 2020 2023 3320 6375  _()        #3 cu
+00004e00: 7374 6f6d 697a 6564 2073 656e 6465 7220  stomized sender 
+00004e10: 2020 2020 2020 2020 0d0a 6060 600d 0a0d          ..```...
+00004e20: 0a3c 4272 3e0d 0a0d 0a23 2320 322d 3130  .<Br>....## 2-10
+00004e30: 2e20 2a42 6565 7020 4e6f 7469 6669 6572  . *Beep Notifier
+00004e40: 2a0d 0a4e 6f20 7365 7475 7020 6973 2072  *..No setup is r
+00004e50: 6571 7569 7265 642e 2055 7365 2061 7320  equired. Use as 
+00004e60: 666f 6c6c 6f77 732e 0d0a 0d0a 6060 6070  follows.....```p
+00004e70: 7974 686f 6e0d 0a66 726f 6d20 4578 6365  ython..from Exce
+00004e80: 7074 6e6f 7469 6669 6572 2069 6d70 6f72  ptnotifier impor
+00004e90: 7420 4578 6365 7074 4265 6570 2c20 5375  t ExceptBeep, Su
+00004ea0: 6363 6573 7342 6565 702c 2053 656e 6442  ccessBeep, SendB
+00004eb0: 6565 7028 292c 2062 6565 7028 290d 0a42  eep(), beep()..B
+00004ec0: 4545 505f 5449 4d45 203d 2031 0d0a 7379  EEP_TIME = 1..sy
+00004ed0: 732e 6578 6365 7074 686f 6f6b 203d 2045  s.excepthook = E
+00004ee0: 7863 6570 7442 6565 702e 5f5f 6361 6c6c  xceptBeep.__call
+00004ef0: 5f5f 0d0a 0d0a 7472 793a 0d0a 2020 2020  __....try:..    
+00004f00: 7072 696e 7428 312f 3230 2920 200d 0a20  print(1/20)  .. 
+00004f10: 2020 2053 7563 6365 7373 4265 6570 2829     SuccessBeep()
+00004f20: 2e5f 5f63 616c 6c5f 5f28 2920 2331 2073  .__call__() #1 s
+00004f30: 7563 6365 7373 2062 6565 702d 6265 6570  uccess beep-beep
+00004f40: 2020 2020 2020 2020 2020 0d0a 0d0a 6578            ....ex
+00004f50: 6365 7074 2045 7863 6570 7442 6565 7020  cept ExceptBeep 
+00004f60: 6173 2065 3a20 2020 2020 2023 3220 6578  as e:      #2 ex
+00004f70: 6365 7074 2062 6565 702d 6265 6570 2020  cept beep-beep  
+00004f80: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00004f90: 2020 2020 7379 732e 6578 6974 2829 0d0a      sys.exit()..
+00004fa0: 0d0a 5365 6e64 4265 6570 2829 2e5f 5f63  ..SendBeep().__c
+00004fb0: 616c 6c5f 5f28 2920 2020 2020 2020 2023  all__()        #
+00004fc0: 3320 6375 7374 6f6d 697a 6564 2062 6565  3 customized bee
+00004fd0: 702d 6265 6570 2020 2020 2020 0d0a 0d0a  p-beep      ....
+00004fe0: 6265 6570 2829 0d0a 0d0a 6060 600d 0a0d  beep()....```...
+00004ff0: 0a3c 4272 3e0d 0a0d 0a0d 0a23 2320 322d  .<Br>......## 2-
+00005000: 3131 2e20 2a44 6573 6b74 6f70 204e 6f74  11. *Desktop Not
+00005010: 6966 6965 722a 0d0a 4e6f 2073 6574 7570  ifier*..No setup
+00005020: 2069 7320 7265 7175 6972 6564 2e20 5573   is required. Us
+00005030: 6520 6173 2066 6f6c 6c6f 7773 2e0d 0a0d  e as follows....
+00005040: 0a60 6060 7079 7468 6f6e 0d0a 6672 6f6d  .```python..from
+00005050: 2045 7863 6570 744e 6f74 6966 6965 7220   ExceptNotifier 
+00005060: 696d 706f 7274 2045 7863 6570 7444 6573  import ExceptDes
+00005070: 6b74 6f70 2c20 5375 6363 6573 7344 6573  ktop, SuccessDes
+00005080: 6b74 6f70 2c20 5365 6e64 4465 736b 746f  ktop, SendDeskto
+00005090: 700d 0a73 7973 2e65 7863 6570 7468 6f6f  p..sys.excepthoo
+000050a0: 6b20 3d20 4578 6365 7074 4465 736b 746f  k = ExceptDeskto
+000050b0: 702e 5f5f 6361 6c6c 5f5f 0d0a 2320 4465  p.__call__..# De
+000050c0: 6669 6e65 2074 6865 206e 6578 7420 7477  fine the next tw
+000050d0: 6f20 7661 7269 6162 6c65 7320 6f70 7469  o variables opti
+000050e0: 6f6e 616c 6c79 2077 6865 6e20 7573 696e  onally when usin
+000050f0: 6720 4f70 656e 4149 2773 2041 5049 2e0d  g OpenAI's API..
+00005100: 0a23 205f 4f50 454e 5f41 495f 4d4f 4445  .# _OPEN_AI_MODE
+00005110: 4c3d 2267 7074 2d33 2e35 2d74 7572 626f  L="gpt-3.5-turbo
+00005120: 2220 2020 200d 0a23 205f 4f50 454e 5f41  "    ..# _OPEN_A
+00005130: 495f 4150 493d 2273 6b2d 7878 7878 7878  I_API="sk-xxxxxx
+00005140: 220d 0a0d 0a74 7279 3a0d 0a20 2020 2070  "....try:..    p
+00005150: 7269 6e74 2831 2f30 2920 200d 0a20 2020  rint(1/0)  ..   
+00005160: 2053 7563 6365 7373 4465 736b 746f 7028   SuccessDesktop(
+00005170: 292e 5f5f 6361 6c6c 5f5f 2829 2023 3120  ).__call__() #1 
+00005180: 7375 6363 6573 7320 7365 6e64 6572 2020  success sender  
+00005190: 2020 2020 2020 2020 0d0a 0d0a 6578 6365          ....exce
+000051a0: 7074 2045 7863 6570 7444 6573 6b74 6f70  pt ExceptDesktop
+000051b0: 2061 7320 653a 2020 2020 2020 2332 2065   as e:      #2 e
+000051c0: 7863 6570 7420 7365 6e64 6572 2020 2020  xcept sender    
+000051d0: 2020 2020 2020 2020 0d0a 2020 2020 7379          ..    sy
+000051e0: 732e 6578 6974 2829 0d0a 0d0a 5365 6e64  s.exit()....Send
+000051f0: 4465 736b 746f 7028 292e 5f5f 6361 6c6c  Desktop().__call
+00005200: 5f5f 2829 2020 2020 2020 2020 2333 2063  __()        #3 c
+00005210: 7573 746f 6d69 7a65 6420 7365 6e64 6572  ustomized sender
+00005220: 2020 2020 2020 2020 200d 0a60 6060 0d0a           ..```..
+00005230: 0d0a 3c42 723e 3c62 723e 3c62 723e 0d0a  ..<Br><br><br>..
+00005240: 0d0a 2320 4c69 6365 6e73 650d 0a4d 4954  ..# License..MIT
+00005250: 0d0a 0d0a 2320 436f 6465 206f 6620 436f  ....# Code of Co
+00005260: 6e64 7563 740d 0a45 7665 7279 6f6e 6520  nduct..Everyone 
+00005270: 7061 7274 6963 6970 6174 696e 6720 696e  participating in
+00005280: 2074 6865 2060 4578 6365 7074 4e6f 7469   the `ExceptNoti
+00005290: 6669 6572 6020 7072 6f6a 6563 742c 2061  fier` project, a
+000052a0: 6e64 2069 6e20 7061 7274 6963 756c 6172  nd in particular
+000052b0: 2069 6e20 7468 6520 6973 7375 6520 7472   in the issue tr
+000052c0: 6163 6b65 722c 2070 756c 6c20 7265 7175  acker, pull requ
+000052d0: 6573 7473 2c20 616e 6420 736f 6369 616c  ests, and social
+000052e0: 206d 6564 6961 2061 6374 6976 6974 792c   media activity,
+000052f0: 2069 7320 6578 7065 6374 6564 2074 6f20   is expected to 
+00005300: 7472 6561 7420 6f74 6865 7220 7065 6f70  treat other peop
+00005310: 6c65 2077 6974 6820 7265 7370 6563 7420  le with respect 
+00005320: 616e 6420 6d6f 7265 2067 656e 6572 616c  and more general
+00005330: 6c79 2074 6f20 666f 6c6c 6f77 2074 6865  ly to follow the
+00005340: 2067 7569 6465 6c69 6e65 7320 6172 7469   guidelines arti
+00005350: 6375 6c61 7465 6420 696e 205b 7468 6520  culated in [the 
+00005360: 5079 7468 6f6e 2043 6f6d 6d75 6e69 7479  Python Community
+00005370: 2043 6f64 6520 6f66 2043 6f6e 6475 6374   Code of Conduct
+00005380: 5d28 6874 7470 733a 2f2f 7777 772e 7079  ](https://www.py
+00005390: 7468 6f6e 2e6f 7267 2f70 7366 2f63 6f6e  thon.org/psf/con
+000053a0: 6475 6374 2f29 2e0d 0a0d 0a23 2323 2323  duct/).....#####
+000053b0: 2054 6865 2070 6163 6b61 6765 2069 7320   The package is 
+000053c0: 6375 7272 656e 746c 7920 696e 2074 6865  currently in the
+000053d0: 2064 6576 656c 6f70 6d65 6e74 2061 6e64   development and
+000053e0: 2051 4120 7374 6167 6573 2c20 616e 6420   QA stages, and 
+000053f0: 7468 6520 6465 7665 6c6f 706d 656e 7420  the development 
+00005400: 7374 6167 6520 7769 6c6c 2062 6520 7570  stage will be up
+00005410: 6461 7465 6420 6174 2074 6865 2074 6f70  dated at the top
+00005420: 206f 6620 7468 6973 2070 6167 652e 2049   of this page. I
+00005430: 6620 6974 2069 7320 6465 7465 726d 696e  f it is determin
+00005440: 6564 2074 6861 7420 7468 6520 7072 6f64  ed that the prod
+00005450: 7563 7420 6973 2073 7461 626c 6520 7468  uct is stable th
+00005460: 726f 7567 6820 6665 6174 7572 6520 696d  rough feature im
+00005470: 7072 6f76 656d 656e 742c 2061 6464 6974  provement, addit
+00005480: 696f 6e2c 2061 6e64 2069 7373 7565 2072  ion, and issue r
+00005490: 6573 6f6c 7574 696f 6e2c 2074 6865 2064  esolution, the d
+000054a0: 6576 656c 6f70 6d65 6e74 2073 7461 6765  evelopment stage
+000054b0: 2077 696c 6c20 7265 6163 6820 7374 6167   will reach stag
+000054c0: 6520 352e 2049 6620 6e6f 206e 6577 2075  e 5. If no new u
+000054d0: 7064 6174 6573 206f 7220 6973 7375 6573  pdates or issues
+000054e0: 2061 7269 7365 2c20 6974 2077 696c 6c20   arise, it will 
+000054f0: 6265 2061 646a 7573 7465 6420 7570 7761  be adjusted upwa
+00005500: 7264 2074 6f20 7374 6167 6520 3620 6f72  rd to stage 6 or
+00005510: 2068 6967 6865 722e 0d0a 0d0a 0d0a        higher.......
```

### Comparing `ExceptNotifier-0.1.6/setup.py` & `ExceptNotifier-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 version = get_version()
 
 
 setup(
     name="ExceptNotifier",
-    version="0.1.6",
+    version="0.1.7",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
```

