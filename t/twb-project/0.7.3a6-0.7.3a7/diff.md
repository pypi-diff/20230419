# Comparing `tmp/twb_project-0.7.3a6.tar.gz` & `tmp/twb_project-0.7.3a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.7.3a6.tar", max compression
+gzip compressed data, was "twb_project-0.7.3a7.tar", max compression
```

## Comparing `twb_project-0.7.3a6.tar` & `twb_project-0.7.3a7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.3a6/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.3a6/README.md
--rw-r--r--   0        0        0      762 2023-04-19 06:27:26.334165 twb_project-0.7.3a6/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.3a6/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.3a6/twb/bip.py
--rw-r--r--   0        0        0    17357 2023-04-19 06:27:17.683004 twb_project-0.7.3a6/twb/builder.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.3a6/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.3a6/twb/downloader.py
--rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.3a6/twb/logger.py
--rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.3a6/twb/modifier.py
--rw-r--r--   0        0        0     9101 2023-04-19 03:52:12.830673 twb_project-0.7.3a6/twb/parallelization.py
--rw-r--r--   0        0        0    11680 2023-04-19 06:20:11.392642 twb_project-0.7.3a6/twb/reader.py
--rw-r--r--   0        0        0     6161 2023-04-19 04:03:30.303243 twb_project-0.7.3a6/twb/utils.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 twb_project-0.7.3a6/setup.py
--rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 twb_project-0.7.3a6/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.3a7/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.3a7/README.md
+-rw-r--r--   0        0        0      762 2023-04-19 07:23:13.079647 twb_project-0.7.3a7/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.3a7/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.3a7/twb/bip.py
+-rw-r--r--   0        0        0    17433 2023-04-19 07:22:55.226411 twb_project-0.7.3a7/twb/builder.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.3a7/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.3a7/twb/downloader.py
+-rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.3a7/twb/logger.py
+-rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.3a7/twb/modifier.py
+-rw-r--r--   0        0        0     9101 2023-04-19 03:52:12.830673 twb_project-0.7.3a7/twb/parallelization.py
+-rw-r--r--   0        0        0    11680 2023-04-19 06:20:11.392642 twb_project-0.7.3a7/twb/reader.py
+-rw-r--r--   0        0        0     6161 2023-04-19 04:03:30.303243 twb_project-0.7.3a7/twb/utils.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 twb_project-0.7.3a7/setup.py
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 twb_project-0.7.3a7/PKG-INFO
```

### Comparing `twb_project-0.7.3a6/LICENSE` & `twb_project-0.7.3a7/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/README.md` & `twb_project-0.7.3a7/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/pyproject.toml` & `twb_project-0.7.3a7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.7.3a6"
+version = "0.7.3a7"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
```

### Comparing `twb_project-0.7.3a6/twb/bip.py` & `twb_project-0.7.3a7/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/builder.py` & `twb_project-0.7.3a7/twb/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .logger import universal_logger_init, twb_logger, cleanup_logger
 from .utils import get_file_list, compress_zstd, get_memory_consumption, cleanup_dir, get_curr_version, \
     prepare_output_dir, COMPRESSION_EXTENSION
 from .bip import BlockInteriorProcessor, DefaultBIP
 from .parallelization import RDSProcessManager, RDSProcessController
 
-_DEFAULT_REVISIONS_PER_BLOCK = 1000000
+_DEFAULT_REVISIONS_PER_BLOCK = 300000
 _DEFAULT_START_INDEX = 0
 _DEFAULT_NUM_PROC = 1
 _DEFAULT_LOG_LEVEL = logging.DEBUG
 
 
 class Builder:
     """
@@ -254,14 +254,16 @@
         def _super_callback(article: dict):
             """
             The super callback for the XML parser. It will be called recursively for each article.
             """
             nonlocal total_article_count, total_block_count, total_revision_count
             nonlocal revision_count, memory_usage_records, all_memory_usage_records, curr_output_path
 
+            controller.logdebug('_super_callback() called.')
+
             # If previous batch is full, store the max memory usage and reset the counters.
             if revision_count >= revisions_per_block:
                 # Store the max memory usage in previous batch.
                 all_memory_usage_records.append(max(memory_usage_records))
                 # Update the block count.
                 total_block_count += 1
                 # Reset the counters.
@@ -397,15 +399,15 @@
     :param output_path: the path to store the JSONL file
     :return: the list of JSONL file paths
     """
     logging.debug(f'Dumping JSONL for {output_path}...')
     dumped_article_jsonl = json.dumps(article) + '\n'
     logging.debug(f'Storing JSONL (len: {len(dumped_article_jsonl)}) to {output_path}...')
     try:
-        with open(output_path, 'a', buffering=1) as f:
+        with open(output_path, 'a', buffering=10 * 1024 * 1024) as f:
             logging.debug(f'Writing to {output_path}...')
             f.write(dumped_article_jsonl)
     except Exception as e:
         logging.fatal(f'Error in writing article: {e}')
     logging.debug(f'Storing JSONL done: {output_path}.')
```

### Comparing `twb_project-0.7.3a6/twb/decompressor.py` & `twb_project-0.7.3a7/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/downloader.py` & `twb_project-0.7.3a7/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/logger.py` & `twb_project-0.7.3a7/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/modifier.py` & `twb_project-0.7.3a7/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/parallelization.py` & `twb_project-0.7.3a7/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/reader.py` & `twb_project-0.7.3a7/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/twb/utils.py` & `twb_project-0.7.3a7/twb/utils.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.3a6/setup.py` & `twb_project-0.7.3a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.7.3a6',
+    'version': '0.7.3a7',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.7.3a6/PKG-INFO` & `twb_project-0.7.3a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.7.3a6
+Version: 0.7.3a7
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
```

