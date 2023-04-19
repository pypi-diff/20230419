# Comparing `tmp/time_tracker-0.3.0.tar.gz` & `tmp/time_tracker-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_tracker-0.3.0.tar", max compression
+gzip compressed data, was "time_tracker-0.4.0.tar", max compression
```

## Comparing `time_tracker-0.3.0.tar` & `time_tracker-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-13 08:38:39.853413 time_tracker-0.3.0/LICENSE
--rw-r--r--   0        0        0     1256 2023-04-13 08:38:39.853577 time_tracker-0.3.0/README.md
--rw-r--r--   0        0        0      536 2023-04-17 21:14:37.834140 time_tracker-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 08:38:39.855268 time_tracker-0.3.0/time_tracker/__init__.py
--rw-r--r--   0        0        0     2739 2023-04-13 08:38:39.855527 time_tracker-0.3.0/time_tracker/log.py
--rw-r--r--   0        0        0     4805 2023-04-13 08:43:50.542303 time_tracker-0.3.0/time_tracker/main.py
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 time_tracker-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 08:38:39.853413 time_tracker-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1256 2023-04-13 08:38:39.853577 time_tracker-0.4.0/README.md
+-rw-r--r--   0        0        0      639 2023-04-19 11:07:31.905125 time_tracker-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 08:38:39.855268 time_tracker-0.4.0/time_tracker/__init__.py
+-rw-r--r--   0        0        0     2768 2023-04-19 11:11:22.506094 time_tracker-0.4.0/time_tracker/log.py
+-rw-r--r--   0        0        0     5179 2023-04-19 11:09:46.230168 time_tracker-0.4.0/time_tracker/main.py
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 time_tracker-0.4.0/PKG-INFO
```

### Comparing `time_tracker-0.3.0/LICENSE` & `time_tracker-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time_tracker-0.3.0/README.md` & `time_tracker-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `time_tracker-0.3.0/pyproject.toml` & `time_tracker-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 [tool.poetry]
 name = "time-tracker"
-version = "0.3.0"
+version = "0.4.0"
 description = "CLI to track time spent on tasks using pomodoro technique"
 authors = ["Jose Cabeda <jecabeda@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 tt = "time_tracker.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = "0.7.0"
 python-dotenv = "^0.19.2"
 pytest = "^7.3.1"
+rich = "^13.3.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 black = "^21.12b0"
-flake8 = "^6.0.0"
 mypy = "^1.2.0"
+ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry>=1.4"]
 build-backend = "poetry.masonry.api"
+
+
+[tool.ruff]
+line-length = 88
+select = [
+    "B",
+    "C",
+    "E",
+    "F",
+    "W"]
```

### Comparing `time_tracker-0.3.0/time_tracker/log.py` & `time_tracker-0.4.0/time_tracker/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
-from datetime import datetime
 import os
-from dotenv import load_dotenv
+from datetime import datetime
 from pathlib import Path
 
+from dotenv import load_dotenv
+
 
 class Logger:
     def __init__(self):
         # Load envs
         load_dotenv()
         self.apply_configs()
 
@@ -88,7 +89,8 @@
         logging.info(data)
 
     def warning(self, data):
         logging.warn(data)
 
     def error(self, data):
         logging.error(data)
+        logging.error(data)
```

### Comparing `time_tracker-0.3.0/time_tracker/main.py` & `time_tracker-0.4.0/time_tracker/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-import time
 import datetime
-import typer
 import os
+import time
 from enum import Enum
+
+import typer
+from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from time_tracker.log import Logger
 
 
 class SessionType(str, Enum):
     workTime = 1
     breakTime = 2
     bigBreakTime = 3
@@ -73,19 +76,30 @@
         if not nextSession:
             typer.echo("Stop session")
             raise typer.Abort()
 
 
 def countdown(workMinutes: int):
     workSeconds = workMinutes * 60
-    while workSeconds > 0:
-        typer.clear()
-        typer.echo(datetime.timedelta(seconds=workSeconds), nl=True)
-        time.sleep(1)
-        workSeconds = workSeconds - 1
+
+    value: int = 0
+
+    with Progress(
+        SpinnerColumn(),
+        TextColumn("[progress.description]{task.description}"),
+        transient=True,
+    ) as progress:
+        task1 = progress.add_task(description="Processing", total=workSeconds)
+        while value < workSeconds:
+            progress.update(
+                task1,
+                description=f"Time: {datetime.timedelta(seconds=workSeconds- value)}",
+            )
+            time.sleep(1)
+            value += 1
 
     print("Finished session!")
 
 
 def notify(title, text):
     os.system(
         f"""
```

### Comparing `time_tracker-0.3.0/PKG-INFO` & `time_tracker-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: time-tracker
-Version: 0.3.0
+Version: 0.4.0
 Summary: CLI to track time spent on tasks using pomodoro technique
 Author: Jose Cabeda
 Author-email: jecabeda@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: python-dotenv (>=0.19.2,<0.20.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: typer (==0.7.0)
 Description-Content-Type: text/markdown
 
 # `time-tracker`
 
 Time tracker cli
```

