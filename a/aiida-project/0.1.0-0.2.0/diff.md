# Comparing `tmp/aiida-project-0.1.0.tar.gz` & `tmp/aiida-project-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-project-0.1.0.tar", last modified: Wed Apr 19 15:03:06 2023, max compression
+gzip compressed data, was "aiida-project-0.2.0.tar", last modified: Wed Apr 19 15:36:14 2023, max compression
```

## Comparing `aiida-project-0.1.0.tar` & `aiida-project-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0      255 2023-04-19 14:02:47.072589 aiida-project-0.1.0/.gitignore
--rw-r--r--   0        0        0     1311 2023-04-19 14:17:00.466431 aiida-project-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      255 2023-04-19 14:14:40.114410 aiida-project-0.1.0/README.md
--rw-r--r--   0        0        0      688 2023-04-19 14:42:52.979252 aiida-project-0.1.0/aiida_project/__init__.py
--rw-r--r--   0        0        0      125 2023-04-19 14:42:52.998063 aiida-project-0.1.0/aiida_project/commands/__init__.py
--rw-r--r--   0        0        0     2365 2023-04-19 14:42:52.996746 aiida-project-0.1.0/aiida_project/commands/create.py
--rw-r--r--   0        0        0       91 2023-04-19 14:42:52.999215 aiida-project-0.1.0/aiida_project/commands/main.py
--rw-r--r--   0        0        0       59 2023-04-19 14:42:53.011017 aiida-project-0.1.0/aiida_project/engine/__init__.py
--rw-r--r--   0        0        0      775 2023-04-19 14:42:53.018996 aiida-project-0.1.0/aiida_project/engine/base.py
--rw-r--r--   0        0        0     1424 2023-04-19 14:42:53.009726 aiida-project-0.1.0/aiida_project/engine/conda.py
--rw-r--r--   0        0        0      287 2023-04-19 14:42:53.012905 aiida-project-0.1.0/aiida_project/engine/factory.py
--rw-r--r--   0        0        0     1119 2023-04-19 14:42:53.027231 aiida-project-0.1.0/aiida_project/engine/virtualenv.py
--rw-r--r--   0        0        0     1036 2023-04-19 14:35:00.161826 aiida-project-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 aiida-project-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1171 2023-04-19 15:36:09.721393 aiida-project-0.2.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1508 2023-04-19 15:36:09.721393 aiida-project-0.2.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      255 2023-04-19 15:36:09.721393 aiida-project-0.2.0/.gitignore
+-rw-r--r--   0        0        0      298 2023-04-19 15:36:09.721393 aiida-project-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1311 2023-04-19 15:36:09.721393 aiida-project-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      255 2023-04-19 15:36:09.721393 aiida-project-0.2.0/README.md
+-rw-r--r--   0        0        0      689 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/__init__.py
+-rw-r--r--   0        0        0      125 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/commands/__init__.py
+-rw-r--r--   0        0        0     2365 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/commands/create.py
+-rw-r--r--   0        0        0       91 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/commands/main.py
+-rw-r--r--   0        0        0       59 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/__init__.py
+-rw-r--r--   0        0        0      775 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/base.py
+-rw-r--r--   0        0        0     1424 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/conda.py
+-rw-r--r--   0        0        0      287 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/factory.py
+-rw-r--r--   0        0        0     1119 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/virtualenv.py
+-rw-r--r--   0        0        0     1036 2023-04-19 15:36:09.721393 aiida-project-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 aiida-project-0.2.0/PKG-INFO
```

### Comparing `aiida-project-0.1.0/LICENSE.txt` & `aiida-project-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-project-0.1.0/aiida_project/__init__.py` & `aiida-project-0.2.0/aiida_project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """The `aiida-project` module."""
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

### Comparing `aiida-project-0.1.0/aiida_project/commands/create.py` & `aiida-project-0.2.0/aiida_project/commands/create.py`

 * *Files identical despite different names*

### Comparing `aiida-project-0.1.0/aiida_project/engine/base.py` & `aiida-project-0.2.0/aiida_project/engine/base.py`

 * *Files identical despite different names*

### Comparing `aiida-project-0.1.0/aiida_project/engine/conda.py` & `aiida-project-0.2.0/aiida_project/engine/conda.py`

 * *Files identical despite different names*

### Comparing `aiida-project-0.1.0/aiida_project/engine/virtualenv.py` & `aiida-project-0.2.0/aiida_project/engine/virtualenv.py`

 * *Files identical despite different names*

### Comparing `aiida-project-0.1.0/pyproject.toml` & `aiida-project-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-project-0.1.0/PKG-INFO` & `aiida-project-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-project
-Version: 0.1.0
+Version: 0.2.0
 Summary: An AiiDA environment manager
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: AiiDA
```

