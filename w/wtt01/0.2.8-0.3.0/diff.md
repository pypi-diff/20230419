# Comparing `tmp/wtt01-0.2.8.tar.gz` & `tmp/wtt01-0.3.0.tar.gz`

## Comparing `wtt01-0.2.8.tar` & `wtt01-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.2.8/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.2.8/tests/test_load.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.2.8/wtt01/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.2.8/wtt01/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.2.8/wtt01/_env.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.2.8/wtt01/cli.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 wtt01-0.2.8/wtt01/main.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.2.8/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.2.8/LICENSE.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.2.8/README.md
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 wtt01-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt01-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 wtt01-0.3.0/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtt01-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 wtt01-0.3.0/tests/test_load.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wtt01-0.3.0/wtt01/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 wtt01-0.3.0/wtt01/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 wtt01-0.3.0/wtt01/_env.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wtt01-0.3.0/wtt01/cli.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 wtt01-0.3.0/wtt01/main.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 wtt01-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 wtt01-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wtt01-0.3.0/README.md
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 wtt01-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 wtt01-0.3.0/PKG-INFO
```

### Comparing `wtt01-0.2.8/tests/test_load.py` & `wtt01-0.3.0/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.2.8/wtt01/cli.py` & `wtt01-0.3.0/wtt01/cli.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.2.8/wtt01/main.py` & `wtt01-0.3.0/wtt01/main.py`

 * *Files identical despite different names*

### Comparing `wtt01-0.2.8/.gitignore` & `wtt01-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wtt01-0.2.8/LICENSE.txt` & `wtt01-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wtt01-0.2.8/pyproject.toml` & `wtt01-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wtt01-0.2.8/PKG-INFO` & `wtt01-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtt01
-Version: 0.2.8
+Version: 0.3.0
 Author-email: Trent Hauck <thauck@wheretrue.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

