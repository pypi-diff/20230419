# Comparing `tmp/pebbles_bot-0.3.0.tar.gz` & `tmp/pebbles_bot-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pebbles_bot-0.3.0.tar", last modified: Sat Apr 15 18:33:31 2023, max compression
+gzip compressed data, was "pebbles_bot-0.3.1.tar", last modified: Wed Apr 19 19:39:48 2023, max compression
```

## Comparing `pebbles_bot-0.3.0.tar` & `pebbles_bot-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/pebbles_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/pb_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/pb_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/pebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/pebbles_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/pebbles_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/pb_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/pb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pebbles_bot/pebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/pebbles_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 19:39:48.000000 pebbles_bot-0.3.1/pebbles_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-19 19:39:48.717073 pebbles_bot-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:39:39.000000 pebbles_bot-0.3.1/setup.py
```

### Comparing `pebbles_bot-0.3.0/LICENSE` & `pebbles_bot-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.0/PKG-INFO` & `pebbles_bot-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pebbles_bot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pebbles_bot-0.3.0/README.md` & `pebbles_bot-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.0/pebbles_bot/pb_main.py` & `pebbles_bot-0.3.1/pebbles_bot/pb_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from telebot.types import (
     InlineKeyboardMarkup as ik_markup,
     InlineKeyboardButton as ik_button,
 )
 
 
 class Pebbles:
-    def __init__(self, api_key, whitelist, notify=False):
+    def __init__(
+        self, api_key: str, whitelist: list[str], notify: bool = False
+    ):
         self.bot = TeleBot(api_key)
         self.tls = Tools()
         self.ssh = SSH_Tools()
         self.pebbles_mode = "local"
 
         self.uid_whitelist = whitelist
 
@@ -25,14 +27,26 @@
             handlers=[
                 logging.FileHandler(f"{str(Path.home())}/.pebbles.log"),
                 logging.StreamHandler(),
             ],
         )
         self.logger = logging.getLogger()
 
+        self.register_command_handlers()
+
+        if notify:
+            self.send_notification(notify)
+        else:
+            self.start_bot()
+
+    def register_command_handlers(self):
+        """
+        Register command handlers for the bot.
+        """
+
         @self.bot.message_handler(commands=["start"])
         def _start(message):
             self.start(message)
 
         @self.bot.message_handler(commands=["help"])
         def _help(message):
             self.help(message)
@@ -57,29 +71,26 @@
         def _rest(message):
             self.rest(message)
 
         @self.bot.callback_query_handler(func=lambda call: True)
         def _callback_worker(call):
             self.callback_worker(call)
 
-        if notify:
-            self.send_notification(notify)
-        else:
-            self.start_bot()
-
     def start_bot(self):
         """
         Start the bot and print a message.
         """
         self.logger.info("Pebbles is awakening...")
         self.logger.info("Awaiting commands")
         try:
             self.bot.polling(interval=0)
         except ApiTelegramException:
-            self.logger.info("Unable to start Pebbles, check your API key")
+            self.logger.exception(
+                "Unable to start Pebbles, check your API key"
+            )
         self.logger.info("Pebbles is entering hibernation...")
 
     def log(self, info, log=""):
         """
         Simplifies the use of logger library,
         and makes logger look cleaner in the code.
         """
@@ -223,14 +234,15 @@
                 self.bot.send_message(message.from_user.id, cout)
             elif err != "":
                 self.bot.send_message(message.from_user.id, err)
             elif cout == "" and err == "":
                 self.bot.send_message(message.from_user.id, "No Output")
         except AttributeError:
             err_msg = "There is no active SSH session"
+            self.logger.exception(err_msg)
             self.bot.send_message(message.from_user.id, err_msg)
 
     def _connect(self, chat_id, con_result):
         """
         Use Paramiko to connect to remote host,
         return connection status.
         """
```

### Comparing `pebbles_bot-0.3.0/pebbles_bot/pb_tools.py` & `pebbles_bot-0.3.1/pebbles_bot/pb_tools.py`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.3.0/pebbles_bot/pebot.py` & `pebbles_bot-0.3.1/pebbles_bot/pebot.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         print("Pebbles API key not found")
         sys.exit(0)
 
     if not whitelist_ids:
         print("Pebbles user whitelist not found")
         sys.exit(0)
 
-    if len(sys.argv) == 1:
-        notify = False
-    elif "--notify" in sys.argv:
+    notify = "--notify" in sys.argv
+    if notify:
+        sys.argv.remove("--notify")
         notify = sys.stdin.read()
 
     pebbles_config = config_reader()
     if pebbles_config:
         whitelist_ids = pebbles_config["whitelist_ids"]
 
     Pebbles(
```

### Comparing `pebbles_bot-0.3.0/pebbles_bot.egg-info/PKG-INFO` & `pebbles_bot-0.3.1/pebbles_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pebbles-bot
-Version: 0.3.0
+Version: 0.3.1
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pebbles_bot-0.3.0/setup.cfg` & `pebbles_bot-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pebbles_bot
-version = 0.3.0
+version = 0.3.1
 description = Telegram bot that runs Linux shell commands
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/pyLookout
 license = MIT
```

