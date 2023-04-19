# Comparing `tmp/pytest-redis-3.0.1.tar.gz` & `tmp/pytest-redis-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-redis-3.0.1.tar", last modified: Mon Mar 27 10:10:28 2023, max compression
+gzip compressed data, was "pytest-redis-3.0.2.tar", last modified: Wed Apr 19 08:28:45 2023, max compression
```

## Comparing `pytest-redis-3.0.1.tar` & `pytest-redis-3.0.2.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17995 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/pytest_redis/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/pytest_redis/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/executor/noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/executor/process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/pytest_redis/factories/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/factories/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/factories/noproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/factories/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/pytest_redis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/pytest_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17995 2023-03-27 10:10:28.000000 pytest-redis-3.0.1/pytest_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-27 10:10:28.000000 pytest-redis-3.0.1/pytest_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:10:28.000000 pytest-redis-3.0.1/pytest_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 10:10:28.000000 pytest-redis-3.0.1/pytest_redis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-27 10:10:28.000000 pytest-redis-3.0.1/pytest_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 10:10:28.000000 pytest-redis-3.0.1/pytest_redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 10:10:27.000000 pytest-redis-3.0.1/pytest_redis.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 10:10:28.148738 pytest-redis-3.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-03-27 10:10:13.000000 pytest-redis-3.0.1/tests/test_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/pytest_redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/pytest_redis/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/executor/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/executor/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/pytest_redis/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/factories/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/factories/noproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/factories/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/pytest_redis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/pytest_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:28:45.000000 pytest-redis-3.0.2/pytest_redis.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:28:45.829139 pytest-redis-3.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-19 08:28:36.000000 pytest-redis-3.0.2/tests/test_redis.py
```

### Comparing `pytest-redis-3.0.1/CHANGES.rst` & `pytest-redis-3.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+3.0.2 (2023-04-19)
+==================
+
+Bugfixes
+--------
+
+- Include py.typed in MANIFEST.in (`#471 <https://https://github.com/ClearcodeHQ/pytest-redis/issues/471>`_)
+
+
 3.0.1 (2023-03-27)
 ==================
 
 Bugfixes
 --------
 
 - Fixed packaging LICENSE file. (`#453 <https://https://github.com/ClearcodeHQ/pytest-redis/issues/453>`_)
```

### Comparing `pytest-redis-3.0.1/CONTRIBUTING.rst` & `pytest-redis-3.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/COPYING.lesser` & `pytest-redis-3.0.2/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/PKG-INFO` & `pytest-redis-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-redis
-Version: 3.0.1
+Version: 3.0.2
 Summary: Redis fixtures and fixture factories for Pytest.
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-redis
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-redis/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-redis/blob/v3.0.1/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-redis/blob/v3.0.2/CHANGES.rst
 Keywords: tests,pytest,fixture,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -186,14 +186,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: COPYING.lesser
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-redis/master/logo.png
     :width: 100px
     :height: 100px
 
 pytest-redis
 ============
```

### Comparing `pytest-redis-3.0.1/README.rst` & `pytest-redis-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pyproject.toml` & `pytest-redis-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pytest-redis"
-version = "3.0.1"
+version = "3.0.2"
 description = "Redis fixtures and fixture factories for Pytest."
 readme = "README.rst"
 keywords = ["tests", "pytest", "fixture", "redis"]
 license = {file = "COPYING.lesser"}
 authors = [
     {name = "Grzegorz Śliwiński", email = "fizyk+pypi@fizyk.dev"}
 ]
@@ -33,15 +33,15 @@
     "redis >= 3",
 ]
 requires-python = ">= 3.8"
 
 [project.urls]
 "Source" = "https://github.com/ClearcodeHQ/pytest-redis"
 "Bug Tracker" = "https://github.com/ClearcodeHQ/pytest-redis/issues"
-"Changelog" = "https://github.com/ClearcodeHQ/pytest-redis/blob/v3.0.1/CHANGES.rst"
+"Changelog" = "https://github.com/ClearcodeHQ/pytest-redis/blob/v3.0.2/CHANGES.rst"
 
 [project.entry-points."pytest11"]
 pytest_redis = "pytest_redis.plugin"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -90,15 +90,15 @@
 showcontent = true
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/ClearcodeHQ/pytest-dynamodb/"
 
 [tool.tbump.version]
-current = "3.0.1"
+current = "3.0.2"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pytest-redis-3.0.1/pytest_redis/__init__.py` & `pytest-redis-3.0.2/pytest_redis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public License
 # along with pytest-redis. If not, see <http://www.gnu.org/licenses/>.
 """Main module for pytest-redis."""
-__version__ = "3.0.1"
+__version__ = "3.0.2"
```

### Comparing `pytest-redis-3.0.1/pytest_redis/config.py` & `pytest-redis-3.0.2/pytest_redis/config.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis/executor/noop.py` & `pytest-redis-3.0.2/pytest_redis/executor/noop.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis/executor/process.py` & `pytest-redis-3.0.2/pytest_redis/executor/process.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis/factories/client.py` & `pytest-redis-3.0.2/pytest_redis/factories/client.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis/factories/noproc.py` & `pytest-redis-3.0.2/pytest_redis/factories/noproc.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis/factories/proc.py` & `pytest-redis-3.0.2/pytest_redis/factories/proc.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis/plugin.py` & `pytest-redis-3.0.2/pytest_redis/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/pytest_redis.egg-info/PKG-INFO` & `pytest-redis-3.0.2/pytest_redis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-redis
-Version: 3.0.1
+Version: 3.0.2
 Summary: Redis fixtures and fixture factories for Pytest.
 Author-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,15 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 Project-URL: Source, https://github.com/ClearcodeHQ/pytest-redis
 Project-URL: Bug Tracker, https://github.com/ClearcodeHQ/pytest-redis/issues
-Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-redis/blob/v3.0.1/CHANGES.rst
+Project-URL: Changelog, https://github.com/ClearcodeHQ/pytest-redis/blob/v3.0.2/CHANGES.rst
 Keywords: tests,pytest,fixture,redis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -186,14 +186,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Framework :: Pytest
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: COPYING.lesser
 
 .. image:: https://raw.githubusercontent.com/ClearcodeHQ/pytest-redis/master/logo.png
     :width: 100px
     :height: 100px
 
 pytest-redis
 ============
```

### Comparing `pytest-redis-3.0.1/pytest_redis.egg-info/SOURCES.txt` & `pytest-redis-3.0.2/pytest_redis.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 CHANGES.rst
 CONTRIBUTING.rst
+COPYING
 COPYING.lesser
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 pytest_redis/__init__.py
 pytest_redis/config.py
 pytest_redis/exception.py
 pytest_redis/plugin.py
+pytest_redis/py.typed
 pytest_redis.egg-info/PKG-INFO
 pytest_redis.egg-info/SOURCES.txt
 pytest_redis.egg-info/dependency_links.txt
 pytest_redis.egg-info/entry_points.txt
 pytest_redis.egg-info/requires.txt
 pytest_redis.egg-info/top_level.txt
 pytest_redis.egg-info/zip-safe
```

### Comparing `pytest-redis-3.0.1/tests/test_executor.py` & `pytest-redis-3.0.2/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pytest-redis-3.0.1/tests/test_redis.py` & `pytest-redis-3.0.2/tests/test_redis.py`

 * *Files identical despite different names*

