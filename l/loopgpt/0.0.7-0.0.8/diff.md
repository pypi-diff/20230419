# Comparing `tmp/loopgpt-0.0.7.tar.gz` & `tmp/loopgpt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopgpt-0.0.7.tar", last modified: Wed Apr 19 04:17:29 2023, max compression
+gzip compressed data, was "loopgpt-0.0.8.tar", last modified: Wed Apr 19 19:51:56 2023, max compression
```

## Comparing `loopgpt-0.0.7.tar` & `loopgpt-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.918767 loopgpt-0.0.7/
--rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      114 2023-04-19 04:17:29.918767 loopgpt-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     9147 2023-04-19 04:16:18.000000 loopgpt-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.886448 loopgpt-0.0.7/loopgpt/
--rw-rw-rw-   0        0        0      486 2023-04-19 04:16:57.000000 loopgpt-0.0.7/loopgpt/__init__.py
--rw-rw-rw-   0        0        0    16188 2023-04-19 02:44:42.000000 loopgpt-0.0.7/loopgpt/agent.py
--rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.7/loopgpt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.894727 loopgpt-0.0.7/loopgpt/embeddings/
--rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/embeddings/openai_.py
--rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/embeddings/provider.py
--rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.7/loopgpt/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.902753 loopgpt-0.0.7/loopgpt/loops/
--rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.7/loopgpt/loops/__init__.py
--rw-rw-rw-   0        0        0     1676 2023-04-19 04:11:46.000000 loopgpt-0.0.7/loopgpt/loops/cli.py
--rw-rw-rw-   0        0        0     6835 2023-04-19 02:27:28.000000 loopgpt-0.0.7/loopgpt/loops/repl.py
--rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.7/loopgpt/loops/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.905758 loopgpt-0.0.7/loopgpt/memory/
--rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/memory/__init__.py
--rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/memory/base_memory.py
--rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/memory/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.905758 loopgpt-0.0.7/loopgpt/models/
--rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.7/loopgpt/models/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.7/loopgpt/models/openai_.py
--rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.7/loopgpt/summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.918767 loopgpt-0.0.7/loopgpt/tools/
--rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.7/loopgpt/tools/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.7/loopgpt/tools/agent_manager.py
--rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/tools/base_tool.py
--rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.7/loopgpt/tools/browser.py
--rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.7/loopgpt/tools/code.py
--rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.7/loopgpt/tools/filesystem.py
--rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.7/loopgpt/tools/google_search.py
--rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.7/loopgpt/tools/memory_manager.py
--rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.7/loopgpt/tools/shell.py
--rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.7/loopgpt/tools/simple_browser.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.918767 loopgpt-0.0.7/loopgpt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.7/loopgpt/utils/__init__.py
--rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.7/loopgpt/utils/spinner.py
-drwxrwxrwx   0        0        0        0 2023-04-19 04:17:29.894727 loopgpt-0.0.7/loopgpt.egg-info/
--rw-rw-rw-   0        0        0      114 2023-04-19 04:17:29.000000 loopgpt-0.0.7/loopgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-04-19 04:17:29.000000 loopgpt-0.0.7/loopgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 04:17:29.000000 loopgpt-0.0.7/loopgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 04:17:29.000000 loopgpt-0.0.7/loopgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-19 04:17:29.000000 loopgpt-0.0.7/loopgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 04:17:29.000000 loopgpt-0.0.7/loopgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 04:17:29.918767 loopgpt-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-04-19 04:17:05.000000 loopgpt-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.123895 loopgpt-0.0.8/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      114 2023-04-19 19:51:56.123895 loopgpt-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     9552 2023-04-19 15:21:15.000000 loopgpt-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.092636 loopgpt-0.0.8/loopgpt/
+-rw-rw-rw-   0        0        0      974 2023-04-19 19:51:26.000000 loopgpt-0.0.8/loopgpt/__init__.py
+-rw-rw-rw-   0        0        0    16210 2023-04-19 19:42:51.000000 loopgpt-0.0.8/loopgpt/agent.py
+-rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.8/loopgpt/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.092636 loopgpt-0.0.8/loopgpt/embeddings/
+-rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/embeddings/openai_.py
+-rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/embeddings/provider.py
+-rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.8/loopgpt/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.108269 loopgpt-0.0.8/loopgpt/loops/
+-rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.8/loopgpt/loops/__init__.py
+-rw-rw-rw-   0        0        0     1711 2023-04-19 15:18:34.000000 loopgpt-0.0.8/loopgpt/loops/cli.py
+-rw-rw-rw-   0        0        0     7084 2023-04-19 18:55:48.000000 loopgpt-0.0.8/loopgpt/loops/repl.py
+-rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.8/loopgpt/loops/ui.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.108269 loopgpt-0.0.8/loopgpt/memory/
+-rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/memory/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/memory/base_memory.py
+-rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/memory/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.108269 loopgpt-0.0.8/loopgpt/models/
+-rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.8/loopgpt/models/__init__.py
+-rw-rw-rw-   0        0        0     1950 2023-04-19 15:18:34.000000 loopgpt-0.0.8/loopgpt/models/openai_.py
+-rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.8/loopgpt/summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.123895 loopgpt-0.0.8/loopgpt/tools/
+-rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.8/loopgpt/tools/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.8/loopgpt/tools/agent_manager.py
+-rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/tools/base_tool.py
+-rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.8/loopgpt/tools/browser.py
+-rw-rw-rw-   0        0        0     3731 2023-04-19 19:22:21.000000 loopgpt-0.0.8/loopgpt/tools/code.py
+-rw-rw-rw-   0        0        0     2645 2023-04-19 19:22:11.000000 loopgpt-0.0.8/loopgpt/tools/filesystem.py
+-rw-rw-rw-   0        0        0     2006 2023-04-19 19:22:43.000000 loopgpt-0.0.8/loopgpt/tools/google_search.py
+-rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.8/loopgpt/tools/memory_manager.py
+-rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.8/loopgpt/tools/shell.py
+-rw-rw-rw-   0        0        0     3136 2023-04-19 19:28:31.000000 loopgpt-0.0.8/loopgpt/tools/simple_browser.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.123895 loopgpt-0.0.8/loopgpt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.8/loopgpt/utils/__init__.py
+-rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.8/loopgpt/utils/spinner.py
+drwxrwxrwx   0        0        0        0 2023-04-19 19:51:56.092636 loopgpt-0.0.8/loopgpt.egg-info/
+-rw-rw-rw-   0        0        0      114 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 19:51:55.000000 loopgpt-0.0.8/loopgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 19:51:56.123895 loopgpt-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      464 2023-04-19 19:51:31.000000 loopgpt-0.0.8/setup.py
```

### Comparing `loopgpt-0.0.7/LICENSE` & `loopgpt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/README.md` & `loopgpt-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 </p>
 </H1>
 <p align="center">
     <b>A Modular Auto-GPT Framework</b>
 </p>
 
 <p align="center">
-    <a href="https://join.slack.com/t/lpgptcommunity/shared_invite/zt-1tsew1e4g-WgHfFLSzWF~a0PVq8QXcoQ">
-        <img src="https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white">
+    <a href="https://discord.gg/rqs26cqx7v">
+        <img src="https://img.shields.io/discord/1098162593291587594?style=for-the-badge">
     </a>
 </p>
 
+
+
+
 L♾️pGPT is a re-implementation of the popular [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT) project as a proper python package, written with modularity and extensibility in mind.
 
 ## 🚀 Features 🚀
 
 *  **"Plug N Play" API** - Extensible and modular "Pythonic" framework, not just a command line tool. Easy to add new features, integrations and custom agent capabilities, all from python code, no nasty config files!
 *  **GPT 3.5 friendly** - Better results than Auto-GPT for those who don't have GPT-4 access yet!
 *  **Minimal prompt overhead** - Every token counts. We are continuously working on getting the best results with the least possible number of tokens.
@@ -45,14 +48,15 @@
 git clone https://www.github.com/farizrahman4u/loopgpt.git@main
 cd loopgpt
 python setup.py develop
 ```
 
 ## 🏎️ Getting Started
 
+**You must set your OpenAI API Key 🔑 in your environment variables for anything to work. See the [Requirements secion](#-requirements) below.**
 
 ### Create a new L♾️pGPT Agent🕵️:
 
 ```python
 from loopgpt.agent import Agent
 
 agent = Agent()
@@ -124,15 +128,15 @@
 
 ```python
 from loopgpt.tools import BaseTool
 
 class GetWeather(BaseTool):
     @property
     def args(self):
-        return {"city": "A string with the name of the city"}
+        return {"city": "name of the city"}
     
     @property
     def resp(self):
         return {"report": "The weather report for the city"}
     
     def run(self, city):
         ...
@@ -167,15 +171,15 @@
         try:
             url = "https://wttr.in/{}?format=%l+%C+%h+%t+%w+%p+%P".format(city)
             data = requests.get(url).text.split(" ")
             keys = ("location", "condition", "humidity", "temperature", "wind", "precipitation", "pressure")
             data = {"report": dict(zip(keys, data))}
             return data
         except Exception as e:
-            return f"An error occured while getting the weather: {e}."
+            return {"report": f"An error occured while getting the weather: {e}."}
 ```
 
 That's it! You've built your first custom tool. Let's register it with a new agent and run it:
 
 ```python
 import loopgpt
 
@@ -273,14 +277,19 @@
 agent = loopgpt.Agent.from_config(agent_config)
 ```
 
 ## 📋 Requirements
 
 - Python 3.8+
 - [An OpenAI API Key](https://platform.openai.com/account/api-keys)
+    - Set environment variable `OPENAI_API_KEY` to the API key
+    - How to set environment variables:
+        - [Windows](https://www.architectryan.com/2018/08/31/how-to-change-environment-variables-on-windows-10/)
+        - [Linux](https://www.freecodecamp.org/news/how-to-set-an-environment-variable-in-linux/)
+        - [Mac](https://phoenixnap.com/kb/set-environment-variable-mac)
 - Google Chrome
 
 ### Optional Requirements
 
 For official google search support:
 - [Google API Key](https://console.developers.google.com) (for Google Search)
     - Set environment variable `GOOGLE_API_KEY` to the API key
@@ -292,8 +301,8 @@
 
 ## 💌 Contribute 
 
 We need A LOT of Help! Please open an issue or a PR if you'd like to contribute.
 
 ## 🌳 Community
 
-Join our [Community Slack](https://join.slack.com/t/lpgptcommunity/shared_invite/zt-1tsew1e4g-WgHfFLSzWF~a0PVq8QXcoQ)
+Need help? Join our [Discord](https://discord.gg/rqs26cqx7v).
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
 ****** Lâ¾ï¸pGPT ******
                          A Modular Auto-GPT Framework
-           [https://img.shields.io/badge/Slack-4A154B?style=for-the-
-                       badge&logo=slack&logoColor=white]
+   [https://img.shields.io/discord/1098162593291587594?style=for-the-badge]
 Lâ¾ï¸pGPT is a re-implementation of the popular [Auto-GPT](https://
 github.com/Significant-Gravitas/Auto-GPT) project as a proper python package,
 written with modularity and extensibility in mind. ## ð Features ð *
 **"Plug N Play" API** - Extensible and modular "Pythonic" framework, not just a
 command line tool. Easy to add new features, integrations and custom agent
 capabilities, all from python code, no nasty config files! * **GPT 3.5
 friendly** - Better results than Auto-GPT for those who don't have GPT-4 access
@@ -16,15 +15,17 @@
 Lâ¾ï¸pGPT can save the complete state of an agent, including memory and the
 states of its tools to a file or python object. No external databases or vector
 stores required (but they are still supported)! ## ð§âð» Installation ###
 Install from PyPI ```bash pip install loopgpt ``` ### Install from source
 ```bash pip install git+https://www.github.com/farizrahman4u/loopgpt.git@main
 ``` ### Install from source (dev) ```bash git clone https://www.github.com/
 farizrahman4u/loopgpt.git@main cd loopgpt python setup.py develop ``` ##
-ðï¸ Getting Started ### Create a new Lâ¾ï¸pGPT Agentðµï¸: ```python
+ðï¸ Getting Started **You must set your OpenAI API Key ð in your
+environment variables for anything to work. See the [Requirements secion](#-
+requirements) below.** ### Create a new Lâ¾ï¸pGPT Agentðµï¸: ```python
 from loopgpt.agent import Agent agent = Agent() ``` Lâ¾ï¸pGPT uses `gpt-3.5-
 turbo` by default and all outputs shown here are made using it. GPT-4 users can
 set `model="gpt-4"` instead: ```python agent = Agent(model="gpt-4") ``` ###
 Setup the Agentðµï¸'s attributes: ```python agent.name = "ResearchGPT"
 agent.description = "an AI assistant that researches and finds the best tech
 products" agent.goals = [ "Search for the best headphones on Google", "Analyze
 specs, prices and reviews to find the top 5 best headphones", "Write the list
@@ -46,30 +47,30 @@
 Let's create WeatherGPT, an AI assistant for all things weather. A tool
 inherits from `BaseTool` and you only need to override 3 methods to get your
 tool up and running! - `args`: A dictionary describing the tool's arguments and
 their descriptions. - `resp`: A dictionary describing the tool's response and
 their descriptions. - `run`: The tool's main logic. It takes the tool's
 arguments as input and returns the tool's response. ```python from
 loopgpt.tools import BaseTool class GetWeather(BaseTool): @property def args
-(self): return {"city": "A string with the name of the city"} @property def
-resp(self): return {"report": "The weather report for the city"} def run(self,
-city): ... ``` Lâ¾ï¸pGPT gives a default ID and description to your tool but
-you can override them if you'd like: ```python class GetWeather(BaseTool): ...
+(self): return {"city": "name of the city"} @property def resp(self): return
+{"report": "The weather report for the city"} def run(self, city): ... ```
+Lâ¾ï¸pGPT gives a default ID and description to your tool but you can
+override them if you'd like: ```python class GetWeather(BaseTool): ...
 @property def id(self): return "get_weather_command" @property def desc(self):
 """A description is recommended so that the agent knows more about what the
 tool does""" return "Quickly get the weather for a given city" ``` Now let's
 define what our tool will do in its `run` method: ```python import requests #
 Define your custom tool class GetWeather(BaseTool): ... def run(self, city):
 try: url = "https://wttr.in/{}?format=%l+%C+%h+%t+%w+%p+%P".format(city) data =
 requests.get(url).text.split(" ") keys = ("location", "condition", "humidity",
 "temperature", "wind", "precipitation", "pressure") data = {"report": dict(zip
-(keys, data))} return data except Exception as e: return f"An error occured
-while getting the weather: {e}." ``` That's it! You've built your first custom
-tool. Let's register it with a new agent and run it: ```python import loopgpt #
-Create Agent agent = loopgpt.Agent() agent.name = "WeatherGPT"
+(keys, data))} return data except Exception as e: return {"report": f"An error
+occured while getting the weather: {e}."} ``` That's it! You've built your
+first custom tool. Let's register it with a new agent and run it: ```python
+import loopgpt # Create Agent agent = loopgpt.Agent() agent.name = "WeatherGPT"
 agent.description = "an AI assistant that tells you the weather" agent.goals =
 [ "Get the weather for NewYork and Beijing", "Give the user tips on how to
 dress for the weather in NewYork and Beijing", "Write the tips to a file called
 'dressing_tips.txt'" ] # Register custom tool type # This is actually not
 required here, but is required when you load a saved agent with custom tools.
 loopgpt.tools.register_tool_type(GetWeather) # Register Tool weather_tool =
 GetWeather() agent.tools[weather_tool.id] = weather_tool # Run the agent's CLI
@@ -94,18 +95,22 @@
 agent.cli() ``` or by running the saved agent from the command line: ```bash
 loopgpt run ResearchGPT.json ``` You can convert the agent state to a json
 compatible python dictionary instead of writing to a file: ```python
 agent_config = agent.config() ``` To get just the configuration without the
 internal state: ```python agent_config = agent.config(include_state=False) ```
 To reload the agent from the config, use: ```python import loopgpt agent =
 loopgpt.Agent.from_config(agent_config) ``` ## ð Requirements - Python 3.8+
-- [An OpenAI API Key](https://platform.openai.com/account/api-keys) - Google
-Chrome ### Optional Requirements For official google search support: - [Google
-API Key](https://console.developers.google.com) (for Google Search) - Set
-environment variable `GOOGLE_API_KEY` to the API key - [Google Custom Search
-Engine ID](https://cse.google.com/cse/create/new) (also for Google Search) -
-Set environment variable `CUSTOM_SEARCH_ENGINE_ID` to the CSE ID In case these
-are absent, Lâ¾ï¸pGPT will fall back to using [DuckDuckGo Search](https://
-pypi.org/project/duckduckgo-search/) ## ð Contribute We need A LOT of Help!
-Please open an issue or a PR if you'd like to contribute. ## ð³ Community
-Join our [Community Slack](https://join.slack.com/t/lpgptcommunity/
-shared_invite/zt-1tsew1e4g-WgHfFLSzWF~a0PVq8QXcoQ)
+- [An OpenAI API Key](https://platform.openai.com/account/api-keys) - Set
+environment variable `OPENAI_API_KEY` to the API key - How to set environment
+variables: - [Windows](https://www.architectryan.com/2018/08/31/how-to-change-
+environment-variables-on-windows-10/) - [Linux](https://www.freecodecamp.org/
+news/how-to-set-an-environment-variable-in-linux/) - [Mac](https://
+phoenixnap.com/kb/set-environment-variable-mac) - Google Chrome ### Optional
+Requirements For official google search support: - [Google API Key](https://
+console.developers.google.com) (for Google Search) - Set environment variable
+`GOOGLE_API_KEY` to the API key - [Google Custom Search Engine ID](https://
+cse.google.com/cse/create/new) (also for Google Search) - Set environment
+variable `CUSTOM_SEARCH_ENGINE_ID` to the CSE ID In case these are absent,
+Lâ¾ï¸pGPT will fall back to using [DuckDuckGo Search](https://pypi.org/
+project/duckduckgo-search/) ## ð Contribute We need A LOT of Help! Please
+open an issue or a PR if you'd like to contribute. ## ð³ Community Need help?
+Join our [Discord](https://discord.gg/rqs26cqx7v).
```

### Comparing `loopgpt-0.0.7/loopgpt/agent.py` & `loopgpt-0.0.8/loopgpt/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
             "model": self.model,
             "temperature": self.temperature,
             "tools": [tool.config() for tool in self.tools.values()],
         }
         if include_state:
             cfg.update(
                 {
-                    "sub_agents": {k: v.config() for k, v in self.sub_agents.items()},
+                    "sub_agents": {k: (v[0].config(), v[1]) for k, v in self.sub_agents.items()},
                     "history": self.history[:],
                     "memory": self.memory.config(),
                     "staging_tool": self.staging_tool,
                     "staging_response": self.staging_response,
                     "tool_response": self.tool_response,
                 }
             )
@@ -383,15 +383,15 @@
         agent.name = config["name"]
         agent.description = config["description"]
         agent.goals = config["goals"][:]
         agent.temperature = config["temperature"]
         agent.model = config["model"]
         agent.tools = {tool.id: tool for tool in map(tool_from_config, config["tools"])}
         agent.sub_agents = {
-            k: cls.from_config(v) for k, v in config.get("sub_agents", {}).items()
+            k: (cls.from_config(v[0]), v[1]) for k, v in config.get("sub_agents", {}).items()
         }
         agent.history = config.get("history", [])
         memory = config.get("memory")
         if memory:
             agent.memory = memory_from_config(memory)
         agent.staging_tool = config.get("staging_tool")
         agent.staging_response = config.get("staging_response")
```

### Comparing `loopgpt-0.0.7/loopgpt/constants.py` & `loopgpt-0.0.8/loopgpt/constants.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/embeddings/__init__.py` & `loopgpt-0.0.8/loopgpt/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/embeddings/openai_.py` & `loopgpt-0.0.8/loopgpt/embeddings/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/loops/cli.py` & `loopgpt-0.0.8/loopgpt/loops/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import argparse
 import json
 
 
 def main():
     parser = argparse.ArgumentParser()
 
-    parser.add_argument("action", choices=["run"], help="Action to perform. If no file is specified, a new agent is created.")
+    parser.add_argument(
+        "action",
+        choices=["run"],
+        help="Action to perform. If no file is specified, a new agent is created.",
+    )
     parser.add_argument("filename", nargs="?", help="Agent state JSON.", default=None)
     parser.add_argument(
         "--readonly",
         help="Read only mode. Does not write agent state to disk.",
         action="store_true",
     )
     parser.add_argument(
```

### Comparing `loopgpt-0.0.7/loopgpt/loops/repl.py` & `loopgpt-0.0.8/loopgpt/loops/repl.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     lst = []
     i = 1
     while True:
         print(
             indent + f"- {Fore.LIGHTBLUE_EX}{item_kind} {i} : {Style.RESET_ALL}", end=""
         )
         inp = input()
+        if inp.lower().strip() == "exit":
+            return -1
         if inp.strip():
             lst.append(inp)
         else:
             break
         i += 1
     print()
     return lst
@@ -76,30 +78,39 @@
     char = "\u2501" if big else "\u2500"
     columns = os.get_terminal_size().columns
     print(char * columns)
 
 
 def check_agent_config(agent):
     if agent.name is None or agent.name == DEFAULT_AGENT_NAME:
-        agent.name = prompt("loopgpt", "Enter the name of your AI agent: ")
+        name = prompt("loopgpt", "Enter the name of your AI agent: ")
+        if name.lower().strip() == "exit":
+            return -1
+        agent.name = name
 
     if agent.description is None or agent.description == DEFAULT_AGENT_DESCRIPTION:
-        agent.description = prompt("loopgpt", "Enter a description for your AI agent: ")
+        description = prompt("loopgpt", "Enter a description for your AI agent: ")
+        if description.lower().strip() == "exit":
+            return -1
+        agent.description = description
 
     if agent.goals == []:
-        agent.goals = listed_prompt(
-            "loopgpt", "Enter the goals of your AI agent: ", "Goal"
-        )
+        goals = listed_prompt("loopgpt", "Enter the goals of your AI agent: ", "Goal")
+        if goals == -1:
+            return -1
+        agent.goals = goals
 
     profiles[agent.name] = Fore.GREEN + agent.name
 
 
 def cli(agent, continuous=False):
     print(HEADER)
-    check_agent_config(agent)
+    res = check_agent_config(agent)
+    if res == -1:
+        return
     write_divider(big=True)
     resp = agent.chat()
     while True:
         if isinstance(resp, str):
             print_line(agent.name, resp)
         else:
             if "thoughts" in resp:
@@ -124,22 +135,22 @@
             if "command" in resp:
                 command = resp["command"]
                 if (
                     isinstance(command, dict)
                     and "name" in command
                     and "args" in command
                 ):
-                    if command["name"] != "do_nothing":
+                    if command["name"]:
                         print_line(
                             "command",
                             f"{command['name']}, Args: {command['args']}",
                             end="\n\n",
                         )
                     while True:
-                        if continuous or command["name"] == "do_nothing":
+                        if continuous:
                             yn = "y"
                         else:
                             yn = input(f"Execute? (Y/N): ")
                             if yn.lower().strip() == "exit":
                                 return
                             yn = yn.lower().strip()
                         if yn in ("y", "n"):
@@ -147,15 +158,14 @@
                     if yn == "y":
                         cmd = agent.staging_tool.get("name", agent.staging_tool)
                         if cmd == "task_complete":
                             return
                         print_line("system", f"Executing command: {cmd}")
                         resp = agent.chat(agent.next_prompt, True)
                         print_line("system", f"{cmd} output: {agent.tool_response}")
-                        print_line("system", f"")
                     elif yn == "n":
                         feedback = input(
                             "Enter feedback (Why not execute the command?): "
                         )
                         if feedback.lower().strip() == "exit":
                             return
                         next_prompt = agent.next_prompt
```

### Comparing `loopgpt-0.0.7/loopgpt/loops/ui.py` & `loopgpt-0.0.8/loopgpt/loops/ui.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/memory/__init__.py` & `loopgpt-0.0.8/loopgpt/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/memory/local_memory.py` & `loopgpt-0.0.8/loopgpt/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/models/openai_.py` & `loopgpt-0.0.8/loopgpt/models/openai_.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 from loopgpt.logger import logger
 import tiktoken
 import time
 import os
 
 
 def _getkey(key: Optional[str] = None):
-    return key or os.environ["OPENAI_API_KEY"]
+    key = key or os.getenv("OPENAI_API_KEY")
+    if key is None:
+        raise ValueError(
+            "OpenAI API Key not found. Please set the `OPENAI_API_KEY` environment variable. "
+            "See https://github.com/farizrahman4u/loopgpt#-requirements for more details"
+        )
 
 
 def chat(
     messages: List[Dict[str, str]],
     model: str = "gpt-3.5-turbo",
     api_key: Optional[str] = None,
     max_tokens: Optional[int] = None,
```

### Comparing `loopgpt-0.0.7/loopgpt/summarizer.py` & `loopgpt-0.0.8/loopgpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/tools/__init__.py` & `loopgpt-0.0.8/loopgpt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/tools/agent_manager.py` & `loopgpt-0.0.8/loopgpt/tools/agent_manager.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/tools/base_tool.py` & `loopgpt-0.0.8/loopgpt/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/tools/browser.py` & `loopgpt-0.0.8/loopgpt/tools/browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/tools/code.py` & `loopgpt-0.0.8/loopgpt/tools/code.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             return self.agent.model
         return "gpt-3.5-turbo"
 
 
 class ExecutePythonFile(_BaseCodeTool):
     @property
     def args(self):
-        return {"file": "The Python file path"}
+        return {"file": "The Python file path as a string."}
 
     @property
     def resp(self):
         return {
             "output": "Value of stdout if the execution was successfull. Else error message."
         }
```

### Comparing `loopgpt-0.0.7/loopgpt/tools/filesystem.py` & `loopgpt-0.0.8/loopgpt/tools/filesystem.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from loopgpt.tools.base_tool import BaseTool
 import os
 
 
 class ReadFromFile(BaseTool):
     @property
     def args(self):
-        return {"file": "Path to the file to read."}
+        return {"file": "Path to the file to read as a string."}
 
     @property
     def resp(self):
         return {
             "content": "Contents of the file. If the file doesn't exist, this field will be empty."
         }
 
@@ -21,16 +21,16 @@
             return {"content": ""}
 
 
 class WriteToFile(BaseTool):
     @property
     def args(self):
         return {
-            "file": "Path of the file to write to.",
-            "content": "Content to be written to the file.",
+            "file": "Path of the file to write to as a string.",
+            "content": "Content to be written to the file as a string.",
         }
 
     @property
     def resp(self):
         return {"success": "true or false"}
 
     def run(self, file, content):
@@ -39,16 +39,16 @@
         return {"success": True}
 
 
 class AppendToFile(BaseTool):
     @property
     def args(self):
         return {
-            "file": "Path of the file to append to.",
-            "content": "Content to be appended to the file.",
+            "file": "Path of the file to append to as a string.",
+            "content": "The content to be appended to the file as a string.",
         }
 
     @property
     def resp(self):
         return {"success": "true or false"}
 
     def run(self, file, content):
@@ -56,15 +56,15 @@
             f.write(content)
         return {"success": True}
 
 
 class DeleteFile(BaseTool):
     @property
     def args(self):
-        return {"file": "Path to the file to be deleted"}
+        return {"file": "Path to the file to be deleted as a string."}
 
     @property
     def resp(self):
         return {"success": "true if the file was successfully deleted. Else false."}
 
     def run(self, file):
         try:
@@ -73,15 +73,15 @@
         except Exception:
             return {"success": False}
 
 
 class CheckIfFileExists(BaseTool):
     @property
     def args(self):
-        return {"file": "Path to the check if file exists."}
+        return {"file": "Path to the check if file exists as a string."}
 
     @property
     def resp(self):
         return {"exists": "true if the file exists, else false."}
 
     def run(self, file):
         return {"exists": os.path.isfile(file)}
```

### Comparing `loopgpt-0.0.7/loopgpt/tools/google_search.py` & `loopgpt-0.0.8/loopgpt/tools/google_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     @property
     def args(self):
         return {"query": "The query to search for"}
 
     @property
     def resp(self):
         return {
-            "results": "A list of results. Each result is of the form [title, link, description]"
+            "results": "A list of results. Each result is a list of the form [title, link, description]"
         }
 
     def _duckduckgo_search(self, query, num_results=8):
         from duckduckgo_search import ddg
 
         results = []
         for result in ddg(query, max_results=num_results):
```

### Comparing `loopgpt-0.0.7/loopgpt/tools/shell.py` & `loopgpt-0.0.8/loopgpt/tools/shell.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt/tools/simple_browser.py` & `loopgpt-0.0.8/loopgpt/tools/simple_browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     @property
     def desc(self):
         return "Scrape answers for a question in a given web page"
 
     @property
     def args(self):
-        return {"url": "URL of the website to scrape", "question": "The question"}
+        return {"url": "URL of the website to scrape as a string", "question": "The question"}
 
     @property
     def resp(self):
         return {
             "text": "Summary of relevant text scraped from the website",
             "links": "list of links from the website, where each item is in the form `[link_text,link_url]`",
         }
```

### Comparing `loopgpt-0.0.7/loopgpt/utils/spinner.py` & `loopgpt-0.0.8/loopgpt/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.7/loopgpt.egg-info/SOURCES.txt` & `loopgpt-0.0.8/loopgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

