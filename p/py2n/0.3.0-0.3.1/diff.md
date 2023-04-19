# Comparing `tmp/py2n-0.3.0.tar.gz` & `tmp/py2n-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2n-0.3.0.tar", last modified: Mon Jan  2 15:20:54 2023, max compression
+gzip compressed data, was "py2n-0.3.1.tar", last modified: Wed Apr 19 15:32:35 2023, max compression
```

## Comparing `py2n-0.3.0.tar` & `py2n-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-02 15:20:54.701916 py2n-0.3.0/
--rw-rw-rw-   0        0        0     1092 2022-12-30 17:18:23.000000 py2n-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     1499 2023-01-02 15:20:54.701916 py2n-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-01-01 19:21:37.000000 py2n-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-02 15:20:54.687085 py2n-0.3.0/py2n/
--rw-rw-rw-   0        0        0     4670 2023-01-02 14:07:44.000000 py2n-0.3.0/py2n/__init__.py
--rw-rw-rw-   0        0        0      337 2023-01-02 14:07:45.000000 py2n-0.3.0/py2n/const.py
--rw-rw-rw-   0        0        0     1221 2023-01-02 14:07:46.000000 py2n-0.3.0/py2n/exceptions.py
--rw-rw-rw-   0        0        0     1127 2023-01-02 14:07:46.000000 py2n-0.3.0/py2n/model.py
--rw-rw-rw-   0        0        0     4478 2023-01-02 15:20:42.000000 py2n-0.3.0/py2n/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-02 15:20:54.700912 py2n-0.3.0/py2n.egg-info/
--rw-rw-rw-   0        0        0     1499 2023-01-02 15:20:54.000000 py2n-0.3.0/py2n.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-01-02 15:20:54.000000 py2n-0.3.0/py2n.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-02 15:20:54.000000 py2n-0.3.0/py2n.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-01-02 15:20:54.000000 py2n-0.3.0/py2n.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-02 15:20:54.000000 py2n-0.3.0/py2n.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-12-30 20:45:24.000000 py2n-0.3.0/py2n.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-01-02 15:20:54.701916 py2n-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1069 2023-01-02 15:20:51.000000 py2n-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:32:35.263144 py2n-0.3.1/
+-rw-rw-rw-   0        0        0     1092 2022-12-30 17:18:23.000000 py2n-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     1637 2023-04-19 15:32:35.263144 py2n-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-01-02 15:22:07.000000 py2n-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:32:35.240105 py2n-0.3.1/py2n/
+-rw-rw-rw-   0        0        0     4671 2023-04-19 15:29:05.000000 py2n-0.3.1/py2n/__init__.py
+-rw-rw-rw-   0        0        0      337 2023-01-02 14:07:45.000000 py2n-0.3.1/py2n/const.py
+-rw-rw-rw-   0        0        0     1221 2023-01-02 14:07:46.000000 py2n-0.3.1/py2n/exceptions.py
+-rw-rw-rw-   0        0        0     1127 2023-01-02 14:07:46.000000 py2n-0.3.1/py2n/model.py
+-rw-rw-rw-   0        0        0     4478 2023-01-02 15:20:42.000000 py2n-0.3.1/py2n/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:32:35.261126 py2n-0.3.1/py2n.egg-info/
+-rw-rw-rw-   0        0        0     1637 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-04-19 15:32:35.000000 py2n-0.3.1/py2n.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-19 15:32:34.000000 py2n-0.3.1/py2n.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-12-30 20:45:24.000000 py2n-0.3.1/py2n.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:32:35.263144 py2n-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1069 2023-04-19 15:30:41.000000 py2n-0.3.1/setup.py
```

### Comparing `py2n-0.3.0/LICENSE` & `py2n-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py2n-0.3.0/PKG-INFO` & `py2n-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2n
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for 2N® devices
 Home-page: https://github.com/elektr0nisch/py2n
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Py2N
 
+<img src="https://user-images.githubusercontent.com/38865194/210242643-8f2cef4d-e426-4280-9263-63bee2b66eef.png" width=20% height=20%>
+
 Asynchronous library to control [2N Telekomunikace® devices](https://www.2n.com)
 
 **This library is under development**
 
 ## Requirements
 
 - Python >= 3.9
```

### Comparing `py2n-0.3.0/README.md` & `py2n-0.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Py2N
 
+<img src="https://user-images.githubusercontent.com/38865194/210242643-8f2cef4d-e426-4280-9263-63bee2b66eef.png" width=20% height=20%>
+
 Asynchronous library to control [2N Telekomunikace® devices](https://www.2n.com)
 
 **This library is under development**
 
 ## Requirements
 
 - Python >= 3.9
```

### Comparing `py2n-0.3.0/py2n/__init__.py` & `py2n-0.3.1/py2n/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         """Get switch status."""
         if not self.initialized:
             raise NotInitialized
 
         if not self._data.switches:
             raise Py2NError("no switches configured")
 
-        if switch_id < 1 | switch_id > len(self._data.switches):
+        if switch_id < 1 or switch_id > len(self._data.switches):
             raise Py2NError("invalid switch id")
 
         return self._data.switches[switch_id - 1].active
 
     async def close(self) -> None:
         """Close http session."""
         if not self.initialized:
```

### Comparing `py2n-0.3.0/py2n/exceptions.py` & `py2n-0.3.1/py2n/exceptions.py`

 * *Files identical despite different names*

### Comparing `py2n-0.3.0/py2n/model.py` & `py2n-0.3.1/py2n/model.py`

 * *Files identical despite different names*

### Comparing `py2n-0.3.0/py2n/utils.py` & `py2n-0.3.1/py2n/utils.py`

 * *Files identical despite different names*

### Comparing `py2n-0.3.0/py2n.egg-info/PKG-INFO` & `py2n-0.3.1/py2n.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2n
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for 2N® devices
 Home-page: https://github.com/elektr0nisch/py2n
 Author: Linus Groschke
 Author-email: linus@elektronisch.dev
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Py2N
 
+<img src="https://user-images.githubusercontent.com/38865194/210242643-8f2cef4d-e426-4280-9263-63bee2b66eef.png" width=20% height=20%>
+
 Asynchronous library to control [2N Telekomunikace® devices](https://www.2n.com)
 
 **This library is under development**
 
 ## Requirements
 
 - Python >= 3.9
```

### Comparing `py2n-0.3.0/setup.py` & `py2n-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for py2n."""
 from pathlib import Path
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 
 setup(
     name='py2n',
     version=VERSION,
     license="MIT",
     url="https://github.com/elektr0nisch/py2n",
     author="Linus Groschke",
```

