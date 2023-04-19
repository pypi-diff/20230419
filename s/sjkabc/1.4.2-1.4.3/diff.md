# Comparing `tmp/sjkabc-1.4.2.tar.gz` & `tmp/sjkabc-1.4.3.tar.gz`

## Comparing `sjkabc-1.4.2.tar` & `sjkabc-1.4.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.python-version
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.travis.yml
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 sjkabc-1.4.2/CHANGELOG.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 sjkabc-1.4.2/README.rst
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 sjkabc-1.4.2/requirements.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sjkabc-1.4.2/test.abc
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/Makefile
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/changelog.rst
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/conf.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/contributing.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/index.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/limitations.rst
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/make.bat
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/sjkabc.rst
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sjkabc-1.4.2/docs/tutorial.rst
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sjkabc-1.4.2/sjkabc/__init__.py
--rwxr-xr-x   0        0        0    19730 2020-02-02 00:00:00.000000 sjkabc-1.4.2/sjkabc/sjkabc.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sjkabc-1.4.2/tests/factories.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 sjkabc-1.4.2/tests/test_expand.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sjkabc-1.4.2/tests/test_header_keys.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 sjkabc-1.4.2/tests/test_parser.py
--rw-r--r--   0        0        0     9869 2020-02-02 00:00:00.000000 sjkabc-1.4.2/tests/test_strip.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 sjkabc-1.4.2/tests/test_tune.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 sjkabc-1.4.2/.gitignore
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 sjkabc-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sjkabc-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.python-version
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.travis.yml
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 sjkabc-1.4.3/CHANGELOG.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 sjkabc-1.4.3/README.rst
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 sjkabc-1.4.3/requirements.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 sjkabc-1.4.3/test.abc
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     6845 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/Makefile
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/changelog.rst
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/conf.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/contributing.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/index.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/limitations.rst
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/make.bat
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/sjkabc.rst
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sjkabc-1.4.3/docs/tutorial.rst
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sjkabc-1.4.3/sjkabc/__init__.py
+-rwxr-xr-x   0        0        0    19735 2020-02-02 00:00:00.000000 sjkabc-1.4.3/sjkabc/sjkabc.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 sjkabc-1.4.3/tests/factories.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 sjkabc-1.4.3/tests/test_expand.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 sjkabc-1.4.3/tests/test_header_keys.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 sjkabc-1.4.3/tests/test_parser.py
+-rw-r--r--   0        0        0     9869 2020-02-02 00:00:00.000000 sjkabc-1.4.3/tests/test_strip.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 sjkabc-1.4.3/tests/test_tune.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 sjkabc-1.4.3/.gitignore
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 sjkabc-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sjkabc-1.4.3/PKG-INFO
```

### Comparing `sjkabc-1.4.2/CHANGELOG.rst` & `sjkabc-1.4.3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/README.rst` & `sjkabc-1.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/requirements.txt` & `sjkabc-1.4.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/test.abc` & `sjkabc-1.4.3/test.abc`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/.pytest_cache/v/cache/nodeids` & `sjkabc-1.4.3/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/docs/Makefile` & `sjkabc-1.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/docs/conf.py` & `sjkabc-1.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/docs/contributing.rst` & `sjkabc-1.4.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/docs/index.rst` & `sjkabc-1.4.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/docs/make.bat` & `sjkabc-1.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/docs/tutorial.rst` & `sjkabc-1.4.3/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/sjkabc/sjkabc.py` & `sjkabc-1.4.3/sjkabc/sjkabc.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,8 +775,8 @@
 
     .. seealso:: :func:`get_id_from_field`
     """
     w = textwrap.TextWrapper()
     w.initial_indent = f'{id}:'
     w.subsequent_indent = f'{prefix}:'
     w.width = max_length
-    return '\n'.join(w.wrap(string))
+    return '\n'.join(w.wrap(str(string)))
```

### Comparing `sjkabc-1.4.2/tests/factories.py` & `sjkabc-1.4.3/tests/factories.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/tests/test_expand.py` & `sjkabc-1.4.3/tests/test_expand.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/tests/test_header_keys.py` & `sjkabc-1.4.3/tests/test_header_keys.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/tests/test_parser.py` & `sjkabc-1.4.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/tests/test_strip.py` & `sjkabc-1.4.3/tests/test_strip.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/tests/test_tune.py` & `sjkabc-1.4.3/tests/test_tune.py`

 * *Files identical despite different names*

### Comparing `sjkabc-1.4.2/pyproject.toml` & `sjkabc-1.4.3/pyproject.toml`

 * *Files identical despite different names*

