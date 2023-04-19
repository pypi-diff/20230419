# Comparing `tmp/pd_db_wrangler-0.8.0.tar.gz` & `tmp/pd_db_wrangler-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pd_db_wrangler-0.8.0.tar", last modified: Fri Sep 25 18:41:49 2020, max compression
+gzip compressed data, was "pd_db_wrangler-0.9.0.tar", last modified: Mon Apr 19 21:25:34 2021, max compression
```

## Comparing `pd_db_wrangler-0.8.0.tar` & `pd_db_wrangler-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-09-25 18:41:49.278706 pd_db_wrangler-0.8.0/
--rw-r--r--   0 justin    (1000) justin    (1000)      166 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/AUTHORS.rst
--rw-r--r--   0 justin    (1000) justin    (1000)     3620 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 justin    (1000) justin    (1000)      644 2020-09-25 18:40:50.000000 pd_db_wrangler-0.8.0/HISTORY.rst
--rw-r--r--   0 justin    (1000) justin    (1000)     1072 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/LICENSE
--rw-r--r--   0 justin    (1000) justin    (1000)      262 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/MANIFEST.in
--rw-r--r--   0 justin    (1000) justin    (1000)     3034 2020-09-25 18:41:49.278706 pd_db_wrangler-0.8.0/PKG-INFO
--rw-r--r--   0 justin    (1000) justin    (1000)      924 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/README.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-09-25 18:41:49.275373 pd_db_wrangler-0.8.0/docs/
--rw-r--r--   0 justin    (1000) justin    (1000)      615 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/Makefile
--rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/authors.rst
--rwxr-xr-x   0 justin    (1000) justin    (1000)     4932 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/conf.py
--rw-r--r--   0 justin    (1000) justin    (1000)       33 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/contributing.rst
--rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/history.rst
--rw-r--r--   0 justin    (1000) justin    (1000)      311 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/index.rst
--rw-r--r--   0 justin    (1000) justin    (1000)     1186 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/installation.rst
--rw-r--r--   0 justin    (1000) justin    (1000)      776 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/make.bat
--rw-r--r--   0 justin    (1000) justin    (1000)       27 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/readme.rst
--rw-r--r--   0 justin    (1000) justin    (1000)       83 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/docs/usage.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-09-25 18:41:49.275373 pd_db_wrangler-0.8.0/pd_db_wrangler/
--rw-r--r--   0 justin    (1000) justin    (1000)      207 2020-09-25 18:37:56.000000 pd_db_wrangler-0.8.0/pd_db_wrangler/__init__.py
--rw-r--r--   0 justin    (1000) justin    (1000)     2408 2020-09-25 18:35:50.000000 pd_db_wrangler-0.8.0/pd_db_wrangler/pd_db_wrangler.py
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-09-25 18:41:49.278706 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/
--rw-r--r--   0 justin    (1000) justin    (1000)     3034 2020-09-25 18:41:49.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/PKG-INFO
--rw-r--r--   0 justin    (1000) justin    (1000)      629 2020-09-25 18:41:49.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/SOURCES.txt
--rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-09-25 18:41:49.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/dependency_links.txt
--rw-r--r--   0 justin    (1000) justin    (1000)       60 2020-09-25 18:41:49.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/entry_points.txt
--rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-09-25 18:39:46.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/not-zip-safe
--rw-r--r--   0 justin    (1000) justin    (1000)       16 2020-09-25 18:41:49.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/requires.txt
--rw-r--r--   0 justin    (1000) justin    (1000)       15 2020-09-25 18:41:49.000000 pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/top_level.txt
--rw-r--r--   0 justin    (1000) justin    (1000)      397 2020-09-25 18:41:49.278706 pd_db_wrangler-0.8.0/setup.cfg
--rw-r--r--   0 justin    (1000) justin    (1000)     1511 2020-09-25 18:38:15.000000 pd_db_wrangler-0.8.0/setup.py
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-09-25 18:41:49.278706 pd_db_wrangler-0.8.0/tests/
--rw-r--r--   0 justin    (1000) justin    (1000)       44 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/tests/__init__.py
--rw-r--r--   0 justin    (1000) justin    (1000)      901 2020-09-25 17:57:30.000000 pd_db_wrangler-0.8.0/tests/test_pd_db_wrangler.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-04-19 21:25:34.219679 pd_db_wrangler-0.9.0/
+-rw-r--r--   0 justin    (1000) justin    (1000)      166 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/AUTHORS.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)     3620 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)      644 2020-09-25 18:40:50.000000 pd_db_wrangler-0.9.0/HISTORY.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)     1072 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/LICENSE
+-rw-r--r--   0 justin    (1000) justin    (1000)      262 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/MANIFEST.in
+-rw-r--r--   0 justin    (1000) justin    (1000)     3034 2021-04-19 21:25:34.219679 pd_db_wrangler-0.9.0/PKG-INFO
+-rw-r--r--   0 justin    (1000) justin    (1000)      924 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/README.rst
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-04-19 21:25:34.216346 pd_db_wrangler-0.9.0/docs/
+-rw-r--r--   0 justin    (1000) justin    (1000)      615 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/Makefile
+-rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/authors.rst
+-rwxr-xr-x   0 justin    (1000) justin    (1000)     4932 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/conf.py
+-rw-r--r--   0 justin    (1000) justin    (1000)       33 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/contributing.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)       28 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/history.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)      311 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/index.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)     1186 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/installation.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)      776 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/make.bat
+-rw-r--r--   0 justin    (1000) justin    (1000)       27 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/readme.rst
+-rw-r--r--   0 justin    (1000) justin    (1000)       83 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/docs/usage.rst
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-04-19 21:25:34.216346 pd_db_wrangler-0.9.0/pd_db_wrangler/
+-rw-r--r--   0 justin    (1000) justin    (1000)      207 2021-04-19 21:24:30.000000 pd_db_wrangler-0.9.0/pd_db_wrangler/__init__.py
+-rw-r--r--   0 justin    (1000) justin    (1000)     2509 2021-04-19 21:16:12.000000 pd_db_wrangler-0.9.0/pd_db_wrangler/pd_db_wrangler.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-04-19 21:25:34.219679 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/
+-rw-r--r--   0 justin    (1000) justin    (1000)     3034 2021-04-19 21:25:34.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/PKG-INFO
+-rw-r--r--   0 justin    (1000) justin    (1000)      629 2021-04-19 21:25:34.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/SOURCES.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)        1 2021-04-19 21:25:34.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/dependency_links.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)       60 2021-04-19 21:25:34.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/entry_points.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-09-25 18:39:46.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/not-zip-safe
+-rw-r--r--   0 justin    (1000) justin    (1000)       16 2021-04-19 21:25:34.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/requires.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)       15 2021-04-19 21:25:34.000000 pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/top_level.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)      381 2021-04-19 21:25:34.219679 pd_db_wrangler-0.9.0/setup.cfg
+-rw-r--r--   0 justin    (1000) justin    (1000)     1511 2021-04-19 21:24:30.000000 pd_db_wrangler-0.9.0/setup.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2021-04-19 21:25:34.219679 pd_db_wrangler-0.9.0/tests/
+-rw-r--r--   0 justin    (1000) justin    (1000)       44 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/tests/__init__.py
+-rw-r--r--   0 justin    (1000) justin    (1000)      901 2020-09-25 17:57:30.000000 pd_db_wrangler-0.9.0/tests/test_pd_db_wrangler.py
```

### Comparing `pd_db_wrangler-0.8.0/CONTRIBUTING.rst` & `pd_db_wrangler-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/HISTORY.rst` & `pd_db_wrangler-0.9.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/LICENSE` & `pd_db_wrangler-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/PKG-INFO` & `pd_db_wrangler-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pd_db_wrangler
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pandas database helper library
 Home-page: https://github.com/kellerjustin/pd_db_wrangler
 Author: Justin Keller
 Author-email: kellerjustin@protonmail.com
 License: MIT license
 Description: ==============
         PD DB Wrangler
```

### Comparing `pd_db_wrangler-0.8.0/README.rst` & `pd_db_wrangler-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/docs/Makefile` & `pd_db_wrangler-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/docs/conf.py` & `pd_db_wrangler-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/docs/installation.rst` & `pd_db_wrangler-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/docs/make.bat` & `pd_db_wrangler-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/pd_db_wrangler/pd_db_wrangler.py` & `pd_db_wrangler-0.9.0/pd_db_wrangler/pd_db_wrangler.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,20 @@
         host='127.0.0.1' dbname=db user=user1 password='p@ssW0rD!'
         A sqlite connection is a file path, so it may look like
         '/path/to/sqlite.db'
         db_type must be set in order to use the df_fetch function
         valid db_types presently implemented: 'postgres', 'sqlite'
         """
         self.DB_TYPE = db_type.lower()
-        with open(filename, "r") as f:
-            self.CONNECT_STRING = f.readline().rstrip()
-            return self.CONNECT_STRING
+        if self.DB_TYPE == "postgres":
+            with open(filename, "r") as f:
+                self.CONNECT_STRING = f.readline().rstrip()
+        else:
+            self.CONNECT_STRING == filename
+        return self.CONNECT_STRING
 
     def read_text_file(self, filename):
         """ Read Text from File """
         with open(filename, "r", encoding='utf-8-sig') as myfile:
             text = myfile.read()
             myfile.close()
         return text
```

### Comparing `pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/PKG-INFO` & `pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pd-db-wrangler
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pandas database helper library
 Home-page: https://github.com/kellerjustin/pd_db_wrangler
 Author: Justin Keller
 Author-email: kellerjustin@protonmail.com
 License: MIT license
 Description: ==============
         PD DB Wrangler
```

### Comparing `pd_db_wrangler-0.8.0/pd_db_wrangler.egg-info/SOURCES.txt` & `pd_db_wrangler-0.9.0/pd_db_wrangler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pd_db_wrangler-0.8.0/setup.py` & `pd_db_wrangler-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,10 +43,10 @@
     keywords="pd_db_wrangler",
     name="pd_db_wrangler",
     packages=find_packages(include=["pd_db_wrangler", "pd_db_wrangler.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/kellerjustin/pd_db_wrangler",
-    version="0.8.0",
+    version="0.9.0",
     zip_safe=False,
 )
```

### Comparing `pd_db_wrangler-0.8.0/tests/test_pd_db_wrangler.py` & `pd_db_wrangler-0.9.0/tests/test_pd_db_wrangler.py`

 * *Files identical despite different names*

