# Comparing `tmp/loopgpt-0.0.5.tar.gz` & `tmp/loopgpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopgpt-0.0.5.tar", last modified: Wed Apr 19 02:59:59 2023, max compression
+gzip compressed data, was "loopgpt-0.0.6.tar", last modified: Wed Apr 19 04:03:43 2023, max compression
```

## Comparing `loopgpt-0.0.5.tar` & `loopgpt-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.403599 loopgpt-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      114 2023-04-19 02:59:59.403599 loopgpt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     8918 2023-04-19 02:58:00.000000 loopgpt-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.379475 loopgpt-0.0.5/loopgpt/
--rw-rw-rw-   0        0        0      486 2023-04-19 02:59:26.000000 loopgpt-0.0.5/loopgpt/__init__.py
--rw-rw-rw-   0        0        0    16188 2023-04-19 02:44:42.000000 loopgpt-0.0.5/loopgpt/agent.py
--rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.387501 loopgpt-0.0.5/loopgpt/embeddings/
--rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/embeddings/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/embeddings/openai_.py
--rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/embeddings/provider.py
--rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.5/loopgpt/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.387501 loopgpt-0.0.5/loopgpt/loops/
--rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.5/loopgpt/loops/__init__.py
--rw-rw-rw-   0        0        0      964 2023-04-18 01:42:45.000000 loopgpt-0.0.5/loopgpt/loops/cli.py
--rw-rw-rw-   0        0        0     6835 2023-04-19 02:27:28.000000 loopgpt-0.0.5/loopgpt/loops/repl.py
--rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.5/loopgpt/loops/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.395563 loopgpt-0.0.5/loopgpt/memory/
--rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/memory/__init__.py
--rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/memory/base_memory.py
--rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/memory/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.395563 loopgpt-0.0.5/loopgpt/models/
--rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.5/loopgpt/models/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.5/loopgpt/models/openai_.py
--rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.403599 loopgpt-0.0.5/loopgpt/tools/
--rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.5/loopgpt/tools/__init__.py
--rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/tools/agent_manager.py
--rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/tools/base_tool.py
--rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.5/loopgpt/tools/browser.py
--rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.5/loopgpt/tools/code.py
--rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.5/loopgpt/tools/filesystem.py
--rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.5/loopgpt/tools/google_search.py
--rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.5/loopgpt/tools/memory_manager.py
--rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.5/loopgpt/tools/shell.py
--rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.5/loopgpt/tools/simple_browser.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.403599 loopgpt-0.0.5/loopgpt/utils/
--rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.5/loopgpt/utils/__init__.py
--rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.5/loopgpt/utils/spinner.py
-drwxrwxrwx   0        0        0        0 2023-04-19 02:59:59.381989 loopgpt-0.0.5/loopgpt.egg-info/
--rw-rw-rw-   0        0        0      114 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 02:59:59.000000 loopgpt-0.0.5/loopgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 02:59:59.403599 loopgpt-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      464 2023-04-19 02:59:31.000000 loopgpt-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.433019 loopgpt-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 06:20:55.000000 loopgpt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      114 2023-04-19 04:03:43.433019 loopgpt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9147 2023-04-19 04:01:55.000000 loopgpt-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.400351 loopgpt-0.0.6/loopgpt/
+-rw-rw-rw-   0        0        0      486 2023-04-19 04:02:49.000000 loopgpt-0.0.6/loopgpt/__init__.py
+-rw-rw-rw-   0        0        0    16188 2023-04-19 02:44:42.000000 loopgpt-0.0.6/loopgpt/agent.py
+-rw-rw-rw-   0        0        0     3962 2023-04-18 22:30:05.000000 loopgpt-0.0.6/loopgpt/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.408372 loopgpt-0.0.6/loopgpt/embeddings/
+-rw-rw-rw-   0        0        0      775 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      810 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/embeddings/openai_.py
+-rw-rw-rw-   0        0        0      426 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/embeddings/provider.py
+-rw-rw-rw-   0        0        0       87 2023-04-19 00:06:55.000000 loopgpt-0.0.6/loopgpt/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.416662 loopgpt-0.0.6/loopgpt/loops/
+-rw-rw-rw-   0        0        0       36 2023-04-17 09:20:22.000000 loopgpt-0.0.6/loopgpt/loops/__init__.py
+-rw-rw-rw-   0        0        0     1424 2023-04-19 03:50:24.000000 loopgpt-0.0.6/loopgpt/loops/cli.py
+-rw-rw-rw-   0        0        0     6835 2023-04-19 02:27:28.000000 loopgpt-0.0.6/loopgpt/loops/repl.py
+-rw-rw-rw-   0        0        0     3108 2023-04-17 03:25:06.000000 loopgpt-0.0.6/loopgpt/loops/ui.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.416662 loopgpt-0.0.6/loopgpt/memory/
+-rw-rw-rw-   0        0        0      698 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/memory/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/memory/base_memory.py
+-rw-rw-rw-   0        0        0     1998 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/memory/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.416662 loopgpt-0.0.6/loopgpt/models/
+-rw-rw-rw-   0        0        0       38 2023-04-15 06:20:55.000000 loopgpt-0.0.6/loopgpt/models/__init__.py
+-rw-rw-rw-   0        0        0     1706 2023-04-17 07:40:41.000000 loopgpt-0.0.6/loopgpt/models/openai_.py
+-rw-rw-rw-   0        0        0     1984 2023-04-18 22:30:05.000000 loopgpt-0.0.6/loopgpt/summarizer.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.425507 loopgpt-0.0.6/loopgpt/tools/
+-rw-rw-rw-   0        0        0     1450 2023-04-17 08:31:57.000000 loopgpt-0.0.6/loopgpt/tools/__init__.py
+-rw-rw-rw-   0        0        0     2276 2023-04-18 22:30:05.000000 loopgpt-0.0.6/loopgpt/tools/agent_manager.py
+-rw-rw-rw-   0        0        0     1112 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/tools/base_tool.py
+-rw-rw-rw-   0        0        0     4158 2023-04-19 00:05:57.000000 loopgpt-0.0.6/loopgpt/tools/browser.py
+-rw-rw-rw-   0        0        0     3718 2023-04-17 07:40:41.000000 loopgpt-0.0.6/loopgpt/tools/code.py
+-rw-rw-rw-   0        0        0     2556 2023-04-18 01:42:45.000000 loopgpt-0.0.6/loopgpt/tools/filesystem.py
+-rw-rw-rw-   0        0        0     1999 2023-04-18 23:51:46.000000 loopgpt-0.0.6/loopgpt/tools/google_search.py
+-rw-rw-rw-   0        0        0      421 2023-04-16 16:37:13.000000 loopgpt-0.0.6/loopgpt/tools/memory_manager.py
+-rw-rw-rw-   0        0        0      675 2023-04-17 03:25:06.000000 loopgpt-0.0.6/loopgpt/tools/shell.py
+-rw-rw-rw-   0        0        0     3124 2023-04-18 22:30:05.000000 loopgpt-0.0.6/loopgpt/tools/simple_browser.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.433019 loopgpt-0.0.6/loopgpt/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-19 00:30:19.000000 loopgpt-0.0.6/loopgpt/utils/__init__.py
+-rw-rw-rw-   0        0        0     4174 2023-04-19 00:30:54.000000 loopgpt-0.0.6/loopgpt/utils/spinner.py
+drwxrwxrwx   0        0        0        0 2023-04-19 04:03:43.408372 loopgpt-0.0.6/loopgpt.egg-info/
+-rw-rw-rw-   0        0        0      114 2023-04-19 04:03:43.000000 loopgpt-0.0.6/loopgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-04-19 04:03:43.000000 loopgpt-0.0.6/loopgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 04:03:43.000000 loopgpt-0.0.6/loopgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-19 04:03:43.000000 loopgpt-0.0.6/loopgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-04-19 04:03:43.000000 loopgpt-0.0.6/loopgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 04:03:43.000000 loopgpt-0.0.6/loopgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 04:03:43.433019 loopgpt-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      464 2023-04-19 04:02:53.000000 loopgpt-0.0.6/setup.py
```

### Comparing `loopgpt-0.0.5/LICENSE` & `loopgpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/README.md` & `loopgpt-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,24 @@
 agent.cli()
 ```
 
 You can exit the CLI by typing "exit".
 
 <img src="/docs/assets/imgs/loopgpt_demo_pic.png?raw=true" height="350">
 
+### 💻 Command Line Only Mode
+
+You can run L♾️pGPT directly from the command line without having to write any python code as well:
+
+```bash
+loopgpt run
+```
+
+Run `loopgpt --help` to see all the available options.
+
 ### 🔁 Continuous Mode 🔁
 
 If `continuous` is set to `True`, the agent will not ask for the user's permission to execute commands. It may go into infinite loops, so use it at your own risk!
 
 ```python
 agent.cli(continuous=True)
 ```
```

#### html2text {}

```diff
@@ -28,30 +28,33 @@
 agent.description = "an AI assistant that researches and finds the best tech
 products" agent.goals = [ "Search for the best headphones on Google", "Analyze
 specs, prices and reviews to find the top 5 best headphones", "Write the list
 of the top 5 best headphones and their prices to a file", "Summarize the pros
 and cons of each headphone and write it to a different file called
 'summary.txt'", ] ``` And we're off! Let's run the Agentðµï¸'s CLI:
 ```python agent.cli() ``` You can exit the CLI by typing "exit". [/docs/assets/
-imgs/loopgpt_demo_pic.png?raw=true] ### ð Continuous Mode ð If
-`continuous` is set to `True`, the agent will not ask for the user's permission
-to execute commands. It may go into infinite loops, so use it at your own risk!
-```python agent.cli(continuous=True) ``` ## âï¸ Adding custom tools âï¸
-Lâ¾ï¸pGPT agents come with a set of builtin tools which allows them to
-perform various basic tasks such as searching the web, filesystem operations,
-etc. You can view these tools with `print(agent.tools)`. In addition to these
-builtin tools, you can also add your own tools to the agent's toolbox. ###
-Example: WeatherGPT ð¦ï¸ Let's create WeatherGPT, an AI assistant for all
-things weather. A tool inherits from `BaseTool` and you only need to override 3
-methods to get your tool up and running! - `args`: A dictionary describing the
-tool's arguments and their descriptions. - `resp`: A dictionary describing the
-tool's response and their descriptions. - `run`: The tool's main logic. It
-takes the tool's arguments as input and returns the tool's response. ```python
-from loopgpt.tools import BaseTool class GetWeather(BaseTool): @property def
-args(self): return {"city": "A string with the name of the city"} @property def
+imgs/loopgpt_demo_pic.png?raw=true] ### ð» Command Line Only Mode You can run
+Lâ¾ï¸pGPT directly from the command line without having to write any python
+code as well: ```bash loopgpt run ``` Run `loopgpt --help` to see all the
+available options. ### ð Continuous Mode ð If `continuous` is set to
+`True`, the agent will not ask for the user's permission to execute commands.
+It may go into infinite loops, so use it at your own risk! ```python agent.cli
+(continuous=True) ``` ## âï¸ Adding custom tools âï¸ Lâ¾ï¸pGPT agents
+come with a set of builtin tools which allows them to perform various basic
+tasks such as searching the web, filesystem operations, etc. You can view these
+tools with `print(agent.tools)`. In addition to these builtin tools, you can
+also add your own tools to the agent's toolbox. ### Example: WeatherGPT ð¦ï¸
+Let's create WeatherGPT, an AI assistant for all things weather. A tool
+inherits from `BaseTool` and you only need to override 3 methods to get your
+tool up and running! - `args`: A dictionary describing the tool's arguments and
+their descriptions. - `resp`: A dictionary describing the tool's response and
+their descriptions. - `run`: The tool's main logic. It takes the tool's
+arguments as input and returns the tool's response. ```python from
+loopgpt.tools import BaseTool class GetWeather(BaseTool): @property def args
+(self): return {"city": "A string with the name of the city"} @property def
 resp(self): return {"report": "The weather report for the city"} def run(self,
 city): ... ``` Lâ¾ï¸pGPT gives a default ID and description to your tool but
 you can override them if you'd like: ```python class GetWeather(BaseTool): ...
 @property def id(self): return "get_weather_command" @property def desc(self):
 """A description is recommended so that the agent knows more about what the
 tool does""" return "Quickly get the weather for a given city" ``` Now let's
 define what our tool will do in its `run` method: ```python import requests #
```

### Comparing `loopgpt-0.0.5/loopgpt/agent.py` & `loopgpt-0.0.6/loopgpt/agent.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/constants.py` & `loopgpt-0.0.6/loopgpt/constants.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/embeddings/__init__.py` & `loopgpt-0.0.6/loopgpt/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/embeddings/openai_.py` & `loopgpt-0.0.6/loopgpt/embeddings/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/loops/cli.py` & `loopgpt-0.0.6/loopgpt/loops/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,37 +3,49 @@
 import argparse
 import json
 
 
 def main():
     parser = argparse.ArgumentParser()
 
-    parser.add_argument("action", choices=["run"], help="Action to perform.")
-    parser.add_argument("filename", help="Agent state JSON.")
+    parser.add_argument("action", choices=["run"], help="Action to perform. If no file is specified, a new agent is created.")
+    parser.add_argument("filename", nargs="?", help="Agent state JSON.", default=None)
     parser.add_argument(
         "--readonly",
         help="Read only mode. Does not write agent state to disk.",
         action="store_true",
     )
     parser.add_argument(
         "--reset",
         help="Reset agent state before use. Name, goals and description are not affected.",
         action="store_true",
     )
+    parser.add_argument(
+        "--save",
+        help="Filename to save the agent. Only applicable when `filename` is not specified.",
+    )
 
     args = parser.parse_args()
 
     filename = args.filename
 
-    with open(filename, "r") as f:
-        agent_state = json.load(f)
-
-    agent = Agent.from_config(agent_state)
-
-    if args.reset:
-        agent.clear_state()
-
-    agent.cli()
-
-    if not args.readonly:
-        with open(filename, "w") as f:
-            json.dump(agent.config(), f)
+    if filename is not None:
+        with open(filename, "r") as f:
+            agent_state = json.load(f)
+
+        agent = Agent.from_config(agent_state)
+
+        if args.reset:
+            agent.clear_state()
+
+        agent.cli()
+
+        if not args.readonly:
+            with open(filename, "w") as f:
+                json.dump(agent.config(), f)
+    else:
+        agent = Agent()
+        agent.cli()
+
+        if args.save:
+            with open(args.save, "w") as f:
+                json.dump(agent.config(), f)
```

### Comparing `loopgpt-0.0.5/loopgpt/loops/repl.py` & `loopgpt-0.0.6/loopgpt/loops/repl.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/loops/ui.py` & `loopgpt-0.0.6/loopgpt/loops/ui.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/memory/__init__.py` & `loopgpt-0.0.6/loopgpt/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/memory/local_memory.py` & `loopgpt-0.0.6/loopgpt/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/models/openai_.py` & `loopgpt-0.0.6/loopgpt/models/openai_.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/summarizer.py` & `loopgpt-0.0.6/loopgpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/__init__.py` & `loopgpt-0.0.6/loopgpt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/agent_manager.py` & `loopgpt-0.0.6/loopgpt/tools/agent_manager.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/base_tool.py` & `loopgpt-0.0.6/loopgpt/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/browser.py` & `loopgpt-0.0.6/loopgpt/tools/browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/code.py` & `loopgpt-0.0.6/loopgpt/tools/code.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/filesystem.py` & `loopgpt-0.0.6/loopgpt/tools/filesystem.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/google_search.py` & `loopgpt-0.0.6/loopgpt/tools/google_search.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/shell.py` & `loopgpt-0.0.6/loopgpt/tools/shell.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/tools/simple_browser.py` & `loopgpt-0.0.6/loopgpt/tools/simple_browser.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt/utils/spinner.py` & `loopgpt-0.0.6/loopgpt/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `loopgpt-0.0.5/loopgpt.egg-info/SOURCES.txt` & `loopgpt-0.0.6/loopgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

