# Comparing `tmp/pydicts-0.3.0.tar.gz` & `tmp/pydicts-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicts-0.3.0.tar", max compression
+gzip compressed data, was "pydicts-0.4.0.tar", max compression
```

## Comparing `pydicts-0.3.0.tar` & `pydicts-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.3.0/LICENSE
--rw-r--r--   0        0        0     2829 2023-04-16 10:00:29.766815 pydicts-0.3.0/README.md
--rw-r--r--   0        0        0      144 2023-04-16 09:59:09.244813 pydicts-0.3.0/pydicts/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.3.0/pydicts/classes.py
--rw-r--r--   0        0        0     5382 2023-04-12 05:11:39.114325 pydicts-0.3.0/pydicts/lod.py
--rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.3.0/pydicts/lod_xyv.py
--rw-r--r--   0        0        0     8792 2023-04-15 22:54:44.487769 pydicts-0.3.0/pydicts/lod_ymv.py
--rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.3.0/pydicts/tests/__init__.py
--rw-r--r--   0        0        0      913 2023-04-12 05:37:22.137372 pydicts-0.3.0/pydicts/tests/test_lod.py
--rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.3.0/pydicts/tests/test_lod_ymv.py
--rw-r--r--   0        0        0      407 2023-04-16 09:58:44.859812 pydicts-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 pydicts-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3384 2023-04-19 18:05:13.360372 pydicts-0.4.0/README.md
+-rw-r--r--   0        0        0      144 2023-04-19 18:03:52.588369 pydicts-0.4.0/pydicts/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.4.0/pydicts/classes.py
+-rw-r--r--   0        0        0      424 2023-04-19 18:07:00.714375 pydicts-0.4.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.4.0/pydicts/locale/en.po
+-rw-r--r--   0        0        0      513 2023-04-19 18:07:00.711375 pydicts-0.4.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0     2755 2023-04-19 17:40:24.132024 pydicts-0.4.0/pydicts/locale/es.po
+-rw-r--r--   0        0        0      633 2023-04-19 17:40:13.925023 pydicts-0.4.0/pydicts/locale/pydicts.pot
+-rw-r--r--   0        0        0     5550 2023-04-19 17:47:51.996037 pydicts-0.4.0/pydicts/lod.py
+-rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.4.0/pydicts/lod_xyv.py
+-rw-r--r--   0        0        0     8792 2023-04-15 22:54:44.487769 pydicts-0.4.0/pydicts/lod_ymv.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.4.0/pydicts/tests/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-19 17:53:54.673048 pydicts-0.4.0/pydicts/tests/test_lod.py
+-rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.4.0/pydicts/tests/test_lod_ymv.py
+-rw-r--r--   0        0        0      797 2023-04-19 18:07:56.169377 pydicts-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3901 1970-01-01 00:00:00.000000 pydicts-0.4.0/PKG-INFO
```

### Comparing `pydicts-0.3.0/LICENSE` & `pydicts-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicts-0.3.0/README.md` & `pydicts-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -77,14 +77,40 @@
 |   1 |   4 |
 |   2 |     |
 +-----+-----+
 ```
 
 ### lod_rename_key
 
+### lod_remove_key
+
+Removes a key in all dictionaries in the list of dictionaries
+
+```python
+from pydicts.lod import lod_print, lod_remove_key
+lod=[{"a":1, "b":4},{"a":2, "b":None}]
+>>> from pydicts.lod import *
+>>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
+>>> lod_print(lod)
++-----+-----+
+|   a |   b |
+|-----+-----|
+|   1 |   4 |
+|   2 |     |
++-----+-----+
+>>> lod_remove_key(lod,"b")
+>>> lod_print(lod)
++-----+
+|   a |
+|-----|
+|   1 |
+|   2 |
++-----+
+```
+
 ### lod_sum
 
 Sums all values from a lod key. None values are ignored by default
 
 ```python
 >>> from pydicts.lod import lod_sum
 >>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
@@ -117,14 +143,19 @@
 ### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.4.0 (2023-04-19)
+- Added poetry support
+- Added poethepoet support
+- Added lod_remove_key
+
 ### 0.3.0 (2023-04-16)
 - Added lod_ymv_transposition_with_porcentages
 
 ### 0.2.0 (2023-04-12)
 - Added lod_print with tabulate module
 - Improving documentation
 - Refactorized modules to lod_xyv, lod_ymmv
```

### Comparing `pydicts-0.3.0/pydicts/classes.py` & `pydicts-0.4.0/pydicts/classes.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.3.0/pydicts/lod.py` & `pydicts-0.4.0/pydicts/lod.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,7 +206,14 @@
     """
         Renames a key(from_) to another key(to_) in each dictionary in ld
     """
     for d in ld:
         d[to_]=d.pop(from_)
     return ld
 
+def lod_remove_key(lod, key):
+    """
+        Removes a key from all dictionaries in a list of dictionaries
+    """
+    for d in lod:
+        del d[key]
+    return lod
```

### Comparing `pydicts-0.3.0/pydicts/lod_xyv.py` & `pydicts-0.4.0/pydicts/lod_xyv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.3.0/pydicts/lod_ymv.py` & `pydicts-0.4.0/pydicts/lod_ymv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.3.0/pydicts/tests/test_lod.py` & `pydicts-0.4.0/pydicts/tests/test_lod.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,13 @@
     
 def tests_lod_sum():
     assert lod.lod_sum(lod_, "c")==0
     assert lod.lod_sum(lod_, "d")==16
     with raises(TypeError) as excinfo:
         lod.lod_sum(lod_, "d", ignore_nones=False)==16
     assert "NoneType" in str(excinfo.value)
+    
+def test_lod_remove_key():
+    assert lod.lod_has_key(lod_, "d")
+    lod.lod_remove_key(lod_, "d")
+    assert not lod.lod_has_key(lod_, "d")
+
```

### Comparing `pydicts-0.3.0/PKG-INFO` & `pydicts-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydicts
-Version: 0.3.0
+Version: 0.4.0
 Summary: Module to use dictionaries in various situations
 License: GPL-3.0
 Author: turulomio
 Author-email: turulomio@yahoo.es
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -92,14 +92,40 @@
 |   1 |   4 |
 |   2 |     |
 +-----+-----+
 ```
 
 ### lod_rename_key
 
+### lod_remove_key
+
+Removes a key in all dictionaries in the list of dictionaries
+
+```python
+from pydicts.lod import lod_print, lod_remove_key
+lod=[{"a":1, "b":4},{"a":2, "b":None}]
+>>> from pydicts.lod import *
+>>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
+>>> lod_print(lod)
++-----+-----+
+|   a |   b |
+|-----+-----|
+|   1 |   4 |
+|   2 |     |
++-----+-----+
+>>> lod_remove_key(lod,"b")
+>>> lod_print(lod)
++-----+
+|   a |
+|-----|
+|   1 |
+|   2 |
++-----+
+```
+
 ### lod_sum
 
 Sums all values from a lod key. None values are ignored by default
 
 ```python
 >>> from pydicts.lod import lod_sum
 >>> lod=[{"a":1, "b":4},{"a":2, "b":None}]
@@ -132,14 +158,19 @@
 ### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.4.0 (2023-04-19)
+- Added poetry support
+- Added poethepoet support
+- Added lod_remove_key
+
 ### 0.3.0 (2023-04-16)
 - Added lod_ymv_transposition_with_porcentages
 
 ### 0.2.0 (2023-04-12)
 - Added lod_print with tabulate module
 - Improving documentation
 - Refactorized modules to lod_xyv, lod_ymmv
```

