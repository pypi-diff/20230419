# Comparing `tmp/twb_project-0.7.3a8.tar.gz` & `tmp/twb_project-0.7.3a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.7.3a8.tar", max compression
+gzip compressed data, was "twb_project-0.7.3a9.tar", max compression
```

## Comparing `twb_project-0.7.3a8.tar` & `twb_project-0.7.3a9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.3a8/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.3a8/README.md
--rw-r--r--   0        0        0      762 2023-04-19 14:43:50.163156 twb_project-0.7.3a8/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.3a8/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.3a8/twb/bip.py
--rw-r--r--   0        0        0    17441 2023-04-19 14:43:35.861331 twb_project-0.7.3a8/twb/builder.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.3a8/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.3a8/twb/downloader.py
--rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.3a8/twb/logger.py
--rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.3a8/twb/modifier.py
--rw-r--r--   0        0        0     9101 2023-04-19 03:52:12.830673 twb_project-0.7.3a8/twb/parallelization.py
--rw-r--r--   0        0        0    11680 2023-04-19 06:20:11.392642 twb_project-0.7.3a8/twb/reader.py
--rw-r--r--   0        0        0     6161 2023-04-19 04:03:30.303243 twb_project-0.7.3a8/twb/utils.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 twb_project-0.7.3a8/setup.py
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 twb_project-0.7.3a8/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.3a9/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.3a9/README.md
+-rw-r--r--   0        0        0      762 2023-04-19 17:36:55.924904 twb_project-0.7.3a9/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.3a9/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.3a9/twb/bip.py
+-rw-r--r--   0        0        0    17389 2023-04-19 17:36:30.165883 twb_project-0.7.3a9/twb/builder.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.3a9/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.3a9/twb/downloader.py
+-rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.3a9/twb/logger.py
+-rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.3a9/twb/modifier.py
+-rw-r--r--   0        0        0     9101 2023-04-19 03:52:12.830673 twb_project-0.7.3a9/twb/parallelization.py
+-rw-r--r--   0        0        0    11680 2023-04-19 06:20:11.392642 twb_project-0.7.3a9/twb/reader.py
+-rw-r--r--   0        0        0     6161 2023-04-19 04:03:30.303243 twb_project-0.7.3a9/twb/utils.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 twb_project-0.7.3a9/setup.py
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 twb_project-0.7.3a9/PKG-INFO
```

### Comparing `twb_project-0.7.3a8/LICENSE` & `twb_project-0.7.3a9/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/README.md` & `twb_project-0.7.3a9/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/pyproject.toml` & `twb_project-0.7.3a9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.7.3a8"
+version = "0.7.3a9"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.7.3a8/twb/bip.py` & `twb_project-0.7.3a9/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/builder.py` & `twb_project-0.7.3a9/twb/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,23 +356,23 @@
     if tag_name != 'page':
         return True
 
     # If the item is not a dictionary, it means that the item is a leaf node, and we don't expect it to be a block.
     if item_type is not dict:
         return True
 
-    logging.debug(f'Start parsing: <{tag_name}>.')
+    logging.debug(f'Start callback: <{tag_name}>.')
 
-    processed_item = item  # processor.parse(tag=tag_name, meta={}, tree=item)
-
-    logging.debug(f'Parsing done: <{tag_name}>.')
+    # processed_item = processor.parse(tag=tag_name, meta={}, tree=item)
 
     # If the item is not None, it means that the item is a block and we should append it to the results.
-    if processed_item is not None:
-        super_callback(processed_item)
+    # if processed_item is not None:
+    #     pass
+
+    super_callback(item)
 
     logging.debug(f'Callback done: <{tag_name}>.')
 
     return True
 
 
 def _parse_xml(path: str, processor: BlockInteriorProcessor, super_callback: Callable[[dict], None]):
```

### Comparing `twb_project-0.7.3a8/twb/decompressor.py` & `twb_project-0.7.3a9/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/downloader.py` & `twb_project-0.7.3a9/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/logger.py` & `twb_project-0.7.3a9/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/modifier.py` & `twb_project-0.7.3a9/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/parallelization.py` & `twb_project-0.7.3a9/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/reader.py` & `twb_project-0.7.3a9/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/twb/utils.py` & `twb_project-0.7.3a9/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a8/setup.py` & `twb_project-0.7.3a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.7.3a8',
+    'version': '0.7.3a9',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.7.3a8/PKG-INFO` & `twb_project-0.7.3a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.7.3a8
+Version: 0.7.3a9
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

