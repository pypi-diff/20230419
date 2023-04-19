# Comparing `tmp/unitn_course_scraper-0.1.5.tar.gz` & `tmp/unitn_course_scraper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitn_course_scraper-0.1.5.tar", last modified: Wed Apr 19 09:42:33 2023, max compression
+gzip compressed data, was "unitn_course_scraper-0.1.6.tar", last modified: Wed Apr 19 11:15:08 2023, max compression
```

## Comparing `unitn_course_scraper-0.1.5.tar` & `unitn_course_scraper-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.990900 unitn_course_scraper-0.1.5/
--rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.1.5/LICENSE
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:42:33.990769 unitn_course_scraper-0.1.5/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.1.5/README.md
--rw-r--r--   0 matte      (501) staff       (20)      993 2023-04-19 09:42:26.000000 unitn_course_scraper-0.1.5/pyproject.toml
--rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 09:42:33.990939 unitn_course_scraper-0.1.5/setup.cfg
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.988988 unitn_course_scraper-0.1.5/src/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.1.5/src/__init__.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.989385 unitn_course_scraper-0.1.5/src/cli/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/cli/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     2459 2023-04-19 09:42:04.000000 unitn_course_scraper-0.1.5/src/cli/cli.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.989627 unitn_course_scraper-0.1.5/src/login/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/login/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     6586 2023-04-19 09:29:20.000000 unitn_course_scraper-0.1.5/src/login/login.py
--rw-r--r--   0 matte      (501) staff       (20)       76 2023-04-19 09:42:04.000000 unitn_course_scraper-0.1.5/src/main.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.989840 unitn_course_scraper-0.1.5/src/scraping/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/scraping/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.5/src/scraping/scraper.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:42:33.990596 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      475 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 matte      (501) staff       (20)       60 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/entry_points.txt
--rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/requires.txt
--rw-r--r--   0 matte      (501) staff       (20)       33 2023-04-19 09:42:33.000000 unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-19 11:15:08.304208 unitn_course_scraper-0.1.6/
+-rw-r--r--   0 marco     (1000) marco     (1000)    34888 2023-04-18 15:44:04.000000 unitn_course_scraper-0.1.6/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     1303 2023-04-19 11:15:08.304208 unitn_course_scraper-0.1.6/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      640 2023-04-18 15:44:04.000000 unitn_course_scraper-0.1.6/README.md
+-rw-r--r--   0 marco     (1000) marco     (1000)      993 2023-04-19 11:13:34.000000 unitn_course_scraper-0.1.6/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-19 11:15:08.304208 unitn_course_scraper-0.1.6/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-19 11:15:08.300874 unitn_course_scraper-0.1.6/src/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-18 15:44:04.000000 unitn_course_scraper-0.1.6/src/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-19 11:15:08.300874 unitn_course_scraper-0.1.6/src/cli/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-18 15:56:07.000000 unitn_course_scraper-0.1.6/src/cli/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2573 2023-04-19 11:11:21.000000 unitn_course_scraper-0.1.6/src/cli/cli.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-19 11:15:08.304208 unitn_course_scraper-0.1.6/src/login/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-18 16:29:13.000000 unitn_course_scraper-0.1.6/src/login/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     6573 2023-04-19 11:11:21.000000 unitn_course_scraper-0.1.6/src/login/login.py
+-rw-r--r--   0 marco     (1000) marco     (1000)       76 2023-04-19 10:11:41.000000 unitn_course_scraper-0.1.6/src/main.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-19 11:15:08.304208 unitn_course_scraper-0.1.6/src/scraping/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-18 15:56:07.000000 unitn_course_scraper-0.1.6/src/scraping/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-18 15:56:07.000000 unitn_course_scraper-0.1.6/src/scraping/scraper.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-19 11:15:08.304208 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1303 2023-04-19 11:15:08.000000 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      475 2023-04-19 11:15:08.000000 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-19 11:15:08.000000 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       60 2023-04-19 11:15:08.000000 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       78 2023-04-19 11:15:08.000000 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       33 2023-04-19 11:15:08.000000 unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/top_level.txt
```

### Comparing `unitn_course_scraper-0.1.5/LICENSE` & `unitn_course_scraper-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.5/PKG-INFO` & `unitn_course_scraper-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn_course_scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unitn_course_scraper-0.1.5/README.md` & `unitn_course_scraper-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.5/pyproject.toml` & `unitn_course_scraper-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='unitn_course_scraper'
-version='0.1.5'
+version='0.1.6'
 authors=[
     { name="DISI Drive Team", email="unitndrive@gmail.com" }
 ]
 description='Interactive scraper for your UniTN courses'
 readme='README.md'
 requires-python=">=3.7"
 classifiers=["Programming Language :: Python :: 3.7",
```

### Comparing `unitn_course_scraper-0.1.5/src/cli/cli.py` & `unitn_course_scraper-0.1.6/src/cli/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from login.login import login
 from login.login import input
 from login.login import get_attended_courses
 from login.login import get_available_courses
+from login.login import saveJSON
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='A python program to scrape unitn courses and store resources in a local folder')
 
     parser.add_argument(
@@ -48,14 +49,14 @@
 
     username, password = input(
         env=args.env
     )
     session, Bearer_auth, tokenRelayState, tokenSAMLResponse, data = login(
         username, password)
 
-    print("ATTENDED COURSES")
-
-    print(get_attended_courses(session, Bearer_auth))
-
-    print("AVAILABLE COURSES")
-
-    print(get_available_courses(session, Bearer_auth))
+    # if args.list_enrolled:
+    #     print("ATTENDED COURSES")
+    #     print(get_attended_courses(session, Bearer_auth))
+
+    # if args.list_available:
+    #     print("AVAILABLE COURSES")
+    #     print(get_available_courses(session, Bearer_auth))
```

### Comparing `unitn_course_scraper-0.1.5/src/login/login.py` & `unitn_course_scraper-0.1.6/src/login/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 
 # clean json courses list
 
 
 def clean_json_list(json_list):
     # removing multi language substring and setting url of each course
     for i in json_list:
-        if 'id' not in i['urlMoodle']:
+        if 'target=' not in i['urlMoodle']:
             json_list.remove(i)
         else:
             if '{mlang other}' in i['fullName']:
                 i['fullName'] = i['fullName'].split('{mlang other}', 1)[
                     1].split('{mlang}', 1)[0]
-
             i['url'] = i['urlMoodle'].split('target=', 1)[1]
 
     return json_list
 
 # function to save HTML text to a file
 
 
@@ -152,15 +151,15 @@
 
 def get_available_courses(session, auth):
     url = 'https://webapps.unitn.it/api/gestionecorsi/v1/studente/possibilicorsi/'
     headers = {'Authorization': auth}
     res = session.get(url, headers=headers, allow_redirects=True)
     # output list of courses
     json_list = res.json()
-    return clean_json_list(json_list)
+    return json_list
 
 
 # get course content
 def get_course_content(session, auth, url):
     res = session.get(
         url, headers={'Authorization': auth}, allow_redirects=True)
     return True
```

### Comparing `unitn_course_scraper-0.1.5/src/unitn_course_scraper.egg-info/PKG-INFO` & `unitn_course_scraper-0.1.6/src/unitn_course_scraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitn-course-scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

