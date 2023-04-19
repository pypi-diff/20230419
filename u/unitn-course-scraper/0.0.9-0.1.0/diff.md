# Comparing `tmp/unitn_course_scraper-0.0.9.tar.gz` & `tmp/unitn_course_scraper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitn_course_scraper-0.0.9.tar", last modified: Wed Apr 19 08:06:14 2023, max compression
+gzip compressed data, was "unitn_course_scraper-0.1.0.tar", last modified: Wed Apr 19 08:16:44 2023, max compression
```

## Comparing `unitn_course_scraper-0.0.9.tar` & `unitn_course_scraper-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:06:14.975157 unitn_course_scraper-0.0.9/
--rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.0.9/LICENSE
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 08:06:14.974994 unitn_course_scraper-0.0.9/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.0.9/README.md
--rw-r--r--   0 matte      (501) staff       (20)      930 2023-04-19 08:06:00.000000 unitn_course_scraper-0.0.9/pyproject.toml
--rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 08:06:14.975197 unitn_course_scraper-0.0.9/setup.cfg
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:06:14.973196 unitn_course_scraper-0.0.9/src/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.0.9/src/__init__.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:06:14.973428 unitn_course_scraper-0.0.9/src/cli/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.9/src/cli/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     2165 2023-04-19 07:49:54.000000 unitn_course_scraper-0.0.9/src/cli/cli.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:06:14.973929 unitn_course_scraper-0.0.9/src/login/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.9/src/login/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     6395 2023-04-19 07:50:02.000000 unitn_course_scraper-0.0.9/src/login/login.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:06:14.974178 unitn_course_scraper-0.0.9/src/scraping/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.9/src/scraping/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.0.9/src/scraping/scraper.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:06:14.974805 unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 08:06:14.000000 unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      412 2023-04-19 08:06:14.000000 unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 08:06:14.000000 unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 08:06:14.000000 unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/requires.txt
--rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 08:06:14.000000 unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:16:44.164741 unitn_course_scraper-0.1.0/
+-rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.1.0/LICENSE
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 08:16:44.164564 unitn_course_scraper-0.1.0/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.1.0/README.md
+-rw-r--r--   0 matte      (501) staff       (20)      929 2023-04-19 08:10:24.000000 unitn_course_scraper-0.1.0/pyproject.toml
+-rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 08:16:44.164787 unitn_course_scraper-0.1.0/setup.cfg
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:16:44.162577 unitn_course_scraper-0.1.0/src/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.1.0/src/__init__.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:16:44.162789 unitn_course_scraper-0.1.0/src/cli/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.0/src/cli/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     2165 2023-04-19 07:49:54.000000 unitn_course_scraper-0.1.0/src/cli/cli.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:16:44.163168 unitn_course_scraper-0.1.0/src/login/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.0/src/login/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     6395 2023-04-19 07:50:02.000000 unitn_course_scraper-0.1.0/src/login/login.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:16:44.163512 unitn_course_scraper-0.1.0/src/scraping/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.0/src/scraping/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.0/src/scraping/scraper.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 08:16:44.164237 unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 08:16:44.000000 unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      412 2023-04-19 08:16:44.000000 unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 08:16:44.000000 unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 08:16:44.000000 unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/requires.txt
+-rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 08:16:44.000000 unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/top_level.txt
```

### Comparing `unitn_course_scraper-0.0.9/LICENSE` & `unitn_course_scraper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.9/PKG-INFO` & `unitn_course_scraper-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn_course_scraper
-Version: 0.0.9
+Version: 0.1.0
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unitn_course_scraper-0.0.9/README.md` & `unitn_course_scraper-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.9/pyproject.toml` & `unitn_course_scraper-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='unitn_course_scraper'
-version='0.0.9'
+version='0.1.0'
 authors=[
     { name="DISI Drive Team", email="unitndrive@gmail.com" }
 ]
 description='Interactive scraper for your UniTN courses'
 readme='README.md'
 requires-python=">=3.7"
 classifiers=["Programming Language :: Python :: 3.7",
@@ -16,8 +16,8 @@
                 "Programming Language :: Python :: 3.9",
                 "Programming Language :: Python :: 3.10",
                 "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
                 "Operating System :: OS Independent",
                 ]
 keywords=['unitn', 'courses', 'scraper', '@unitn.it',
               'moodle', 'dol', 'gestionecorsi', 'didatticaonline']
-dependencies=['python-dotenv >= 1.0.0', 'requests >= 2.28.2', 'grequests >= 0.6.0', 'beautifulsoup4 >= 4.12.2']
+dependencies=['python-dotenv >= 1.0.0', 'requests >= 2.28.2', 'grequests >= 0.6.0', 'beautifulsoup4 >= 4.12.2']
```

### Comparing `unitn_course_scraper-0.0.9/src/cli/cli.py` & `unitn_course_scraper-0.1.0/src/cli/cli.py`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.9/src/login/login.py` & `unitn_course_scraper-0.1.0/src/login/login.py`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.0.9/src/unitn_course_scraper.egg-info/PKG-INFO` & `unitn_course_scraper-0.1.0/src/unitn_course_scraper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn-course-scraper
-Version: 0.0.9
+Version: 0.1.0
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

