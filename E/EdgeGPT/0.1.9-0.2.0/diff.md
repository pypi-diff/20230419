# Comparing `tmp/EdgeGPT-0.1.9.tar.gz` & `tmp/EdgeGPT-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-0.1.9.tar", last modified: Sat Mar 25 02:59:03 2023, max compression
+gzip compressed data, was "EdgeGPT-0.2.0.tar", last modified: Wed Apr 19 10:30:37 2023, max compression
```

## Comparing `EdgeGPT-0.1.9.tar` & `EdgeGPT-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-25 02:59:03.521855 EdgeGPT-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:59:03.517855 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-25 02:59:03.000000 EdgeGPT-0.1.9/src/EdgeGPT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/src/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-03-25 02:58:41.000000 EdgeGPT-0.1.9/src/ImageGen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:30:37.898569 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 10:30:37.000000 EdgeGPT-0.2.0/src/EdgeGPT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/src/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 10:30:02.000000 EdgeGPT-0.2.0/src/ImageGen.py
```

### Comparing `EdgeGPT-0.1.9/LICENSE` & `EdgeGPT-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-0.1.9/PKG-INFO` & `EdgeGPT-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-Metadata-Version: 2.1
-Name: EdgeGPT
-Version: 0.1.9
-Summary: Reverse engineered Edge Chat API
-Home-page: https://github.com/acheong08/EdgeGPT
-Author: Antonio Cheong
-Author-email: acheong@student.dalat.org
-License: GNU General Public License v2.0
-Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
+<a>English</a> -
+<a href="./README_zh.md">中文</a> -
+<a href="./README_es.md">Español</a> -
+<a href="./README_ja.md">日本語</a>
+
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
     <img alt="PyPI version" src="https://img.shields.io/pypi/v/EdgeGPT">
   </a>
   <img alt="Python version" src="https://img.shields.io/badge/python-3.8+-blue.svg">
+
+  <img alt="Total downloads" src="https://static.pepy.tech/badge/edgegpt">
+
 </p>
 
 ---
 
 ## Setup
 
 ### Install package
@@ -43,14 +32,15 @@
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
 - A Microsoft Account with early access to <https://bing.com/chat> (Required)
+- Required in a supported country with New Bing (Chinese mainland VPN required)
 
 <details>
   <summary>
 
 ### Checking access (Required)
 
   </summary>
@@ -68,15 +58,15 @@
 ### Getting authentication (Required)
 
   </summary>
 
 - Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 - Go to `bing.com`
 - Open the extension
-- Click "Export" on the bottom right (This saves your cookies to clipboard)
+- Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
 - Paste your cookies into a file `cookies.json`
 
 </details>
 
 <details>
 
 <summary>
@@ -97,56 +87,77 @@
         By: Antonio Cheong
 
         !help for help
 
         Type !exit to exit
         Enter twice to send message or set --enter-once to send one line message
 
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--style {creative,balanced,precise}] --cookie-file COOKIE_FILE
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style {creative,balanced,precise}]
+                  [--cookie-file COOKIE_FILE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
   --no-stream
+  --rich
+  --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
+  --wss-link WSS_LINK   WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)
   --style {creative,balanced,precise}
   --cookie-file COOKIE_FILE
+                        needed if environment variable COOKIE_FILE is not set
 ```
 
 ---
 
+## Running with Docker
+
+This assumes you have a file cookies.json in your current working directory
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt
+```
+
+You can add any extra flags as following
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
+```
+
 ### Developer demo
 
 Three ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
-- Specify the path to `cookies.json` in the argument `cookiePath` like this:
+- Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
-  bot = Chatbot(cookiePath='./cookie.json')
+  bot = Chatbot(cookie_path='./cookies.json')
   ```
 
 - Pass in the cookies directly by the argument `cookies`, like this:
 
   ```python
-  with open('./cookie.json', 'r') as f:
+  with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
   bot = Chatbot(cookies=cookies)
   ```
 
 Use Async for the best experience
 
 Reference code for more advanced example of usage:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = Chatbot()
-    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
+    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
@@ -159,33 +170,41 @@
 
 ## Image generator
 
 </summary>
 
 ```bash
 $ python3 -m ImageGen -h
-usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR]
+usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -U U                  Auth cookie from browser
   --cookie-file COOKIE_FILE
                         File containing auth cookie
   --prompt PROMPT       Prompt to generate images for
   --output-dir OUTPUT_DIR
                         Output directory
+  --quiet               Disable pipeline messages
+  --asyncio             Run ImageGen using asyncio
 ```
 
 ### Developer demo
 
 ```python
 from ImageGen import ImageGen
-if __name__ == "__main__":
-    import argparse
+import argparse
+import json
+
+async def async_image_gen(args) -> None:
+    async with ImageGenAsync(args.U, args.quiet) as image_generator:
+        images = await image_generator.get_images(args.prompt)
+        await image_generator.save_images(images, output_dir=args.output_dir)
 
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-U", help="Auth cookie from browser", type=str)
     parser.add_argument("--cookie-file", help="File containing auth cookie", type=str)
     parser.add_argument(
         "--prompt",
         help="Prompt to generate images for",
         type=str,
@@ -193,32 +212,41 @@
     )
     parser.add_argument(
         "--output-dir",
         help="Output directory",
         type=str,
         default="./output",
     )
+    parser.add_argument(
+        "--quiet", help="Disable pipeline messages", action="store_true"
+    )
+    parser.add_argument(
+        "--asyncio", help="Run ImageGen using asyncio", action="store_true"
+    )
     args = parser.parse_args()
     # Load auth cookie
     with open(args.cookie_file, encoding="utf-8") as file:
         cookie_json = json.load(file)
         for cookie in cookie_json:
             if cookie.get("name") == "_U":
                 args.U = cookie.get("value")
                 break
 
     if args.U is None:
         raise Exception("Could not find auth cookie")
 
-    # Create image generator
-    image_generator = ImageGen(args.U)
-    image_generator.save_images(
-        image_generator.get_images(args.prompt),
-        output_dir=args.output_dir,
-    )
+    if not args.asyncio:
+        # Create image generator
+        image_generator = ImageGen(args.U, args.quiet)
+        image_generator.save_images(
+            image_generator.get_images(args.prompt),
+            output_dir=args.output_dir,
+        )
+    else:
+        asyncio.run(async_image_gen(args))
 
 ```
 
 </details>
 
 ## Star History
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,70 +1,79 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.1.9 Summary: Reverse engineered
-Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
-Cheong Author-email: acheong@student.dalat.org License: GNU General Public
-License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
-issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-                               version of Bing_
-                        [PyPI_version] [Python version]
+           version of Bing_ English - ä¸­æ - EspaÃ±ol - æ¥æ¬èª
+               [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
-bing.com/chat> (Required)   ### Checking access (Required)  - Install the
+bing.com/chat> (Required) - Required in a supported country with New Bing
+(Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
 set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows
 NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0
 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension
 like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/
 webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and
 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-
 switcher/). - Open [bing.com/chat](https://bing.com/chat) - If you see a chat
 feature, you are good to go    ### Getting authentication (Required)  - Install
 the cookie editor extension for [Chrome](https://chrome.google.com/webstore/
 detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
 addons.mozilla.org/en-US/firefox/addon/cookie-editor/) - Go to `bing.com` -
-Open the extension - Click "Export" on the bottom right (This saves your
-cookies to clipboard) - Paste your cookies into a file `cookies.json`    ##
-Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT -h EdgeGPT - A demo
-of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/EdgeGPT
-By: Antonio Cheong !help for help Type !exit to exit Enter twice to send
-message or set --enter-once to send one line message usage: EdgeGPT.py [-h] [--
-enter-once] [--no-stream] [--style {creative,balanced,precise}] --cookie-file
-COOKIE_FILE options: -h, --help show this help message and exit --enter-once --
-no-stream --style {creative,balanced,precise} --cookie-file COOKIE_FILE ``` --
-- ### Developer demo Three ways to pass in cookies: - Environment variable:
-`export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
-`cookies.json` in the argument `cookiePath` like this: ```python bot = Chatbot
-(cookiePath='./cookie.json') ``` - Pass in the cookies directly by the argument
-`cookies`, like this: ```python with open('./cookie.json', 'r') as f: cookies =
-json.load(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best
-experience Reference code for more advanced example of usage: ```python import
-asyncio from EdgeGPT import Chatbot, ConversationStyle async def main(): bot =
-Chatbot() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
--m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
-prompt PROMPT [--output-dir OUTPUT_DIR] options: -h, --help show this help
-message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE File
-containing auth cookie --prompt PROMPT Prompt to generate images for --output-
-dir OUTPUT_DIR Output directory ``` ### Developer demo ```python from ImageGen
-import ImageGen if __name__ == "__main__": import argparse parser =
-argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
-browser", type=str) parser.add_argument("--cookie-file", help="File containing
-auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
-generate images for", type=str, required=True, ) parser.add_argument( "--
-output-dir", help="Output directory", type=str, default="./output", ) args =
-parser.parse_args() # Load auth cookie with open(args.cookie_file,
-encoding="utf-8") as file: cookie_json = json.load(file) for cookie in
-cookie_json: if cookie.get("name") == "_U": args.U = cookie.get("value") break
-if args.U is None: raise Exception("Could not find auth cookie") # Create image
-generator image_generator = ImageGen(args.U) image_generator.save_images
-( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) ```
-## Star History [![Star History Chart](https://api.star-history.com/
-svg?repos=acheong08/EdgeGPT&type=Date)](https://star-history.com/#acheong08/
-EdgeGPT&Date) ## Contributors This project exists thanks to all the people who
-contribute. [https://contrib.rocks/image?repo=acheong08/EdgeGPT]
+Open the extension - Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) - Paste your cookies into a file
+`cookies.json`    ## Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT
+-h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
+github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
+exit Enter twice to send message or set --enter-once to send one line message
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
+-wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
+COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
+-no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
+link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
+{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
+variable COOKIE_FILE is not set ``` --- ## Running with Docker This assumes you
+have a file cookies.json in your current working directory ``` bash docker run
+--rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
+ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
+cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
+Developer demo Three ways to pass in cookies: - Environment variable: `export
+COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
+argument `cookie_path` like this: ```python bot = Chatbot(cookie_path='./
+cookies.json') ``` - Pass in the cookies directly by the argument `cookies`,
+like this: ```python with open('./cookies.json', 'r') as f: cookies = json.load
+(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best experience
+Reference code for more advanced example of usage: ```python import asyncio
+from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = Chatbot
+() print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
+sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
+()) ```    ## Image generator  ```bash $ python3 -m ImageGen -h usage:
+ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-
+dir OUTPUT_DIR] [--quiet] [--asyncio] optional arguments: -h, --help show this
+help message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE
+File containing auth cookie --prompt PROMPT Prompt to generate images for --
+output-dir OUTPUT_DIR Output directory --quiet Disable pipeline messages --
+asyncio Run ImageGen using asyncio ``` ### Developer demo ```python from
+ImageGen import ImageGen import argparse import json async def async_image_gen
+(args) -> None: async with ImageGenAsync(args.U, args.quiet) as
+image_generator: images = await image_generator.get_images(args.prompt) await
+image_generator.save_images(images, output_dir=args.output_dir) if __name__ ==
+"__main__": parser = argparse.ArgumentParser() parser.add_argument("-U",
+help="Auth cookie from browser", type=str) parser.add_argument("--cookie-file",
+help="File containing auth cookie", type=str) parser.add_argument( "--prompt",
+help="Prompt to generate images for", type=str, required=True, )
+parser.add_argument( "--output-dir", help="Output directory", type=str,
+default="./output", ) parser.add_argument( "--quiet", help="Disable pipeline
+messages", action="store_true" ) parser.add_argument( "--asyncio", help="Run
+ImageGen using asyncio", action="store_true" ) args = parser.parse_args() #
+Load auth cookie with open(args.cookie_file, encoding="utf-8") as file:
+cookie_json = json.load(file) for cookie in cookie_json: if cookie.get("name")
+== "_U": args.U = cookie.get("value") break if args.U is None: raise Exception
+("Could not find auth cookie") if not args.asyncio: # Create image generator
+image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
+( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
+asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
+(https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
+star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
+thanks to all the people who contribute. [https://contrib.rocks/
+image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.1.9/setup.py` & `EdgeGPT-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,46 @@
+from pathlib import Path
+
 from setuptools import find_packages
 from setuptools import setup
 
+DOCS_PATH = Path(__file__).parents[0] / "docs/README.md"
+PATH = Path("README.md")
+if not PATH.exists():
+    with open(DOCS_PATH, encoding="utf-8") as f1:
+        with open(PATH, "w+", encoding="utf-8") as f2:
+            f2.write(f1.read())
+
 setup(
     name="EdgeGPT",
-    version="0.1.9",
+    version="0.2.0",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/EdgeGPT",
     project_urls={"Bug Report": "https://github.com/acheong08/EdgeGPT/issues/new"},
+    entry_points={
+        "console_scripts": [
+            "edge-gpt = EdgeGPT:main",
+            "edge-gpt-image = ImageGen:main",
+        ],
+    },
     install_requires=[
         "httpx",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
-        "regex",
         "requests",
+        "BingImageCreator>=0.1.1.1",
     ],
-    long_description=open("README.md", encoding="utf-8").read(),
+    long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
```

### Comparing `EdgeGPT-0.1.9/src/EdgeGPT.egg-info/PKG-INFO` & `EdgeGPT-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT
-Version: 0.1.9
+Version: 0.2.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/acheong08/EdgeGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -20,21 +20,29 @@
 <div align="center">
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
 
+<a>English</a> -
+<a href="./README_zh.md">中文</a> -
+<a href="./README_es.md">Español</a> -
+<a href="./README_ja.md">日本語</a>
+
 </div>
 
 <p align="center">
   <a href="https://github.com/acheong08/EdgeGPT">
     <img alt="PyPI version" src="https://img.shields.io/pypi/v/EdgeGPT">
   </a>
   <img alt="Python version" src="https://img.shields.io/badge/python-3.8+-blue.svg">
+
+  <img alt="Total downloads" src="https://static.pepy.tech/badge/edgegpt">
+
 </p>
 
 ---
 
 ## Setup
 
 ### Install package
@@ -43,14 +51,15 @@
 python3 -m pip install EdgeGPT --upgrade
 ```
 
 ### Requirements
 
 - python 3.8+
 - A Microsoft Account with early access to <https://bing.com/chat> (Required)
+- Required in a supported country with New Bing (Chinese mainland VPN required)
 
 <details>
   <summary>
 
 ### Checking access (Required)
 
   </summary>
@@ -68,15 +77,15 @@
 ### Getting authentication (Required)
 
   </summary>
 
 - Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
 - Go to `bing.com`
 - Open the extension
-- Click "Export" on the bottom right (This saves your cookies to clipboard)
+- Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
 - Paste your cookies into a file `cookies.json`
 
 </details>
 
 <details>
 
 <summary>
@@ -97,56 +106,77 @@
         By: Antonio Cheong
 
         !help for help
 
         Type !exit to exit
         Enter twice to send message or set --enter-once to send one line message
 
-usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--style {creative,balanced,precise}] --cookie-file COOKIE_FILE
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [--wss-link WSS_LINK] [--style {creative,balanced,precise}]
+                  [--cookie-file COOKIE_FILE]
 
 options:
   -h, --help            show this help message and exit
   --enter-once
   --no-stream
+  --rich
+  --proxy PROXY         Proxy URL (e.g. socks5://127.0.0.1:1080)
+  --wss-link WSS_LINK   WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)
   --style {creative,balanced,precise}
   --cookie-file COOKIE_FILE
+                        needed if environment variable COOKIE_FILE is not set
 ```
 
 ---
 
+## Running with Docker
+
+This assumes you have a file cookies.json in your current working directory
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt
+```
+
+You can add any extra flags as following
+
+``` bash
+
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative
+```
+
 ### Developer demo
 
 Three ways to pass in cookies:
 
 - Environment variable: `export COOKIE_FILE=/path/to/cookies.json`.
-- Specify the path to `cookies.json` in the argument `cookiePath` like this:
+- Specify the path to `cookies.json` in the argument `cookie_path` like this:
 
   ```python
-  bot = Chatbot(cookiePath='./cookie.json')
+  bot = Chatbot(cookie_path='./cookies.json')
   ```
 
 - Pass in the cookies directly by the argument `cookies`, like this:
 
   ```python
-  with open('./cookie.json', 'r') as f:
+  with open('./cookies.json', 'r') as f:
       cookies = json.load(f)
   bot = Chatbot(cookies=cookies)
   ```
 
 Use Async for the best experience
 
 Reference code for more advanced example of usage:
 
 ```python
 import asyncio
 from EdgeGPT import Chatbot, ConversationStyle
 
 async def main():
     bot = Chatbot()
-    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative))
+    print(await bot.ask(prompt="Hello world", conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/sydney/ChatHub"))
     await bot.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
@@ -159,33 +189,41 @@
 
 ## Image generator
 
 </summary>
 
 ```bash
 $ python3 -m ImageGen -h
-usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR]
+usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-dir OUTPUT_DIR] [--quiet] [--asyncio]
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
   -U U                  Auth cookie from browser
   --cookie-file COOKIE_FILE
                         File containing auth cookie
   --prompt PROMPT       Prompt to generate images for
   --output-dir OUTPUT_DIR
                         Output directory
+  --quiet               Disable pipeline messages
+  --asyncio             Run ImageGen using asyncio
 ```
 
 ### Developer demo
 
 ```python
 from ImageGen import ImageGen
-if __name__ == "__main__":
-    import argparse
+import argparse
+import json
 
+async def async_image_gen(args) -> None:
+    async with ImageGenAsync(args.U, args.quiet) as image_generator:
+        images = await image_generator.get_images(args.prompt)
+        await image_generator.save_images(images, output_dir=args.output_dir)
+
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-U", help="Auth cookie from browser", type=str)
     parser.add_argument("--cookie-file", help="File containing auth cookie", type=str)
     parser.add_argument(
         "--prompt",
         help="Prompt to generate images for",
         type=str,
@@ -193,32 +231,41 @@
     )
     parser.add_argument(
         "--output-dir",
         help="Output directory",
         type=str,
         default="./output",
     )
+    parser.add_argument(
+        "--quiet", help="Disable pipeline messages", action="store_true"
+    )
+    parser.add_argument(
+        "--asyncio", help="Run ImageGen using asyncio", action="store_true"
+    )
     args = parser.parse_args()
     # Load auth cookie
     with open(args.cookie_file, encoding="utf-8") as file:
         cookie_json = json.load(file)
         for cookie in cookie_json:
             if cookie.get("name") == "_U":
                 args.U = cookie.get("value")
                 break
 
     if args.U is None:
         raise Exception("Could not find auth cookie")
 
-    # Create image generator
-    image_generator = ImageGen(args.U)
-    image_generator.save_images(
-        image_generator.get_images(args.prompt),
-        output_dir=args.output_dir,
-    )
+    if not args.asyncio:
+        # Create image generator
+        image_generator = ImageGen(args.U, args.quiet)
+        image_generator.save_images(
+            image_generator.get_images(args.prompt),
+            output_dir=args.output_dir,
+        )
+    else:
+        asyncio.run(async_image_gen(args))
 
 ```
 
 </details>
 
 ## Star History
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,70 +1,89 @@
-Metadata-Version: 2.1 Name: EdgeGPT Version: 0.1.9 Summary: Reverse engineered
+Metadata-Version: 2.1 Name: EdgeGPT Version: 0.2.0 Summary: Reverse engineered
 Edge Chat API Home-page: https://github.com/acheong08/EdgeGPT Author: Antonio
 Cheong Author-email: acheong@student.dalat.org License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/acheong08/EdgeGPT/
 issues/new Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
    [EdgeGPT] # Edge GPT _The reverse engineering the chat feature of the new
-                               version of Bing_
-                        [PyPI_version] [Python version]
+           version of Bing_ English - ä¸­æ - EspaÃ±ol - æ¥æ¬èª
+               [PyPI_version] [Python version] [Total downloads]
 --- ## Setup ### Install package ```bash python3 -m pip install EdgeGPT --
 upgrade ``` ### Requirements - python 3.8+ - A Microsoft Account with early
 access to
-bing.com/chat> (Required)   ### Checking access (Required)  - Install the
+bing.com/chat> (Required) - Required in a supported country with New Bing
+(Chinese mainland VPN required)   ### Checking access (Required)  - Install the
 latest version of Microsoft Edge - Alternatively, you can use any browser and
 set the user-agent to look like you're using Edge (e.g., `Mozilla/5.0 (Windows
 NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0
 Safari/537.36 Edg/111.0.1661.51`). You can do this easily with an extension
 like "User-Agent Switcher and Manager" for [Chrome](https://chrome.google.com/
 webstore/detail/user-agent-switcher-and-m/bhchdcejhohfmigjafbampogmaanbfkg) and
 [Firefox](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-
 switcher/). - Open [bing.com/chat](https://bing.com/chat) - If you see a chat
 feature, you are good to go    ### Getting authentication (Required)  - Install
 the cookie editor extension for [Chrome](https://chrome.google.com/webstore/
 detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://
 addons.mozilla.org/en-US/firefox/addon/cookie-editor/) - Go to `bing.com` -
-Open the extension - Click "Export" on the bottom right (This saves your
-cookies to clipboard) - Paste your cookies into a file `cookies.json`    ##
-Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT -h EdgeGPT - A demo
-of reverse engineering the Bing GPT chatbot Repo: github.com/acheong08/EdgeGPT
-By: Antonio Cheong !help for help Type !exit to exit Enter twice to send
-message or set --enter-once to send one line message usage: EdgeGPT.py [-h] [--
-enter-once] [--no-stream] [--style {creative,balanced,precise}] --cookie-file
-COOKIE_FILE options: -h, --help show this help message and exit --enter-once --
-no-stream --style {creative,balanced,precise} --cookie-file COOKIE_FILE ``` --
-- ### Developer demo Three ways to pass in cookies: - Environment variable:
-`export COOKIE_FILE=/path/to/cookies.json`. - Specify the path to
-`cookies.json` in the argument `cookiePath` like this: ```python bot = Chatbot
-(cookiePath='./cookie.json') ``` - Pass in the cookies directly by the argument
-`cookies`, like this: ```python with open('./cookie.json', 'r') as f: cookies =
-json.load(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best
-experience Reference code for more advanced example of usage: ```python import
-asyncio from EdgeGPT import Chatbot, ConversationStyle async def main(): bot =
-Chatbot() print(await bot.ask(prompt="Hello world",
-conversation_style=ConversationStyle.creative)) await bot.close() if __name__
-== "__main__": asyncio.run(main()) ```    ## Image generator  ```bash $ python3
--m ImageGen -h usage: ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --
-prompt PROMPT [--output-dir OUTPUT_DIR] options: -h, --help show this help
-message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE File
-containing auth cookie --prompt PROMPT Prompt to generate images for --output-
-dir OUTPUT_DIR Output directory ``` ### Developer demo ```python from ImageGen
-import ImageGen if __name__ == "__main__": import argparse parser =
-argparse.ArgumentParser() parser.add_argument("-U", help="Auth cookie from
-browser", type=str) parser.add_argument("--cookie-file", help="File containing
-auth cookie", type=str) parser.add_argument( "--prompt", help="Prompt to
-generate images for", type=str, required=True, ) parser.add_argument( "--
-output-dir", help="Output directory", type=str, default="./output", ) args =
-parser.parse_args() # Load auth cookie with open(args.cookie_file,
-encoding="utf-8") as file: cookie_json = json.load(file) for cookie in
-cookie_json: if cookie.get("name") == "_U": args.U = cookie.get("value") break
-if args.U is None: raise Exception("Could not find auth cookie") # Create image
-generator image_generator = ImageGen(args.U) image_generator.save_images
-( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) ```
-## Star History [![Star History Chart](https://api.star-history.com/
-svg?repos=acheong08/EdgeGPT&type=Date)](https://star-history.com/#acheong08/
-EdgeGPT&Date) ## Contributors This project exists thanks to all the people who
-contribute. [https://contrib.rocks/image?repo=acheong08/EdgeGPT]
+Open the extension - Click "Export" on the bottom right, then "Export as JSON"
+(This saves your cookies to clipboard) - Paste your cookies into a file
+`cookies.json`    ## Chatbot  ## Usage ### Quick start ``` $ python3 -m EdgeGPT
+-h EdgeGPT - A demo of reverse engineering the Bing GPT chatbot Repo:
+github.com/acheong08/EdgeGPT By: Antonio Cheong !help for help Type !exit to
+exit Enter twice to send message or set --enter-once to send one line message
+usage: EdgeGPT.py [-h] [--enter-once] [--no-stream] [--rich] [--proxy PROXY] [-
+-wss-link WSS_LINK] [--style {creative,balanced,precise}] [--cookie-file
+COOKIE_FILE] options: -h, --help show this help message and exit --enter-once -
+-no-stream --rich --proxy PROXY Proxy URL (e.g. socks5://127.0.0.1:1080) --wss-
+link WSS_LINK WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub) --style
+{creative,balanced,precise} --cookie-file COOKIE_FILE needed if environment
+variable COOKIE_FILE is not set ``` --- ## Running with Docker This assumes you
+have a file cookies.json in your current working directory ``` bash docker run
+--rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/cookies.json'
+ghcr.io/acheong08/edgegpt ``` You can add any extra flags as following ``` bash
+docker run --rm -it -v $(pwd)/cookies.json:/cookies.json:ro -e COOKIE_FILE='/
+cookies.json' ghcr.io/acheong08/edgegpt --rich --style creative ``` ###
+Developer demo Three ways to pass in cookies: - Environment variable: `export
+COOKIE_FILE=/path/to/cookies.json`. - Specify the path to `cookies.json` in the
+argument `cookie_path` like this: ```python bot = Chatbot(cookie_path='./
+cookies.json') ``` - Pass in the cookies directly by the argument `cookies`,
+like this: ```python with open('./cookies.json', 'r') as f: cookies = json.load
+(f) bot = Chatbot(cookies=cookies) ``` Use Async for the best experience
+Reference code for more advanced example of usage: ```python import asyncio
+from EdgeGPT import Chatbot, ConversationStyle async def main(): bot = Chatbot
+() print(await bot.ask(prompt="Hello world",
+conversation_style=ConversationStyle.creative, wss_link="wss://sydney.bing.com/
+sydney/ChatHub")) await bot.close() if __name__ == "__main__": asyncio.run(main
+()) ```    ## Image generator  ```bash $ python3 -m ImageGen -h usage:
+ImageGen.py [-h] [-U U] [--cookie-file COOKIE_FILE] --prompt PROMPT [--output-
+dir OUTPUT_DIR] [--quiet] [--asyncio] optional arguments: -h, --help show this
+help message and exit -U U Auth cookie from browser --cookie-file COOKIE_FILE
+File containing auth cookie --prompt PROMPT Prompt to generate images for --
+output-dir OUTPUT_DIR Output directory --quiet Disable pipeline messages --
+asyncio Run ImageGen using asyncio ``` ### Developer demo ```python from
+ImageGen import ImageGen import argparse import json async def async_image_gen
+(args) -> None: async with ImageGenAsync(args.U, args.quiet) as
+image_generator: images = await image_generator.get_images(args.prompt) await
+image_generator.save_images(images, output_dir=args.output_dir) if __name__ ==
+"__main__": parser = argparse.ArgumentParser() parser.add_argument("-U",
+help="Auth cookie from browser", type=str) parser.add_argument("--cookie-file",
+help="File containing auth cookie", type=str) parser.add_argument( "--prompt",
+help="Prompt to generate images for", type=str, required=True, )
+parser.add_argument( "--output-dir", help="Output directory", type=str,
+default="./output", ) parser.add_argument( "--quiet", help="Disable pipeline
+messages", action="store_true" ) parser.add_argument( "--asyncio", help="Run
+ImageGen using asyncio", action="store_true" ) args = parser.parse_args() #
+Load auth cookie with open(args.cookie_file, encoding="utf-8") as file:
+cookie_json = json.load(file) for cookie in cookie_json: if cookie.get("name")
+== "_U": args.U = cookie.get("value") break if args.U is None: raise Exception
+("Could not find auth cookie") if not args.asyncio: # Create image generator
+image_generator = ImageGen(args.U, args.quiet) image_generator.save_images
+( image_generator.get_images(args.prompt), output_dir=args.output_dir, ) else:
+asyncio.run(async_image_gen(args)) ```  ## Star History [![Star History Chart]
+(https://api.star-history.com/svg?repos=acheong08/EdgeGPT&type=Date)](https://
+star-history.com/#acheong08/EdgeGPT&Date) ## Contributors This project exists
+thanks to all the people who contribute. [https://contrib.rocks/
+image?repo=acheong08/EdgeGPT]
```

### Comparing `EdgeGPT-0.1.9/src/EdgeGPT.py` & `EdgeGPT-0.2.0/src/EdgeGPT.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,33 @@
 from __future__ import annotations
 
 import argparse
 import asyncio
 import json
 import os
 import random
+import re
 import ssl
+import sys
 import uuid
 from enum import Enum
+from pathlib import Path
 from typing import Generator
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 import certifi
 import httpx
 import websockets.client as websockets
 from prompt_toolkit import PromptSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.history import InMemoryHistory
+from prompt_toolkit.key_binding import KeyBindings
 from rich.live import Live
 from rich.markdown import Markdown
 
 DELIMITER = "\x1e"
 
 
 # Generate random IP between range 13.104.0.0/14
@@ -81,38 +85,45 @@
     "x-forwarded-for": FORWARDED_IP,
 }
 
 ssl_context = ssl.create_default_context()
 ssl_context.load_verify_locations(certifi.where())
 
 
-class NotAllowedToAccess(Exception):
+class _NotAllowedToAccess(Exception):
     pass
 
 
-class ConversationStyle(Enum):
-    creative = "h3relaxedimg"
+class _ConversationStyle(Enum):
+    creative = "h3imaginative,clgalileo,gencontentv3"
     balanced = "galileo"
-    precise = "h3precise"
+    precise = "h3precise,clgalileo"
 
 
 CONVERSATION_STYLE_TYPE = Optional[
-    Union[ConversationStyle, Literal["creative", "balanced", "precise"]]
+    Union[_ConversationStyle, Literal["creative", "balanced", "precise"]]
 ]
 
 
-def append_identifier(msg: dict) -> str:
+def _append_identifier(msg: dict) -> str:
     """
     Appends special character to end of message to identify end of message
     """
     # Convert dict to json string
     return json.dumps(msg) + DELIMITER
 
 
-class ChatHubRequest:
+def _get_ran_hex(length: int = 32) -> str:
+    """
+    Returns random hex string
+    """
+    return "".join(random.choice("0123456789abcdef") for _ in range(length))
+
+
+class _ChatHubRequest:
     """
     Request object for ChatHub
     """
 
     def __init__(
         self,
         conversation_signature: str,
@@ -140,28 +151,39 @@
             options = [
                 "deepleo",
                 "enable_debug_commands",
                 "disable_emoji_spoken_text",
                 "enablemm",
             ]
         if conversation_style:
-            if not isinstance(conversation_style, ConversationStyle):
-                conversation_style = getattr(ConversationStyle, conversation_style)
+            if not isinstance(conversation_style, _ConversationStyle):
+                conversation_style = getattr(_ConversationStyle, conversation_style)
             options = [
+                "nlu_direct_response_filter",
                 "deepleo",
-                "enable_debug_commands",
                 "disable_emoji_spoken_text",
+                "responsible_ai_policy_235",
                 "enablemm",
                 conversation_style.value,
+                "dtappid",
+                "cricinfo",
+                "cricinfov2",
+                "dv3sugg",
             ]
         self.struct = {
             "arguments": [
                 {
                     "source": "cib",
                     "optionsSets": options,
+                    "sliceIds": [
+                        "222dtappid",
+                        "225cricinfo",
+                        "224locals0",
+                    ],
+                    "traceId": _get_ran_hex(32),
                     "isStartOfSession": self.invocation_id == 0,
                     "message": {
                         "author": "user",
                         "inputMethod": "Keyboard",
                         "text": prompt,
                         "messageType": "Chat",
                     },
@@ -175,287 +197,349 @@
             "invocationId": str(self.invocation_id),
             "target": "chat",
             "type": 4,
         }
         self.invocation_id += 1
 
 
-class Conversation:
+class _Conversation:
     """
     Conversation API
     """
 
     def __init__(
         self,
-        cookiePath: str = "",
-        cookies: dict | None = None,
+        cookies: dict,
         proxy: str | None = None,
     ) -> None:
         self.struct: dict = {
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "result": {"value": "Success", "message": None},
         }
+        self.proxy = proxy
+        proxy = (
+            proxy
+            or os.environ.get("all_proxy")
+            or os.environ.get("ALL_PROXY")
+            or os.environ.get("https_proxy")
+            or os.environ.get("HTTPS_PROXY")
+            or None
+        )
+        if proxy is not None and proxy.startswith("socks5h://"):
+            proxy = "socks5://" + proxy[len("socks5h://") :]
         self.session = httpx.Client(
             proxies=proxy,
             timeout=30,
             headers=HEADERS_INIT_CONVER,
         )
-        if cookies is not None:
-            cookie_file = cookies
-        else:
-            f = (
-                open(cookiePath, encoding="utf8").read()
-                if cookiePath
-                else open(os.environ.get("COOKIE_FILE"), encoding="utf-8").read()
-            )
-            cookie_file = json.loads(f)
-        for cookie in cookie_file:
+        for cookie in cookies:
             self.session.cookies.set(cookie["name"], cookie["value"])
 
         # Send GET request
         response = self.session.get(
             url=os.environ.get("BING_PROXY_URL")
-            or "https://edgeservices.bing.com/edgesvc/turing/conversation/create"
+            or "https://edgeservices.bing.com/edgesvc/turing/conversation/create",
         )
         if response.status_code != 200:
             response = self.session.get(
-                "https://edge.churchless.tech/edgesvc/turing/conversation/create"
+                "https://edge.churchless.tech/edgesvc/turing/conversation/create",
             )
-            if response.status_code != 200:
-                print(f"Status code: {response.status_code}")
-                print(response.text)
-                print(response.url)
-                raise Exception("Authentication failed")
+        if response.status_code != 200:
+            print(f"Status code: {response.status_code}")
+            print(response.text)
+            print(response.url)
+            raise Exception("Authentication failed")
         try:
             self.struct = response.json()
-            if self.struct["result"]["value"] == "UnauthorizedRequest":
-                raise NotAllowedToAccess(self.struct["result"]["message"])
-        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
+        except (json.decoder.JSONDecodeError, _NotAllowedToAccess) as exc:
             raise Exception(
                 "Authentication failed. You have not been accepted into the beta.",
             ) from exc
+        if self.struct["result"]["value"] == "UnauthorizedRequest":
+            raise _NotAllowedToAccess(self.struct["result"]["message"])
 
 
-class ChatHub:
+class _ChatHub:
     """
     Chat API
     """
 
-    def __init__(self, conversation: Conversation) -> None:
+    def __init__(self, conversation: _Conversation) -> None:
         self.wss: websockets.WebSocketClientProtocol | None = None
-        self.request: ChatHubRequest
+        self.request: _ChatHubRequest
         self.loop: bool
         self.task: asyncio.Task
-        self.request = ChatHubRequest(
+        self.request = _ChatHubRequest(
             conversation_signature=conversation.struct["conversationSignature"],
             client_id=conversation.struct["clientId"],
             conversation_id=conversation.struct["conversationId"],
         )
 
     async def ask_stream(
         self,
         prompt: str,
+        wss_link: str,
         conversation_style: CONVERSATION_STYLE_TYPE = None,
+        raw: bool = False,
+        options: dict = None,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
-        if self.wss:
-            if not self.wss.closed:
-                await self.wss.close()
+        if self.wss and not self.wss.closed:
+            await self.wss.close()
         # Check if websocket is closed
         self.wss = await websockets.connect(
-            "wss://sydney.bing.com/sydney/ChatHub",
+            wss_link,
             extra_headers=HEADERS,
             max_size=None,
             ssl=ssl_context,
         )
-        await self.__initial_handshake()
+        await self._initial_handshake()
         # Construct a ChatHub request
-        self.request.update(prompt=prompt, conversation_style=conversation_style)
+        self.request.update(
+            prompt=prompt,
+            conversation_style=conversation_style,
+            options=options,
+        )
         # Send request
-        await self.wss.send(append_identifier(self.request.struct))
+        await self.wss.send(_append_identifier(self.request.struct))
         final = False
         while not final:
             objects = str(await self.wss.recv()).split(DELIMITER)
             for obj in objects:
-                if obj is None or obj == "":
+                if obj is None or not obj:
                     continue
                 response = json.loads(obj)
-                if response.get("type") == 1 and response["arguments"][0].get(
+                if response.get("type") != 2 and raw:
+                    yield False, response
+                elif response.get("type") == 1 and response["arguments"][0].get(
                     "messages",
                 ):
                     resp_txt = response["arguments"][0]["messages"][0]["adaptiveCards"][
                         0
                     ]["body"][0].get("text")
                     yield False, resp_txt
                 elif response.get("type") == 2:
                     final = True
                     yield True, response
 
-    async def __initial_handshake(self):
-        await self.wss.send(append_identifier({"protocol": "json", "version": 1}))
+    async def _initial_handshake(self) -> None:
+        await self.wss.send(_append_identifier({"protocol": "json", "version": 1}))
         await self.wss.recv()
 
-    async def close(self):
+    async def close(self) -> None:
         """
         Close the connection
         """
         if self.wss and not self.wss.closed:
             await self.wss.close()
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
     """
 
     def __init__(
         self,
-        cookiePath: str = "",
-        cookies: dict | None = None,
+        cookies: dict = None,
         proxy: str | None = None,
+        cookie_path: str = None,
     ) -> None:
-        self.cookiePath: str = cookiePath
-        self.cookies: dict | None = cookies
+        if cookies is None:
+            cookies = {}
+        if cookie_path is not None:
+            try:
+                with open(cookie_path, encoding="utf-8") as f:
+                    self.cookies = json.load(f)
+            except FileNotFoundError as exc:
+                raise FileNotFoundError("Cookie file not found") from exc
+        else:
+            self.cookies = cookies
         self.proxy: str | None = proxy
-        self.chat_hub: ChatHub = ChatHub(
-            Conversation(self.cookiePath, self.cookies, self.proxy)
+        self.chat_hub: _ChatHub = _ChatHub(
+            _Conversation(self.cookies, self.proxy),
         )
 
     async def ask(
         self,
         prompt: str,
+        wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
+        options: dict = None,
     ) -> dict:
         """
         Ask a question to the bot
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
+            wss_link=wss_link,
+            options=options,
         ):
             if final:
                 return response
-        self.chat_hub.wss.close()
+        await self.chat_hub.wss.close()
+        return None
 
     async def ask_stream(
         self,
         prompt: str,
+        wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
+        raw: bool = False,
+        options: dict = None,
     ) -> Generator[str, None, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
+            wss_link=wss_link,
+            raw=raw,
+            options=options,
         ):
             yield response
 
-    async def close(self):
+    async def close(self) -> None:
         """
         Close the connection
         """
         await self.chat_hub.close()
 
-    async def reset(self):
+    async def reset(self) -> None:
         """
         Reset the conversation
         """
         await self.close()
-        self.chat_hub = ChatHub(Conversation(self.cookiePath, self.cookies))
+        self.chat_hub = _ChatHub(_Conversation(self.cookies))
 
 
-async def get_input_async(
+async def _get_input_async(
     session: PromptSession = None,
     completer: WordCompleter = None,
 ) -> str:
     """
     Multiline input function.
     """
     return await session.prompt_async(
         completer=completer,
         multiline=True,
         auto_suggest=AutoSuggestFromHistory(),
     )
 
 
-def create_session() -> PromptSession:
-    return PromptSession(history=InMemoryHistory())
+def _create_session() -> PromptSession:
+    kb = KeyBindings()
+
+    @kb.add("enter")
+    def _(event):
+        buffer_text = event.current_buffer.text
+        if buffer_text.startswith("!"):
+            event.current_buffer.validate_and_handle()
+        else:
+            event.current_buffer.insert_text("\n")
+
+    @kb.add("escape")
+    def _(event):
+        if event.current_buffer.complete_state:
+            # event.current_buffer.cancel_completion()
+            event.current_buffer.text = ""
+
+    return PromptSession(key_bindings=kb, history=InMemoryHistory())
 
 
-async def main():
+def _create_completer(commands: list, pattern_str: str = "$"):
+    return WordCompleter(words=commands, pattern=re.compile(pattern_str))
+
+
+async def async_main(args: argparse.Namespace) -> None:
     """
     Main function
     """
     print("Initializing...")
     print("Enter `alt+enter` or `escape+enter` to send a message")
-    bot = Chatbot(proxy=args.proxy)
-    session = create_session()
+    bot = Chatbot(proxy=args.proxy, cookies=args.cookies)
+    session = _create_session()
+    completer = _create_completer(["!help", "!exit", "!reset"])
+    initial_prompt = args.prompt
+
     while True:
         print("\nYou:")
-        if not args.enter_once:
-            question = await get_input_async(session=session)
+        if initial_prompt:
+            question = initial_prompt
+            print(question)
+            initial_prompt = None
         else:
-            question = input()
+            question = (
+                input()
+                if args.enter_once
+                else await _get_input_async(session=session, completer=completer)
+            )
         print()
         if question == "!exit":
             break
-        elif question == "!help":
+        if question == "!help":
             print(
                 """
             !help - Show this help message
             !exit - Exit the program
             !reset - Reset the conversation
             """,
             )
             continue
-        elif question == "!reset":
+        if question == "!reset":
             await bot.reset()
             continue
         print("Bot:")
         if args.no_stream:
             print(
-                (await bot.ask(prompt=question, conversation_style=args.style))["item"][
-                    "messages"
-                ][1]["adaptiveCards"][0]["body"][0]["text"],
+                (
+                    await bot.ask(
+                        prompt=question,
+                        conversation_style=args.style,
+                        wss_link=args.wss_link,
+                    )
+                )["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"],
             )
         else:
+            wrote = 0
             if args.rich:
-                wrote = 0
                 md = Markdown("")
                 with Live(md, auto_refresh=False) as live:
                     async for final, response in bot.ask_stream(
                         prompt=question,
                         conversation_style=args.style,
+                        wss_link=args.wss_link,
                     ):
                         if not final:
                             if wrote > len(response):
                                 print(md)
                                 print(Markdown("***Bing revoked the response.***"))
                             wrote = len(response)
                             md = Markdown(response)
                             live.update(md, refresh=True)
             else:
-                wrote = 0
                 async for final, response in bot.ask_stream(
                     prompt=question,
                     conversation_style=args.style,
+                    wss_link=args.wss_link,
                 ):
                     if not final:
                         print(response[wrote:], end="", flush=True)
                         wrote = len(response)
                 print()
     await bot.close()
 
 
-if __name__ == "__main__":
+def main() -> None:
     print(
         """
         EdgeGPT - A demo of reverse engineering the Bing GPT chatbot
         Repo: github.com/acheong08/EdgeGPT
         By: Antonio Cheong
 
         !help for help
@@ -464,30 +548,54 @@
     """,
     )
     parser = argparse.ArgumentParser()
     parser.add_argument("--enter-once", action="store_true")
     parser.add_argument("--no-stream", action="store_true")
     parser.add_argument("--rich", action="store_true")
     parser.add_argument(
-        "--proxy", help="Proxy URL (e.g. socks5://127.0.0.1:1080)", type=str
+        "--proxy",
+        help="Proxy URL (e.g. socks5://127.0.0.1:1080)",
+        type=str,
+    )
+    parser.add_argument(
+        "--wss-link",
+        help="WSS URL(e.g. wss://sydney.bing.com/sydney/ChatHub)",
+        type=str,
+        default="wss://sydney.bing.com/sydney/ChatHub",
     )
     parser.add_argument(
         "--style",
         choices=["creative", "balanced", "precise"],
         default="balanced",
     )
     parser.add_argument(
         "--cookie-file",
         type=str,
-        default="cookies.json",
+        default=os.environ.get("COOKIE_FILE", ""),
+        required=False,
+        help="Cookie file used for authentication (defaults to COOKIE_FILE environment variable)",
+    )
+    parser.add_argument(
+        "--prompt",
+        type=str,
+        default="",
         required=False,
-        help="needed if environment variable COOKIE_FILE is not set",
+        help="prompt to start with",
     )
     args = parser.parse_args()
-    if os.path.exists(args.cookie_file):
-        os.environ["COOKIE_FILE"] = args.cookie_file
-    else:
+    if args.cookie_file == "":
         parser.print_help()
         parser.exit(
-            1, "ERROR: use --cookied-file or set environemnt variable COOKIE_FILE"
+            1,
+            "ERROR: use --cookie-file or set the COOKIE_FILE environment variable",
         )
-    asyncio.run(main())
+    try:
+        args.cookies = json.loads(Path(args.cookie_file).read_text(encoding="utf-8"))
+    except OSError as exc:
+        print(f"Could not open cookie file: {exc}", file=sys.stderr)
+        sys.exit(1)
+
+    asyncio.run(async_main(args))
+
+
+if __name__ == "__main__":
+    main()
```

