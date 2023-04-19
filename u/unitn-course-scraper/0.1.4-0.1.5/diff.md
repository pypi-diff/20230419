# Comparing `tmp/unitn_course_scraper-0.1.4.tar.gz` & `tmp/unitn_course_scraper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitn_course_scraper-0.1.4.tar", last modified: Wed Apr 19 09:41:25 2023, max compression
+gzip compressed data, was "unitn_course_scraper-0.1.5.tar", last modified: Wed Apr 19 09:42:33 2023, max compression
```

## Comparing `unitn_course_scraper-0.1.4.tar` & `unitn_course_scraper-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:41:25.755207 unitn_course_scraper-0.1.4/
--rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.1.4/LICENSE
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:41:25.755052 unitn_course_scraper-0.1.4/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.1.4/README.md
--rw-r--r--   0 matte      (501) staff       (20)      993 2023-04-19 09:41:18.000000 unitn_course_scraper-0.1.4/pyproject.toml
--rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 09:41:25.755254 unitn_course_scraper-0.1.4/setup.cfg
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:41:25.753098 unitn_course_scraper-0.1.4/src/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.1.4/src/__init__.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:41:25.753303 unitn_course_scraper-0.1.4/src/cli/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.4/src/cli/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     2475 2023-04-19 09:29:20.000000 unitn_course_scraper-0.1.4/src/cli/cli.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:41:25.753559 unitn_course_scraper-0.1.4/src/login/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.4/src/login/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     6586 2023-04-19 09:29:20.000000 unitn_course_scraper-0.1.4/src/login/login.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:41:25.753849 unitn_course_scraper-0.1.4/src/scraping/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.4/src/scraping/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.4/src/scraping/scraper.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:41:25.754851 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:41:25.000000 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      463 2023-04-19 09:41:25.000000 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 09:41:25.000000 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 matte      (501) staff       (20)       60 2023-04-19 09:41:25.000000 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/entry_points.txt
--rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 09:41:25.000000 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/requires.txt
--rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 09:41:25.000000 unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.990900 unitn_course_scraper-0.1.5/
+-rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.1.5/LICENSE
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:42:33.990769 unitn_course_scraper-0.1.5/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.1.5/README.md
+-rw-r--r--   0 matte      (501) staff       (20)      993 2023-04-19 09:42:26.000000 unitn_course_scraper-0.1.5/pyproject.toml
+-rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 09:42:33.990939 unitn_course_scraper-0.1.5/setup.cfg
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.988988 unitn_course_scraper-0.1.5/src/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.1.5/src/__init__.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.989385 unitn_course_scraper-0.1.5/src/cli/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/cli/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     2459 2023-04-19 09:42:04.000000 unitn_course_scraper-0.1.5/src/cli/cli.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.989627 unitn_course_scraper-0.1.5/src/login/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/login/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     6586 2023-04-19 09:29:20.000000 unitn_course_scraper-0.1.5/src/login/login.py
+-rw-r--r--   0 matte      (501) staff       (20)       76 2023-04-19 09:42:04.000000 unitn_course_scraper-0.1.5/src/main.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.989840 unitn_course_scraper-0.1.5/src/scraping/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/scraping/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/scraping/scraper.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.990596 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      475 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 matte      (501) staff       (20)       60 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/requires.txt
+-rw-r--r--   0 matte      (501) staff       (20)       33 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/top_level.txt
```

### Comparing `unitn_course_scraper-0.1.4/LICENSE` & `unitn_course_scraper-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.4/PKG-INFO` & `unitn_course_scraper-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn_course_scraper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unitn_course_scraper-0.1.4/README.md` & `unitn_course_scraper-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.4/pyproject.toml` & `unitn_course_scraper-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='unitn_course_scraper'
-version='0.1.4'
+version='0.1.5'
 authors=[
     { name="DISI Drive Team", email="unitndrive@gmail.com" }
 ]
 description='Interactive scraper for your UniTN courses'
 readme='README.md'
 requires-python=">=3.7"
 classifiers=["Programming Language :: Python :: 3.7",
```

### Comparing `unitn_course_scraper-0.1.4/src/cli/cli.py` & `unitn_course_scraper-0.1.5/src/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
-from src.login.login import login
-from src.login.login import input
-from src.login.login import get_attended_courses
-from src.login.login import get_available_courses
+from login.login import login
+from login.login import input
+from login.login import get_attended_courses
+from login.login import get_available_courses
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='A python program to scrape unitn courses and store resources in a local folder')
 
     parser.add_argument(
```

### Comparing `unitn_course_scraper-0.1.4/src/login/login.py` & `unitn_course_scraper-0.1.5/src/login/login.py`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.4/src/unitn_course_scraper.egg-info/PKG-INFO` & `unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn-course-scraper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

