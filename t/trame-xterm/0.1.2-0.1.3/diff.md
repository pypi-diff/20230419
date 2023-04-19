# Comparing `tmp/trame-xterm-0.1.2.tar.gz` & `tmp/trame-xterm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-xterm-0.1.2.tar", last modified: Wed Apr 12 22:08:28 2023, max compression
+gzip compressed data, was "trame-xterm-0.1.3.tar", last modified: Wed Apr 19 16:42:13 2023, max compression
```

## Comparing `trame-xterm-0.1.2.tar` & `trame-xterm-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/
--rw-r--r--   0 root         (0) root         (0)     1070 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      570 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      901 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.336667 trame-xterm-0.1.2/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.336667 trame-xterm-0.1.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/modules/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame/widgets/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame_xterm/
--rw-r--r--   0 root         (0) root         (0)       93 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame_xterm/module/
--rw-r--r--   0 root         (0) root         (0)      236 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/trame_xterm/module/serve/
--rw-r--r--   0 root         (0) root         (0)     3425 2023-04-12 22:08:24.000000 trame-xterm-0.1.2/trame_xterm/module/serve/style.css
--rw-r--r--   0 root         (0) root         (0)   396472 2023-04-12 22:08:24.000000 trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.mjs
--rw-r--r--   0 root         (0) root         (0)   278894 2023-04-12 22:08:24.000000 trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.344667 trame-xterm-0.1.2/trame_xterm/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14722 2023-04-12 22:08:04.000000 trame-xterm-0.1.2/trame_xterm/widgets/xterm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 22:08:28.340667 trame-xterm-0.1.2/trame_xterm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1317 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-12 22:08:28.000000 trame-xterm-0.1.2/trame_xterm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.657469 trame-xterm-0.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-19 16:42:13.657469 trame-xterm-0.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      570 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      901 2023-04-19 16:42:13.657469 trame-xterm-0.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame/modules/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame/widgets/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame_xterm/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame_xterm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame_xterm/module/
+-rw-r--r--   0 root         (0) root         (0)      236 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame_xterm/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame_xterm/module/serve/
+-rw-r--r--   0 root         (0) root         (0)     3425 2023-04-19 16:42:09.000000 trame-xterm-0.1.3/trame_xterm/module/serve/style.css
+-rw-r--r--   0 root         (0) root         (0)   396472 2023-04-19 16:42:09.000000 trame-xterm-0.1.3/trame_xterm/module/serve/trame-xterm.mjs
+-rw-r--r--   0 root         (0) root         (0)   278894 2023-04-19 16:42:10.000000 trame-xterm-0.1.3/trame_xterm/module/serve/trame-xterm.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.657469 trame-xterm-0.1.3/trame_xterm/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame_xterm/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame_xterm/utils/terminal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.657469 trame-xterm-0.1.3/trame_xterm/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame_xterm/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15821 2023-04-19 16:41:54.000000 trame-xterm-0.1.3/trame_xterm/widgets/xterm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 16:42:13.653469 trame-xterm-0.1.3/trame_xterm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-04-19 16:42:13.000000 trame-xterm-0.1.3/trame_xterm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      635 2023-04-19 16:42:13.000000 trame-xterm-0.1.3/trame_xterm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 16:42:13.000000 trame-xterm-0.1.3/trame_xterm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-19 16:42:13.000000 trame-xterm-0.1.3/trame_xterm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-19 16:42:13.000000 trame-xterm-0.1.3/trame_xterm.egg-info/top_level.txt
```

### Comparing `trame-xterm-0.1.2/LICENSE` & `trame-xterm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.2/PKG-INFO` & `trame-xterm-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-xterm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Trame widget to expose xterm.js
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-xterm-0.1.2/README.rst` & `trame-xterm-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.2/setup.cfg` & `trame-xterm-0.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-xterm
-version = 0.1.2
+version = 0.1.3
 description = Trame widget to expose xterm.js
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-xterm-0.1.2/trame_xterm/module/serve/style.css` & `trame-xterm-0.1.3/trame_xterm/module/serve/style.css`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.mjs` & `trame-xterm-0.1.3/trame_xterm/module/serve/trame-xterm.mjs`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.2/trame_xterm/module/serve/trame-xterm.umd.js` & `trame-xterm-0.1.3/trame_xterm/module/serve/trame-xterm.umd.js`

 * *Files identical despite different names*

### Comparing `trame-xterm-0.1.2/trame_xterm/widgets/xterm.py` & `trame-xterm-0.1.3/trame_xterm/widgets/xterm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,42 @@
+import json
 from termcolor import colored
 from trame_client.widgets.core import AbstractElement
-
 from .. import module
 
+try:
+    from ..utils.terminal import Terminal
+
+    TERMINAL_AVAILABLE = True
+except ModuleNotFoundError:
+    TERMINAL_AVAILABLE = False
+
+
 __ALL__ = ["XTerm", "colored"]
 
 
 class HtmlElement(AbstractElement):
     def __init__(self, _elem_name, children=None, **kwargs):
         super().__init__(_elem_name, children, **kwargs)
         if self.server:
             self.server.enable_module(module)
 
 
 # Expose your vue component(s)
 class XTerm(HtmlElement):
     _next_id = 0
 
-    def __init__(self, **kwargs):
+    def __init__(self, shell=None, **kwargs):
         """
         Create an XTerm element
 
+        Argument:
+
+        :param shell: Shell command as an array (i.e. shell=['/bin/bash']). This is not available on Windows.
+
         Properties:
 
         :param options: XTerm.js option which are only read at creation. (http://xtermjs.org/docs/api/terminal/interfaces/iterminaloptions/ and http://xtermjs.org/docs/api/terminal/interfaces/iterminalinitonlyoptions/)
         :param listen: Specifies the list of event you aim to listen to. [bell, binary, cursorMove, input, key, lineFeed, render, writeParsed, resize, scroll, selectionChange, titleChange]
 
         Events:
 
@@ -76,14 +88,35 @@
             "writeParsed",
             "resize",
             "scroll",
             "selectionChange",
             "titleChange",
         ]
 
+        if shell is not None:
+            if not TERMINAL_AVAILABLE:
+                raise NotImplementedError(
+                    "The shell argument is not implemented for Windows"
+                )
+
+            self._terminal = Terminal(shell, self.write)
+            if self.listen is None:
+                self.listen = "['input', 'resize']"
+            else:
+                array = json.loads(self.listen)
+                if "input" not in array:
+                    array.append("input")
+                if "resize" not in array:
+                    array.append("resize")
+                self.listen = json.dumps(array)
+
+            self.resize = (self._terminal.set_size, "[]", "$event")
+            self.input = (self._terminal.input, "[$event]")
+            self.opened = self._terminal.start
+
     def fit(self):
         """Trigger a fit on the available space"""
         self.server.js_call(self.__ref, "fit")
 
     def blur(self):
         """Trigger a blur on the xterm.js widget"""
         self.server.js_call(self.__ref, "blur")
```

### Comparing `trame-xterm-0.1.2/trame_xterm.egg-info/PKG-INFO` & `trame-xterm-0.1.3/trame_xterm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-xterm
-Version: 0.1.2
+Version: 0.1.3
 Summary: Trame widget to expose xterm.js
 Author: Kitware Inc.
 License: MIT License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `trame-xterm-0.1.2/trame_xterm.egg-info/SOURCES.txt` & `trame-xterm-0.1.3/trame_xterm.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 trame_xterm.egg-info/dependency_links.txt
 trame_xterm.egg-info/requires.txt
 trame_xterm.egg-info/top_level.txt
 trame_xterm/module/__init__.py
 trame_xterm/module/serve/style.css
 trame_xterm/module/serve/trame-xterm.mjs
 trame_xterm/module/serve/trame-xterm.umd.js
+trame_xterm/utils/__init__.py
+trame_xterm/utils/terminal.py
 trame_xterm/widgets/__init__.py
 trame_xterm/widgets/xterm.py
```

