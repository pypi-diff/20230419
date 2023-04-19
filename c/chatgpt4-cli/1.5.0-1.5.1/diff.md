# Comparing `tmp/chatgpt4-cli-1.5.0.tar.gz` & `tmp/chatgpt4-cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.5.0.tar", last modified: Tue Apr 18 21:58:28 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.1.tar", last modified: Wed Apr 19 13:16:25 2023, max compression
```

## Comparing `chatgpt4-cli-1.5.0.tar` & `chatgpt4-cli-1.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:28.364807 chatgpt4-cli-1.5.0/GPTCLI/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/bard.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/emage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29365 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/gptcli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31039 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:16:25.000000 chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:16:25.770380 chatgpt4-cli-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-19 13:16:03.000000 chatgpt4-cli-1.5.1/setup.py
```

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/__init__.py` & `chatgpt4-cli-1.5.1/GPTCLI/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 __author__ = "Smartwa Caleb"
 __repo__ = "https://github.com/Simatwa/gpt-cli"
 
 import logging
 
 logging.basicConfig(
-    format="%(levelname)s - %(message)s - (%(asctime)s)",
+    format="%(levelname)s - %(message)s - (%(asctime)s) ",#[%(module)s,%(lineno)s]",
     datefmt="%d-%b-%Y %H:%M:%S",
     level=logging.INFO,
 )
 
 getExc = lambda e: e.args[1] if isinstance(e.args, list) else str(e)
 
 
@@ -19,17 +19,15 @@
     Args:
         resp (Any, optional): Value to be returned incase of exception. Defaults to None.
     """
 
     def wrapper(func):
         def main(*args, **kwargs):
             try:
-                rp = func(*args, **kwargs)
+                return func(*args, **kwargs)
             except Exception as e:
                 logging.error(getExc(e))
-                rp = resp() if callable(resp) else resp
-            finally:
-                return rp
+                return resp() if callable(resp) else resp
 
         return main
 
     return wrapper
```

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/addons.py` & `chatgpt4-cli-1.5.1/GPTCLI/addons.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/bard.py` & `chatgpt4-cli-1.5.1/GPTCLI/bard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from Bard import Chatbot
 from . import logging, error_handler
 from sys import exit
 from os import environ
-from json import loads
+from json import load
 from time import sleep
 
 
 class Bard:
     def __init__(self, args: object):
         self.args = args
         self.session = environ.get("BARD_SESSION") or self.__get_sess()
@@ -20,17 +20,17 @@
                 resp = self.args.bkey
             elif self.args.bkey_path:
                 with open(self.args.bkey_path) as fh:
                     resp = fh.read()
             else:
                 resp = None
                 with open(self.args.bcookie_file) as fh:
-                    entries = loads(fh)
+                    entries = load(fh)
                 for entry in entries:
-                    if entry["value"] == "__Secure-1PSID":
+                    if entry["name"] == "__Secure-1PSID":
                         resp = entry["value"]
             return resp
         else:
             logging.error("Bard's session not found!")
 
     @error_handler("Error while communicating with Bard")
     def chat(self, prompt: str, stream: bool = True) -> str:
@@ -42,13 +42,14 @@
 
         Returns:
             str: Bard's Response
         """
         if not self.session:
             return logging.error("Bard's session not found!")
         resp = self.active_link.ask(prompt)["content"]
-        if stream:
+        if stream and not self.args.disable_stream:
             for value in resp:
                 yield value
                 sleep(self.args.stream_interval)
         else:
-            return resp["content"]
+            for val in resp:
+                yield val
```

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/emage.py` & `chatgpt4-cli-1.5.1/GPTCLI/emage.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.1/GPTCLI/gptcli.py`

 * *Files 4% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 
 config_h = config_handler()
 args = config_h.main()
 from sys import exit, stderr
 import json
 import openai
 import cmd
-from . import logging, getExc
+from . import logging, getExc, error_handler
 from .image import imager
 from .emage import emager
 from re import sub
 from datetime import datetime
 from os import system, remove, path, environ, makedirs
 from threading import Thread as thr
 from appdirs import AppDirs
@@ -585,14 +585,15 @@
                 resp = False
         return resp
 
     def default(self, raw, return_fb=False, no_check=False):
         raw = self.parser(raw)
         run_against_system = False
         if not raw:
+            self.do__prompt(self.prompt_disp)
             return
         # out = lambda b: print(self.color_dict[args.output_color] + b + Fore.RESET)
         if raw[0:2] == "./":
             system((raw[2:]).strip())
         else:
             if "--system" in raw:
                 run_against_system = True
@@ -615,36 +616,81 @@
             print(Fore.RESET)
         self.do__prompt(self.prompt_disp)
 
     def do_gpt4(self, line):
         """Interact with ChatGPT4"""
         self.default(line, no_check=True)
 
-    def do_bard(self, line):
+    def do_bard(self, line, return_fb=False, chat=False):
         """Interact with Google's bard"""
         if "--gpt4" in line:
             return self.default(line.replace("--gpt4", ""), no_check=True)
 
         args.message = line
-        print(self.color_dict[args.output_color], end="")
+        if chat:
+            print(self.color_dict[args.input_color], end="")
+        else:
+            print(self.color_dict[args.output_color], end="")
         if args.disable_stream:
-            info = self.bard.chat(line, False)
+            inf, info = self.bard.chat(line, False), ""
+            for value in inf:
+                info = info + value
             gpt3.out(info)
         else:
             info = ""
             for val in self.bard.chat(line):
                 print(val, end="", flush=True)
                 info = info + val
-        record_keeper.main(info)
-        print(Fore.RESET)
+        if not chat:
+            record_keeper.main(info)
+        print(self.color_dict[args.input_color])
+        self.do__prompt(self.prompt_disp)
+        if return_fb:
+            return info
+
+    @error_handler()
+    def do__botchat(self, line):
+        rich_print("Let the bots talk:")
+
+        def get_value(msg: str, type1: object = str) -> str:
+            while True:
+                val = input(f"[*] " + msg + f" >>")
+                if val:
+                    if type1 == int:
+                        if val.isdigit():
+                            return int(val)
+                    else:
+                        return val
+
+        def gpt_chat(msg):
+            print("[ChatGPT]")
+            return self.default(msg, return_fb=True)
+
+        def bard_chat(msg):
+            print("[Bard]")
+            return self.do_bard(bard, return_fb=True, chat=True)
+
+        gpt = get_value("Enter prompt for ChatGPT")
+        bard = get_value("Enter prompt for Bard")
+        amount = get_value("Enter amount of chat cycles [0 - infinity]", int)
+        for x in range(amount if amount else 1000000):
+            if x == 0:
+                gpt = gpt_chat(gpt)
+                bard = bard_chat(bard)
+            else:
+                if x % 2 == 0:
+                    bard = bard_chat(gpt)
+                else:
+                    gpt = gpt_chat(bard)
 
     def do_txt2img(self, line):
         """Generate images based on GPT description"""
         line = self.parser(line)
         if not line:
+            self.do__prompt(self.prompt_disp)
             return
         print(
             self.color_dict[args.output_color] + ">>[*] Querying description from GPT",
             end="\r",
         )
         imagiser = imager(line.split(" "))
         description = self.default(imagiser.args.prompt, return_fb=True)
@@ -803,15 +849,15 @@
 def get_api_key() -> str:
     """Gets API from Key_path or args.key"""
     if any([args.key, environ.get("OPENAI_API_KEY")]):
         return args.key or environ.get("OPENAI_API_KEY")
     if args.key_path:
         try:
             with open(args.key_path, encoding="utf-8") as fh:
-                return fh.readlines()[0]
+                return fh.readlines()[0].replace("\n", "")
         except Exception as e:
             exit(logging.critical("While opening Key_Path " + getExc(e)))
 
 
 def intro_train(
     error_msg: str = "Initializing default configurations - Kindly Wait",
 ) -> None:
@@ -856,14 +902,15 @@
         except KeyError:
             logging.warning(error_msg)
     else:
         logging.warning(error_msg)
     del prompt_dict, keys
 
 
+@error_handler()
 def main():
     global chatbot, gpt4, record_keeper
     args.disable_stream = True if args.markdown else args.disable_stream
     record_keeper = tracker(args.output)
     args.api_key = get_api_key()
     predefined_prompt_used = intro_train()
     openai.api_key = args.api_key
@@ -903,19 +950,20 @@
         if args.message:
             prompt = (
                 " ".join(run.parser(args.message))
                 if args.message is list
                 else args.message
             )
             if args.bard:
-                run.bard(prompt)
+                run.do_bard(prompt)
             else:
                 run.default(prompt)
         run.cmdloop()
     except (KeyboardInterrupt, EOFError):
         exit(logging.info("Stopping program"))
     except Exception as e:
+        logging.exception(e)
         logging.error(getExc(e))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/helper.py` & `chatgpt4-cli-1.5.1/GPTCLI/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,13 +69,16 @@
 12. gpt4 : Specifies to use ChatGPT in case `--bard` was made default
     e.g gpt4 How do you make?
 
 13. _help : Show this help info
 
 * You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
+* Use `_botchat` to let the 2 GPTs chat to each other
+
 * Use double `./` (fullstop and foward slash) to interact with system commands
       e.g './ifconfig'
+      
 * Use {{f.text-filename}} to issue prompt contained in  the 'text-filename'
 
 * _exit or `CTRL+C` : Quits the program.
         """
```

### Comparing `chatgpt4-cli-1.5.0/GPTCLI/image.py` & `chatgpt4-cli-1.5.1/GPTCLI/image.py`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.0/LICENSE` & `chatgpt4-cli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.5.0/PKG-INFO` & `chatgpt4-cli-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.0
-Summary: Terminal for ChatGPT
+Version: 1.5.1
+Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -33,40 +33,45 @@
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
-CLI tool for interacting with [ChatGPT](https://openai.com). 
-> Chat and generate images.
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com). 
+> Generate images with Bing and ChatGPT's DALL-E model.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
 * [Numpy](https://github.com/numpy/numpy)
 * [Colorama](https://github.com/tartley/colorama)
 * [revChatGPT](https://github.com/acheong08/ChatGPT)
 
 ### Features
 
-- Chat with ChatGPT conversationally.
-- Stream or Non-stream responses
-- Maintain record of the chats
-- Generate Images - Based on your prompt or ChatGPT generated description
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-- Fully customizable Commandline Interface
-- Interact with system commands on the fly
+- Chat with ChatGPT and Bard conversationally.
+- Let **ChatGPT** and **Bard** chat to each other.
+- Generate Images - Based on your prompt or GPT generated description.
+- Stream or Non-stream responses.
+- Maintain record of the chats.
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily.
+- Fully customizable Commandline Interface.
+- Interact with system commands on the fly.
 
 ### Prerequisites
 
 - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
 
+- [x] [Bard Cookies](https://bard.google.com)
+
+- [x] [Bing cookies](https://bing.com)
+
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
 - From pypi
 
@@ -208,14 +213,16 @@
  - e.g ```gpt4 How do you make?```
 
 13._help : Show this help info
 
 * Use  `./` (fullstop and forward slash) to interact with **system commands**
  - e.g ```./ifconfig```
 
+ * Use `_botchat` to let the 2 GPTs chat to each other
+
 > **Note** You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
 * Use *{{f.text-filename}}* to issue prompt contained in the 'text-filename'
 
 </details>
 
 <details>
```

#### html2text {}

```diff
@@ -1,58 +1,60 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.0 Summary: Terminal for
-ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
-Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
-Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Classifier: License :: OSI Approved :: MIT License Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: License :: Free For Home Use
-Classifier: Topic :: Home Automation Classifier: Intended Audience :: Customer
-Service Classifier: Programming Language :: Python Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Programming
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.1 Summary: Interact with
+ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
+Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
+Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
+issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: License :: Free For Home
+Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
+Customer Service Classifier: Programming Language :: Python Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
-CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
-generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
-assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
-//github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
+bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
+[screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
+Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
+github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
-github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT
-conversationally. - Stream or Non-stream responses - Maintain record of the
-chats - Generate Images - Based on your prompt or ChatGPT generated description
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
-easily - Fully customizable Commandline Interface - Interact with system
-commands on the fly ### Prerequisites - [x] [OPENAI_API_KEY](https://
-platform.openai.com/account/api-keys) ## Installation Either of the following
-ways will get you ready. 1. Using pip - From pypi ```sh $ sudo pip install
-chatgpt4-cli ``` - Installing from source ```sh $ sudo pip install git+https://
-github.com/Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh $ git
-clone https://github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3
-setup.py install #or $ python3 setup.py install ``` ## Usage - Make
-OPENAI_API_KEY an environment variable. `$ export OPENAI_API_KEY=` After that
-you can launch the script with or without a prompt > For instance : ```sh
-#Without a prompt $ gpt-cli # With a prompt $ gpt-cli Write a conversation
-between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as one of the arguments
-Run `$ gpt-cli -k  ` at the terminal. > For instance : ```sh $ gpt-cli -
-k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP? ``` The
-[awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be
-parsed to the script through the following ways: - Specifying the role -
-(*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the index of
-the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
-act,prompt and their **indexes** You can as well generate images using EdgeGPT
-(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
-github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
-cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
-image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
-Highlight
+github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
+conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
+Images - Based on your prompt or GPT generated description. - Stream or Non-
+stream responses. - Maintain record of the chats. - Parse [awesome-chatgpt-
+prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
+customizable Commandline Interface. - Interact with system commands on the fly.
+### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
+api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
+(https://bing.com) ## Installation Either of the following ways will get you
+ready. 1. Using pip - From pypi ```sh $ sudo pip install chatgpt4-cli ``` -
+Installing from source ```sh $ sudo pip install git+https://github.com/Simatwa/
+gpt-cli.git ``` 2. Cloning locally and install ```sh $ git clone https://
+github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or
+$ python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
+variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
+or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
+prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
+OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
+For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
+vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
+f/awesome-chatgpt-prompts) can be parsed to the script through the following
+ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
+Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
+cli --dump show` to view the act,prompt and their **indexes** You can as well
+generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
+uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
+``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
+learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
+environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
+or `$gpt-cli-emage -h`. ## Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
@@ -74,18 +76,19 @@
 ```load DAN.json``` 8._save : Save the current Chat Configurations - e.g
 ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) - e.g
 ```_rollback 2``` 10._reset : Reset current chat and start new - e.g ```_reset
 Chat as if you are a 10 year old child``` 11.bard : Specifies to use bard GPT -
 e.g ```bard Explain the composite concept in business``` 12.gpt4 : Specifies to
 use ChatGPT in case `--bard` was made default - e.g ```gpt4 How do you make?```
 13._help : Show this help info * Use `./` (fullstop and forward slash) to
-interact with **system commands** - e.g ```./ifconfig``` > **Note** You can
-further specify the GPT to be used by appending `--gpt4` or `--bard` in the
-prompt. * Use *{{f.text-filename}}* to issue prompt contained in the 'text-
-filename'    For more info run `gpt-cli -h`.  ```
+interact with **system commands** - e.g ```./ifconfig``` * Use `_botchat` to
+let the 2 GPTs chat to each other > **Note** You can further specify the GPT to
+be used by appending `--gpt4` or `--bard` in the prompt. * Use *{{f.text-
+filename}}* to issue prompt contained in the 'text-filename'    For more info
+run `gpt-cli -h`.  ```
 â­âââââââââââââââââââââââââââââââ
 gpt-cli v1.4.9
 ââââââââââââââââââââââââââââââââ®
 â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
 Caleb â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
```

### Comparing `chatgpt4-cli-1.5.0/README.md` & `chatgpt4-cli-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
-CLI tool for interacting with [ChatGPT](https://openai.com). 
-> Chat and generate images.
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com). 
+> Generate images with Bing and ChatGPT's DALL-E model.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
 * [Numpy](https://github.com/numpy/numpy)
 * [Colorama](https://github.com/tartley/colorama)
 * [revChatGPT](https://github.com/acheong08/ChatGPT)
 
 ### Features
 
-- Chat with ChatGPT conversationally.
-- Stream or Non-stream responses
-- Maintain record of the chats
-- Generate Images - Based on your prompt or ChatGPT generated description
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-- Fully customizable Commandline Interface
-- Interact with system commands on the fly
+- Chat with ChatGPT and Bard conversationally.
+- Let **ChatGPT** and **Bard** chat to each other.
+- Generate Images - Based on your prompt or GPT generated description.
+- Stream or Non-stream responses.
+- Maintain record of the chats.
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily.
+- Fully customizable Commandline Interface.
+- Interact with system commands on the fly.
 
 ### Prerequisites
 
 - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
 
+- [x] [Bard Cookies](https://bard.google.com)
+
+- [x] [Bing cookies](https://bing.com)
+
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
 - From pypi
 
@@ -181,14 +186,16 @@
  - e.g ```gpt4 How do you make?```
 
 13._help : Show this help info
 
 * Use  `./` (fullstop and forward slash) to interact with **system commands**
  - e.g ```./ifconfig```
 
+ * Use `_botchat` to let the 2 GPTs chat to each other
+
 > **Note** You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
 * Use *{{f.text-filename}}* to issue prompt contained in the 'text-filename'
 
 </details>
 
 <details>
```

#### html2text {}

```diff
@@ -1,44 +1,46 @@
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
-CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
-generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
-assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
-//github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
+bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
+[screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
+Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
+github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
-github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT
-conversationally. - Stream or Non-stream responses - Maintain record of the
-chats - Generate Images - Based on your prompt or ChatGPT generated description
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
-easily - Fully customizable Commandline Interface - Interact with system
-commands on the fly ### Prerequisites - [x] [OPENAI_API_KEY](https://
-platform.openai.com/account/api-keys) ## Installation Either of the following
-ways will get you ready. 1. Using pip - From pypi ```sh $ sudo pip install
-chatgpt4-cli ``` - Installing from source ```sh $ sudo pip install git+https://
-github.com/Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh $ git
-clone https://github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3
-setup.py install #or $ python3 setup.py install ``` ## Usage - Make
-OPENAI_API_KEY an environment variable. `$ export OPENAI_API_KEY=` After that
-you can launch the script with or without a prompt > For instance : ```sh
-#Without a prompt $ gpt-cli # With a prompt $ gpt-cli Write a conversation
-between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as one of the arguments
-Run `$ gpt-cli -k  ` at the terminal. > For instance : ```sh $ gpt-cli -
-k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP? ``` The
-[awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be
-parsed to the script through the following ways: - Specifying the role -
-(*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the index of
-the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
-act,prompt and their **indexes** You can as well generate images using EdgeGPT
-(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
-github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
-cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
-image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
-Highlight
+github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
+conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
+Images - Based on your prompt or GPT generated description. - Stream or Non-
+stream responses. - Maintain record of the chats. - Parse [awesome-chatgpt-
+prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
+customizable Commandline Interface. - Interact with system commands on the fly.
+### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
+api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
+(https://bing.com) ## Installation Either of the following ways will get you
+ready. 1. Using pip - From pypi ```sh $ sudo pip install chatgpt4-cli ``` -
+Installing from source ```sh $ sudo pip install git+https://github.com/Simatwa/
+gpt-cli.git ``` 2. Cloning locally and install ```sh $ git clone https://
+github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or
+$ python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
+variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
+or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
+prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
+OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
+For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
+vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
+f/awesome-chatgpt-prompts) can be parsed to the script through the following
+ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
+Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
+cli --dump show` to view the act,prompt and their **indexes** You can as well
+generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
+uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
+``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
+learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
+environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
+or `$gpt-cli-emage -h`. ## Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
@@ -60,18 +62,19 @@
 ```load DAN.json``` 8._save : Save the current Chat Configurations - e.g
 ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) - e.g
 ```_rollback 2``` 10._reset : Reset current chat and start new - e.g ```_reset
 Chat as if you are a 10 year old child``` 11.bard : Specifies to use bard GPT -
 e.g ```bard Explain the composite concept in business``` 12.gpt4 : Specifies to
 use ChatGPT in case `--bard` was made default - e.g ```gpt4 How do you make?```
 13._help : Show this help info * Use `./` (fullstop and forward slash) to
-interact with **system commands** - e.g ```./ifconfig``` > **Note** You can
-further specify the GPT to be used by appending `--gpt4` or `--bard` in the
-prompt. * Use *{{f.text-filename}}* to issue prompt contained in the 'text-
-filename'    For more info run `gpt-cli -h`.  ```
+interact with **system commands** - e.g ```./ifconfig``` * Use `_botchat` to
+let the 2 GPTs chat to each other > **Note** You can further specify the GPT to
+be used by appending `--gpt4` or `--bard` in the prompt. * Use *{{f.text-
+filename}}* to issue prompt contained in the 'text-filename'    For more info
+run `gpt-cli -h`.  ```
 â­âââââââââââââââââââââââââââââââ
 gpt-cli v1.4.9
 ââââââââââââââââââââââââââââââââ®
 â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
 Caleb â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
```

### Comparing `chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.1/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.5.0
-Summary: Terminal for ChatGPT
+Version: 1.5.1
+Summary: Interact with ChatGPT and Bard at the terminal.
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -33,40 +33,45 @@
 <a href="#"><img src="https://img.shields.io/static/v1?label=License&message=MIT&color=green&logo=MIT" alt="license"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Development&message=Beta&color=Orange&logo=progress" alt="Progress"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Code Style&message=Black&color=black&logo=Black" alt="Code-style"/></a>
 <a href="#"><img src="https://img.shields.io/static/v1?label=Coverage&message=80%&color=green" alt="Coverage"/></a>
 <a href="https://pepy.tech/project/chatgpt4-cli"><img src="https://static.pepy.tech/badge/chatgpt4-cli" alt="Downloads"/></a>
 </p>
 
-CLI tool for interacting with [ChatGPT](https://openai.com). 
-> Chat and generate images.
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://bard.google.com). 
+> Generate images with Bing and ChatGPT's DALL-E model.
 
 ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/Screenshot1.png)
 
 ## [Independencies](requirements.txt)
 
 * [Openai](https://github.com/openai/openai-python)
 * [Numpy](https://github.com/numpy/numpy)
 * [Colorama](https://github.com/tartley/colorama)
 * [revChatGPT](https://github.com/acheong08/ChatGPT)
 
 ### Features
 
-- Chat with ChatGPT conversationally.
-- Stream or Non-stream responses
-- Maintain record of the chats
-- Generate Images - Based on your prompt or ChatGPT generated description
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily
-- Fully customizable Commandline Interface
-- Interact with system commands on the fly
+- Chat with ChatGPT and Bard conversationally.
+- Let **ChatGPT** and **Bard** chat to each other.
+- Generate Images - Based on your prompt or GPT generated description.
+- Stream or Non-stream responses.
+- Maintain record of the chats.
+- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) easily.
+- Fully customizable Commandline Interface.
+- Interact with system commands on the fly.
 
 ### Prerequisites
 
 - [x] [OPENAI_API_KEY](https://platform.openai.com/account/api-keys)
 
+- [x] [Bard Cookies](https://bard.google.com)
+
+- [x] [Bing cookies](https://bing.com)
+
 ## Installation
 
 Either of the following ways will get you ready.
 
 1. Using pip
 - From pypi
 
@@ -208,14 +213,16 @@
  - e.g ```gpt4 How do you make?```
 
 13._help : Show this help info
 
 * Use  `./` (fullstop and forward slash) to interact with **system commands**
  - e.g ```./ifconfig```
 
+ * Use `_botchat` to let the 2 GPTs chat to each other
+
 > **Note** You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
 * Use *{{f.text-filename}}* to issue prompt contained in the 'text-filename'
 
 </details>
 
 <details>
```

#### html2text {}

```diff
@@ -1,58 +1,60 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.0 Summary: Terminal for
-ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
-Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
-Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
-Classifier: License :: OSI Approved :: MIT License Classifier: Development
-Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
-Natural Language :: English Classifier: License :: Free For Home Use
-Classifier: Topic :: Home Automation Classifier: Intended Audience :: Customer
-Service Classifier: Programming Language :: Python Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Programming
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.1 Summary: Interact with
+ChatGPT and Bard at the terminal. Home-page: https://github.com/Simatwa/gpt-cli
+Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
+Caleb License: MIT Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/
+issues/new Classifier: License :: OSI Approved :: MIT License Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: License :: Free For Home
+Use Classifier: Topic :: Home Automation Classifier: Intended Audience ::
+Customer Service Classifier: Programming Language :: Python Classifier: Topic
+:: Software Development :: Libraries :: Python Modules Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown License-File: LICENSE
                              ****** gpt-cli ******
    [Gihtub] [Pypi]_[wakatime]_[license]_[Progress]_[Code-style]_[Coverage]_
                                   [Downloads]
-CLI tool for interacting with [ChatGPT](https://openai.com). > Chat and
-generate images. ![screenshot](https://github.com/Simatwa/gpt-cli/raw/main/
-assets/Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https:
-//github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
+CLI tool for interacting with [ChatGPT](https://openai.com) and [Bard](https://
+bard.google.com). > Generate images with Bing and ChatGPT's DALL-E model. !
+[screenshot](https://github.com/Simatwa/gpt-cli/raw/main/assets/
+Screenshot1.png) ## [Independencies](requirements.txt) * [Openai](https://
+github.com/openai/openai-python) * [Numpy](https://github.com/numpy/numpy) *
 [Colorama](https://github.com/tartley/colorama) * [revChatGPT](https://
-github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT
-conversationally. - Stream or Non-stream responses - Maintain record of the
-chats - Generate Images - Based on your prompt or ChatGPT generated description
-- Parse [awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
-easily - Fully customizable Commandline Interface - Interact with system
-commands on the fly ### Prerequisites - [x] [OPENAI_API_KEY](https://
-platform.openai.com/account/api-keys) ## Installation Either of the following
-ways will get you ready. 1. Using pip - From pypi ```sh $ sudo pip install
-chatgpt4-cli ``` - Installing from source ```sh $ sudo pip install git+https://
-github.com/Simatwa/gpt-cli.git ``` 2. Cloning locally and install ```sh $ git
-clone https://github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3
-setup.py install #or $ python3 setup.py install ``` ## Usage - Make
-OPENAI_API_KEY an environment variable. `$ export OPENAI_API_KEY=` After that
-you can launch the script with or without a prompt > For instance : ```sh
-#Without a prompt $ gpt-cli # With a prompt $ gpt-cli Write a conversation
-between Sun and Pluto.` ``` - Parsing OPENAI_API_KEY as one of the arguments
-Run `$ gpt-cli -k  ` at the terminal. > For instance : ```sh $ gpt-cli -
-k xxxxxxxxxxxxxxxxxx How to scan for SMB vulnerability using NMAP? ``` The
-[awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) can be
-parsed to the script through the following ways: - Specifying the role -
-(*case-sensitive*) e.g `$ gpt-cli UX/UI Developer` - Specifying the index of
-the prompt: e.g `$ gpt-cli 29` Run `$ gpt-cli --dump show` to view the
-act,prompt and their **indexes** You can as well generate images using EdgeGPT
-(DALL-E) or ChatGPT independent of `gpt-cli`, uninteractively at the terminal:
-1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file   ``` - Visit [EdgeGPT](https://
-github.com/acheong08/EdgeGPT#requirements) to learn more on how to get the
-cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY environment variable $ gpt-cli-
-image  ``` For more info run `$gpt-cli-image -h` or `$gpt-cli-emage -h`. ##
-Highlight
+github.com/acheong08/ChatGPT) ### Features - Chat with ChatGPT and Bard
+conversationally. - Let **ChatGPT** and **Bard** chat to each other. - Generate
+Images - Based on your prompt or GPT generated description. - Stream or Non-
+stream responses. - Maintain record of the chats. - Parse [awesome-chatgpt-
+prompts](https://github.com/f/awesome-chatgpt-prompts) easily. - Fully
+customizable Commandline Interface. - Interact with system commands on the fly.
+### Prerequisites - [x] [OPENAI_API_KEY](https://platform.openai.com/account/
+api-keys) - [x] [Bard Cookies](https://bard.google.com) - [x] [Bing cookies]
+(https://bing.com) ## Installation Either of the following ways will get you
+ready. 1. Using pip - From pypi ```sh $ sudo pip install chatgpt4-cli ``` -
+Installing from source ```sh $ sudo pip install git+https://github.com/Simatwa/
+gpt-cli.git ``` 2. Cloning locally and install ```sh $ git clone https://
+github.com/Simatwa/gpt-cli.git $ cd gpt-cli $ sudo python3 setup.py install #or
+$ python3 setup.py install ``` ## Usage - Make OPENAI_API_KEY an environment
+variable. `$ export OPENAI_API_KEY=` After that you can launch the script with
+or without a prompt > For instance : ```sh #Without a prompt $ gpt-cli # With a
+prompt $ gpt-cli Write a conversation between Sun and Pluto.` ``` - Parsing
+OPENAI_API_KEY as one of the arguments Run `$ gpt-cli -k  ` at the terminal. >
+For instance : ```sh $ gpt-cli -k xxxxxxxxxxxxxxxxxx How to scan for SMB
+vulnerability using NMAP? ``` The [awesome-chatgpt-prompts](https://github.com/
+f/awesome-chatgpt-prompts) can be parsed to the script through the following
+ways: - Specifying the role - (*case-sensitive*) e.g `$ gpt-cli UX/UI
+Developer` - Specifying the index of the prompt: e.g `$ gpt-cli 29` Run `$ gpt-
+cli --dump show` to view the act,prompt and their **indexes** You can as well
+generate images using EdgeGPT (DALL-E) or ChatGPT independent of `gpt-cli`,
+uninteractively at the terminal: 1. EdgeGPT ```sh $ gpt-cli-emage --cookie-file
+``` - Visit [EdgeGPT](https://github.com/acheong08/EdgeGPT#requirements) to
+learn more on how to get the cookies. 2. ChatGPT ```sh # Make OPENAI_API_KEY
+environment variable $ gpt-cli-image  ``` For more info run `$gpt-cli-image -h`
+or `$gpt-cli-emage -h`. ## Highlight
 No. Command           Action
 0   ./{command}       Run command against system
 1   img               Generate image ChatGPT based on prompt
 2   emg               Generate image with EdgeGPT based on prompt
 3   txt2img           Generate image based on GPT description
 4   _font_color       Modify font-color
 5   _background_color Modify background_color
@@ -74,18 +76,19 @@
 ```load DAN.json``` 8._save : Save the current Chat Configurations - e.g
 ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) - e.g
 ```_rollback 2``` 10._reset : Reset current chat and start new - e.g ```_reset
 Chat as if you are a 10 year old child``` 11.bard : Specifies to use bard GPT -
 e.g ```bard Explain the composite concept in business``` 12.gpt4 : Specifies to
 use ChatGPT in case `--bard` was made default - e.g ```gpt4 How do you make?```
 13._help : Show this help info * Use `./` (fullstop and forward slash) to
-interact with **system commands** - e.g ```./ifconfig``` > **Note** You can
-further specify the GPT to be used by appending `--gpt4` or `--bard` in the
-prompt. * Use *{{f.text-filename}}* to issue prompt contained in the 'text-
-filename'    For more info run `gpt-cli -h`.  ```
+interact with **system commands** - e.g ```./ifconfig``` * Use `_botchat` to
+let the 2 GPTs chat to each other > **Note** You can further specify the GPT to
+be used by appending `--gpt4` or `--bard` in the prompt. * Use *{{f.text-
+filename}}* to issue prompt contained in the 'text-filename'    For more info
+run `gpt-cli -h`.  ```
 â­âââââââââââââââââââââââââââââââ
 gpt-cli v1.4.9
 ââââââââââââââââââââââââââââââââ®
 â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
 Caleb â
 â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
```

### Comparing `chatgpt4-cli-1.5.0/setup.py` & `chatgpt4-cli-1.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
     name="chatgpt4-cli",
     packages=["GPTCLI"],
     version=__version__,
     license="MIT",
     author=__author__,
     maintainer=__author__,
     author_email="smartwacaleb@gmail.com",
-    description="Terminal for ChatGPT",
+    description="Interact with ChatGPT and Bard at the terminal.",
     url=__repo__,
     project_urls={"Bug Report": f"{__repo__}/issues/new"},
     install_requires=[
         "numpy>=1.23.4",
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
         "appdirs>=1.4.4",
         "requests>=2.28.2",
         "tabulate>=0.9.0",
-        "GoogleBard==0.0.7"
+        "GoogleBard==0.0.7",
     ],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

