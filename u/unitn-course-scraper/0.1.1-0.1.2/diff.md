# Comparing `tmp/unitn_course_scraper-0.1.1.tar.gz` & `tmp/unitn_course_scraper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitn_course_scraper-0.1.1.tar", last modified: Wed Apr 19 09:28:13 2023, max compression
+gzip compressed data, was "unitn_course_scraper-0.1.2.tar", last modified: Wed Apr 19 09:30:57 2023, max compression
```

## Comparing `unitn_course_scraper-0.1.1.tar` & `unitn_course_scraper-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:28:13.747543 unitn_course_scraper-0.1.1/
--rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.1.1/LICENSE
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:28:13.747413 unitn_course_scraper-0.1.1/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.1.1/README.md
--rw-r--r--   0 matte      (501) staff       (20)     1009 2023-04-19 09:28:06.000000 unitn_course_scraper-0.1.1/pyproject.toml
--rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 09:28:13.747581 unitn_course_scraper-0.1.1/setup.cfg
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:28:13.745442 unitn_course_scraper-0.1.1/src/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.1.1/src/__init__.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:28:13.745627 unitn_course_scraper-0.1.1/src/cli/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.1/src/cli/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     2165 2023-04-19 07:49:54.000000 unitn_course_scraper-0.1.1/src/cli/cli.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:28:13.746099 unitn_course_scraper-0.1.1/src/login/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.1/src/login/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)     6395 2023-04-19 07:50:02.000000 unitn_course_scraper-0.1.1/src/login/login.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:28:13.746503 unitn_course_scraper-0.1.1/src/scraping/
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.1/src/scraping/__init__.py
--rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.1/src/scraping/scraper.py
-drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:28:13.747250 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/
--rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:28:13.000000 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/PKG-INFO
--rw-r--r--   0 matte      (501) staff       (20)      463 2023-04-19 09:28:13.000000 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 09:28:13.000000 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 matte      (501) staff       (20)       76 2023-04-19 09:28:13.000000 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/entry_points.txt
--rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 09:28:13.000000 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/requires.txt
--rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 09:28:13.000000 unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:30:57.619751 unitn_course_scraper-0.1.2/
+-rw-r--r--   0 matte      (501) staff       (20)    34888 2023-04-18 07:48:40.000000 unitn_course_scraper-0.1.2/LICENSE
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:30:57.619608 unitn_course_scraper-0.1.2/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      640 2023-04-18 15:16:50.000000 unitn_course_scraper-0.1.2/README.md
+-rw-r--r--   0 matte      (501) staff       (20)      997 2023-04-19 09:30:48.000000 unitn_course_scraper-0.1.2/pyproject.toml
+-rw-r--r--   0 matte      (501) staff       (20)       38 2023-04-19 09:30:57.619795 unitn_course_scraper-0.1.2/setup.cfg
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:30:57.610224 unitn_course_scraper-0.1.2/src/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-18 13:17:27.000000 unitn_course_scraper-0.1.2/src/__init__.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:30:57.610407 unitn_course_scraper-0.1.2/src/cli/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.2/src/cli/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     2475 2023-04-19 09:29:20.000000 unitn_course_scraper-0.1.2/src/cli/cli.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:30:57.610791 unitn_course_scraper-0.1.2/src/login/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.2/src/login/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)     6586 2023-04-19 09:29:20.000000 unitn_course_scraper-0.1.2/src/login/login.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:30:57.611178 unitn_course_scraper-0.1.2/src/scraping/
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.2/src/scraping/__init__.py
+-rw-r--r--   0 matte      (501) staff       (20)        0 2023-04-19 06:43:18.000000 unitn_course_scraper-0.1.2/src/scraping/scraper.py
+drwxr-xr-x   0 matte      (501) staff       (20)        0 2023-04-19 09:30:57.619414 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/
+-rw-r--r--   0 matte      (501) staff       (20)     1303 2023-04-19 09:30:57.000000 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 matte      (501) staff       (20)      463 2023-04-19 09:30:57.000000 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 matte      (501) staff       (20)        1 2023-04-19 09:30:57.000000 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 matte      (501) staff       (20)       64 2023-04-19 09:30:57.000000 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 matte      (501) staff       (20)       78 2023-04-19 09:30:57.000000 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/requires.txt
+-rw-r--r--   0 matte      (501) staff       (20)       28 2023-04-19 09:30:57.000000 unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/top_level.txt
```

### Comparing `unitn_course_scraper-0.1.1/LICENSE` & `unitn_course_scraper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.1/PKG-INFO` & `unitn_course_scraper-0.1.2/src/unitn_course_scraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unitn_course_scraper
-Version: 0.1.1
+Name: unitn-course-scraper
+Version: 0.1.2
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `unitn_course_scraper-0.1.1/README.md` & `unitn_course_scraper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unitn_course_scraper-0.1.1/pyproject.toml` & `unitn_course_scraper-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name='unitn_course_scraper'
-version='0.1.1'
+version='0.1.2'
 authors=[
     { name="DISI Drive Team", email="unitndrive@gmail.com" }
 ]
 description='Interactive scraper for your UniTN courses'
 readme='README.md'
 requires-python=">=3.7"
 classifiers=["Programming Language :: Python :: 3.7",
@@ -19,8 +19,8 @@
                 "Operating System :: OS Independent",
                 ]
 keywords=['unitn', 'courses', 'scraper', '@unitn.it',
               'moodle', 'dol', 'gestionecorsi', 'didatticaonline']
 dependencies=['python-dotenv >= 1.0.0', 'requests >= 2.28.2', 'grequests >= 0.6.0', 'beautifulsoup4 >= 4.12.2']
 
 [project.scripts]
-unitn-course-scraper = "unitn_course_scraper.__main__:main"
+unitn-course-scraper = "src.cli.cli:parse_args"
```

### Comparing `unitn_course_scraper-0.1.1/src/cli/cli.py` & `unitn_course_scraper-0.1.2/src/cli/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
-from src.login.login import scrape
 from src.login.login import login
+from src.login.login import input
+from src.login.login import get_attended_courses
+from src.login.login import get_available_courses
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description='A python program to scrape unitn courses and store resources in a local folder')
 
     parser.add_argument(
@@ -40,12 +42,20 @@
         parser.print_help()
         exit(1)
 
     if args.list_enrolled == None and args.list_available == None:
         args.list_enrolled = True
         args.list_available = True
 
-    scrape(
-        env=args.env,
-        list_enrolled=args.list_enrolled,
-        list_available=args.list_available
+    username, password = input(
+        env=args.env
     )
+    session, Bearer_auth, tokenRelayState, tokenSAMLResponse, data = login(
+        username, password)
+
+    print("ATTENDED COURSES")
+
+    print(get_attended_courses(session, Bearer_auth))
+
+    print("AVAILABLE COURSES")
+
+    print(get_available_courses(session, Bearer_auth))
```

### Comparing `unitn_course_scraper-0.1.1/src/login/login.py` & `unitn_course_scraper-0.1.2/src/login/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 from dotenv import load_dotenv
 import requests
 import os
 from bs4 import BeautifulSoup as BS
 import json
 
 
+# get username and password input
+def input(env: str):
+    load_dotenv(dotenv_path=env)
+    username = os.getenv('username')
+    password = os.getenv('password')
+
+    if username == "" or password == "" or username == None or password == None:
+        raise ValueError('Fill your username and password in .env')
+
+    return username, password
+
 # clean json courses list
+
+
 def clean_json_list(json_list):
     # removing multi language substring and setting url of each course
     for i in json_list:
         if 'id' not in i['urlMoodle']:
             json_list.remove(i)
+        else:
+            if '{mlang other}' in i['fullName']:
+                i['fullName'] = i['fullName'].split('{mlang other}', 1)[
+                    1].split('{mlang}', 1)[0]
 
-        if '{mlang other}' in i['fullName']:
-            i['fullName'] = i['fullName'].split('{mlang other}', 1)[
-                1].split('{mlang}', 1)[0]
-
-        #i['url'] = i['urlMoodle'].split('target=', 1)[1]
+            i['url'] = i['urlMoodle'].split('target=', 1)[1]
 
     return json_list
 
 # function to save HTML text to a file
 
 
 def saveHTML(name, res):
@@ -142,56 +155,52 @@
     headers = {'Authorization': auth}
     res = session.get(url, headers=headers, allow_redirects=True)
     # output list of courses
     json_list = res.json()
     return clean_json_list(json_list)
 
 
-def scrape(env: str,
-           list_enrolled: bool,
-           list_available: bool) -> None:
+# get course content
+def get_course_content(session, auth, url):
+    res = session.get(
+        url, headers={'Authorization': auth}, allow_redirects=True)
+    return True
 
-    load_dotenv(dotenv_path=env)
-    username = os.getenv('username')
-    password = os.getenv('password')
 
-    if username == "" or password == "" or username == None or password == None:
-        raise ValueError('Fill your username and password in .env')
+# def scrape(env: str,
+#            list_enrolled: bool,
+#            list_available: bool) -> None:
 
-    session, auth, tokenRelayState, tokenSAMLResponse, data = login(
-        username, password)
 
-    #get_attended_courses(session, auth)
-    json = get_available_courses(session, auth)
+#     #get_attended_courses(session, auth)
+#     json = get_available_courses(session, auth)
 
-    # print_courses_list(list)
+#     # print_courses_list(list)
 
-    # visiting first course
-    course = json[0]
+#     # visiting first course
+#     course = json[0]
 
-    # ACTUALLY THE SECOND AUTHENTICATION
-    res = session.get(course['urlMoodle'], allow_redirects=True)
+#     # ACTUALLY THE SECOND AUTHENTICATION
+#     res = session.get(course['urlMoodle'], allow_redirects=True)
 
-    # extract RelayState and SAMLResponse from last request
-    tokenRelayState = extract_RelayState_from_HTML(res)
-    tokenSAMLResponse = extract_SAMLResponse_from_HTML(res)
+#     # extract RelayState and SAMLResponse from last request
+#     tokenRelayState = extract_RelayState_from_HTML(res)
+#     tokenSAMLResponse = extract_SAMLResponse_from_HTML(res)
 
-    # post to dol with tokens
-    url = 'https://didatticaonline.unitn.it/Shibboleth.sso/SAML2/POST'
-    data = {'RelayState': tokenRelayState, 'SAMLResponse': tokenSAMLResponse}
-    res = session.post(url, data=data, allow_redirects=True)
+#     # post to dol with tokens
+#     url = 'https://didatticaonline.unitn.it/Shibboleth.sso/SAML2/POST'
+#     data = {'RelayState': tokenRelayState, 'SAMLResponse': tokenSAMLResponse}
+#     res = session.post(url, data=data, allow_redirects=True)
 
-    # should be redirected to course page
-    print(res.url)
+#     # should be redirected to course page
+#     print(res.url)
 
 
 # # print courses names
 # for i in json:
 #     print(i['fullName'])
 #     print()
 
 # # print history of requests
 # for i in res.history:
 #     print(i.status_code, i.url)
 # print(res.url)
-if __name__ == "__main__":
-    scrape()
```

### Comparing `unitn_course_scraper-0.1.1/src/unitn_course_scraper.egg-info/PKG-INFO` & `unitn_course_scraper-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unitn-course-scraper
-Version: 0.1.1
+Name: unitn_course_scraper
+Version: 0.1.2
 Summary: Interactive scraper for your UniTN courses
 Author-email: DISI Drive Team <unitndrive@gmail.com>
 Keywords: unitn,courses,scraper,@unitn.it,moodle,dol,gestionecorsi,didatticaonline
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

