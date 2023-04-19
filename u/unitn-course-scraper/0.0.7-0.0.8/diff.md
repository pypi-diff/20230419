# Comparing `tmp/unitn_course_scraper-0.0.7.tar.gz` & `tmp/unitn_course_scraper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitn_course_scraper-0.0.7.tar", last modified: Wed Apr 19 07:55:46 2023, max compression
+gzip compressed data, was "unitn_course_scraper-0.0.8.tar", last modified: Wed Apr 19 08:00:18 2023, max compression
```

## Comparing `unitn_course_scraper-0.0.7.tar` & `unitn_course_scraper-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 07:55:46.302885 unitn_course_scraper-0.0.7/
--rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.0.7/LICENSE
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 07:55:46.302736 unitn_course_scraper-0.0.7/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.0.7/README.md
--rw-r--r--   0 matte      (501) staff       (20)      977 2023-04-19 07:51:48.000000 unitn_course_scraper-0.0.7/pyproject.toml
--rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 07:55:46.302929 unitn_course_scraper-0.0.7/setup.cfg
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 07:55:46.300822 unitn_course_scraper-0.0.7/src/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.0.7/src/__init__.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 07:55:46.301020 unitn_course_scraper-0.0.7/src/cli/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.7/src/cli/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     2165 2023-04-19 07:49:54.000000 unitn_course_scraper-0.0.7/src/cli/cli.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 07:55:46.301483 unitn_course_scraper-0.0.7/src/login/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.7/src/login/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     6395 2023-04-19 07:50:02.000000 unitn_course_scraper-0.0.7/src/login/login.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 07:55:46.301728 unitn_course_scraper-0.0.7/src/scraping/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.7/src/scraping/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.7/src/scraping/scraper.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 07:55:46.302516 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 07:55:46.000000 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      463 2023-04-19 07:55:46.000000 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 07:55:46.000000 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 matte      (501) staff       (20)       45 2023-04-19 07:55:46.000000 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/entry_points.txt
--rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 07:55:46.000000 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/requires.txt
--rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 07:55:46.000000 unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:00:18.204221 unitn_course_scraper-0.0.8/
+-rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.0.8/LICENSE
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 08:00:18.204067 unitn_course_scraper-0.0.8/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.0.8/README.md
+-rw-r--r--   0 matte      (501) staff       (20)      977 2023-04-19 08:00:11.000000 unitn_course_scraper-0.0.8/pyproject.toml
+-rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 08:00:18.204267 unitn_course_scraper-0.0.8/setup.cfg
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:00:18.202174 unitn_course_scraper-0.0.8/src/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.0.8/src/__init__.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:00:18.202376 unitn_course_scraper-0.0.8/src/cli/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.8/src/cli/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     2165 2023-04-19 07:49:54.000000 unitn_course_scraper-0.0.8/src/cli/cli.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:00:18.202763 unitn_course_scraper-0.0.8/src/login/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.8/src/login/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     6395 2023-04-19 07:50:02.000000 unitn_course_scraper-0.0.8/src/login/login.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:00:18.203000 unitn_course_scraper-0.0.8/src/scraping/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.8/src/scraping/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.8/src/scraping/scraper.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:00:18.203825 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 08:00:18.000000 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      463 2023-04-19 08:00:18.000000 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 08:00:18.000000 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 matte      (501) staff       (20)       45 2023-04-19 08:00:18.000000 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 08:00:18.000000 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/requires.txt
+-rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 08:00:18.000000 unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/top_level.txt
```

### Comparing `unitn_course_scraper-0.0.7/LICENSE` & `unitn_course_scraper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.7/PKG-INFO` & `unitn_course_scraper-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn_course_scraper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unitn_course_scraper-0.0.7/README.md` & `unitn_course_scraper-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.7/pyproject.toml` & `unitn_course_scraper-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='unitn_course_scraper'
-version='0.0.7'
+version='0.0.8'
 authors=[
     { name="DISI Drive Team", email="unitndrive@gmail.com" }
 ]
 description='Interactive scraper for your UniTN courses'
 readme='README.md'
 requires-python=">=3.7"
 classifiers=["Programming Language :: Python :: 3.7",
```

### Comparing `unitn_course_scraper-0.0.7/src/cli/cli.py` & `unitn_course_scraper-0.0.8/src/cli/cli.py`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.7/src/login/login.py` & `unitn_course_scraper-0.0.8/src/login/login.py`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.7/src/unitn_course_scraper.egg-info/PKG-INFO` & `unitn_course_scraper-0.0.8/src/unitn_course_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn-course-scraper
-Version: 0.0.7
+Version: 0.0.8
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

