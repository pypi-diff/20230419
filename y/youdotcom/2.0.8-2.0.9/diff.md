# Comparing `tmp/youdotcom-2.0.8.tar.gz` & `tmp/youdotcom-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youdotcom-2.0.8.tar", max compression
+gzip compressed data, was "youdotcom-2.0.9.tar", max compression
```

## Comparing `youdotcom-2.0.8.tar` & `youdotcom-2.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1074 2023-02-07 20:03:08.000000 youdotcom-2.0.8/LICENSE
--rwxr-xr-x   0        0        0    15123 2023-02-07 20:04:40.000000 youdotcom-2.0.8/README.md
--rwxr-xr-x   0        0        0     3893 2023-02-16 16:24:50.000000 youdotcom-2.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      613 2023-02-16 15:26:12.000000 youdotcom-2.0.8/youdotcom/__init__.py
--rwxr-xr-x   0        0        0     3897 2023-02-16 16:24:46.000000 youdotcom-2.0.8/youdotcom/__main__.py
--rwxr-xr-x   0        0        0     4347 2023-02-16 14:58:38.000000 youdotcom-2.0.8/youdotcom/api_1.py
--rwxr-xr-x   0        0        0     8459 2023-02-16 14:58:58.000000 youdotcom-2.0.8/youdotcom/api_2.py
--rwxr-xr-x   0        0        0     3090 2023-02-07 20:04:40.000000 youdotcom-2.0.8/youdotcom/apps.py
--rwxr-xr-x   0        0        0     3880 2023-02-07 20:04:42.000000 youdotcom-2.0.8/youdotcom/code.py
--rwxr-xr-x   0        0        0      544 2023-02-07 20:04:40.000000 youdotcom-2.0.8/youdotcom/config.json
--rwxr-xr-x   0        0        0     1727 2023-02-07 20:04:40.000000 youdotcom-2.0.8/youdotcom/imagine.py
--rwxr-xr-x   0        0        0     5342 2023-02-13 18:30:18.000000 youdotcom-2.0.8/youdotcom/init.py
--rwxr-xr-x   0        0        0     1498 2023-02-07 20:04:40.000000 youdotcom-2.0.8/youdotcom/search.py
--rwxr-xr-x   0        0        0       80 2023-02-14 20:28:42.000000 youdotcom-2.0.8/youdotcom/test.py
--rwxr-xr-x   0        0        0     1645 2023-02-07 20:04:42.000000 youdotcom-2.0.8/youdotcom/write.py
--rwxr-xr-x   0        0        0     1939 2023-02-13 18:30:34.000000 youdotcom-2.0.8/youdotcom/youchat.py
--rw-r--r--   0        0        0    16789 1970-01-01 00:00:00.000000 youdotcom-2.0.8/setup.py
--rw-r--r--   0        0        0    16805 1970-01-01 00:00:00.000000 youdotcom-2.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2023-02-07 20:03:08.000000 youdotcom-2.0.9/LICENSE
+-rwxr-xr-x   0        0        0    15123 2023-02-07 20:04:40.000000 youdotcom-2.0.9/README.md
+-rwxr-xr-x   0        0        0     3893 2023-02-16 16:30:56.000000 youdotcom-2.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      613 2023-02-16 15:26:12.000000 youdotcom-2.0.9/youdotcom/__init__.py
+-rwxr-xr-x   0        0        0     3966 2023-02-16 16:30:50.000000 youdotcom-2.0.9/youdotcom/__main__.py
+-rwxr-xr-x   0        0        0     4347 2023-02-16 14:58:38.000000 youdotcom-2.0.9/youdotcom/api_1.py
+-rwxr-xr-x   0        0        0     8459 2023-02-16 14:58:58.000000 youdotcom-2.0.9/youdotcom/api_2.py
+-rwxr-xr-x   0        0        0     3090 2023-02-07 20:04:40.000000 youdotcom-2.0.9/youdotcom/apps.py
+-rwxr-xr-x   0        0        0     3880 2023-02-07 20:04:42.000000 youdotcom-2.0.9/youdotcom/code.py
+-rwxr-xr-x   0        0        0      544 2023-02-07 20:04:40.000000 youdotcom-2.0.9/youdotcom/config.json
+-rwxr-xr-x   0        0        0     1727 2023-02-07 20:04:40.000000 youdotcom-2.0.9/youdotcom/imagine.py
+-rwxr-xr-x   0        0        0     5342 2023-02-13 18:30:18.000000 youdotcom-2.0.9/youdotcom/init.py
+-rwxr-xr-x   0        0        0     1498 2023-02-07 20:04:40.000000 youdotcom-2.0.9/youdotcom/search.py
+-rwxr-xr-x   0        0        0       80 2023-02-14 20:28:42.000000 youdotcom-2.0.9/youdotcom/test.py
+-rwxr-xr-x   0        0        0     1645 2023-02-07 20:04:42.000000 youdotcom-2.0.9/youdotcom/write.py
+-rwxr-xr-x   0        0        0     1939 2023-02-13 18:30:34.000000 youdotcom-2.0.9/youdotcom/youchat.py
+-rw-r--r--   0        0        0    16789 1970-01-01 00:00:00.000000 youdotcom-2.0.9/setup.py
+-rw-r--r--   0        0        0    16805 1970-01-01 00:00:00.000000 youdotcom-2.0.9/PKG-INFO
```

### Comparing `youdotcom-2.0.8/LICENSE` & `youdotcom-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/README.md` & `youdotcom-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/pyproject.toml` & `youdotcom-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "youdotcom"
-version = "2.0.8"
+version = "2.0.9"
 description = "official api wrapper for you.com and all of its apps"
 readme = "README.md"
 authors = ["SilkePilon <silkepilon2009@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/You-OpenSource/You-Python"
 homepage = "https://github.com/You-OpenSource/You-Python"
```

### Comparing `youdotcom-2.0.8/youdotcom/__init__.py` & `youdotcom-2.0.9/youdotcom/__init__.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/__main__.py` & `youdotcom-2.0.9/youdotcom/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import time
 from enum import Enum
 from importlib import metadata as importlib_metadata
 from random import choice
 import subprocess
 import requests
 import typer
+import pathlib
+import glob
 from click_shell import shell
 from colorama import Fore
 from rich.console import Console
 import click
 from click_shell import make_click_shell
 
 import youdotcom
@@ -73,23 +75,23 @@
     print(f"[API] - using context: {ctx}")
     p = subprocess.Popen(['pip', 'show', 'youdotcom'], stdout=subprocess.PIPE)
     out = p.stdout.read().decode("utf-8") 
 
     data = out.split("\n")
     for line in data:
         if line.startswith("Location: "):
-            if "\\\\" in line:
-                line = line.replace("\\\\", "/")
-            path = line[10:] + "/youdotcom/"
-            path = str(path)
+            path = line[10:]
+            path1 = glob.glob(f'{path}/youdotcom/api_1.py', recursive=True)[0]
+            path2 = glob.glob(f'{path}/youdotcom/api_2.py', recursive=True)[0]
             
-    print(f"[API] - using path {path}")
+            
+    print(f"[API] - using path {path1}\n{path2}")
     
-    api = subprocess.Popen(["python",f"{path}api_1.py"], stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-    backend = subprocess.Popen(["python",f"{path}api_2.py"])
+    api = subprocess.Popen(["python",f"{path1}"], stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+    backend = subprocess.Popen(["python",f"{path2}"])
     # api.terminate()
     # backend.terminate()
     
 
 
 @app.command()
 def chat():
```

### Comparing `youdotcom-2.0.8/youdotcom/api_1.py` & `youdotcom-2.0.9/youdotcom/api_1.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/api_2.py` & `youdotcom-2.0.9/youdotcom/api_2.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/apps.py` & `youdotcom-2.0.9/youdotcom/apps.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/code.py` & `youdotcom-2.0.9/youdotcom/code.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/config.json` & `youdotcom-2.0.9/youdotcom/config.json`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/imagine.py` & `youdotcom-2.0.9/youdotcom/imagine.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/init.py` & `youdotcom-2.0.9/youdotcom/init.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/search.py` & `youdotcom-2.0.9/youdotcom/search.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/write.py` & `youdotcom-2.0.9/youdotcom/write.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/youdotcom/youchat.py` & `youdotcom-2.0.9/youdotcom/youchat.py`

 * *Files identical despite different names*

### Comparing `youdotcom-2.0.8/setup.py` & `youdotcom-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'uvicorn>=0.20.0,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['youdotcom = youdotcom.__main__:app']}
 
 setup_kwargs = {
     'name': 'youdotcom',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': 'official api wrapper for you.com and all of its apps',
     'long_description': '\n<h1 align="center">\n  <br>\n  <a href="https://github.com/SilkePilon/youdotcom/"><img src="https://github.com/SilkePilon/youdotcom/blob/main/youdotcom.png?raw=true" alt="YouDotCom" width="200"></a>\n  <br>\n  <br>\n  YouDotCom for python v1.2.0\n  <br>\n</h1>\n\n<h4 align="center">An python library for <a href="http://you.com/" target="_blank">you.com</a> and all of its apps.</h4>\n\n<div align="center">\n\n  [![Python Version](https://img.shields.io/pypi/pyversions/youdotcom.svg)](https://pypi.org/project/youdotcom/)\n  [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/silkepilon/youdotcom/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n  [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n  [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n  [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/silkepilon/youdotcom/blob/master/.pre-commit-config.yaml)\n  [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/silkepilon/youdotcom/releases)\n  [![License](https://img.shields.io/github/license/silkepilon/youdotcom)](https://github.com/silkepilon/youdotcom/blob/master/LICENSE)\n  ![Coverage Report](assets/images/coverage.svg)\n  \n</div>\n\n<p align="center">\n  <a href="#about">About</a> •\n  <a href="#key-features">Key Features</a> •\n  <a href="#how-to-use">How To Use</a> •\n  <a href="#how-to-install">Install</a> •\n  <a href="#credits">Credits</a> •\n  <a href="#license">License</a>\n</p>\n\n<!-- ![screenshot](https://raw.githubusercontent.com/SilkePilon/youdotcom/main/assets/images/YouDotCom.jpg) -->\n\n## About\nWelcome to the YouDotCom Python Library!\n\nThis library allows users to easily access and utilize all of the functionality of the You.com platform through a simple and intuitive Python interface. With the library, users can access a variety of You.com apps and services, including but not limited to:\n\n* Search\n* YouChat\n* YouCode\n* YouWrite\n\nTo get started with the YouDotCom Python Library, simply <a href="#install">install</a> the package using pip and import it into your Python script. From there, you can use the provided functions and classes to easily interact with the You.com platform.\n\nWe hope you enjoy using the YouDotCom Python Library and all of the features it has to offer!\n> by Chat GPT\n\n\n## Key Features\n* Bypass CloudFlare\n* Interact with YouChat\n* Find code examples\n* Server ready\n  - Supports non-gui operating systems.\n* Cross platform\n  - Windows, macOS and Linux ready.\n\n\n## How to install\n\nTo install the YouDotCom Python Library, use the following command:\n\n```\npip install youdotcom\n```\nThis will install the latest version of the youdotcom package. Always make sure to be up-to-date so you don\'t miss any features, use:\n\n```\npip install youdotcom --upgrade\n```\n\nOnce the installation is complete, you can use the youdotcom package in your Python scripts by importing it:\n\n```python\nimport youdotcom\n```\n\n\n## How To Use\n\nTo help users get started with the YouDotCom Python Library, we have provided a selection of code examples that demonstrate common use cases for the library. These examples can be found below and cover a range of functionality.\n\nTo use the code examples, simply copy and paste the relevant code into your Python script and customize it to fit your specific needs. You can also use the examples as a starting point for your own code, using them as a guide to understand how the library functions can be used to build your own applications and integrations with the You.com platform.\n\nWe hope that these code examples will make it easier for users to get up and running with the YouDotCom Python Library and start building with the You.com platform.\n> :warning: **Warning!**\n> Do not spam or harm the you.com servers in any way!\n\n\n<details>\n<summary>YouChat example</summary>\n<br>\n<h1 align="center">\n  <br>\n  <a href="https://github.com/SilkePilon/youdotcom/"><img src="https://github.com/You-OpenSource/You-Python/blob/main/assets/images/YouChat.png?raw=true" alt="YouChat" width="200"></a>\n  <br>\n</h1>\n\n\n> **Note**\n> YouChat is currently disabled because you.com does not yet support the trafic.\n\n\n```python\nfrom youdotcom import Chat # import all the classes\n\nchat = Chat.send_message(message="how is your day?", api_key="YOUR API KEY HERE") # send a message to YouChat. passing the message and your api key.\n\n# you can get an api key form the site: https://api.betterapi.net/ (with is also made by me)\n\nprint(chat)  # returns the message and some other data\n```\n\n\n#### Context\n> **Note**\n> at the moment there is no context support YET. becuase of new api.\n  \n \n> **Note**\n> Your context will not always be used in the response message is is not a code bug but a YouChat thing. Note its still in beta\n  \nYouDotCom\'s YouChat feature is a powerful tool that allows for context to be utilized in your conversations. By passing a list or a file in the JSON format, you can provide the chatbot with additional information to better understand and respond to your questions.\n\nTo use the context option, you can change the way you send your message by changing the `Chat.send_message` method. This method allows you to pass in a driver, a message, and a context_form_file or a context parameter.\n\nFor example, if you want to use a file, you can pass the file name as the `context_form_file` parameter, like this:\n  \n```python\nChat.send_message(driver=driver, message="YOUR QUESTION HERE", context_form_file="FILE_NAME.json")\n```\n  \nMake sure to change the `FILE_NAME` to the name of the file you are using and include a question in the `message` parameter.\n\nAlternatively, you can also use the context directly without a file by passing in a list as the `context` parameter. Like this:\n  \n```python\nChat.send_message(driver=driver, message="YOUR QUESTION HERE", context=[\'context #1\', \'#2\', \'etc...\'])\n```\n\nBy providing context to your conversations, you can expect more accurate and personalized responses from YouChat, which can help to improve your overall experience.\n\nThe following is an example of a JSON file that can be used as the `context_form_file` parameter in the `Chat.send_message` method:\n\n```json\n{  \n    "context": [ \n        "my name is test",\n        "i love coding",\n        "my hobby\'s are making pictures in nature"\n    ]  \n}  \n```\n\nIn this example, the `context` field contains an array of strings that provide additional information about the user. The strings can include any relevant information that could help the chatbot understand the context of the conversation.\n\n  \n</details>\n\n<details>\n<summary>YouCode example</summary>\n<br>\n\n<h1 align="center">\n  <br>\n  <a href="https://github.com/SilkePilon/youdotcom/"><img src="https://cdn.you.com/img/app-icons/icon-youcode.svg" alt="YouCode" width="200"></a>\n  <br>\n</h1>\n\n\n\n#### Find code\n\n  \n```python\nfrom youdotcom import Webdriver, Code # import all the classes\n\ndriver = Webdriver().driver # setting up the webdriver. use `webdriver_path=` if the pre-installed one does not work.\n\ncode = Code.find_code(driver, search="how to make an python loop?") # get all the code displayed on screen. passing the driver and search string.\n\nfor string in code[\'response\']: # loop through all the code\n    print(string) # print 1 at an time.\n    \nprint(code[\'time\']) # print the time taken to complete you search.\n```\n  \nThis code imports the Code and Webdriver classes from the youdotcom library. The Code class is used to search for code snippets, while the Webdriver class is used to set up a webdriver.\n\nFirst, the Webdriver class is instantiated with Webdriver(). The driver attribute of the resulting object is then stored in the driver variable. The driver attribute returns a webdriver object that can be used to automate web browsing tasks.\n\nNext, the find_code method of the Code class is called with driver and a search string as arguments. This method searches for code snippets related to the specified search string using the webdriver. The result of the method call is stored in the code variable.\n\nThe code variable is a dictionary containing a list of code snippets in the response field and the time taken to complete the search in the time field. The code then loops through the response list and prints each code snippet to the console one at a time. Finally, the time taken to complete the search is printed to the console.\n  \n---\n  \n#### Generate code\n  \n> **Note**\n> Code complete has an daily limit of 20 requests.\n\n```python\nfrom youdotcom import Code # import the write class \n\ntext = Code.gen_code("python loop") # make an api call\n\nprint(text[\'response\']) # print the AI made code\n\nprint(text[\'time\']) # print total time taken to complete your request\n```\n  \nThis code imports the Code class from the youdotcom module. It then calls the gen_code method of the Code class, passing in the string "python loop" as an argument. The gen_code method makes an API call and returns a dictionary with two keys: response and time. The code then prints the value associated with the response key, which is the AI-generated code. It also prints the value associated with the time key, which is the total time taken to complete the request.\n  \n</details>\n\n<details>\n<summary>Search example</summary>\n<br>\n  \n```python\nfrom youdotcom import Search # import the Search class\n\nsearch_results = Search.search_for("how to make an python loop?") # search! No need to use the Webdriver class.\n\nprint(search_results[\'results\']) # print all the search results\n\nprint(search_results[\'time\']) # print the total time taken (les then 3 seconds on average)\n```\n  \nThis code imports the Search class from the youdotcom module. It then calls the search_for method of the Search class, passing in the string "how to make an python loop?" as an argument. The search_for method returns a dictionary with two keys: results and time. The code then prints the value associated with the results key, which is a list of search results. It also prints the value associated with the time key, which is the total time taken to perform the search.\n  \n</details>\n\n<details>\n<summary>YouWrite example</summary>\n<br>\n  \n  \n<h1 align="center">\n  <br>\n  <a href="https://github.com/SilkePilon/youdotcom/"><img src="https://cdn.you.com/img/app-icons/icon-youwrite.svg" alt="YouCode" width="200"></a>\n  <br>\n</h1>\n  \n> **Note**\n> YouWrite has an daily limit of 10 requests.\n  \n```python\nfrom youdotcom import Write # import the write class \n\ntext = Write.write("how to write well?") # make an api call\n\nprint(text[\'response\']) # print the AI made text\n\nprint(text[\'time\']) # print total time taken to complete your request\n```\n  \nThis code imports the Write class from the youdotcom module. It then calls the write method of the Write class, passing in the string "how to write well?" as an argument. The write method makes an API call and returns a dictionary with two keys: response and time. The code then prints the value associated with the response key, which is a text generated by an AI. It also prints the value associated with the time key, which is the total time taken to complete the request.\n  \n</details>\n\n> **Note**\n> YouDotCom is in Alpha and there will be bugs!\n\n\n## Interactive shell\nThe YouDotCom python library offers a wide range of functionality to its users, and one of the ways in which users can access and utilize this functionality is through an interactive terminal shell. With the interactive shell, users are able to execute commands and manipulate the library in real-time, allowing for a more flexible and dynamic experience.\n\nto use the interactive shell, use the following command in your terminal:\n\n```\nyoudotcom\n```\n\nyou will get something like this:\n\n```bash\nWelcome to YouShell an interactive shell for all YouDotCom commands\nEnter \'help\' for a list of available commands.\nType \'exit\' to stop.\n\n\nYouShell >\n```\n\n> **Note**\n> You may sometimes get the following error message: \n> ```\n> Detected a Cloudflare version 2 Captcha challenge, This feature is not available in the opensource (free) version.\n> ```\n\n\n\n\n\n## API\n\n> **Note**\n> The request limit is 5 per minute.\n\nWelcome to the YouDotCom Python library! Our library now features an easy-to-use public API that allows you to interact with YouChat. With this API, you can easily integrate YouChat into your own projects and applications, providing a convenient and user-friendly way for your users to access and utilize the capabilities of the chat bot.\n\nTo get started, you will first need to register for an API key on our website. This key will be required to authenticate each API request.\n\nbase url: `api.betterapi.net`\n\nTo send a message to YouChat and receive a JSON response, you can make an HTTP GET request to the endpoint `/youdotcom/chat`, including the message to be sent as a query parameter. The key is `message` and the value should be the message text encoded in URL format. For example, to send the message `hello there`, the endpoint would be `/youdotcom/chat?message=hello%20there`. The JSON response will include the message sent by YouChat, time, v2Captcha, and type of the request.\n\nAnother endpoint is provided to convert the output text into speech, the endpoint is `/youdotcom/cts`. The message to be converted should be included as a query parameter in the URL, with the key `message` and the value being the message text. For example, to convert the message `hello there` into speech, the endpoint would be `/youdotcom/cts?message=hello%20there`\n\nMake sure to include the API key in the url of each request to authenticate it.\n\n\nWe are constantly improving and updating the YouDotCom library and API, so make sure to check back for new features and updates. If you have any questions or need assistance, feel free to reach out in the Discusions tab. I\'m always happy to help.\n\n\n## YouDotCom roadmap\n* [x] add youchat\n* [x] add youcode\n* [ ] swith to using you.com/api\n* [ ] make code faster\n* [ ] add code translate \n* [ ] add all of you.com apps\n\n\n\n\n## Why You.com?\n<p float="left">\n  <img src="https://github.com/You-OpenSource/You-Python/blob/main/assets/images/1.png?raw=true" width="250" />\n  <img src="https://github.com/You-OpenSource/You-Python/blob/main/assets/images/2.png?raw=true" width="250" /> \n  <img src="https://github.com/You-OpenSource/You-Python/blob/main/assets/images/3.png?raw=true" width="250" />\n</p>\n\n\n\n## Discord\nIn addition to the YouDotCom Python Library, we also have an active [Discord server](https://discord.gg/SD7wZMFSvV) where you can chat with developers and get help with using the library. Our Discord community is a great place to ask questions, share your projects, and get feedback from other developers.\n\n\n## Credits\n\nThis software uses the following open source packages:\n\n- [undetected-chromedriver](https://github.com/ultrafunkamsterdam/undetected-chromedriver)\n\n\n## License\n\nMIT\n\n---\n',
     'author': 'SilkePilon',
     'author_email': 'silkepilon2009@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/You-OpenSource/You-Python',
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 magic>=1.6,<2.0', 'chromedriver-autoinstaller>=0.4.0,<0.5.0', 'click-
 shell>=2.1,<3.0', 'cloudscraper>=1.2.66,<2.0.0', 'fastapi-queue>=0.1.1,<0.2.0',
 'fastapi>=0.92.0,<0.93.0', 'gtts>=2.3.1,<3.0.0', 'markdownify>=0.11.6,<0.12.0',
 'pydantic>=1.10.5,<2.0.0', 'ratelimit>=2.2.1,<3.0.0', 'rich>=10.14,<14.0',
 'slowapi>=0.1.7,<0.2.0', 'typer[all]>=0.4.0,<0.5.0', 'undetected-
 chromedriver>=3.2.1,<4.0.0', 'uvicorn>=0.20.0,<0.21.0'] entry_points = \
 {'console_scripts': ['youdotcom = youdotcom.__main__:app']} setup_kwargs =
-{ 'name': 'youdotcom', 'version': '2.0.8', 'description': 'official api wrapper
+{ 'name': 'youdotcom', 'version': '2.0.9', 'description': 'official api wrapper
 for you.com and all of its apps', 'long_description': '\n
                                   ****** \n
                                \n [YouDotCom]\n
                                       \n
                        \n YouDotCom for python v1.2.0\n
                                    \n ******
 \n\n
```

### Comparing `youdotcom-2.0.8/PKG-INFO` & `youdotcom-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youdotcom
-Version: 2.0.8
+Version: 2.0.9
 Summary: official api wrapper for you.com and all of its apps
 Home-page: https://github.com/You-OpenSource/You-Python
 License: MIT
 Author: SilkePilon
 Author-email: silkepilon2009@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: youdotcom Version: 2.0.8 Summary: official api
+Metadata-Version: 2.1 Name: youdotcom Version: 2.0.9 Summary: official api
 wrapper for you.com and all of its apps Home-page: https://github.com/You-
 OpenSource/You-Python License: MIT Author: SilkePilon Author-email:
 silkepilon2009@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

