# Comparing `tmp/nuldc-0.7.1.tar.gz` & `tmp/nuldc-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuldc-0.7.1.tar", max compression
+gzip compressed data, was "nuldc-0.7.2.tar", max compression
```

## Comparing `nuldc-0.7.1.tar` & `nuldc-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-03-25 03:10:22.334369 nuldc-0.7.1/LICENSE
--rw-r--r--   0        0        0     4014 2023-03-25 03:10:22.334369 nuldc-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-03-25 03:10:22.334369 nuldc-0.7.1/nuldc/__init__.py
--rw-r--r--   0        0        0     2641 2023-03-25 03:10:22.334369 nuldc-0.7.1/nuldc/commandline.py
--rw-r--r--   0        0        0     3426 2023-03-25 03:10:22.334369 nuldc-0.7.1/nuldc/dump.py
--rw-r--r--   0        0        0     6927 2023-03-25 03:10:22.334369 nuldc-0.7.1/nuldc/helpers.py
--rw-r--r--   0        0        0      552 2023-03-25 03:10:22.334369 nuldc-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 nuldc-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-19 02:07:59.644353 nuldc-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4014 2023-04-19 02:07:59.644353 nuldc-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 02:07:59.644353 nuldc-0.7.2/nuldc/__init__.py
+-rw-r--r--   0        0        0     2641 2023-04-19 02:07:59.644353 nuldc-0.7.2/nuldc/commandline.py
+-rw-r--r--   0        0        0     3426 2023-04-19 02:07:59.644353 nuldc-0.7.2/nuldc/dump.py
+-rw-r--r--   0        0        0     6955 2023-04-19 02:07:59.644353 nuldc-0.7.2/nuldc/helpers.py
+-rw-r--r--   0        0        0      552 2023-04-19 02:07:59.644353 nuldc-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 nuldc-0.7.2/PKG-INFO
```

### Comparing `nuldc-0.7.1/LICENSE` & `nuldc-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nuldc-0.7.1/README.md` & `nuldc-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `nuldc-0.7.1/nuldc/commandline.py` & `nuldc-0.7.2/nuldc/commandline.py`

 * *Files identical despite different names*

### Comparing `nuldc-0.7.1/nuldc/dump.py` & `nuldc-0.7.2/nuldc/dump.py`

 * *Files identical despite different names*

### Comparing `nuldc-0.7.1/nuldc/helpers.py` & `nuldc-0.7.2/nuldc/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,29 +64,29 @@
     # set next url to blank
     results['pagination']['next_url'] = ''
 
     return results
 
 
 def get_collection_by_id(api_base_url, identifier,
-                         parameters, all_results=False):
+                         parameters, all_results=False, page_limit=200):
     """returns a collection as IIIF or json"""
 
     url = f"{api_base_url}/collections/{identifier}"
     results = requests.get(url, params=parameters).json()
 
     if all_results and parameters.get('as') == 'iiif':
         # fire off a search for total pagecount this powers the progressbar
         count_params = parameters
         count_params['as'] = 'opensearch'
         count_params['query'] = f'collection.id:{identifier}'
         url = f"{api_base_url}/search"
         total_pages = requests.get(url, count_params).json()[
             'pagination']['total_pages']
-        results = get_all_iiif(results, total_pages)
+        results = get_all_iiif(results, total_pages, page_limit)
 
     return results
 
 
 def get_nested_field(field, source_dict):
     """Handles nested fields using dotted notation from the cli fields and
     flattens nested data"""
```

### Comparing `nuldc-0.7.1/PKG-INFO` & `nuldc-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuldc
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 License: MIT
 Author: davidschober
 Author-email: davidschob@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

