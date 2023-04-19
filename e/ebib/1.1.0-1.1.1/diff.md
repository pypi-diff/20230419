# Comparing `tmp/ebib-1.1.0.tar.gz` & `tmp/ebib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebib-1.1.0.tar", last modified: Wed Apr 19 16:50:44 2023, max compression
+gzip compressed data, was "ebib-1.1.1.tar", last modified: Wed Apr 19 17:22:36 2023, max compression
```

## Comparing `ebib-1.1.0.tar` & `ebib-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.1.0/LICENSE
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 16:50:44.718486 ebib-1.1.0/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.1.0/README.md
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/ebib/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.1.0/ebib/__init__.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/ebib/assets/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.1.0/ebib/assets/english-stemmer.js
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 16:37:29.000000 ebib-1.1.0/ebib/assets/index.html
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5967 2023-04-19 16:35:50.000000 ebib-1.1.0/ebib/assets/index.js
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5815 2023-04-19 16:45:20.000000 ebib-1.1.0/ebib/cli.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.1.0/ebib/english_stemmer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.1.0/ebib/indexer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.1.0/ebib/lexer.py
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-12 12:47:10.000000 ebib-1.1.0/ebib/utils.py
-drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 16:50:44.718486 ebib-1.1.0/ebib.egg-info/
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/PKG-INFO
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      374 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/SOURCES.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/dependency_links.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/entry_points.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/requires.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 16:50:44.000000 ebib-1.1.0/ebib.egg-info/top_level.txt
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)      609 2023-04-19 16:47:40.000000 ebib-1.1.0/pyproject.toml
--rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 16:50:44.718486 ebib-1.1.0/setup.cfg
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:22:36.212543 ebib-1.1.1/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    35149 2023-03-30 01:00:35.000000 ebib-1.1.1/LICENSE
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 17:22:36.212543 ebib-1.1.1/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      241 2023-03-29 13:24:13.000000 ebib-1.1.1/README.md
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:22:36.212543 ebib-1.1.1/ebib/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      775 2023-04-12 12:47:10.000000 ebib-1.1.1/ebib/__init__.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:22:36.212543 ebib-1.1.1/ebib/assets/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    38403 2023-04-19 12:43:51.000000 ebib-1.1.1/ebib/assets/english-stemmer.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     3798 2023-04-19 16:37:29.000000 ebib-1.1.1/ebib/assets/index.html
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5967 2023-04-19 16:35:50.000000 ebib-1.1.1/ebib/assets/index.js
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5930 2023-04-19 17:10:16.000000 ebib-1.1.1/ebib/cli.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)    32769 2023-03-30 01:11:34.000000 ebib-1.1.1/ebib/english_stemmer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     5703 2023-04-19 13:23:21.000000 ebib-1.1.1/ebib/indexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1576 2023-04-19 13:21:21.000000 ebib-1.1.1/ebib/lexer.py
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)     1137 2023-04-19 17:10:28.000000 ebib-1.1.1/ebib/utils.py
+drwxr-xr-x   0 ernesto   (1000) ernesto   (1000)        0 2023-04-19 17:22:36.212543 ebib-1.1.1/ebib.egg-info/
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      635 2023-04-19 17:22:36.000000 ebib-1.1.1/ebib.egg-info/PKG-INFO
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      374 2023-04-19 17:22:36.000000 ebib-1.1.1/ebib.egg-info/SOURCES.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        1 2023-04-19 17:22:36.000000 ebib-1.1.1/ebib.egg-info/dependency_links.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 17:22:36.000000 ebib-1.1.1/ebib.egg-info/entry_points.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       23 2023-04-19 17:22:36.000000 ebib-1.1.1/ebib.egg-info/requires.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)        5 2023-04-19 17:22:36.000000 ebib-1.1.1/ebib.egg-info/top_level.txt
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)      609 2023-04-19 17:19:40.000000 ebib-1.1.1/pyproject.toml
+-rw-r--r--   0 ernesto   (1000) ernesto   (1000)       38 2023-04-19 17:22:36.212543 ebib-1.1.1/setup.cfg
```

### Comparing `ebib-1.1.0/LICENSE` & `ebib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/PKG-INFO` & `ebib-1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 1.1.0
+Version: 1.1.1
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-1.1.0/ebib/__init__.py` & `ebib-1.1.1/ebib/__init__.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/assets/english-stemmer.js` & `ebib-1.1.1/ebib/assets/english-stemmer.js`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/assets/index.html` & `ebib-1.1.1/ebib/assets/index.html`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/assets/index.js` & `ebib-1.1.1/ebib/assets/index.js`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/cli.py` & `ebib-1.1.1/ebib/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,14 +140,18 @@
 	run_command(['git', 'commit', '-m', 'Added tag' + ('s' if len(tags) > 0 else '') + ' ' + mtags + ' to ' + filename + '.pdf'])
 	print(['git', 'commit', '-m', 'Added tag' + ('s' if len(tags) > 0 else '') + ' ' + mtags + ' to ' + filename + '.pdf'])
 
 @click.command()
 @click.argument('name')
 @click.option('--gitlab', is_flag = True, help = 'Include gitlab ci')
 def init(name, gitlab):
+	info_ebib = Path('info.ebib')
+	if info_ebib.is_file():
+		print('ERROR: Repository already Initialized')
+		exit(1)
 	run_command(['git', 'init'])
 	ebib_info = {'name': name, 'pdfs': {}}
 	save_info(ebib_info)
 	with open('.gitignore', 'w') as f:
 		f.write('public')
 	if gitlab:
 		shutil.copy2(files('ebib/assets/').joinpath('.gitlab-ci.yml'), '.')
```

### Comparing `ebib-1.1.0/ebib/english_stemmer.py` & `ebib-1.1.1/ebib/english_stemmer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/indexer.py` & `ebib-1.1.1/ebib/indexer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/lexer.py` & `ebib-1.1.1/ebib/lexer.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib/utils.py` & `ebib-1.1.1/ebib/utils.py`

 * *Files identical despite different names*

### Comparing `ebib-1.1.0/ebib.egg-info/PKG-INFO` & `ebib-1.1.1/ebib.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebib
-Version: 1.1.0
+Version: 1.1.1
 Summary: ebib is a bibliography manager system aimed to work with Gitlab/Github pages
 Author-email: Ernesto Lanchares <elancha98@gmail.com>
 Project-URL: Homepage, https://gitlab.com/elancha/ebib
 Project-URL: Bug Tracker, https://gitlab.com/elancha/ebib/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ebib-1.1.0/pyproject.toml` & `ebib-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ebib"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
 	{ name = "Ernesto Lanchares", email = "elancha98@gmail.com" },
 ]
 description = "ebib is a bibliography manager system aimed to work with Gitlab/Github pages"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["Click", "requests", "pymupdf"]
```

