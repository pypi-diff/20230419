# Comparing `tmp/twb_project-0.7.2.tar.gz` & `tmp/twb_project-0.7.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-0.7.2.tar", max compression
+gzip compressed data, was "twb_project-0.7.3a0.tar", max compression
```

## Comparing `twb_project-0.7.2.tar` & `twb_project-0.7.3a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.2/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.2/README.md
--rw-r--r--   0        0        0      760 2023-04-12 00:39:34.393087 twb_project-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.2/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.2/twb/bip.py
--rw-r--r--   0        0        0    16138 2023-03-26 23:28:51.163801 twb_project-0.7.2/twb/builder.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.2/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.2/twb/downloader.py
--rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.2/twb/logger.py
--rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.2/twb/modifier.py
--rw-r--r--   0        0        0    11632 2023-03-26 21:37:48.900993 twb_project-0.7.2/twb/parallelization.py
--rw-r--r--   0        0        0    11317 2023-04-12 00:22:13.542074 twb_project-0.7.2/twb/reader.py
--rw-r--r--   0        0        0     6161 2023-04-12 00:33:50.301793 twb_project-0.7.2/twb/utils.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-0.7.2/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-0.7.3a0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-0.7.3a0/README.md
+-rw-r--r--   0        0        0      762 2023-04-19 04:08:06.714997 twb_project-0.7.3a0/pyproject.toml
+-rw-r--r--   0        0        0      201 2023-03-26 05:00:17.199386 twb_project-0.7.3a0/twb/__init__.py
+-rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-0.7.3a0/twb/bip.py
+-rw-r--r--   0        0        0    16931 2023-04-19 04:07:41.134103 twb_project-0.7.3a0/twb/builder.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-0.7.3a0/twb/decompressor.py
+-rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-0.7.3a0/twb/downloader.py
+-rw-r--r--   0        0        0     3607 2023-03-26 19:24:30.197127 twb_project-0.7.3a0/twb/logger.py
+-rw-r--r--   0        0        0      546 2023-03-26 05:47:24.185465 twb_project-0.7.3a0/twb/modifier.py
+-rw-r--r--   0        0        0     9101 2023-04-19 03:52:12.830673 twb_project-0.7.3a0/twb/parallelization.py
+-rw-r--r--   0        0        0    11539 2023-04-19 03:53:32.772172 twb_project-0.7.3a0/twb/reader.py
+-rw-r--r--   0        0        0     6161 2023-04-19 04:03:30.303243 twb_project-0.7.3a0/twb/utils.py
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 twb_project-0.7.3a0/setup.py
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 twb_project-0.7.3a0/PKG-INFO
```

### Comparing `twb_project-0.7.2/LICENSE` & `twb_project-0.7.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/README.md` & `twb_project-0.7.3a0/README.md`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/pyproject.toml` & `twb_project-0.7.3a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "twb-project"
-version = "0.7.2"
+version = "0.7.3a0"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
 homepage = "https://twb.lingxi.li/"
 repository = "https://github.com/lilingxi01/twb-project"
 documentation = "https://twb.lingxi.li/docs/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-py7zr = "^0.20.4"
+py7zr = "^0.20.5"
 xmltodict = "^0.13.0"
 jsonlines = "^3.1.0"
-zstandard = "^0.20.0"
-psutil = "^5.9.4"
+zstandard = "^0.21.0"
+psutil = "^5.9.5"
 requests = "^2.28.2"
-beautifulsoup4 = "^4.11.2"
+beautifulsoup4 = "^4.12.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `twb_project-0.7.2/twb/bip.py` & `twb_project-0.7.3a0/twb/bip.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/twb/builder.py` & `twb_project-0.7.3a0/twb/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,43 +276,59 @@
                 curr_article_revision_count = 1
 
             # Update the counters.
             revision_count += curr_article_revision_count
             total_revision_count += curr_article_revision_count
             total_article_count += 1
 
+            controller.logdebug(f'Total revision count: {total_revision_count}')
+
             # Store the article into the current output file.
             _store_article_to_jsonl(article=article, output_path=curr_output_path)
 
+            controller.logdebug(f'Stored.')
+
             # Record the memory usage.
             memory_usage_records.append(get_memory_consumption())
 
+            controller.logdebug(f'Memory: {memory_usage_records[-1]} MB')
+
+        controller.logdebug(f'Big parsing loop started. (revisions_per_block={revisions_per_block})')
+
         # We store articles into JSONL files in a streaming manner, along the way of parsing XML files.
         # Therefore, we don't have to keep all the results in the memory, which is a huge problem.
         for path in decompressed_files:
             _parse_xml(path=path, processor=block_interior_processor, super_callback=_super_callback)
 
+        controller.logdebug('Big parsing loop done.')
+
         if len(memory_usage_records) > 0:
             all_memory_usage_records.append(max(memory_usage_records))
 
         controller.logdebug(f'Parsing done. {total_article_count} articles processed.',
                             f'({total_revision_count} revisions are processed into {total_block_count} blocks)',
                             f'(Highest Memory: {max(all_memory_usage_records)} MB)')
 
         cleanup_dir(decompression_temp_dir)  # Delete temporary files used for decompression.
 
+        controller.logdebug(f'Cleaning up decompression temp dir done.')
+
         if should_compress:
             # Store the results to JSONL files.
             json_files = get_file_list(compression_temp_dir)
 
+            controller.logdebug(f'Compression started. {len(json_files)} files to compress.')
+
             # Compress the files.
             for json_file in json_files:
+                controller.logdebug(f'Compressing {json_file}...')
                 _compress_file(path=json_file, output_dir=output_dir, controller=controller)
 
             controller.logdebug(f'Compression done. {len(json_files)} files compressed in total.')
+
     except Exception as e:
         controller.logerr(f'Parsing failed at {path}:', e)
     finally:
         # Clean up the temporary directory.
         cleanup_dir(temp_dir)
         controller.logdebug(f'Temporary directory cleaned up: {temp_id}.')
 
@@ -338,20 +354,26 @@
     if tag_name != 'page':
         return True
 
     # If the item is not a dictionary, it means that the item is a leaf node, and we don't expect it to be a block.
     if item_type is not dict:
         return True
 
+    logging.debug(f'Start parsing {tag_name}.')
+
     processed_item = processor.parse(tag=tag_name, meta={}, tree=item)
 
+    logging.debug(f'Parsing done: {tag_name}.')
+
     # If the item is not None, it means that the item is a block and we should append it to the results.
     if processed_item is not None:
         super_callback(processed_item)
 
+    logging.debug(f'Callback done: {tag_name}.')
+
     return True
 
 
 def _parse_xml(path: str, processor: BlockInteriorProcessor, super_callback: Callable[[dict], None]):
     """
     Parse the XML file into a list of JSON objects.
     :param path: the path of the XML file
@@ -361,14 +383,16 @@
     with open(path, 'rb') as xml_file:
         xmltodict.parse(
             xml_file,
             item_depth=processor.read_depth,
             item_callback=lambda x, y: _xml_parser_callback(x, y, processor, super_callback)
         )
 
+        logging.debug(f'Parsing done: {path}')
+
 
 def _store_article_to_jsonl(article: dict, output_path: str):
     """
     Store the blocks to a JSONL file.
     :param article: the article to store
     :param output_path: the path to store the JSONL file
     :return: the list of JSONL file paths
```

### Comparing `twb_project-0.7.2/twb/decompressor.py` & `twb_project-0.7.3a0/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/twb/downloader.py` & `twb_project-0.7.3a0/twb/downloader.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/twb/logger.py` & `twb_project-0.7.3a0/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/twb/modifier.py` & `twb_project-0.7.3a0/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-0.7.2/twb/parallelization.py` & `twb_project-0.7.3a0/twb/parallelization.py`

 * *Files 16% similar despite different names*

```diff
@@ -79,59 +79,14 @@
                     self.logerr(f'Temporary directory ({prev_temporary_dir}) for current pid is undeleted!')
                     cleanup_dir(prev_temporary_dir)
             self.pid_map[pid] = temporary_dir
         except Exception as e:
             self.logfatal(f'Failed to register the process: {e}')
             return
 
-        # Count the number of inactive processes being removed. (for logging)
-        dirs_to_be_removed = []
-
-        # Acquire parallel lock so that other processes will not do the same thing again under the same condition.
-        with self.parallel_lock:
-            # We initialize the active process list count when the number of possible processes exceeds the desired
-            # number of processes or when we are already counting the number of active processes.
-            if len(self.active_pids) > 0 or len(self.pid_map.keys()) > self.num_proc:
-                try:
-                    if pid in self.active_pids:
-                        self.active_pids.remove(pid)
-                    self.active_pids.append(pid)
-                except Exception as e:
-                    self.logfatal(f'Failed to update active_pids: {e}')
-                    return
-
-                # Remove the inactive processes when the number of active processes reaches the desired number.
-                if len(self.active_pids) >= self.num_proc:
-                    try:
-                        self.logwarn('Scanning inactive processes...')
-                        inactive_pids = set(self.pid_map.keys()) - set(self.active_pids)
-                        for inactive_pid in inactive_pids:
-                            temp_folder = self.pid_map[inactive_pid]
-                            if os.path.exists(temp_folder):
-                                dirs_to_be_removed.append((inactive_pid, temp_folder))
-                            del self.pid_map[inactive_pid]
-                        # Clear the active process list for preparation of the next possible leak.
-                        while len(self.active_pids) > 0:
-                            self.active_pids.pop()
-                    except Exception as e:
-                        self.logfatal(f'Failed to scan inactive processes: {e}')
-                        return
-
-        # Cleanup the temporary directories without lock, so that the lock will not be held for a long time.
-
-        try:
-            if len(dirs_to_be_removed) > 0:
-                self.logwarn(f'Cleaning up {len(dirs_to_be_removed)} inactive processes...')
-            for dir_to_be_removed in dirs_to_be_removed:
-                inactive_pid, broken_dir = dir_to_be_removed
-                self.logwarn(f'Removing temporary directory for pid: {inactive_pid}')
-                cleanup_dir(broken_dir)
-        except Exception as e:
-            self.logfatal(f'Failed to clean up inactive processes: {e}')
-
     def unregister(self):
         """
         Unregister the process.
         """
         try:
             temp_dir = None
             pid = os.getpid()
```

### Comparing `twb_project-0.7.2/twb/reader.py` & `twb_project-0.7.3a0/twb/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,21 +217,27 @@
                     callback=_success_callback,
                     error_callback=_error_callback
                 )
 
             pm.close()
             pm.join()
 
+            twb_logger.info(f'Finished modifying {len(line_positions)} blocks. Compressing...')
+
             # Compress the file.
             output_path = os.path.join(output_dir, os.path.basename(target_path) + COMPRESSION_EXTENSION)
             compress_zstd(target_path, output_path)
 
+            twb_logger.info(f'Finished compressing. Cleaning up...')
+
             # Clean up the temporary directory at this step.
             cleanup_dir(temp_dir)
 
+            twb_logger.info(f'Finished cleaning up.')
+
             file_end_time = time.time()
             file_execution_duration = file_end_time - file_start_time
 
             twb_logger.info(f'Finished: {file_path} -- (took {file_execution_duration:.2f}s)')
 
             # Log the progress.
             curr_count += 1
```

### Comparing `twb_project-0.7.2/twb/utils.py` & `twb_project-0.7.3a0/twb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     else:
         return os.path.getsize(path) * 2
 
 
 def get_memory_consumption() -> int:
     process = psutil.Process(os.getpid())
     memory_usage_mb = process.memory_info().rss / 1024 / 1024
-    return round(memory_usage_mb, 3)
+    return round(memory_usage_mb, 2)
 
 
 def get_line_positions(path: str):
     """
     Get all line positions in the given file. So that it could be re-used to read the file for a specific line.
     """
     line_positions = []
```

### Comparing `twb_project-0.7.2/setup.py` & `twb_project-0.7.3a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 packages = \
 ['twb']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beautifulsoup4>=4.11.2,<5.0.0',
+['beautifulsoup4>=4.12.2,<5.0.0',
  'jsonlines>=3.1.0,<4.0.0',
- 'psutil>=5.9.4,<6.0.0',
- 'py7zr>=0.20.4,<0.21.0',
+ 'psutil>=5.9.5,<6.0.0',
+ 'py7zr>=0.20.5,<0.21.0',
  'requests>=2.28.2,<3.0.0',
  'xmltodict>=0.13.0,<0.14.0',
- 'zstandard>=0.20.0,<0.21.0']
+ 'zstandard>=0.21.0,<0.22.0']
 
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '0.7.2',
+    'version': '0.7.3a0',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
     'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
```

### Comparing `twb_project-0.7.2/PKG-INFO` & `twb_project-0.7.3a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 0.7.2
+Version: 0.7.3a0
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: py7zr (>=0.20.4,<0.21.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: py7zr (>=0.20.5,<0.21.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
-Requires-Dist: zstandard (>=0.20.0,<0.21.0)
+Requires-Dist: zstandard (>=0.21.0,<0.22.0)
 Project-URL: Documentation, https://twb.lingxi.li/docs/
 Project-URL: Repository, https://github.com/lilingxi01/twb-project
 Description-Content-Type: text/markdown
 
 <img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />
 
 # Temporal Wikipedia Blocks (TWB)
```

