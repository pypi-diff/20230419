# Comparing `tmp/python-vlc-http-0.0.8.tar.gz` & `tmp/python-vlc-http-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-vlc-http-0.0.8.tar", last modified: Mon Oct 12 10:23:57 2020, max compression
+gzip compressed data, was "dist/python-vlc-http-0.0.9.tar", last modified: Mon Oct 12 12:10:08 2020, max compression
```

## Comparing `python-vlc-http-0.0.8.tar` & `python-vlc-http-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matejplavevski   (501) staff       (20)        0 2020-10-12 10:23:57.413281 python-vlc-http-0.0.8/
--rw-r--r--   0 matejplavevski   (501) staff       (20)     1819 2020-06-13 19:00:52.000000 python-vlc-http-0.0.8/.gitignore
--rw-r--r--   0 matejplavevski   (501) staff       (20)     3364 2020-07-05 21:34:11.000000 python-vlc-http-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 matejplavevski   (501) staff       (20)     1055 2020-04-27 20:22:59.000000 python-vlc-http-0.0.8/LICENSE
--rw-r--r--   0 matejplavevski   (501) staff       (20)     5390 2020-10-12 10:23:57.412551 python-vlc-http-0.0.8/PKG-INFO
--rw-r--r--   0 matejplavevski   (501) staff       (20)     2929 2020-07-05 21:33:46.000000 python-vlc-http-0.0.8/README.md
-drwxr-xr-x   0 matejplavevski   (501) staff       (20)        0 2020-10-12 10:23:57.406035 python-vlc-http-0.0.8/python_vlc_http/
--rw-r--r--   0 matejplavevski   (501) staff       (20)       39 2020-06-13 18:58:13.000000 python-vlc-http-0.0.8/python_vlc_http/__init__.py
--rw-r--r--   0 matejplavevski   (501) staff       (20)     7676 2020-10-10 18:20:05.000000 python-vlc-http-0.0.8/python_vlc_http/vlc.py
-drwxr-xr-x   0 matejplavevski   (501) staff       (20)        0 2020-10-12 10:23:57.410995 python-vlc-http-0.0.8/python_vlc_http.egg-info/
--rw-r--r--   0 matejplavevski   (501) staff       (20)     5390 2020-10-12 10:23:55.000000 python-vlc-http-0.0.8/python_vlc_http.egg-info/PKG-INFO
--rw-r--r--   0 matejplavevski   (501) staff       (20)      301 2020-10-12 10:23:56.000000 python-vlc-http-0.0.8/python_vlc_http.egg-info/SOURCES.txt
--rw-r--r--   0 matejplavevski   (501) staff       (20)        1 2020-10-12 10:23:55.000000 python-vlc-http-0.0.8/python_vlc_http.egg-info/dependency_links.txt
--rw-r--r--   0 matejplavevski   (501) staff       (20)       19 2020-10-12 10:23:55.000000 python-vlc-http-0.0.8/python_vlc_http.egg-info/requires.txt
--rw-r--r--   0 matejplavevski   (501) staff       (20)       16 2020-10-12 10:23:55.000000 python-vlc-http-0.0.8/python_vlc_http.egg-info/top_level.txt
--rw-r--r--   0 matejplavevski   (501) staff       (20)       38 2020-10-12 10:23:57.414021 python-vlc-http-0.0.8/setup.cfg
--rw-r--r--   0 matejplavevski   (501) staff       (20)     1542 2020-10-11 20:26:17.000000 python-vlc-http-0.0.8/setup.py
+drwxr-xr-x   0 matejplavevski   (501) staff       (20)        0 2020-10-12 12:10:08.849348 python-vlc-http-0.0.9/
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     1819 2020-06-13 19:00:52.000000 python-vlc-http-0.0.9/.gitignore
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     3364 2020-07-05 21:34:11.000000 python-vlc-http-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     1055 2020-04-27 20:22:59.000000 python-vlc-http-0.0.9/LICENSE
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     5390 2020-10-12 12:10:08.849059 python-vlc-http-0.0.9/PKG-INFO
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     2929 2020-07-05 21:33:46.000000 python-vlc-http-0.0.9/README.md
+drwxr-xr-x   0 matejplavevski   (501) staff       (20)        0 2020-10-12 12:10:08.845965 python-vlc-http-0.0.9/python_vlc_http/
+-rw-r--r--   0 matejplavevski   (501) staff       (20)       87 2020-10-12 12:05:30.000000 python-vlc-http-0.0.9/python_vlc_http/__init__.py
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     7564 2020-10-12 12:05:30.000000 python-vlc-http-0.0.9/python_vlc_http/vlc.py
+drwxr-xr-x   0 matejplavevski   (501) staff       (20)        0 2020-10-12 12:10:08.848494 python-vlc-http-0.0.9/python_vlc_http.egg-info/
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     5390 2020-10-12 12:10:08.000000 python-vlc-http-0.0.9/python_vlc_http.egg-info/PKG-INFO
+-rw-r--r--   0 matejplavevski   (501) staff       (20)      301 2020-10-12 12:10:08.000000 python-vlc-http-0.0.9/python_vlc_http.egg-info/SOURCES.txt
+-rw-r--r--   0 matejplavevski   (501) staff       (20)        1 2020-10-12 12:10:08.000000 python-vlc-http-0.0.9/python_vlc_http.egg-info/dependency_links.txt
+-rw-r--r--   0 matejplavevski   (501) staff       (20)       19 2020-10-12 12:10:08.000000 python-vlc-http-0.0.9/python_vlc_http.egg-info/requires.txt
+-rw-r--r--   0 matejplavevski   (501) staff       (20)       16 2020-10-12 12:10:08.000000 python-vlc-http-0.0.9/python_vlc_http.egg-info/top_level.txt
+-rw-r--r--   0 matejplavevski   (501) staff       (20)       38 2020-10-12 12:10:08.849485 python-vlc-http-0.0.9/setup.cfg
+-rw-r--r--   0 matejplavevski   (501) staff       (20)     1542 2020-10-12 12:05:37.000000 python-vlc-http-0.0.9/setup.py
```

### Comparing `python-vlc-http-0.0.8/.gitignore` & `python-vlc-http-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `python-vlc-http-0.0.8/CODE_OF_CONDUCT.md` & `python-vlc-http-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `python-vlc-http-0.0.8/LICENSE` & `python-vlc-http-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-vlc-http-0.0.8/PKG-INFO` & `python-vlc-http-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-vlc-http
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python module that enables communication with the VLC http server 
 Home-page: https://github.com/matejmecka/python-vlc-http
 Author: Matej Plavevski
 Author-email: matej.plavevski+github@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/python-vlc-http/
 Description: # python-vlc-http
```

### Comparing `python-vlc-http-0.0.8/README.md` & `python-vlc-http-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python-vlc-http-0.0.8/python_vlc_http/vlc.py` & `python-vlc-http-0.0.9/python_vlc_http/vlc.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     """Exception related to Invalid Credntials"""
     pass
 
 class RequestFailed(Exception):
     """Exception related to an Invalid Request"""
     pass
 
-class FailedConnecting(Exception):
-    """Exception related to when the plugin fails to connect"""
-    pass
-
 class MissingHost(Exception):
     """Exception related when a host is missing"""
     pass
 
 class HttpVLC:
     def __init__(self, host=None, username=None, password=None):
         self.host = host
@@ -50,15 +46,15 @@
             url = f'{url}?command={command}'
         try:
             request = requests.get(url, auth=(self.username, self.password))
             self.status_code(request)
             data = xmltodict.parse(request.text, process_namespaces=True).get("root")
             return data
         except (requests.exceptions.ConnectionError, requests.exceptions.Timeout) as error:
-            raise FailedConnecting(f"The VLC Server is unreachable. Error code: {error}")
+            raise RequestFailed(f"The VLC Server is unreachable. Error code: {error}")
 
     def fetch_data(self, command=None):
         return self.fetch_status(command)
 
     def parse_data(self, command=None, option='state', in_information=False):
         response_data = self.fetch_data(command=command)
         if not in_information:
```

### Comparing `python-vlc-http-0.0.8/python_vlc_http.egg-info/PKG-INFO` & `python-vlc-http-0.0.9/python_vlc_http.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-vlc-http
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python module that enables communication with the VLC http server 
 Home-page: https://github.com/matejmecka/python-vlc-http
 Author: Matej Plavevski
 Author-email: matej.plavevski+github@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/python-vlc-http/
 Description: # python-vlc-http
```

### Comparing `python-vlc-http-0.0.8/setup.py` & `python-vlc-http-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 setup_args = dict(
     name='python-vlc-http',
-    version='0.0.8',
+    version='0.0.9',
     description='Python module that enables communication with the VLC http server ',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Matej Plavevski',
     author_email='matej.plavevski+github@gmail.com',
```

