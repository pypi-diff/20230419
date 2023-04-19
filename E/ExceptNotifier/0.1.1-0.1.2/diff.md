# Comparing `tmp/ExceptNotifier-0.1.1.tar.gz` & `tmp/ExceptNotifier-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExceptNotifier-0.1.1.tar", last modified: Thu Apr 13 17:12:27 2023, max compression
+gzip compressed data, was "ExceptNotifier-0.1.2.tar", last modified: Wed Apr 19 10:33:47 2023, max compression
```

## Comparing `ExceptNotifier-0.1.1.tar` & `ExceptNotifier-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:12:27.635241 ExceptNotifier-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:12:27.618622 ExceptNotifier-0.1.1/ExceptNotifier/
--rw-rw-rw-   0        0        0      251 2023-04-13 17:11:59.000000 ExceptNotifier-0.1.1/ExceptNotifier/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-13 17:10:33.000000 ExceptNotifier-0.1.1/ExceptNotifier/__main__.py
--rw-rw-rw-   0        0        0     4439 2023-04-13 17:09:44.000000 ExceptNotifier-0.1.1/ExceptNotifier/mail_sender.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:12:27.632732 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/
--rw-rw-rw-   0        0        0     3401 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 17:12:27.000000 ExceptNotifier-0.1.1/ExceptNotifier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3401 2023-04-13 17:12:27.634231 ExceptNotifier-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-13 17:11:44.000000 ExceptNotifier-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 17:12:27.636241 ExceptNotifier-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1981 2023-04-13 17:11:56.000000 ExceptNotifier-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:33:47.806156 ExceptNotifier-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-19 10:33:47.778097 ExceptNotifier-0.1.2/ExceptNotifier/
+-rw-rw-rw-   0        0        0     2569 2023-04-19 10:32:22.000000 ExceptNotifier-0.1.2/ExceptNotifier/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-04-19 10:33:31.000000 ExceptNotifier-0.1.2/ExceptNotifier/__main__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-19 10:16:54.000000 ExceptNotifier-0.1.2/ExceptNotifier/beep_notifier.py
+-rw-rw-rw-   0        0        0     6104 2023-04-19 10:16:55.000000 ExceptNotifier-0.1.2/ExceptNotifier/chime_notifier.py
+-rw-rw-rw-   0        0        0     5196 2023-04-19 10:29:29.000000 ExceptNotifier-0.1.2/ExceptNotifier/desktop_notifier.py
+-rw-rw-rw-   0        0        0     5644 2023-04-19 10:28:50.000000 ExceptNotifier-0.1.2/ExceptNotifier/discord_notifier.py
+-rw-rw-rw-   0        0        0     5950 2023-04-19 10:17:01.000000 ExceptNotifier-0.1.2/ExceptNotifier/kakao_notifier.py
+-rw-rw-rw-   0        0        0     5469 2023-04-19 10:28:37.000000 ExceptNotifier-0.1.2/ExceptNotifier/line_notifier.py
+-rw-rw-rw-   0        0        0     6814 2023-04-19 10:17:05.000000 ExceptNotifier-0.1.2/ExceptNotifier/mail_notifier.py
+-rw-rw-rw-   0        0        0     5488 2023-04-19 10:17:07.000000 ExceptNotifier-0.1.2/ExceptNotifier/slack_notifier.py
+-rw-rw-rw-   0        0        0     5477 2023-04-19 10:17:09.000000 ExceptNotifier-0.1.2/ExceptNotifier/sms_notifier.py
+-rw-rw-rw-   0        0        0     5412 2023-04-19 10:27:10.000000 ExceptNotifier-0.1.2/ExceptNotifier/teams_notifier.py
+-rw-rw-rw-   0        0        0     5602 2023-04-19 10:26:40.000000 ExceptNotifier-0.1.2/ExceptNotifier/telegram_notifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:33:47.802011 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/
+-rw-rw-rw-   0        0        0     6500 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 10:33:47.000000 ExceptNotifier-0.1.2/ExceptNotifier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-04-13 16:54:50.000000 ExceptNotifier-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6500 2023-04-19 10:33:47.805020 ExceptNotifier-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5401 2023-04-19 10:27:50.000000 ExceptNotifier-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 10:33:47.806156 ExceptNotifier-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1965 2023-04-19 10:32:00.000000 ExceptNotifier-0.1.2/setup.py
```

### Comparing `ExceptNotifier-0.1.1/ExceptNotifier/__main__.py` & `ExceptNotifier-0.1.2/ExceptNotifier/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import argparse
 import subprocess
 
-from ExceptNotifier import (chime_sender,
-                        desktop_sender,
-                        dingtalk_sender,
-                        discord_sender,
-                        email_sender,
-                        matrix_sender,
-                        rocketchat_sender,
-                        slack_sender,
-                        sms_sender,
-                        teams_sender,
-                        telegram_sender,
-                        wechat_sender,)
+from ExceptNotifier import (
+                        chime_notifier,
+                        desktop_notifier,
+                        discord_notifier,
+                        mail_notifier,
+                        whatsapp_notifier,    # Whatsapp is excluded because it requires complex settings to send personalized messages. However, you can refer to whatsapp_sender for further work.
+                        sms_notifier,
+                        teams_notifier,
+                        telegram_notifier,
+                        wechat_notifier,      # WeChat requests information that is not accessible to people in other countries, such as residence outside of China, so it is excluded.
+                        slack_notifier,
+                        discord_notifier,
+                        kakao_notifier,
+                        line_notifier
+                        )
 
-def main():
-    parser = argparse.ArgumentParser(
-        description="ExceptCatch: Use Python's try-except statement to receive notifications more flexibly.")
-    parser.add_argument("--verbose", required=False, action="store_true",
-                        help="Show All Commands")
-    subparsers = parser.add_subparsers()
+# def main():
+#     parser = argparse.ArgumentParser(
+#         description="ExceptNotifier: Use Python's try-except statement to receive notifications more flexibly.")
+#     parser.add_argument("--verbose", required=False, action="store_true",
+#                         help="Show All Commands")
+#     subparsers = parser.add_subparsers()
     
-    # Email
-    email_parser = subparsers.add_parser(
-        name="email", description="Send an email before and after function " +
-        "execution, with start and end status (sucessfully or crashed).")
-    email_parser.add_argument(
-        "--gmail_receiver", type=str, required=True,
-        help="The email addresses to notify")
-    email_parser.add_argument(
-        "--gmail_sender", type=str, required=False,
-        help="The email adress to send the messages." +
-        "(default: use the same address as the first email in `gmail_receiver`)")
-    email_parser.set_defaults(sender_func=email_sender)
+#     # Email
+#     email_parser = subparsers.add_parser(
+#         name="email", description="Send an email before and after function " +
+#         "execution, with start and end status (sucessfully or crashed).")
+#     email_parser.add_argument(
+#         "--recipient_addr", type=str, required=True,
+#         help="The email addresses to notify")
+#     email_parser.add_argument(
+#         "--gmail_sender", type=str, required=False,
+#         help="The email adress to send the messages." +
+#         "(default: use the same address as the first email in `recipient_addr`)")
+#     email_parser.set_defaults(sender_func=mail_notifier)
```

### Comparing `ExceptNotifier-0.1.1/LICENSE` & `ExceptNotifier-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ExceptNotifier-0.1.1/setup.py` & `ExceptNotifier-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,44 +11,43 @@
     if not match:
         raise RuntimeError("{} doesn't contain __version__".format(filename))
     version = match.groups()[0]
     return version
 
 
 def get_long_description():
-    with open("README.md") as f:
+    with open("README.md", encoding='UTF-8') as f:
         long_description = f.read()
         return long_description
 
 
 version = get_version()
 
 
 setup(
     name="ExceptNotifier",
-    version="0.1.1",
-    author="parkminwoo",
+    version="0.1.2",
+    author="daniel park",
     author_email="parkminwoo1991@gmail.com",
-    description="With Python's try-except statement, experience a significantly more flexible way to receive notifications.",
+    description="With Python's try-except to receive notifications about Errors or Successes in your code through messenger app or email.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/ExceptNotifier",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
-    install_requires=[],
+    install_requires=['twilio', 'plyer', 'openai'],
     keywords="Exception, Python, Python Exception Alarm, Error notifications, Customizable notifications, Traceback management, Single line alarm",
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: Implementation :: CPython",
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     entry_points={"console_scripts": ["ExceptNotifier=ExceptNotifier.cli:main"]},
 )
```

