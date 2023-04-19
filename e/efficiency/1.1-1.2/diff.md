# Comparing `tmp/efficiency-1.1.tar.gz` & `tmp/efficiency-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficiency-1.1.tar", last modified: Tue Aug 23 06:25:28 2022, max compression
+gzip compressed data, was "efficiency-1.2.tar", last modified: Wed Apr 19 16:43:12 2023, max compression
```

## Comparing `efficiency-1.1.tar` & `efficiency-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2022-08-23 06:25:28.000000 efficiency-1.1/
--rw-r--r--   0 zjin      (7600) is        (1040)     1079 2022-08-23 06:17:41.000000 efficiency-1.1/LICENSE.txt
--rw-r--r--   0 zjin      (7600) is        (1040)     1913 2022-08-23 06:25:28.000000 efficiency-1.1/PKG-INFO
--rw-r--r--   0 zjin      (7600) is        (1040)     1612 2022-08-23 06:17:41.000000 efficiency-1.1/README.md
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2022-08-23 06:25:28.000000 efficiency-1.1/efficiency/
--rw-r--r--   0 zjin      (7600) is        (1040)      201 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/__init__.py
--rw-r--r--   0 zjin      (7600) is        (1040)     1011 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/file_manager.py
--rw-r--r--   0 zjin      (7600) is        (1040)     6584 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/function.py
--rw-r--r--   0 zjin      (7600) is        (1040)    10998 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/log.py
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2022-08-23 06:25:28.000000 efficiency-1.1/efficiency/mt/
--rw-r--r--   0 zjin      (7600) is        (1040)       55 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/mt/__init__.py
--rw-r--r--   0 zjin      (7600) is        (1040)     5695 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/mt/loss_plot.py
--rw-r--r--   0 zjin      (7600) is        (1040)     5695 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/mt/tensorboard_logging.py
--rw-r--r--   0 zjin      (7600) is        (1040)     1480 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/nlp.py
--rw-r--r--   0 zjin      (7600) is        (1040)     9206 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/plotter.py
--rw-r--r--   0 zjin      (7600) is        (1040)      520 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/record.py
--rw-r--r--   0 zjin      (7600) is        (1040)    11694 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/text.py
--rw-r--r--   0 zjin      (7600) is        (1040)      573 2022-08-23 06:17:41.000000 efficiency-1.1/efficiency/web.py
-drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2022-08-23 06:25:28.000000 efficiency-1.1/efficiency.egg-info/
--rw-r--r--   0 zjin      (7600) is        (1040)     1913 2022-08-23 06:25:25.000000 efficiency-1.1/efficiency.egg-info/PKG-INFO
--rw-r--r--   0 zjin      (7600) is        (1040)      488 2022-08-23 06:25:28.000000 efficiency-1.1/efficiency.egg-info/SOURCES.txt
--rw-r--r--   0 zjin      (7600) is        (1040)        1 2022-08-23 06:25:26.000000 efficiency-1.1/efficiency.egg-info/dependency_links.txt
--rw-r--r--   0 zjin      (7600) is        (1040)        6 2022-08-23 06:25:26.000000 efficiency-1.1/efficiency.egg-info/requires.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       11 2022-08-23 06:25:27.000000 efficiency-1.1/efficiency.egg-info/top_level.txt
--rw-r--r--   0 zjin      (7600) is        (1040)       79 2022-08-23 06:25:28.000000 efficiency-1.1/setup.cfg
--rw-r--r--   0 zjin      (7600) is        (1040)      517 2022-08-23 06:24:33.000000 efficiency-1.1/setup.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/
+-rw-r--r--   0 zjin      (7600) is        (1040)     1079 2023-04-19 16:43:03.000000 efficiency-1.2/LICENSE.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)     1862 2023-04-19 16:43:12.649815 efficiency-1.2/PKG-INFO
+-rw-r--r--   0 zjin      (7600) is        (1040)     1612 2023-04-19 16:43:03.000000 efficiency-1.2/README.md
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/efficiency/
+-rw-r--r--   0 zjin      (7600) is        (1040)      201 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/__init__.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     1011 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/file_manager.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     6584 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/function.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    12306 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/log.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/efficiency/mt/
+-rw-r--r--   0 zjin      (7600) is        (1040)       55 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/mt/__init__.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/mt/loss_plot.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     5695 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/mt/tensorboard_logging.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     8294 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/nlp.py
+-rw-r--r--   0 zjin      (7600) is        (1040)     9206 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/plotter.py
+-rw-r--r--   0 zjin      (7600) is        (1040)      520 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/record.py
+-rw-r--r--   0 zjin      (7600) is        (1040)    11694 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/text.py
+-rw-r--r--   0 zjin      (7600) is        (1040)      573 2023-04-19 16:43:03.000000 efficiency-1.2/efficiency/web.py
+drwxr-xr-x   0 zjin      (7600) is        (1040)        0 2023-04-19 16:43:12.649815 efficiency-1.2/efficiency.egg-info/
+-rw-r--r--   0 zjin      (7600) is        (1040)     1862 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/PKG-INFO
+-rw-r--r--   0 zjin      (7600) is        (1040)      488 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/SOURCES.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)        1 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/dependency_links.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       24 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/requires.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       11 2023-04-19 16:43:12.000000 efficiency-1.2/efficiency.egg-info/top_level.txt
+-rw-r--r--   0 zjin      (7600) is        (1040)       79 2023-04-19 16:43:12.649815 efficiency-1.2/setup.cfg
+-rw-r--r--   0 zjin      (7600) is        (1040)      507 2023-04-19 16:43:03.000000 efficiency-1.2/setup.py
```

### Comparing `efficiency-1.1/LICENSE.txt` & `efficiency-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/PKG-INFO` & `efficiency-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: efficiency
-Version: 1.1
+Version: 1.2
 Summary: A package for efficient programming
 Home-page: https://github.com/zhijing-jin/efficiency
-Author: Z
-Author-email: zhijing.jin@connect.hku.hk
+Author: Zhijing Jin
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # efficiency
 [![Pypi](https://img.shields.io/pypi/v/efficiency.svg)](https://pypi.org/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency)](https://pepy.tech/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency/month)](https://pepy.tech/project/efficiency/month)
@@ -62,9 +60,7 @@
 ## Useful Functions
 ```python
 >>> from efficiency.function import shell
 >>> stdout, stderr = shell("cat temp.txt")
 >>> stdout
 b'This is handy!'
 ```
-
-
```

### Comparing `efficiency-1.1/README.md` & `efficiency-1.2/README.md`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/file_manager.py` & `efficiency-1.2/efficiency/file_manager.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/function.py` & `efficiency-1.2/efficiency/function.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/log.py` & `efficiency-1.2/efficiency/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 def get_total_num_lines_in_large_files(file_list, verbose=True, return_each_file2num_lines=False):
     from efficiency.function import shell
     file2num_lines = {}
     for f in sorted(file_list):
         cmd = "wc -l {} | cut -d ' ' -f 1".format(f)
-        stdout, stderr = shell(cmd)
+        stdout, stderr = shell(cmd, verbose=False)
         num_lines = int(stdout)
         file2num_lines[f] = num_lines
         if verbose:
             from efficiency.log import show_var
             show_var(['cmd', 'num_lines'], joiner='\t')
 
     if return_each_file2num_lines:
@@ -174,25 +174,43 @@
 
     text = json.dumps(new_data, cls=_NoIndentEncoder, sort_keys=True, indent=2)
     if file_path:
         (text, file_path)
     return text
 
 
-def fwrite(new_doc, path, mode='w', no_overwrite=False, verbose=False):
+def fwrite(new_doc, path, mode='w', no_overwrite=False, mkdir=True, verbose=False):
     import os
     if not path:
         print("[Info] Path does not exist in fwrite():", str(path))
         return
     if no_overwrite and os.path.isfile(path):
         print("[Error] pls choose whether to continue, as file already exists:",
               path)
         import pdb
         pdb.set_trace()
         return
+
+    from pathlib import Path
+    path_in_os = Path(path)
+    folder = path_in_os.parent
+
+    if mkdir:
+        if not os.path.isdir(folder):
+            if verbose:
+                print('[Info] Establishing new folder: ' + str(folder))
+            folder.mkdir(parents=True, exist_ok=True)
+    else:
+        import os
+        if not os.path.exists():
+            print("[Error] The parent folder does not exist: " + str(folder))
+            import pdb
+            pdb.set_trace()
+            return
+
     if verbose:
         try:
             import ast
             data = ast.literal_eval(new_doc)
             if isinstance(data, dict) or isinstance(data, list):
                 length = len(data)
                 print('[Info] Writing {} samples into {}'.format(length, path))
@@ -201,32 +219,35 @@
             print('[Info] Writing {} lines into {}'.format(length, path))
 
     with open(path, mode) as f:
         f.write(new_doc)
 
 
 def fread(path, if_strip=False, delete_empty=False, csv2list_or_dict='dict', encoding='utf-8', return_df=False,
-          verbose=True):
+          verbose=True, if_empty_return=[]):
     from efficiency.log import show_time
 
     if verbose:
         show_time('[Info] Starting to read file: ' + path)
+    if not os.path.isfile(path):
+        print('[Warn] This file does not exist: ' + path)
+        return if_empty_return
+
     if path.endswith('.jsonl'):
         if verbose: print('[Info] Reading the file in jsonl format')
         import json
         with open(path) as f:
             data = []
             for line_ix, line in enumerate(f):
                 try:
                     data_line = json.loads(line)
+                    data.append(data_line)
                 except:
                     import pdb;
                     pdb.set_trace()
-                    data_line = None
-                data.append(data_line)
 
             # [json.loads(line) for line in f]
 
     elif path.endswith('.json'):
         import json
         with open(path) as f:
             data = json.load(f)
@@ -256,40 +277,57 @@
             data = [line.strip() for line in data]
 
     if delete_empty:
         data = [line for line in data if line]
     if return_df:
         import pandas as pd
         data = pd.DataFrame(data)
+
+    if verbose: show_time(f'[Info] Finished reading {len(data)} samples from the file {path}')
+
     return data
 
 
-def write_rows_to_csv(rows, file, verbose=False):
+def write_rows_to_csv(rows, file, verbose=False, mode='w'):
     if verbose:
         print('[Info] Writing {} lines into {}'.format(len(rows), file))
 
     import csv
-    with open(file, 'w') as f:
+    with open(file, mode) as f:
         writer = csv.writer(f)
         writer.writerows(rows)
 
 
-def write_dict_to_csv(data, file, verbose=False):
+def write_dict_to_csv(data, file, verbose=False, mode='w'):
     if verbose:
         print('[Info] Writing {} lines into {}'.format(len(data), file))
 
     import csv
 
     if not len(data): return
 
     fieldnames = data[0].keys()
-    with open(file, mode='w') as csv_file:
+    lines = fread(file, verbose=False)
+    existing = len(lines) >= 2
+    if existing:
+        fieldnames_existing = lines[0].keys()
+        if set(fieldnames) - set(fieldnames_existing):
+            print(f'[Warn] The existing csv columns ({fieldnames_existing}) are not compatible with the new csv '
+                  f'columns ({fieldnames}).')
+            import pdb;
+            pdb.set_trace()
+        fieldnames = fieldnames_existing
+    with open(file, mode=mode) as csv_file:
         writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
-        writer.writeheader()
+        if not existing: writer.writeheader()
         writer.writerows(data)
+    '''
+    df = pd.DataFrame(data_to_save)
+    df.to_csv(output_file, index=False)
+    '''
 
 
 def show_time(what_happens='', cat_server=False, printout=True):
     import datetime
 
     disp = '⏰ Time: ' + \
            datetime.datetime.now().strftime('%m%d%H%M-%S')
```

### Comparing `efficiency-1.1/efficiency/mt/loss_plot.py` & `efficiency-1.2/efficiency/mt/loss_plot.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/mt/tensorboard_logging.py` & `efficiency-1.2/efficiency/mt/tensorboard_logging.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/plotter.py` & `efficiency-1.2/efficiency/plotter.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/record.py` & `efficiency-1.2/efficiency/record.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/text.py` & `efficiency-1.2/efficiency/text.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency/web.py` & `efficiency-1.2/efficiency/web.py`

 * *Files identical despite different names*

### Comparing `efficiency-1.1/efficiency.egg-info/PKG-INFO` & `efficiency-1.2/efficiency.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: efficiency
-Version: 1.1
+Version: 1.2
 Summary: A package for efficient programming
 Home-page: https://github.com/zhijing-jin/efficiency
-Author: Z
-Author-email: zhijing.jin@connect.hku.hk
+Author: Zhijing Jin
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # efficiency
 [![Pypi](https://img.shields.io/pypi/v/efficiency.svg)](https://pypi.org/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency)](https://pepy.tech/project/efficiency)
 [![Downloads](https://pepy.tech/badge/efficiency/month)](https://pepy.tech/project/efficiency/month)
@@ -62,9 +60,7 @@
 ## Useful Functions
 ```python
 >>> from efficiency.function import shell
 >>> stdout, stderr = shell("cat temp.txt")
 >>> stdout
 b'This is handy!'
 ```
-
-
```

