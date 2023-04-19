# Comparing `tmp/haki_crawler-0.6.tar.gz` & `tmp/haki_crawler-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haki_crawler-0.6.tar", last modified: Wed Apr 19 07:05:09 2023, max compression
+gzip compressed data, was "haki_crawler-0.7.tar", last modified: Wed Apr 19 10:31:43 2023, max compression
```

## Comparing `haki_crawler-0.6.tar` & `haki_crawler-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:09.901063 haki_crawler-0.6/
--rw-rw-rw-   0        0        0      634 2023-04-19 07:05:09.901063 haki_crawler-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:09.886063 haki_crawler-0.6/haki_crawler/
--rw-rw-rw-   0        0        0        0 2023-04-17 04:16:01.000000 haki_crawler-0.6/haki_crawler/__init__.py
--rw-rw-rw-   0        0        0     3711 2023-04-19 07:01:16.000000 haki_crawler-0.6/haki_crawler/appfigures.py
--rw-rw-rw-   0        0        0     7966 2023-04-17 04:16:01.000000 haki_crawler-0.6/haki_crawler/sensortower.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:09.900062 haki_crawler-0.6/haki_crawler.egg-info/
--rw-rw-rw-   0        0        0      634 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-19 07:05:09.000000 haki_crawler-0.6/haki_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 07:05:09.902063 haki_crawler-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1264 2023-04-19 07:03:06.000000 haki_crawler-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:31:43.156982 haki_crawler-0.7/
+-rw-rw-rw-   0        0        0      634 2023-04-19 10:31:43.156982 haki_crawler-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 10:31:43.124117 haki_crawler-0.7/haki_crawler/
+-rw-rw-rw-   0        0        0        0 2023-04-17 04:16:01.000000 haki_crawler-0.7/haki_crawler/__init__.py
+-rw-rw-rw-   0        0        0     4644 2023-04-19 10:29:15.000000 haki_crawler-0.7/haki_crawler/appfigures.py
+-rw-rw-rw-   0        0        0     7966 2023-04-17 04:16:01.000000 haki_crawler-0.7/haki_crawler/sensortower.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:31:43.155982 haki_crawler-0.7/haki_crawler.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-04-19 10:31:42.000000 haki_crawler-0.7/haki_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-04-19 10:31:42.000000 haki_crawler-0.7/haki_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 10:31:42.000000 haki_crawler-0.7/haki_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 10:31:42.000000 haki_crawler-0.7/haki_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-19 10:31:42.000000 haki_crawler-0.7/haki_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 10:31:43.157982 haki_crawler-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-04-19 10:31:22.000000 haki_crawler-0.7/setup.py
```

### Comparing `haki_crawler-0.6/PKG-INFO` & `haki_crawler-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haki_crawler
-Version: 0.6
+Version: 0.7
 Summary: A short description of your package
 Home-page: https://example.com
 Author: namhn1495
 Author-email: namhn1495@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `haki_crawler-0.6/haki_crawler/appfigures.py` & `haki_crawler-0.7/haki_crawler/appfigures.py`

 * *Files 13% similar despite different names*

```diff
@@ -82,7 +82,32 @@
         print("status: {}".format(status))
         if status != 'running':
             return response_data
 
         i = i + 1
         time.sleep(1)
     return response_data
+
+
+def keyword_rank_fast(cookie, keyword):
+    """
+    This function retrieves keyword ranking using Appfigures ASO API, given a cookie and a keyword, but faster.
+
+    :param cookie: Dictionary containing '_af_session' and '_af_user_token' keys
+    :param keyword: The keyword for which the ranking is to be retrieved
+    :return: JSON response containing keyword ranking
+    """
+    url = f"https://appfigures.com/api/aso-ranks?term={keyword}&country=US&storefront=google_play&page=&device=handheld&count=15"
+
+    _af_session = cookie['_af_session']
+    x_st = cookie['x_st']
+
+    headers = {
+        'Cookie': f'_af_session={_af_session}; G_ENABLED_IDPS=google',
+        'X-Requested-With': 'XMLHttpRequest',
+        'X-ST': x_st,
+    }
+
+    # Keep sending requests until status is not 'running'
+    response = requests.get(url, headers=headers)
+    response_data = response.json()
+    return response_data
```

### Comparing `haki_crawler-0.6/haki_crawler/sensortower.py` & `haki_crawler-0.7/haki_crawler/sensortower.py`

 * *Files identical despite different names*

### Comparing `haki_crawler-0.6/haki_crawler.egg-info/PKG-INFO` & `haki_crawler-0.7/haki_crawler.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haki-crawler
-Version: 0.6
+Version: 0.7
 Summary: A short description of your package
 Home-page: https://example.com
 Author: namhn1495
 Author-email: namhn1495@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `haki_crawler-0.6/setup.py` & `haki_crawler-0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         shutil.rmtree(thu_muc)
         print(f"Đã xóa thư mục: {thu_muc}")
     else:
         print(f"Thư mục {thu_muc} không tồn tại")
 
 setup(
     name=LIB_NAME,
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     install_requires=[
         # Danh sách các gói phụ thuộc của gói này
         "requests",
     ],
     author="namhn1495",
     author_email="namhn1495@gmail.com",
```

