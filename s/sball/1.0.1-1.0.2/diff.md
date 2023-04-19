# Comparing `tmp/sball-1.0.1.tar.gz` & `tmp/sball-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-1.0.1.tar", last modified: Sat Apr 15 18:13:28 2023, max compression
+gzip compressed data, was "sball-1.0.2.tar", last modified: Wed Apr 19 01:06:04 2023, max compression
```

## Comparing `sball-1.0.1.tar` & `sball-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:28.460538 sball-1.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-15 03:14:00.000000 sball-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4267 2023-04-15 18:13:28.459538 sball-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-1.0.1/README.md
--rw-rw-rw-   0        0        0      632 2023-04-15 18:12:34.000000 sball-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 18:13:28.460538 sball-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:28.423540 sball-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:28.447538 sball-1.0.1/src/sball/
--rw-rw-rw-   0        0        0       38 2023-04-15 18:12:43.000000 sball-1.0.1/src/sball/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-1.0.1/src/sball/__main__.py
--rw-rw-rw-   0        0        0     4974 2023-04-15 18:12:52.000000 sball-1.0.1/src/sball/sball.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:13:28.457542 sball-1.0.1/src/sball.egg-info/
--rw-rw-rw-   0        0        0     4267 2023-04-15 18:13:28.000000 sball-1.0.1/src/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-15 18:13:28.000000 sball-1.0.1/src/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:13:28.000000 sball-1.0.1/src/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-15 18:13:28.000000 sball-1.0.1/src/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 18:13:28.000000 sball-1.0.1/src/sball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 01:06:04.629793 sball-1.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 03:14:00.000000 sball-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4267 2023-04-19 01:06:04.628793 sball-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-1.0.2/README.md
+-rw-rw-rw-   0        0        0      632 2023-04-19 01:03:58.000000 sball-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 01:06:04.629793 sball-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 01:06:04.594794 sball-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 01:06:04.617793 sball-1.0.2/src/sball/
+-rw-rw-rw-   0        0        0       38 2023-04-19 01:04:13.000000 sball-1.0.2/src/sball/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-1.0.2/src/sball/__main__.py
+-rw-rw-rw-   0        0        0     5042 2023-04-19 01:05:17.000000 sball-1.0.2/src/sball/sball.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:06:04.626796 sball-1.0.2/src/sball.egg-info/
+-rw-rw-rw-   0        0        0     4267 2023-04-19 01:06:04.000000 sball-1.0.2/src/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-19 01:06:04.000000 sball-1.0.2/src/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:06:04.000000 sball-1.0.2/src/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-19 01:06:04.000000 sball-1.0.2/src/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 01:06:04.000000 sball-1.0.2/src/sball.egg-info/top_level.txt
```

### Comparing `sball-1.0.1/LICENSE` & `sball-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sball-1.0.1/PKG-INFO` & `sball-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 1.0.1
+Version: 1.0.2
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sball-1.0.1/README.md` & `sball-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sball-1.0.1/pyproject.toml` & `sball-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires=['setuptools', 'wheel']
 build-backend='setuptools.build_meta'
 
 [project]
 name='sball'
-version='1.0.1'
+version='1.0.2'
 description="Submit scripts in job arrays using Yale's dSQ."
 readme='README.md'
 authors=[{name="Michael Wilson", email='michael.a.wilson@yale.edu'}]
 classifiers=[
 	'Development Status :: 4 - Beta',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
```

### Comparing `sball-1.0.1/src/sball/sball.py` & `sball-1.0.2/src/sball/sball.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,23 +82,27 @@
 			'--status-dir', log_dir + os.path.sep,
 			'--job-name', name + formatter,
 			'--output', os.path.join(log_dir, name + formatter + '-%A_%a.txt'),
 			'--batch-file', os.path.join(dirname, name + formatter + '.sh'),
 			*options, 
 			*args
 		], stdout=subprocess.DEVNULL)
-		time.sleep(2)
+		while x.poll() is None:
+			time.sleep(0.5)
+		
 		x.kill()
 		
 		x = subprocess.Popen([
 			'sbatch',
 			*args,
 			os.path.join(dirname, name + formatter + '.sh')
 		])
-		time.sleep(1)
+		while x.poll() is None:
+			time.sleep(0.5)
+		
 		x.kill()
 		
 		# os.remove(joblist_file)
 		os.remove(os.path.join(dirname, name + formatter + '.sh'))
 
 def sbatch_all(s):
 	'''
```

### Comparing `sball-1.0.1/src/sball.egg-info/PKG-INFO` & `sball-1.0.2/src/sball.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 1.0.1
+Version: 1.0.2
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

