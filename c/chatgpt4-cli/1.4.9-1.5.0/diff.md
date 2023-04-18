# Comparing `tmp/chatgpt4-cli-1.4.9.tar.gz` & `tmp/chatgpt4-cli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt4-cli-1.4.9.tar", last modified: Mon Apr 17 09:35:51 2023, max compression
+gzip compressed data, was "chatgpt4-cli-1.5.0.tar", last modified: Tue Apr 18 21:58:28 2023, max compression
```

## Comparing `chatgpt4-cli-1.4.9.tar` & `chatgpt4-cli-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:35:51.614052 chatgpt4-cli-1.4.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:35:51.610719 chatgpt4-cli-1.4.9/GPTCLI/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-16 20:57:25.000000 chatgpt4-cli-1.4.9/GPTCLI/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/GPTCLI/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3412 2023-04-09 14:37:59.000000 chatgpt4-cli-1.4.9/GPTCLI/addons.py
--rw-r--r--   0 root         (0) root         (0)     7281 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/GPTCLI/emage.py
--rwxr-xr-x   0 root         (0) root         (0)    27488 2023-04-10 22:33:29.000000 chatgpt4-cli-1.4.9/GPTCLI/gptcli.py
--rw-r--r--   0 root         (0) root         (0)     5759 2023-04-08 11:57:02.000000 chatgpt4-cli-1.4.9/GPTCLI/helper.py
--rw-r--r--   0 root         (0) root         (0)     5638 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/GPTCLI/image.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-06 14:49:38.000000 chatgpt4-cli-1.4.9/GPTCLI/test.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-04-03 15:13:44.000000 chatgpt4-cli-1.4.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13107 2023-04-17 09:35:51.610719 chatgpt4-cli-1.4.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12063 2023-04-16 20:57:36.000000 chatgpt4-cli-1.4.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 09:35:51.610719 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13107 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      115 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-17 09:35:51.000000 chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 09:35:51.614052 chatgpt4-cli-1.4.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1616 2023-04-17 09:20:13.000000 chatgpt4-cli-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:28.364807 chatgpt4-cli-1.5.0/GPTCLI/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/bard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/emage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29365 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/gptcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/GPTCLI/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 21:58:28.000000 chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:58:28.368807 chatgpt4-cli-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-18 21:58:06.000000 chatgpt4-cli-1.5.0/setup.py
```

### Comparing `chatgpt4-cli-1.4.9/GPTCLI/addons.py` & `chatgpt4-cli-1.5.0/GPTCLI/addons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import re
 from os import remove, system
 from time import sleep
 from . import logging, getExc
+
+
 class file_parser:
     """Handles contents from text file"""
 
     def __init__(self, prompt):
         self.prompt = prompt
 
     def get_match(self):
@@ -42,15 +44,15 @@
         self.all_interpreters = ["bash", "python", "java", "php", "node"]
 
     def get_interpreter(self, commands: list) -> list:
         st = commands[0]
         for inter in self.all_interpreters:
             if st.startswith(inter):
                 commands.remove(st)
-                commands.insert(0,st.replace(inter,''))
+                commands.insert(0, st.replace(inter, ""))
                 self.interpreter = inter
                 break
 
         return list(set(commands))
 
     def get_command(self, raw: bool = False):
         """Extracts commands from raw text
@@ -105,9 +107,9 @@
         try:
             remove(self.file_name)
         except Exception as e:
             logging.error(getExc(e))
 
 
 if __name__ == "__main__":
-    st = file_parser("I want youn to debug this python code {f.test.py}")
+    st = file_parser("I want you to debug this python code {f.test.py}")
     print(st.parse)
```

### Comparing `chatgpt4-cli-1.4.9/GPTCLI/emage.py` & `chatgpt4-cli-1.5.0/GPTCLI/emage.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             pass
         image_num = 0
         try:
             for link in links:
                 with self.session.get(link, stream=True) as response:
                     # save response to file
                     response.raise_for_status()
-                    with open(f"{output_dir}/{image_num}.jpeg", "wb") as output_file:
+                    with open(f"{output_dir}/{image_num}.jpg", "wb") as output_file:
                         for chunk in response.iter_content(chunk_size=8192):
                             output_file.write(chunk)
 
                 image_num += 1
         except requests.exceptions.MissingSchema as url_exception:
             raise Exception(
                 "Inappropriate contents found in the generated images. Please try again or try another prompt."
```

### Comparing `chatgpt4-cli-1.4.9/GPTCLI/gptcli.py` & `chatgpt4-cli-1.5.0/GPTCLI/gptcli.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,14 +255,39 @@
         parser.add_argument(
             "-cf",
             "--cookie-file",
             help="Path to Bing's cookies - for Edge Image Generation",
             metavar="path",
         )
         parser.add_argument(
+            "-bk", "--bard-key", dest="bkey", metavar="KEY", help="Bard's session value"
+        )
+        parser.add_argument(
+            "-bkp",
+            "--bard-key-path",
+            dest="bkey_path",
+            metavar="PATH",
+            help="Path to Bard's key path",
+        )
+        parser.add_argument(
+            "-bcf",
+            "--bard-cookie-file",
+            dest="bcookie_file",
+            metavar="PATH",
+            help="Path to Bard's cookie file",
+        )
+        parser.add_argument(
+            "-si",
+            "--stream-interval",
+            metavar="TIME",
+            help="Interval for printing responses in (s)",
+            type=float,
+            default=0.01,
+        )
+        parser.add_argument(
             "--disable-stream",
             help="Specifies not to stream responses from ChatGPT",
             action="store_true",
         )
         parser.add_argument(
             "--new-record",
             help="Override previous chats under the filepath",
@@ -275,14 +300,17 @@
         )
         parser.add_argument(
             "--zero-show",
             help="Specifies not to stdout prompt of the act parsed",
             action="store_true",
         )
         parser.add_argument(
+            "--bard", help="Make Bard the default GPT", action="store_true"
+        )
+        parser.add_argument(
             "--markdown",
             help="Stdout responses in markdown-format - disables streaming",
             action="store_true",
         )
         parser.add_argument(
             "--update",
             help="Download latest prompts - [awesome-chatgpt-prompts]",
@@ -311,14 +339,15 @@
 from re import sub
 from datetime import datetime
 from os import system, remove, path, environ, makedirs
 from threading import Thread as thr
 from appdirs import AppDirs
 from rich.markdown import Markdown
 from .addons import file_parser, system_control
+from .bard import Bard
 
 app_dir = AppDirs(
     "smartwa",
     "gpt-cli",
 ).user_data_dir
 
 first_time_run = False
@@ -395,15 +424,15 @@
         self.feedback = None
         self.failed_to_record = False
 
     def save_record(self) -> None:
         """Write prompts and responses in a file"""
         info_to_write = f"\n\n{date_stamp(args.prompt_prefix)}{args.message}\n\n{date_stamp(args.response_prefix)}{self.feedback}"
         try:
-            with open(self.filepath, "a",encoding="utf-8") as fp:
+            with open(self.filepath, "a", encoding="utf-8") as fp:
                 fp.write(info_to_write)
         except Exception as e:
             logging.error(f"Failed to keep record - {getExc(e)}")
             self.failed_to_record = True
 
     def main(self, response: str) -> None:
         """Main method"""
@@ -431,39 +460,38 @@
 
         try:
             logging.info("Updating acts and prompts")
 
             for key, value in self.links.items():
                 resp = get(value)
                 if resp.status_code == 200:
-                    with open(path.join(app_dir, key), "w",encoding="utf-8") as fh:
+                    with open(path.join(app_dir, key), "w", encoding="utf-8") as fh:
                         fh.write(resp.text)
                 else:
                     logging.error(
                         f'Failed to get prompts from "{value}" - [{resp.status_code} : {resp.reason}]'
                     )
         except Exception as e:
             logging.error(getExc(e))
 
     def read_contents(
         self, filename: str = None, delimiter: str = ",", resp: dict = {}
     ):
         """Read prompts and return in dict {act:prompt}"""
         import csv
 
-        with open(filename or self.fnm,encoding="utf-8") as fh:
+        with open(filename or self.fnm, encoding="utf-8") as fh:
             for row in csv.DictReader(fh, delimiter=delimiter):
                 resp[row["act"]] = row["prompt"]
         return resp
 
     def display_info(self, resp: dict) -> None:
         """Displays acts and roles"""
         x = 0
         if args.dump:
-
             # with open(args.dump, "w") as fh:
             if args.dump in ("keys", "roles", "acts", "act", "role"):
                 from tabulate import tabulate
 
                 data = []
                 for key in resp.keys():
                     data.append([key])
@@ -484,15 +512,15 @@
                 for key, value in resp.items():
                     print(
                         f"{config_h.color_dict[args.input_color]}>>[{x}] {key} : {config_h.color_dict[args.output_color]}{value}{Fore.RESET}",
                         end="\n\n",
                     )
                     x += 1
             else:
-                with open(args.dump, "w",encoding="utf-8") as fh:
+                with open(args.dump, "w", encoding="utf-8") as fh:
                     from json import dumps
 
                     data = json.dumps(resp, indent=4)
                     fh.write(data)
                     print(data)
             exit(0)
 
@@ -536,14 +564,15 @@
     )
     prompt = time_now_format(prompt_disp)
     config_handler = config_handler()
     color_dict = config_handler.color_dict
     bcolor_dict = config_handler.bcolor_dict
     interactive = local_interactor()
     parser = lambda self, line: file_parser(line).parse()
+    bard = Bard(args)
 
     def apply_color(self):
         print(
             self.bcolor_dict[args.background_color] + self.color_dict[args.input_color]
         )
 
     def prompt_is_error_free(self, prompt, resp=True) -> bool:
@@ -552,26 +581,28 @@
             if len(prompt) >= 2 and prompt[0:2] == ["I'm", "sorry"]:
                 resp = False
         else:
             if prompt.startswith("I'm sorry"):
                 resp = False
         return resp
 
-    def default(self, raw, return_fb=False):
+    def default(self, raw, return_fb=False, no_check=False):
         raw = self.parser(raw)
         run_against_system = False
         if not raw:
             return
         # out = lambda b: print(self.color_dict[args.output_color] + b + Fore.RESET)
         if raw[0:2] == "./":
             system((raw[2:]).strip())
         else:
             if "--system" in raw:
                 run_against_system = True
                 raw = raw.replace("--system", "")
+            if any(["--bard" in raw, args.bard]) and not no_check:
+                return self.do_bard(raw.replace("--bard", ""))
             args.message = raw
             print(self.color_dict[args.output_color], end="")
             rp = gpt3.main()
             if rp[0]:
                 feedback = sub("\n\n", "\n", rp[1], 1)
                 if return_fb:
                     return feedback.strip()
@@ -580,14 +611,36 @@
                     system_control(feedback).execute(args.sudo)
 
             else:
                 logging.error(str(rp[1]))
             print(Fore.RESET)
         self.do__prompt(self.prompt_disp)
 
+    def do_gpt4(self, line):
+        """Interact with ChatGPT4"""
+        self.default(line, no_check=True)
+
+    def do_bard(self, line):
+        """Interact with Google's bard"""
+        if "--gpt4" in line:
+            return self.default(line.replace("--gpt4", ""), no_check=True)
+
+        args.message = line
+        print(self.color_dict[args.output_color], end="")
+        if args.disable_stream:
+            info = self.bard.chat(line, False)
+            gpt3.out(info)
+        else:
+            info = ""
+            for val in self.bard.chat(line):
+                print(val, end="", flush=True)
+                info = info + val
+        record_keeper.main(info)
+        print(Fore.RESET)
+
     def do_txt2img(self, line):
         """Generate images based on GPT description"""
         line = self.parser(line)
         if not line:
             return
         print(
             self.color_dict[args.output_color] + ">>[*] Querying description from GPT",
@@ -749,15 +802,15 @@
 
 def get_api_key() -> str:
     """Gets API from Key_path or args.key"""
     if any([args.key, environ.get("OPENAI_API_KEY")]):
         return args.key or environ.get("OPENAI_API_KEY")
     if args.key_path:
         try:
-            with open(args.key_path,encoding="utf-8") as fh:
+            with open(args.key_path, encoding="utf-8") as fh:
                 return fh.readlines()[0]
         except Exception as e:
             exit(logging.critical("While opening Key_Path " + getExc(e)))
 
 
 def intro_train(
     error_msg: str = "Initializing default configurations - Kindly Wait",
@@ -844,21 +897,25 @@
         exit(logging.critical(getExc(e)))
 
     try:
         if args.new_record and path.isfile(args.output):
             remove(args.output)
         run = main_gpt()
         if args.message:
-            run.default(
+            prompt = (
                 " ".join(run.parser(args.message))
                 if args.message is list
                 else args.message
             )
+            if args.bard:
+                run.bard(prompt)
+            else:
+                run.default(prompt)
         run.cmdloop()
     except (KeyboardInterrupt, EOFError):
         exit(logging.info("Stopping program"))
     except Exception as e:
-        print(getExc(e))
+        logging.error(getExc(e))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatgpt4-cli-1.4.9/GPTCLI/helper.py` & `chatgpt4-cli-1.5.0/GPTCLI/helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -59,15 +59,23 @@
 
 8. _rollback : Rollback the Chat by  {{n}} time(s)
     e.g '_rollback 2'
 
 9. _reset : Reset current chat and start new
     e.g '_reset Chat as if you are a 10 year old child'
 
-10. _help : Show this help info
+11. bard : Specifies to use bard GPT
+    e.g bard Explain the composite concept in business.
+
+12. gpt4 : Specifies to use ChatGPT in case `--bard` was made default
+    e.g gpt4 How do you make?
+
+13. _help : Show this help info
+
+* You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
 
 * Use double `./` (fullstop and foward slash) to interact with system commands
       e.g './ifconfig'
 * Use {{f.text-filename}} to issue prompt contained in  the 'text-filename'
 
 * _exit or `CTRL+C` : Quits the program.
         """
```

### Comparing `chatgpt4-cli-1.4.9/GPTCLI/image.py` & `chatgpt4-cli-1.5.0/GPTCLI/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             """Saves the image"""
             if not path.isdir(self.args.dir):
                 from os import makedirs
 
                 makedirs(self.args.dir)
             cpath = path.join(
                 self.args.dir,
-                f'{self.args.output}{self.save_count if self.save_count else ""}.png',
+                f'{self.args.output}{self.save_count if self.save_count else ""}.jpg',
             )
             if path.isfile(cpath):
                 self.save_count += 1
                 return self.write_buff(data)
 
             with open(cpath, "wb") as fh:
                 fh.write(data)
```

### Comparing `chatgpt4-cli-1.4.9/LICENSE` & `chatgpt4-cli-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt4-cli-1.4.9/PKG-INFO` & `chatgpt4-cli-1.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.4.9
+Version: 1.5.0
 Summary: Terminal for ChatGPT
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -183,65 +183,78 @@
 4._font_color : modifies font-color
  - e.g ```font_color input red```
 
 5._background_color : modifies background_color
  - e.g ```background_color cyan```
 
 6._prompt : Modify CMD prompt
- - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
+ - e.g ```prompt ┌─[Smartwa@GPT-CLI]─(%H:%M:%S)```
 
 7._load : Load configurations from the json file
  - e.g ```load DAN.json```
 
 8._save : Save the current Chat Configurations
  - e.g ```save DAN.json```
 
 9._rollback : Rollback the Chat by the {n} time(s)
  - e.g ```_rollback 2```
 
 10._reset : Reset current chat and start new
  - e.g ```_reset Chat as if you are a 10 year old child```
 
-11._help : Show this help info
+11.bard : Specifies to use bard GPT
+ - e.g ```bard Explain the composite concept in business```
 
-* Use double `./` *(fullstop and forward slash)* to interact with
+12.gpt4 : Specifies to use ChatGPT in case `--bard` was made default
+ - e.g ```gpt4 How do you make?```
 
-**system commands**
+13._help : Show this help info
 
-  e.g ```./ifconfig```
+* Use  `./` (fullstop and forward slash) to interact with **system commands**
+ - e.g ```./ifconfig```
+
+> **Note** You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
+
+* Use *{{f.text-filename}}* to issue prompt contained in the 'text-filename'
 
 </details>
 
 <details>
 
 <summary>
 
 For more info run `gpt-cli -h`.
 
 </summary>
 
 ```
+╭─────────────────────────────── gpt-cli v1.4.9 ───────────────────────────────╮
+│                                                                              │
+│             Repo : https://github.com/Simatwa/gpt-cli                        │
+│             By   : Smartwa Caleb                                             │
+╰──────────────────────────────────────────────────────────────────────────────╯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
                [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
                [-fp path] [-o path] [-pp prefix] [-rp prefix]
-               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
-               [--disable-stream] [--new-record] [--disable-recording]
-               [--zero-show] [--markdown] [--update]
+               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path] [-bk KEY]
+               [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream]
+               [--new-record] [--disable-recording] [--zero-show] [--bard]
+               [--markdown] [--update] [--sudo]
                [message ...]
 
 Interact with ChatGPT at the terminal
 
 positional arguments:
   message               Message to be send.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
                         ChatGPT model to be used
   -t [0.1-1], --temperature [0.1-1]
                         Charge of the generated text's randomness
   -mt [1-7000], --max-tokens [1-7000]
@@ -279,41 +292,52 @@
                         Path to .csv file containing role and prompt -
                         [act,prompt]
   -o path, --output path
                         Filepath for saving the chats - default
                         [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
   -pp prefix, --prompt-prefix prefix
                         Text to append before saving each prompt - default
-                        [>>timestamp]
+                        [>>> timestamp]
   -rp prefix, --response-prefix prefix
                         Text to append before saving each response - default
                         [None]
   -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
                         Stdout [keys,values]; Save all prompts in json format
                         to a file
   -dl symbol, --delimiter symbol
                         Delimeter for the .CSV file - [act,prompt]
   -cf path, --cookie-file path
                         Path to Bing's cookies - for Edge Image Generation
+  -bk KEY, --bard-key KEY
+                        Bard's session value
+  -bkp PATH, --bard-key-path PATH
+                        Path to Bard's key path
+  -bcf PATH, --bard-cookie-file PATH
+                        Path to Bard's cookie file
+  -si TIME, --stream-interval TIME
+                        Interval for printing responses in (s)
   --disable-stream      Specifies not to stream responses from ChatGPT
   --new-record          Override previous chats under the filepath
   --disable-recording   Disable saving prompts and responses
   --zero-show           Specifies not to stdout prompt of the act parsed
+  --bard                Make Bard the default GPT
   --markdown            Stdout responses in markdown-format - disables
                         streaming
   --update              Download latest prompts - [awesome-chatgpt-prompts]
+  --sudo                Run commands against system with sudo privileges
 
 ```
 
 </details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
 > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
 
+Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on how to get the Bard's cookie file and Sessions.
 
 ## Motive
 
 <details>
 
 <summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.9 Summary: Terminal for
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.0 Summary: Terminal for
 ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
 Classifier: Topic :: Home Automation Classifier: Intended Audience :: Customer
@@ -65,70 +65,88 @@
 12  {Any Other}       Chat with ChatGPT
  1.img : Text-to-Image converter - ChatGPT - e.g ```img Toddler cartoon coding
 in Python``` 2.emg : Text-to-Image converter - EdgeGPT - e.g ```emg Toddler
 cartoon coding in Python``` 3.txt2img : Generate image based on GPT description
 - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
 4._font_color : modifies font-color - e.g ```font_color input red```
 5._background_color : modifies background_color - e.g ```background_color
-cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ
-[Smartwa@ChatGPT4]â(%H:%M:%S)``` 7._load : Load configurations from the json
-file - e.g ```load DAN.json``` 8._save : Save the current Chat Configurations -
-e.g ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) -
-e.g ```_rollback 2``` 10._reset : Reset current chat and start new - e.g
-```_reset Chat as if you are a 10 year old child``` 11._help : Show this help
-info * Use double `./` *(fullstop and forward slash)* to interact with **system
-commands** e.g ```./ifconfig```    For more info run `gpt-cli -h`.  ``` usage:
-gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-
-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
+cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ[Smartwa@GPT-
+CLI]â(%H:%M:%S)``` 7._load : Load configurations from the json file - e.g
+```load DAN.json``` 8._save : Save the current Chat Configurations - e.g
+```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) - e.g
+```_rollback 2``` 10._reset : Reset current chat and start new - e.g ```_reset
+Chat as if you are a 10 year old child``` 11.bard : Specifies to use bard GPT -
+e.g ```bard Explain the composite concept in business``` 12.gpt4 : Specifies to
+use ChatGPT in case `--bard` was made default - e.g ```gpt4 How do you make?```
+13._help : Show this help info * Use `./` (fullstop and forward slash) to
+interact with **system commands** - e.g ```./ifconfig``` > **Note** You can
+further specify the GPT to be used by appending `--gpt4` or `--bard` in the
+prompt. * Use *{{f.text-filename}}* to issue prompt contained in the 'text-
+filename'    For more info run `gpt-cli -h`.  ```
+â­âââââââââââââââââââââââââââââââ
+gpt-cli v1.4.9
+ââââââââââââââââââââââââââââââââ®
+â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
+Caleb â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
+[1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
-[-cf path] [--disable-stream] [--new-record] [--disable-recording] [--zero-
-show] [--markdown] [--update] [message ...] Interact with ChatGPT at the
-terminal positional arguments: message Message to be send. optional arguments:
--h, --help show this help message and exit -v, --version show program's version
-number and exit -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-
-4|gpt-4-32k ChatGPT model to be used -t [0.1-1], --temperature [0.1-1] Charge
-of the generated text's randomness -mt [1-7000], --max-tokens [1-7000] Maximum
-number of tokens to be generated upon completion -tp [0.1-1], --top-p [0.1-1]
-Sampling threshold during inference time -f [0.1-2], --frequency-penalty [0.1-
-2] Chances of word being repeated -p [0.1-2], --presence-frequency [0.1-2]
-Chances of topic being repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --
-key-path path Path to text-file containing GPT-api key -ic
-[cyan|green|yellow|red], --input-color [cyan|green|yellow|red] Font color for
-inputs -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red] Font
-color for outputs -bc [blue,magenta,black,reset], --background-color
-[blue,magenta,black,reset] Console's background-color -pc
-[cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red] Prompt's
-display color --prompt [SETTINGS ...] Customizes the prompt display -tm value,
---timeout value Request timeout while making request - (Soon) -pr PROXY, --
-proxy PROXY Pivot request through this proxy -rc value, --reply-count value
-Number of responses to be received -g 1,4, --gpt 1,4 ChatGPT version to be used
--sp [text ...], --system-prompt [text ...] Text to train ChatGPT at the start -
-fp path, --file-path path Path to .csv file containing role and prompt -
-[act,prompt] -o path, --output path Filepath for saving the chats - default [/
-home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp prefix, --prompt-prefix
-prefix Text to append before saving each prompt - default [>>timestamp] -rp
-prefix, --response-prefix prefix Text to append before saving each response -
-default [None] -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm} Stdout
-[keys,values]; Save all prompts in json format to a file -dl symbol, --
-delimiter symbol Delimeter for the .CSV file - [act,prompt] -cf path, --cookie-
-file path Path to Bing's cookies - for Edge Image Generation --disable-stream
-Specifies not to stream responses from ChatGPT --new-record Override previous
-chats under the filepath --disable-recording Disable saving prompts and
-responses --zero-show Specifies not to stdout prompt of the act parsed --
-markdown Stdout responses in markdown-format - disables streaming --update
-Download latest prompts - [awesome-chatgpt-prompts] ```  > **Note** : **gpt-4**
-*(model)* supports upto *7000* tokens and others *3000*. > **Warning** : **gpt-
-1** Has issues - *(To be fixed later)* ## Motive   Love for `Terminal` â¤ï¸
-As a `terminal guy` I used to find it uncomfortable to keep shifting from one
-window to next in order to access ChatGPT even after trying out the [gpt-login]
-(https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/
-Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https://
-github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/
-gpt-cli/issues) without any **guideline** or submitting a [pull request](https:
-//github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue
-prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://github.com/
-Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
-(https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
-acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream] [--
+new-record] [--disable-recording] [--zero-show] [--bard] [--markdown] [--
+update] [--sudo] [message ...] Interact with ChatGPT at the terminal positional
+arguments: message Message to be send. options: -h, --help show this help
+message and exit -v, --version show program's version number and exit -m gpt-
+3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k ChatGPT model
+to be used -t [0.1-1], --temperature [0.1-1] Charge of the generated text's
+randomness -mt [1-7000], --max-tokens [1-7000] Maximum number of tokens to be
+generated upon completion -tp [0.1-1], --top-p [0.1-1] Sampling threshold
+during inference time -f [0.1-2], --frequency-penalty [0.1-2] Chances of word
+being repeated -p [0.1-2], --presence-frequency [0.1-2] Chances of topic being
+repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --key-path path Path to
+text-file containing GPT-api key -ic [cyan|green|yellow|red], --input-color
+[cyan|green|yellow|red] Font color for inputs -oc [cyan|green|yellow|red], --
+output-color [cyan|green|yellow|red] Font color for outputs -bc
+[blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
+Console's background-color -pc [cyan|green|yellow|red], --prompt-color
+[cyan|green|yellow|red] Prompt's display color --prompt [SETTINGS ...]
+Customizes the prompt display -tm value, --timeout value Request timeout while
+making request - (Soon) -pr PROXY, --proxy PROXY Pivot request through this
+proxy -rc value, --reply-count value Number of responses to be received -g 1,4,
+--gpt 1,4 ChatGPT version to be used -sp [text ...], --system-prompt [text ...]
+Text to train ChatGPT at the start -fp path, --file-path path Path to .csv file
+containing role and prompt - [act,prompt] -o path, --output path Filepath for
+saving the chats - default [/home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp
+prefix, --prompt-prefix prefix Text to append before saving each prompt -
+default [>>> timestamp] -rp prefix, --response-prefix prefix Text to append
+before saving each response - default [None] -dm keys|values|show|{fnm}, --dump
+keys|values|show|{fnm} Stdout [keys,values]; Save all prompts in json format to
+a file -dl symbol, --delimiter symbol Delimeter for the .CSV file -
+[act,prompt] -cf path, --cookie-file path Path to Bing's cookies - for Edge
+Image Generation -bk KEY, --bard-key KEY Bard's session value -bkp PATH, --
+bard-key-path PATH Path to Bard's key path -bcf PATH, --bard-cookie-file PATH
+Path to Bard's cookie file -si TIME, --stream-interval TIME Interval for
+printing responses in (s) --disable-stream Specifies not to stream responses
+from ChatGPT --new-record Override previous chats under the filepath --disable-
+recording Disable saving prompts and responses --zero-show Specifies not to
+stdout prompt of the act parsed --bard Make Bard the default GPT --markdown
+Stdout responses in markdown-format - disables streaming --update Download
+latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against system
+with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto *7000*
+tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be fixed
+later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on
+how to get the Bard's cookie file and Sessions. ## Motive   Love for `Terminal`
+â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep shifting
+from one window to next in order to access ChatGPT even after trying out the
+[gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://
+github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https:
+//github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/
+Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull
+request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue
+- [x] Issue prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://
+github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1.
+[remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
+github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
+prompts)
```

### Comparing `chatgpt4-cli-1.4.9/README.md` & `chatgpt4-cli-1.5.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -156,65 +156,78 @@
 4._font_color : modifies font-color
  - e.g ```font_color input red```
 
 5._background_color : modifies background_color
  - e.g ```background_color cyan```
 
 6._prompt : Modify CMD prompt
- - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
+ - e.g ```prompt ┌─[Smartwa@GPT-CLI]─(%H:%M:%S)```
 
 7._load : Load configurations from the json file
  - e.g ```load DAN.json```
 
 8._save : Save the current Chat Configurations
  - e.g ```save DAN.json```
 
 9._rollback : Rollback the Chat by the {n} time(s)
  - e.g ```_rollback 2```
 
 10._reset : Reset current chat and start new
  - e.g ```_reset Chat as if you are a 10 year old child```
 
-11._help : Show this help info
+11.bard : Specifies to use bard GPT
+ - e.g ```bard Explain the composite concept in business```
 
-* Use double `./` *(fullstop and forward slash)* to interact with
+12.gpt4 : Specifies to use ChatGPT in case `--bard` was made default
+ - e.g ```gpt4 How do you make?```
 
-**system commands**
+13._help : Show this help info
 
-  e.g ```./ifconfig```
+* Use  `./` (fullstop and forward slash) to interact with **system commands**
+ - e.g ```./ifconfig```
+
+> **Note** You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
+
+* Use *{{f.text-filename}}* to issue prompt contained in the 'text-filename'
 
 </details>
 
 <details>
 
 <summary>
 
 For more info run `gpt-cli -h`.
 
 </summary>
 
 ```
+╭─────────────────────────────── gpt-cli v1.4.9 ───────────────────────────────╮
+│                                                                              │
+│             Repo : https://github.com/Simatwa/gpt-cli                        │
+│             By   : Smartwa Caleb                                             │
+╰──────────────────────────────────────────────────────────────────────────────╯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
                [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
                [-fp path] [-o path] [-pp prefix] [-rp prefix]
-               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
-               [--disable-stream] [--new-record] [--disable-recording]
-               [--zero-show] [--markdown] [--update]
+               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path] [-bk KEY]
+               [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream]
+               [--new-record] [--disable-recording] [--zero-show] [--bard]
+               [--markdown] [--update] [--sudo]
                [message ...]
 
 Interact with ChatGPT at the terminal
 
 positional arguments:
   message               Message to be send.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
                         ChatGPT model to be used
   -t [0.1-1], --temperature [0.1-1]
                         Charge of the generated text's randomness
   -mt [1-7000], --max-tokens [1-7000]
@@ -252,41 +265,52 @@
                         Path to .csv file containing role and prompt -
                         [act,prompt]
   -o path, --output path
                         Filepath for saving the chats - default
                         [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
   -pp prefix, --prompt-prefix prefix
                         Text to append before saving each prompt - default
-                        [>>timestamp]
+                        [>>> timestamp]
   -rp prefix, --response-prefix prefix
                         Text to append before saving each response - default
                         [None]
   -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
                         Stdout [keys,values]; Save all prompts in json format
                         to a file
   -dl symbol, --delimiter symbol
                         Delimeter for the .CSV file - [act,prompt]
   -cf path, --cookie-file path
                         Path to Bing's cookies - for Edge Image Generation
+  -bk KEY, --bard-key KEY
+                        Bard's session value
+  -bkp PATH, --bard-key-path PATH
+                        Path to Bard's key path
+  -bcf PATH, --bard-cookie-file PATH
+                        Path to Bard's cookie file
+  -si TIME, --stream-interval TIME
+                        Interval for printing responses in (s)
   --disable-stream      Specifies not to stream responses from ChatGPT
   --new-record          Override previous chats under the filepath
   --disable-recording   Disable saving prompts and responses
   --zero-show           Specifies not to stdout prompt of the act parsed
+  --bard                Make Bard the default GPT
   --markdown            Stdout responses in markdown-format - disables
                         streaming
   --update              Download latest prompts - [awesome-chatgpt-prompts]
+  --sudo                Run commands against system with sudo privileges
 
 ```
 
 </details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
 > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
 
+Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on how to get the Bard's cookie file and Sessions.
 
 ## Motive
 
 <details>
 
 <summary>
```

#### html2text {}

```diff
@@ -51,70 +51,88 @@
 12  {Any Other}       Chat with ChatGPT
  1.img : Text-to-Image converter - ChatGPT - e.g ```img Toddler cartoon coding
 in Python``` 2.emg : Text-to-Image converter - EdgeGPT - e.g ```emg Toddler
 cartoon coding in Python``` 3.txt2img : Generate image based on GPT description
 - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
 4._font_color : modifies font-color - e.g ```font_color input red```
 5._background_color : modifies background_color - e.g ```background_color
-cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ
-[Smartwa@ChatGPT4]â(%H:%M:%S)``` 7._load : Load configurations from the json
-file - e.g ```load DAN.json``` 8._save : Save the current Chat Configurations -
-e.g ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) -
-e.g ```_rollback 2``` 10._reset : Reset current chat and start new - e.g
-```_reset Chat as if you are a 10 year old child``` 11._help : Show this help
-info * Use double `./` *(fullstop and forward slash)* to interact with **system
-commands** e.g ```./ifconfig```    For more info run `gpt-cli -h`.  ``` usage:
-gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-
-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
+cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ[Smartwa@GPT-
+CLI]â(%H:%M:%S)``` 7._load : Load configurations from the json file - e.g
+```load DAN.json``` 8._save : Save the current Chat Configurations - e.g
+```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) - e.g
+```_rollback 2``` 10._reset : Reset current chat and start new - e.g ```_reset
+Chat as if you are a 10 year old child``` 11.bard : Specifies to use bard GPT -
+e.g ```bard Explain the composite concept in business``` 12.gpt4 : Specifies to
+use ChatGPT in case `--bard` was made default - e.g ```gpt4 How do you make?```
+13._help : Show this help info * Use `./` (fullstop and forward slash) to
+interact with **system commands** - e.g ```./ifconfig``` > **Note** You can
+further specify the GPT to be used by appending `--gpt4` or `--bard` in the
+prompt. * Use *{{f.text-filename}}* to issue prompt contained in the 'text-
+filename'    For more info run `gpt-cli -h`.  ```
+â­âââââââââââââââââââââââââââââââ
+gpt-cli v1.4.9
+ââââââââââââââââââââââââââââââââ®
+â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
+Caleb â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
+[1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
-[-cf path] [--disable-stream] [--new-record] [--disable-recording] [--zero-
-show] [--markdown] [--update] [message ...] Interact with ChatGPT at the
-terminal positional arguments: message Message to be send. optional arguments:
--h, --help show this help message and exit -v, --version show program's version
-number and exit -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-
-4|gpt-4-32k ChatGPT model to be used -t [0.1-1], --temperature [0.1-1] Charge
-of the generated text's randomness -mt [1-7000], --max-tokens [1-7000] Maximum
-number of tokens to be generated upon completion -tp [0.1-1], --top-p [0.1-1]
-Sampling threshold during inference time -f [0.1-2], --frequency-penalty [0.1-
-2] Chances of word being repeated -p [0.1-2], --presence-frequency [0.1-2]
-Chances of topic being repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --
-key-path path Path to text-file containing GPT-api key -ic
-[cyan|green|yellow|red], --input-color [cyan|green|yellow|red] Font color for
-inputs -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red] Font
-color for outputs -bc [blue,magenta,black,reset], --background-color
-[blue,magenta,black,reset] Console's background-color -pc
-[cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red] Prompt's
-display color --prompt [SETTINGS ...] Customizes the prompt display -tm value,
---timeout value Request timeout while making request - (Soon) -pr PROXY, --
-proxy PROXY Pivot request through this proxy -rc value, --reply-count value
-Number of responses to be received -g 1,4, --gpt 1,4 ChatGPT version to be used
--sp [text ...], --system-prompt [text ...] Text to train ChatGPT at the start -
-fp path, --file-path path Path to .csv file containing role and prompt -
-[act,prompt] -o path, --output path Filepath for saving the chats - default [/
-home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp prefix, --prompt-prefix
-prefix Text to append before saving each prompt - default [>>timestamp] -rp
-prefix, --response-prefix prefix Text to append before saving each response -
-default [None] -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm} Stdout
-[keys,values]; Save all prompts in json format to a file -dl symbol, --
-delimiter symbol Delimeter for the .CSV file - [act,prompt] -cf path, --cookie-
-file path Path to Bing's cookies - for Edge Image Generation --disable-stream
-Specifies not to stream responses from ChatGPT --new-record Override previous
-chats under the filepath --disable-recording Disable saving prompts and
-responses --zero-show Specifies not to stdout prompt of the act parsed --
-markdown Stdout responses in markdown-format - disables streaming --update
-Download latest prompts - [awesome-chatgpt-prompts] ```  > **Note** : **gpt-4**
-*(model)* supports upto *7000* tokens and others *3000*. > **Warning** : **gpt-
-1** Has issues - *(To be fixed later)* ## Motive   Love for `Terminal` â¤ï¸
-As a `terminal guy` I used to find it uncomfortable to keep shifting from one
-window to next in order to access ChatGPT even after trying out the [gpt-login]
-(https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/
-Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https://
-github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/
-gpt-cli/issues) without any **guideline** or submitting a [pull request](https:
-//github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue
-prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://github.com/
-Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
-(https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
-acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream] [--
+new-record] [--disable-recording] [--zero-show] [--bard] [--markdown] [--
+update] [--sudo] [message ...] Interact with ChatGPT at the terminal positional
+arguments: message Message to be send. options: -h, --help show this help
+message and exit -v, --version show program's version number and exit -m gpt-
+3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k ChatGPT model
+to be used -t [0.1-1], --temperature [0.1-1] Charge of the generated text's
+randomness -mt [1-7000], --max-tokens [1-7000] Maximum number of tokens to be
+generated upon completion -tp [0.1-1], --top-p [0.1-1] Sampling threshold
+during inference time -f [0.1-2], --frequency-penalty [0.1-2] Chances of word
+being repeated -p [0.1-2], --presence-frequency [0.1-2] Chances of topic being
+repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --key-path path Path to
+text-file containing GPT-api key -ic [cyan|green|yellow|red], --input-color
+[cyan|green|yellow|red] Font color for inputs -oc [cyan|green|yellow|red], --
+output-color [cyan|green|yellow|red] Font color for outputs -bc
+[blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
+Console's background-color -pc [cyan|green|yellow|red], --prompt-color
+[cyan|green|yellow|red] Prompt's display color --prompt [SETTINGS ...]
+Customizes the prompt display -tm value, --timeout value Request timeout while
+making request - (Soon) -pr PROXY, --proxy PROXY Pivot request through this
+proxy -rc value, --reply-count value Number of responses to be received -g 1,4,
+--gpt 1,4 ChatGPT version to be used -sp [text ...], --system-prompt [text ...]
+Text to train ChatGPT at the start -fp path, --file-path path Path to .csv file
+containing role and prompt - [act,prompt] -o path, --output path Filepath for
+saving the chats - default [/home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp
+prefix, --prompt-prefix prefix Text to append before saving each prompt -
+default [>>> timestamp] -rp prefix, --response-prefix prefix Text to append
+before saving each response - default [None] -dm keys|values|show|{fnm}, --dump
+keys|values|show|{fnm} Stdout [keys,values]; Save all prompts in json format to
+a file -dl symbol, --delimiter symbol Delimeter for the .CSV file -
+[act,prompt] -cf path, --cookie-file path Path to Bing's cookies - for Edge
+Image Generation -bk KEY, --bard-key KEY Bard's session value -bkp PATH, --
+bard-key-path PATH Path to Bard's key path -bcf PATH, --bard-cookie-file PATH
+Path to Bard's cookie file -si TIME, --stream-interval TIME Interval for
+printing responses in (s) --disable-stream Specifies not to stream responses
+from ChatGPT --new-record Override previous chats under the filepath --disable-
+recording Disable saving prompts and responses --zero-show Specifies not to
+stdout prompt of the act parsed --bard Make Bard the default GPT --markdown
+Stdout responses in markdown-format - disables streaming --update Download
+latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against system
+with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto *7000*
+tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be fixed
+later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on
+how to get the Bard's cookie file and Sessions. ## Motive   Love for `Terminal`
+â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep shifting
+from one window to next in order to access ChatGPT even after trying out the
+[gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://
+github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https:
+//github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/
+Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull
+request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue
+- [x] Issue prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://
+github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1.
+[remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
+github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
+prompts)
```

### Comparing `chatgpt4-cli-1.4.9/chatgpt4_cli.egg-info/PKG-INFO` & `chatgpt4-cli-1.5.0/chatgpt4_cli.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt4-cli
-Version: 1.4.9
+Version: 1.5.0
 Summary: Terminal for ChatGPT
 Home-page: https://github.com/Simatwa/gpt-cli
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
@@ -183,65 +183,78 @@
 4._font_color : modifies font-color
  - e.g ```font_color input red```
 
 5._background_color : modifies background_color
  - e.g ```background_color cyan```
 
 6._prompt : Modify CMD prompt
- - e.g ```prompt ┌─[Smartwa@ChatGPT4]─(%H:%M:%S)```
+ - e.g ```prompt ┌─[Smartwa@GPT-CLI]─(%H:%M:%S)```
 
 7._load : Load configurations from the json file
  - e.g ```load DAN.json```
 
 8._save : Save the current Chat Configurations
  - e.g ```save DAN.json```
 
 9._rollback : Rollback the Chat by the {n} time(s)
  - e.g ```_rollback 2```
 
 10._reset : Reset current chat and start new
  - e.g ```_reset Chat as if you are a 10 year old child```
 
-11._help : Show this help info
+11.bard : Specifies to use bard GPT
+ - e.g ```bard Explain the composite concept in business```
 
-* Use double `./` *(fullstop and forward slash)* to interact with
+12.gpt4 : Specifies to use ChatGPT in case `--bard` was made default
+ - e.g ```gpt4 How do you make?```
 
-**system commands**
+13._help : Show this help info
 
-  e.g ```./ifconfig```
+* Use  `./` (fullstop and forward slash) to interact with **system commands**
+ - e.g ```./ifconfig```
+
+> **Note** You can further specify the GPT to be used by appending `--gpt4` or `--bard` in the prompt.
+
+* Use *{{f.text-filename}}* to issue prompt contained in the 'text-filename'
 
 </details>
 
 <details>
 
 <summary>
 
 For more info run `gpt-cli -h`.
 
 </summary>
 
 ```
+╭─────────────────────────────── gpt-cli v1.4.9 ───────────────────────────────╮
+│                                                                              │
+│             Repo : https://github.com/Simatwa/gpt-cli                        │
+│             By   : Smartwa Caleb                                             │
+╰──────────────────────────────────────────────────────────────────────────────╯
 usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]]
                [-mt [1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY]
                [-kp path] [-ic [cyan|green|yellow|red]]
                [-oc [cyan|green|yellow|red]] [-bc [blue,magenta,black,reset]]
                [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS ...]]
                [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]]
                [-fp path] [-o path] [-pp prefix] [-rp prefix]
-               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path]
-               [--disable-stream] [--new-record] [--disable-recording]
-               [--zero-show] [--markdown] [--update]
+               [-dm keys|values|show|{fnm}] [-dl symbol] [-cf path] [-bk KEY]
+               [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream]
+               [--new-record] [--disable-recording] [--zero-show] [--bard]
+               [--markdown] [--update] [--sudo]
                [message ...]
 
 Interact with ChatGPT at the terminal
 
 positional arguments:
   message               Message to be send.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k
                         ChatGPT model to be used
   -t [0.1-1], --temperature [0.1-1]
                         Charge of the generated text's randomness
   -mt [1-7000], --max-tokens [1-7000]
@@ -279,41 +292,52 @@
                         Path to .csv file containing role and prompt -
                         [act,prompt]
   -o path, --output path
                         Filepath for saving the chats - default
                         [/home/smartwa/git/gpt-cli/.chatgpt-history.txt]
   -pp prefix, --prompt-prefix prefix
                         Text to append before saving each prompt - default
-                        [>>timestamp]
+                        [>>> timestamp]
   -rp prefix, --response-prefix prefix
                         Text to append before saving each response - default
                         [None]
   -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm}
                         Stdout [keys,values]; Save all prompts in json format
                         to a file
   -dl symbol, --delimiter symbol
                         Delimeter for the .CSV file - [act,prompt]
   -cf path, --cookie-file path
                         Path to Bing's cookies - for Edge Image Generation
+  -bk KEY, --bard-key KEY
+                        Bard's session value
+  -bkp PATH, --bard-key-path PATH
+                        Path to Bard's key path
+  -bcf PATH, --bard-cookie-file PATH
+                        Path to Bard's cookie file
+  -si TIME, --stream-interval TIME
+                        Interval for printing responses in (s)
   --disable-stream      Specifies not to stream responses from ChatGPT
   --new-record          Override previous chats under the filepath
   --disable-recording   Disable saving prompts and responses
   --zero-show           Specifies not to stdout prompt of the act parsed
+  --bard                Make Bard the default GPT
   --markdown            Stdout responses in markdown-format - disables
                         streaming
   --update              Download latest prompts - [awesome-chatgpt-prompts]
+  --sudo                Run commands against system with sudo privileges
 
 ```
 
 </details>
 
 > **Note** : **gpt-4** *(model)* supports upto *7000* tokens and others *3000*.
 
 > **Warning** : **gpt-1**  Has issues - *(To be fixed later)*
 
+Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on how to get the Bard's cookie file and Sessions.
 
 ## Motive
 
 <details>
 
 <summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.4.9 Summary: Terminal for
+Metadata-Version: 2.1 Name: chatgpt4-cli Version: 1.5.0 Summary: Terminal for
 ChatGPT Home-page: https://github.com/Simatwa/gpt-cli Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com Maintainer: Smartwa Caleb License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/gpt-cli/issues/new
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
 Classifier: Topic :: Home Automation Classifier: Intended Audience :: Customer
@@ -65,70 +65,88 @@
 12  {Any Other}       Chat with ChatGPT
  1.img : Text-to-Image converter - ChatGPT - e.g ```img Toddler cartoon coding
 in Python``` 2.emg : Text-to-Image converter - EdgeGPT - e.g ```emg Toddler
 cartoon coding in Python``` 3.txt2img : Generate image based on GPT description
 - e.g ```txt2img Describe phenotype anatomy of ancient dinosaurs```
 4._font_color : modifies font-color - e.g ```font_color input red```
 5._background_color : modifies background_color - e.g ```background_color
-cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ
-[Smartwa@ChatGPT4]â(%H:%M:%S)``` 7._load : Load configurations from the json
-file - e.g ```load DAN.json``` 8._save : Save the current Chat Configurations -
-e.g ```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) -
-e.g ```_rollback 2``` 10._reset : Reset current chat and start new - e.g
-```_reset Chat as if you are a 10 year old child``` 11._help : Show this help
-info * Use double `./` *(fullstop and forward slash)* to interact with **system
-commands** e.g ```./ifconfig```    For more info run `gpt-cli -h`.  ``` usage:
-gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt [1-
-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
+cyan``` 6._prompt : Modify CMD prompt - e.g ```prompt ââ[Smartwa@GPT-
+CLI]â(%H:%M:%S)``` 7._load : Load configurations from the json file - e.g
+```load DAN.json``` 8._save : Save the current Chat Configurations - e.g
+```save DAN.json``` 9._rollback : Rollback the Chat by the {n} time(s) - e.g
+```_rollback 2``` 10._reset : Reset current chat and start new - e.g ```_reset
+Chat as if you are a 10 year old child``` 11.bard : Specifies to use bard GPT -
+e.g ```bard Explain the composite concept in business``` 12.gpt4 : Specifies to
+use ChatGPT in case `--bard` was made default - e.g ```gpt4 How do you make?```
+13._help : Show this help info * Use `./` (fullstop and forward slash) to
+interact with **system commands** - e.g ```./ifconfig``` > **Note** You can
+further specify the GPT to be used by appending `--gpt4` or `--bard` in the
+prompt. * Use *{{f.text-filename}}* to issue prompt contained in the 'text-
+filename'    For more info run `gpt-cli -h`.  ```
+â­âââââââââââââââââââââââââââââââ
+gpt-cli v1.4.9
+ââââââââââââââââââââââââââââââââ®
+â â â Repo : https://github.com/Simatwa/gpt-cli â â By : Smartwa
+Caleb â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+usage: gpt-cli [-h] [-v] [-m gpt-3.5-turbo|gpt-4|gpt-4-32k] [-t [0.1-1]] [-mt
+[1-7000]] [-tp [0.1-1]] [-f [0.1-2]] [-p [0.1-2]] [-k KEY] [-kp path] [-ic
 [cyan|green|yellow|red]] [-oc [cyan|green|yellow|red]] [-bc
 [blue,magenta,black,reset]] [-pc [cyan|green|yellow|red]] [--prompt [SETTINGS
 ...]] [-tm value] [-pr PROXY] [-rc value] [-g 1,4] [-sp [text ...]] [-fp path]
 [-o path] [-pp prefix] [-rp prefix] [-dm keys|values|show|{fnm}] [-dl symbol]
-[-cf path] [--disable-stream] [--new-record] [--disable-recording] [--zero-
-show] [--markdown] [--update] [message ...] Interact with ChatGPT at the
-terminal positional arguments: message Message to be send. optional arguments:
--h, --help show this help message and exit -v, --version show program's version
-number and exit -m gpt-3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-
-4|gpt-4-32k ChatGPT model to be used -t [0.1-1], --temperature [0.1-1] Charge
-of the generated text's randomness -mt [1-7000], --max-tokens [1-7000] Maximum
-number of tokens to be generated upon completion -tp [0.1-1], --top-p [0.1-1]
-Sampling threshold during inference time -f [0.1-2], --frequency-penalty [0.1-
-2] Chances of word being repeated -p [0.1-2], --presence-frequency [0.1-2]
-Chances of topic being repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --
-key-path path Path to text-file containing GPT-api key -ic
-[cyan|green|yellow|red], --input-color [cyan|green|yellow|red] Font color for
-inputs -oc [cyan|green|yellow|red], --output-color [cyan|green|yellow|red] Font
-color for outputs -bc [blue,magenta,black,reset], --background-color
-[blue,magenta,black,reset] Console's background-color -pc
-[cyan|green|yellow|red], --prompt-color [cyan|green|yellow|red] Prompt's
-display color --prompt [SETTINGS ...] Customizes the prompt display -tm value,
---timeout value Request timeout while making request - (Soon) -pr PROXY, --
-proxy PROXY Pivot request through this proxy -rc value, --reply-count value
-Number of responses to be received -g 1,4, --gpt 1,4 ChatGPT version to be used
--sp [text ...], --system-prompt [text ...] Text to train ChatGPT at the start -
-fp path, --file-path path Path to .csv file containing role and prompt -
-[act,prompt] -o path, --output path Filepath for saving the chats - default [/
-home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp prefix, --prompt-prefix
-prefix Text to append before saving each prompt - default [>>timestamp] -rp
-prefix, --response-prefix prefix Text to append before saving each response -
-default [None] -dm keys|values|show|{fnm}, --dump keys|values|show|{fnm} Stdout
-[keys,values]; Save all prompts in json format to a file -dl symbol, --
-delimiter symbol Delimeter for the .CSV file - [act,prompt] -cf path, --cookie-
-file path Path to Bing's cookies - for Edge Image Generation --disable-stream
-Specifies not to stream responses from ChatGPT --new-record Override previous
-chats under the filepath --disable-recording Disable saving prompts and
-responses --zero-show Specifies not to stdout prompt of the act parsed --
-markdown Stdout responses in markdown-format - disables streaming --update
-Download latest prompts - [awesome-chatgpt-prompts] ```  > **Note** : **gpt-4**
-*(model)* supports upto *7000* tokens and others *3000*. > **Warning** : **gpt-
-1** Has issues - *(To be fixed later)* ## Motive   Love for `Terminal` â¤ï¸
-As a `terminal guy` I used to find it uncomfortable to keep shifting from one
-window to next in order to access ChatGPT even after trying out the [gpt-login]
-(https://github.com/Simatwa/gpt-login), the rest is [here.](https://github.com/
-Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https://
-github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/Simatwa/
-gpt-cli/issues) without any **guideline** or submitting a [pull request](https:
-//github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue - [x] Issue
-prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://github.com/
-Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1. [remo7777]
-(https://github.com/remo7777/T-Header) 2. [acheong08](https://github.com/
-acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-prompts)
+[-cf path] [-bk KEY] [-bkp PATH] [-bcf PATH] [-si TIME] [--disable-stream] [--
+new-record] [--disable-recording] [--zero-show] [--bard] [--markdown] [--
+update] [--sudo] [message ...] Interact with ChatGPT at the terminal positional
+arguments: message Message to be send. options: -h, --help show this help
+message and exit -v, --version show program's version number and exit -m gpt-
+3.5-turbo|gpt-4|gpt-4-32k, --model gpt-3.5-turbo|gpt-4|gpt-4-32k ChatGPT model
+to be used -t [0.1-1], --temperature [0.1-1] Charge of the generated text's
+randomness -mt [1-7000], --max-tokens [1-7000] Maximum number of tokens to be
+generated upon completion -tp [0.1-1], --top-p [0.1-1] Sampling threshold
+during inference time -f [0.1-2], --frequency-penalty [0.1-2] Chances of word
+being repeated -p [0.1-2], --presence-frequency [0.1-2] Chances of topic being
+repeated -k KEY, --key KEY OPENAI-API-KEY -kp path, --key-path path Path to
+text-file containing GPT-api key -ic [cyan|green|yellow|red], --input-color
+[cyan|green|yellow|red] Font color for inputs -oc [cyan|green|yellow|red], --
+output-color [cyan|green|yellow|red] Font color for outputs -bc
+[blue,magenta,black,reset], --background-color [blue,magenta,black,reset]
+Console's background-color -pc [cyan|green|yellow|red], --prompt-color
+[cyan|green|yellow|red] Prompt's display color --prompt [SETTINGS ...]
+Customizes the prompt display -tm value, --timeout value Request timeout while
+making request - (Soon) -pr PROXY, --proxy PROXY Pivot request through this
+proxy -rc value, --reply-count value Number of responses to be received -g 1,4,
+--gpt 1,4 ChatGPT version to be used -sp [text ...], --system-prompt [text ...]
+Text to train ChatGPT at the start -fp path, --file-path path Path to .csv file
+containing role and prompt - [act,prompt] -o path, --output path Filepath for
+saving the chats - default [/home/smartwa/git/gpt-cli/.chatgpt-history.txt] -pp
+prefix, --prompt-prefix prefix Text to append before saving each prompt -
+default [>>> timestamp] -rp prefix, --response-prefix prefix Text to append
+before saving each response - default [None] -dm keys|values|show|{fnm}, --dump
+keys|values|show|{fnm} Stdout [keys,values]; Save all prompts in json format to
+a file -dl symbol, --delimiter symbol Delimeter for the .CSV file -
+[act,prompt] -cf path, --cookie-file path Path to Bing's cookies - for Edge
+Image Generation -bk KEY, --bard-key KEY Bard's session value -bkp PATH, --
+bard-key-path PATH Path to Bard's key path -bcf PATH, --bard-cookie-file PATH
+Path to Bard's cookie file -si TIME, --stream-interval TIME Interval for
+printing responses in (s) --disable-stream Specifies not to stream responses
+from ChatGPT --new-record Override previous chats under the filepath --disable-
+recording Disable saving prompts and responses --zero-show Specifies not to
+stdout prompt of the act parsed --bard Make Bard the default GPT --markdown
+Stdout responses in markdown-format - disables streaming --update Download
+latest prompts - [awesome-chatgpt-prompts] --sudo Run commands against system
+with sudo privileges ```  > **Note** : **gpt-4** *(model)* supports upto *7000*
+tokens and others *3000*. > **Warning** : **gpt-1** Has issues - *(To be fixed
+later)* Visit [acheong08/Bard](https://github.com/acheong08/Bard) for info on
+how to get the Bard's cookie file and Sessions. ## Motive   Love for `Terminal`
+â¤ï¸  As a `terminal guy` I used to find it uncomfortable to keep shifting
+from one window to next in order to access ChatGPT even after trying out the
+[gpt-login](https://github.com/Simatwa/gpt-login), the rest is [here.](https://
+github.com/Simatwa/gpt-cli)  ## Contributions - Anyone is free to [fork](https:
+//github.com/Simatwa/gpt-cli/fork), submit an [issue](https://github.com/
+Simatwa/gpt-cli/issues) without any **guideline** or submitting a [pull
+request](https://github.com/Simatwa/gpt-cli/pulls). ### ToDo - [x] Use dialogue
+- [x] Issue prompt from a file - [ ] Busy bar > Review [CHANGELOG](https://
+github.com/Simatwa/gpt-cli/blob/main/CHANGELOG.md) ## Acknowledgements 1.
+[remo7777](https://github.com/remo7777/T-Header) 2. [acheong08](https://
+github.com/acheong08/ChatGPT) 3. [f](https://github.com/f/awesome-chatgpt-
+prompts)
```

### Comparing `chatgpt4-cli-1.4.9/setup.py` & `chatgpt4-cli-1.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         "numpy>=1.23.4",
         "colorama>=0.4.6",
         "openai>=0.26.4",
         "revChatGPT==4.0.6",
         "appdirs>=1.4.4",
         "requests>=2.28.2",
         "tabulate>=0.9.0",
+        "GoogleBard==0.0.7"
     ],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

