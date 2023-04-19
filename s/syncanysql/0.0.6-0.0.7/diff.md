# Comparing `tmp/syncanysql-0.0.6.tar.gz` & `tmp/syncanysql-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.0.6.tar", last modified: Sat Apr  1 08:27:36 2023, max compression
+gzip compressed data, was "syncanysql-0.0.7.tar", last modified: Wed Apr 19 09:46:19 2023, max compression
```

## Comparing `syncanysql-0.0.6.tar` & `syncanysql-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-01 08:27:36.517749 syncanysql-0.0.6/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.6/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-01 08:27:36.520751 syncanysql-0.0.6/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2645 2023-03-29 06:12:04.000000 syncanysql-0.0.6/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-01 08:27:36.530750 syncanysql-0.0.6/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-03-30 01:43:52.000000 syncanysql-0.0.6/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-01 08:27:35.172904 syncanysql-0.0.6/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.6/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-01 08:27:35.594733 syncanysql-0.0.6/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.6/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.6/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      869 2023-03-23 03:17:03.000000 syncanysql-0.0.6/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-01 08:27:35.943768 syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7462 2023-03-03 09:07:45.000000 syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5978 2023-03-14 10:29:03.000000 syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1442 2023-03-02 09:37:13.000000 syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3352 2023-03-02 09:57:08.000000 syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   119265 2023-04-01 04:07:42.000000 syncanysql-0.0.6/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.6/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.6/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.6/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.6/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.6/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7229 2023-03-13 06:34:00.000000 syncanysql-0.0.6/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-01 08:27:36.473750 syncanysql-0.0.6/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.6/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.6/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.6/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.6/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.6/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.6/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.6/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.6/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.6/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.6/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-03-30 01:42:51.000000 syncanysql-0.0.6/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-01 08:27:35.425907 syncanysql-0.0.6/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-01 08:27:33.000000 syncanysql-0.0.6/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-01 08:27:34.000000 syncanysql-0.0.6/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-01 08:27:33.000000 syncanysql-0.0.6/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-01 08:27:33.000000 syncanysql-0.0.6/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.6/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-01 08:27:33.000000 syncanysql-0.0.6/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-01 08:27:33.000000 syncanysql-0.0.6/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.974063 syncanysql-0.0.7/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.0.7/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-19 09:46:19.976065 syncanysql-0.0.7/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2645 2023-03-29 06:12:04.000000 syncanysql-0.0.7/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-19 09:46:19.985341 syncanysql-0.0.7/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2011 2023-04-19 08:35:52.000000 syncanysql-0.0.7/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:18.607060 syncanysql-0.0.7/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8404 2023-03-29 07:10:45.000000 syncanysql-0.0.7/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.057426 syncanysql-0.0.7/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1050 2023-03-25 04:42:07.000000 syncanysql-0.0.7/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.0.7/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      975 2023-04-19 08:11:25.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.392873 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8741 2023-04-19 07:56:30.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5980 2023-04-19 07:56:30.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5340 2023-04-19 08:22:16.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4221 2023-04-19 08:31:29.000000 syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   119772 2023-04-19 08:03:18.000000 syncanysql-0.0.7/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12011 2023-03-27 03:03:08.000000 syncanysql-0.0.7/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.0.7/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7245 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3590 2023-03-25 04:39:43.000000 syncanysql-0.0.7/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.0.7/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7259 2023-04-19 08:39:44.000000 syncanysql-0.0.7/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:19.925892 syncanysql-0.0.7/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.0.7/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1513 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1394 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3519 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18357 2023-03-29 02:07:07.000000 syncanysql-0.0.7/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2744 2023-03-29 02:07:49.000000 syncanysql-0.0.7/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1173 2023-03-29 02:06:08.000000 syncanysql-0.0.7/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      641 2023-02-19 14:49:39.000000 syncanysql-0.0.7/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-04-19 08:35:52.000000 syncanysql-0.0.7/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-19 09:46:18.891060 syncanysql-0.0.7/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3908 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1119 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-02-25 12:53:08.000000 syncanysql-0.0.7/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      407 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-04-19 09:46:17.000000 syncanysql-0.0.7/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.0.6/LICENSE` & `syncanysql-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/PKG-INFO` & `syncanysql-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
```

### Comparing `syncanysql-0.0.6/README.md` & `syncanysql-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/setup.py` & `syncanysql-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.6"
+version = "0.0.7"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=10.6.2",
-        "syncany>=0.2.3",
+        "syncany>=0.2.4",
         'Pygments>=2.14.0',
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
```

### Comparing `syncanysql-0.0.6/syncanysql/__init__.py` & `syncanysql-0.0.7/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/calculaters/__init__.py` & `syncanysql-0.0.7/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.0.7/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.0.7/syncanysql/calculaters/mysql_calculater.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 from syncany.calculaters.calculater import Calculater
 from . import mysql_funcs
 
 
 class MysqlCalculater(Calculater):
     funcs = mysql_funcs.funcs
 
+    def __init__(self, *args, **kwargs):
+        super(MysqlCalculater, self).__init__(*args, **kwargs)
+
+        self.func = self.funcs.get(self.name[7:])
+
     def calculate(self, *args):
-        func_name = self.name[7:]
         try:
             if len(args) == 1 and isinstance(args[0], list) and args[0] and isinstance(args[0][0], dict):
                 try:
-                    self.funcs[func_name](*tuple(args[0]))
+                    self.func(*tuple(args[0]))
                 except TypeError:
                     pass
-            return self.funcs[func_name](*args)
+            return self.func(*args)
         except Exception as e:
-            get_logger().warning("mysql calculater execute %s(%s) error: %s\n%s", func_name, args, e,
+            get_logger().warning("mysql calculater execute %s(%s) error: %s\n%s", self.name[7:], args, e,
                                  traceback.format_exc())
             return None
```

### Comparing `syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,47 @@
 def mysql_currenttime():
     dt = datetime.datetime.now(tz=get_timezone())
     return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
 
 def mysql_sysdate():
     return datetime.datetime.now(tz=get_timezone())
 
+def mysql_date(dt):
+    if isinstance(dt, str):
+        dt = parse_datetime(dt, None, get_timezone())
+    if isinstance(dt, datetime.datetime):
+        return datetime.date(dt.year, dt.month, dt.day)
+    if isinstance(dt, datetime.date):
+        return dt
+    return None
+
+def mysql_datetime(dt):
+    if isinstance(dt, str):
+        dt = parse_datetime(dt, None, get_timezone())
+    if isinstance(dt, datetime.datetime):
+        return dt
+    if isinstance(dt, datetime.date):
+        return datetime.datetime(dt.year, dt.month, dt.day, tzinfo=get_timezone())
+    if isinstance(dt, datetime.time):
+        now = datetime.datetime.now(tz=get_timezone())
+        return datetime.datetime(now.year, now.month, now.day, dt.hour, dt.minute,
+                                 dt.second, dt.microsecond, tzinfo=get_timezone())
+    return None
+
+def mysql_time(dt):
+    if isinstance(dt, str):
+        dt = parse_datetime(dt, None, get_timezone())
+    if isinstance(dt, datetime.time):
+        return dt
+    if isinstance(dt, datetime.datetime):
+        return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond, tzinfo=get_timezone())
+    if isinstance(dt, datetime.date):
+        return datetime.time(tzinfo=get_timezone())
+    return None
+
 def mysql_unix_timestamp(dt=None):
     if dt is None:
         return int(time.time())
     return int(time.mktime(dt.utctimetuple()))
 
 def mysql_from_unixtime(t):
     return datetime.datetime.utcfromtimestamp(t).replace(tzinfo=pytz.UTC).astimezone(tz=get_timezone())
@@ -201,8 +234,9 @@
     dt = datetime.datetime.utcnow()
     return datetime.time(dt.hour, dt.minute, dt.second, dt.microsecond)
 
 def mysql_utc_timestamp():
     dt = datetime.datetime.utcnow()
     return dt.replace(tzinfo=pytz.UTC)
 
-funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
+
+funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
```

### Comparing `syncanysql-0.0.6/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.0.7/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -181,8 +181,8 @@
             json.loads(val)
             return 1
         except:
             return 0
     return 1
 
 
-funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
+funcs = {key[6:]: value for key, value in globals().items() if key.startswith("mysql_")}
```

### Comparing `syncanysql-0.0.6/syncanysql/compiler.py` & `syncanysql-0.0.7/syncanysql/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1018,19 +1018,26 @@
             else:
                 typing_filter = None
             value_column = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             if typing_filter:
                 return ["#if", ["#const", True], value_column, None, ":$.*|" + typing_filter]
             return value_column
         elif isinstance(expression, sqlglot_expressions.Binary):
+            func_name = expression.key.lower()
             return [
-                "@" + expression.key.lower(),
+                ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
                 self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
             ]
+        elif isinstance(expression, sqlglot_expressions.BitwiseNot):
+            func_name = expression.key.lower()
+            return [
+                ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
+                self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
+            ]
         elif isinstance(expression, sqlglot_expressions.If):
             return [
                 "#if",
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
                 self.compile_calculate(expression.args["true"], config, arguments, primary_table, column_join_tables, 
                                        join_index) if expression.args.get("true") else False,
                 self.compile_calculate(expression.args["false"], config, arguments, primary_table, column_join_tables, 
@@ -1778,15 +1785,15 @@
         return isinstance(expression, (sqlglot_expressions.Literal, sqlglot_expressions.Boolean,
                                        sqlglot_expressions.Null, sqlglot_expressions.HexString, sqlglot_expressions.BitString,
                                        sqlglot_expressions.ByteString, sqlglot_expressions.Parameter))
 
     def is_calculate(self, expression, config, arguments):
         return isinstance(expression, (sqlglot_expressions.Neg, sqlglot_expressions.Anonymous, sqlglot_expressions.Binary, sqlglot_expressions.Func,
                                        sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union, sqlglot_expressions.Not,
-                                       sqlglot_expressions.Tuple))
+                                       sqlglot_expressions.BitwiseNot, sqlglot_expressions.Tuple))
 
     def is_aggregate(self, expression, config, arguments):
         if isinstance(expression, (sqlglot_expressions.Count, sqlglot_expressions.Sum, sqlglot_expressions.Max,
                                        sqlglot_expressions.Min, sqlglot_expressions.Avg)):
             return True
         if isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
```

### Comparing `syncanysql-0.0.6/syncanysql/config.py` & `syncanysql-0.0.7/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/executor.py` & `syncanysql-0.0.7/syncanysql/executor.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/main.py` & `syncanysql-0.0.7/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/parser.py` & `syncanysql-0.0.7/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/prompt.py` & `syncanysql-0.0.7/syncanysql/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                     lineno += 1
                     self.executor.runners.clear()
             except KeyboardInterrupt:
                 continue  # Control-C pressed. Try again.
             except EOFError:
                 return 130
             except Exception as e:
-                print(str(e))
+                print(e.__class__.__name__ + ": " + str(e))
         return 0
 
     def check_complete(self, content):
         content = content.strip()
         if not content or content[:4] == "exit" or content[0] in ("!", "%"):
             return False
         sql_parser = SqlParser(content)
```

### Comparing `syncanysql-0.0.6/syncanysql/taskers/delete.py` & `syncanysql-0.0.7/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/execute.py` & `syncanysql-0.0.7/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/explain.py` & `syncanysql-0.0.7/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/into.py` & `syncanysql-0.0.7/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/query.py` & `syncanysql-0.0.7/syncanysql/taskers/query.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/set.py` & `syncanysql-0.0.7/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/show.py` & `syncanysql-0.0.7/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/taskers/use.py` & `syncanysql-0.0.7/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql/utils.py` & `syncanysql-0.0.7/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.0.6/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.0.7/syncanysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
```

### Comparing `syncanysql-0.0.6/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.0.7/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

