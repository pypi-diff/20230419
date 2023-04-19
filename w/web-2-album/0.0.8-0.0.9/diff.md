# Comparing `tmp/web_2_album-0.0.8.tar.gz` & `tmp/web_2_album-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/web_2_album-0.0.8.tar", last modified: Mon Mar 16 23:58:22 2020, max compression
+gzip compressed data, was "dist/web_2_album-0.0.9.tar", last modified: Tue Mar 17 00:02:12 2020, max compression
```

## Comparing `web_2_album-0.0.8.tar` & `web_2_album-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-16 23:58:22.000000 web_2_album-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      798 2020-03-16 23:58:22.000000 web_2_album-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      209 2020-03-16 00:43:30.000000 web_2_album-0.0.8/README.md
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-03-16 23:58:22.000000 web_2_album-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      880 2020-03-16 23:57:56.000000 web_2_album-0.0.8/setup.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2428 2020-03-16 23:58:19.000000 web_2_album-0.0.8/web_2_album/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      798 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      216 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      101 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       12 2020-03-16 23:58:22.000000 web_2_album-0.0.8/web_2_album.egg-info/top_level.txt
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-17 00:02:12.000000 web_2_album-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      798 2020-03-17 00:02:12.000000 web_2_album-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      209 2020-03-16 00:43:30.000000 web_2_album-0.0.9/README.md
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-03-17 00:02:12.000000 web_2_album-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      880 2020-03-17 00:01:03.000000 web_2_album-0.0.9/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     2432 2020-03-17 00:00:59.000000 web_2_album-0.0.9/web_2_album/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      798 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      216 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      101 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       12 2020-03-17 00:02:12.000000 web_2_album-0.0.9/web_2_album.egg-info/top_level.txt
```

### Comparing `web_2_album-0.0.8/PKG-INFO` & `web_2_album-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web_2_album
-Version: 0.0.8
+Version: 0.0.9
 Summary: Return photo list and caption (markdown format) from web.
 Home-page: https://github.com/gaoyunzhi/web_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # web_2_album
```

### Comparing `web_2_album-0.0.8/setup.py` & `web_2_album-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="web_2_album",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Return photo list and caption (markdown format) from web.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/web_2_album",
     packages=setuptools.find_packages(),
```

### Comparing `web_2_album-0.0.8/web_2_album/__init__.py` & `web_2_album-0.0.9/web_2_album/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 	candidates = [
 		lambda x: x.find('div', class_='weibo-text'), 
 		lambda x: x.find('blockquote'),
 	]
 	candidate = getCandidate(candidates, b, '')
 	if not candidate:
 		return ''
-	quote = candidate.text(separator="\n").strip()
+	quote = candidate.get_text(separator="\n").strip()
 	for link in candidate.find_all('a', title=True, href=True):
 		url = link['title']
 		url = clearUrl(export_to_telegraph.export(url) or url)
 		quote = quote.replace(link['href'], ' ' + url + ' ')
 	return quote
 
 def getAuthor(b):
```

### Comparing `web_2_album-0.0.8/web_2_album.egg-info/PKG-INFO` & `web_2_album-0.0.9/web_2_album.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-2-album
-Version: 0.0.8
+Version: 0.0.9
 Summary: Return photo list and caption (markdown format) from web.
 Home-page: https://github.com/gaoyunzhi/web_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # web_2_album
```

