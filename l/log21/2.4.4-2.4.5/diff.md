# Comparing `tmp/log21-2.4.4.tar.gz` & `tmp/log21-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.4.4.tar", last modified: Fri Apr 14 18:35:28 2023, max compression
+gzip compressed data, was "log21-2.4.5.tar", last modified: Wed Apr 19 08:03:38 2023, max compression
```

## Comparing `log21-2.4.4.tar` & `log21-2.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-14 18:35:20.000000 log21-2.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-04-14 18:35:28.828293 log21-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-04-14 18:35:20.000000 log21-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-14 18:35:20.000000 log21-2.4.4/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-14 18:35:20.000000 log21-2.4.4/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 18:35:20.000000 log21-2.4.4/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-14 18:35:20.000000 log21-2.4.4/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-14 18:35:20.000000 log21-2.4.4/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-14 18:35:20.000000 log21-2.4.4/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-04-14 18:35:20.000000 log21-2.4.4/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-04-14 18:35:20.000000 log21-2.4.4/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-14 18:35:20.000000 log21-2.4.4/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-14 18:35:20.000000 log21-2.4.4/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-04-14 18:35:20.000000 log21-2.4.4/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:35:28.828293 log21-2.4.4/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 18:35:28.000000 log21-2.4.4/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:35:28.828293 log21-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 18:35:20.000000 log21-2.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-19 08:03:28.000000 log21-2.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-19 08:03:38.226023 log21-2.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-19 08:03:28.000000 log21-2.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/log21/CrashReporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-19 08:03:28.000000 log21-2.4.5/log21/CrashReporter/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-04-19 08:03:28.000000 log21-2.4.5/log21/CrashReporter/Reporters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-19 08:03:28.000000 log21-2.4.5/log21/CrashReporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-19 08:03:28.000000 log21-2.4.5/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-04-19 08:03:28.000000 log21-2.4.5/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-19 08:03:28.000000 log21-2.4.5/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25534 2023-04-19 08:03:28.000000 log21-2.4.5/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-19 08:03:28.000000 log21-2.4.5/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-04-19 08:03:28.000000 log21-2.4.5/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-19 08:03:28.000000 log21-2.4.5/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-04-19 08:03:28.000000 log21-2.4.5/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:03:38.226023 log21-2.4.5/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 08:03:38.000000 log21-2.4.5/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:03:38.226023 log21-2.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-19 08:03:28.000000 log21-2.4.5/setup.py
```

### Comparing `log21-2.4.4/LICENSE.txt` & `log21-2.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/PKG-INFO` & `log21-2.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.4
+Version: 2.4.5
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
@@ -68,17 +69,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.4
+### 2.4.5
 
-Some bug fixes.
+Added `no_color` parameter to ProgressBar.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.4/README.md` & `log21-2.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.4
+### 2.4.5
 
-Some bug fixes.
+Added `no_color` parameter to ProgressBar.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.4/log21/Argparse.py` & `log21-2.4.5/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/Colors.py` & `log21-2.4.5/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/CrashReporter/Formatters.py` & `log21-2.4.5/log21/CrashReporter/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/CrashReporter/Reporters.py` & `log21-2.4.5/log21/CrashReporter/Reporters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/FileHandler.py` & `log21-2.4.5/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/Formatters.py` & `log21-2.4.5/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/Logger.py` & `log21-2.4.5/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/LoggingWindow.py` & `log21-2.4.5/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/Manager.py` & `log21-2.4.5/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/PPrint.py` & `log21-2.4.5/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/ProgressBar.py` & `log21-2.4.5/log21/ProgressBar.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,28 +37,29 @@
         |████████████████████████████████████████████████████████████████████████████████████████████| 100%
         >>> # Of course, You should try it yourself to see the progress! XD
         >>>
     """
 
     def __init__(self, *args, width: int = None, show_percentage: bool = True, prefix: str = '|', suffix: str = '|',
                  fill: str = '█', empty: str = ' ', format_: str = None, style: str = '%',
-                 new_line_when_complete: bool = True, colors: dict = None, logger: '_log21.Logger' = _logger,
-                 additional_variables: _Dict[str, _Any] = None):
+                 new_line_when_complete: bool = True, colors: dict = None, no_color: bool = False,
+                 logger: '_log21.Logger' = _logger, additional_variables: _Dict[str, _Any] = None):
         """
         :param args: Prevents the use of positional arguments
         :param width: The width of the progress bar
         :param show_percentage: Whether to show the percentage of the progress
         :param prefix: The prefix of the progress bar
         :param suffix: The suffix of the progress bar
         :param fill: The fill character of the progress bar
         :param empty: The empty character of the progress bar
         :param format_: The format of the progress bar
         :param style: The style that is used to format the progress bar
         :param new_line_when_complete: Whether to print a new line when the progress is complete or failed
         :param colors: The colors of the progress bar
+        :param no_color: If True, removes the colors of the progress bar
         :param logger: The logger to use
         :param additional_variables: Additional variables to use in the format and their default values
         """
         # Sets a default value for the width
         if width is None:
             try:
                 width = _shutil.get_terminal_size().columns - 1
@@ -79,14 +80,16 @@
             raise TypeError('`suffix` must be a string')
         if len(fill) != 1:
             raise ValueError('`fill` must be a single character')
         if len(empty) != 1:
             raise ValueError('`empty` must be a single character')
         if style not in ['%', '{']:
             raise ValueError('`style` must be either `%` or `{`')
+        if colors and no_color:
+            raise PermissionError('You cannot use `no_color` and `colors` parameters together!')
         if additional_variables:
             if not isinstance(additional_variables, dict):
                 raise TypeError('`additional_variables` must be a dictionary')
             for key, value in additional_variables.items():
                 if not isinstance(key, str):
                     raise TypeError('`additional_variables` keys must be strings')
                 if not isinstance(value, str):
@@ -122,14 +125,16 @@
                 '%(prefix)s%(bar)s%(suffix)s'
             style = '%'
         self.style = style
         self.new_line_when_complete = new_line_when_complete
         if colors:
             for key, value in colors.items():
                 self.colors[key] = value
+        if no_color:
+            self.colors = {name: '' for name in self.colors}
         self.logger = logger
         self.additional_variables = additional_variables
         self.i = 0
 
     def get_bar(self, progress: float, total: float, **kwargs) -> str:
         if progress == total:
             return self.progress_complete(**kwargs)
```

### Comparing `log21-2.4.4/log21/StreamHandler.py` & `log21-2.4.5/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/TreePrint.py` & `log21-2.4.5/log21/TreePrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/log21/__init__.py` & `log21-2.4.5/log21/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.4.4"
+__version__ = "2.4.5"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
 __all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
            'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
            'INFO', 'DEBUG', 'NOTSET', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
            'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
            'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
```

### Comparing `log21-2.4.4/log21.egg-info/PKG-INFO` & `log21-2.4.5/log21.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.4.4
+Version: 2.4.5
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Home-page: https://github.com/MPCodeWriter21/log21
 Author: CodeWriter21(Mehrad Pooryoussof)
 Author-email: <CodeWriter21@gmail.com>
 License: Apache-2.0 License
 Keywords: python,log,colorize,color,logging
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 log21
 =====
 
 ![version](https://img.shields.io/pypi/v/log21)
@@ -68,17 +69,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.4.4
+### 2.4.5
 
-Some bug fixes.
+Added `no_color` parameter to ProgressBar.
 
 [Full Changes Log](https://github.com/MPCodeWriter21/log21/blob/master/CHANGES-LOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.4.4/log21.egg-info/SOURCES.txt` & `log21-2.4.5/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `log21-2.4.4/setup.py` & `log21-2.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 DESCRIPTION = 'A simple logging package that helps you log colorized messages in Windows console.'
-VERSION = '2.4.4'
+VERSION = '2.4.5'
 
 setup(
     name='log21',
     version=VERSION,
     url='https://github.com/MPCodeWriter21/log21',
     author='CodeWriter21(Mehrad Pooryoussof)',
     author_email='<CodeWriter21@gmail.com>',
@@ -23,12 +23,13 @@
     packages=find_packages(),
     keywords=['python', 'log', 'colorize', 'color', 'logging'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows"
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: MacOS :: MacOS X"
     ]
 )
```

