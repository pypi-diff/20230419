# Comparing `tmp/al2var-0.0.3.tar.gz` & `tmp/al2var-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-mcf2_zq_/al2var-0.0.3.tar", last modified: Wed Apr 19 02:46:26 2023, max compression
+gzip compressed data, was "/Users/hendrixj/Dropbox/subDrop/devel_al2var/forPypi/dist/.tmp-0lxy4i09/al2var-0.0.4.tar", last modified: Wed Apr 19 02:48:44 2023, max compression
```

## Comparing `al2var-0.0.3.tar` & `al2var-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 02:46:26.501597 al2var-0.0.3/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.3/LICENSE
--rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.3/MANIFEST.in
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-04-19 02:46:26.501826 al2var-0.0.3/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310     6499 2023-04-19 02:14:41.000000 al2var-0.0.3/README.md
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 02:46:26.499547 al2var-0.0.3/al2var.egg-info/
--rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-04-19 02:46:26.000000 al2var-0.0.3/al2var.egg-info/PKG-INFO
--rw-r--r--   0 hendrixj (1692218720) 1934156310      208 2023-04-19 02:46:26.000000 al2var-0.0.3/al2var.egg-info/SOURCES.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-04-19 02:46:26.000000 al2var-0.0.3/al2var.egg-info/dependency_links.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310       32 2023-04-19 02:46:26.000000 al2var-0.0.3/al2var.egg-info/requires.txt
--rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-04-19 02:46:26.000000 al2var-0.0.3/al2var.egg-info/top_level.txt
-drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 02:46:26.500345 al2var-0.0.3/bin/
--rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.3/bin/al2var
--rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-04-19 02:46:26.502618 al2var-0.0.3/setup.cfg
--rw-r--r--   0 hendrixj (1692218720) 1934156310      866 2023-04-19 02:46:01.000000 al2var-0.0.3/setup.py
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 02:48:44.310681 al2var-0.0.4/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     1122 2022-10-08 19:49:45.000000 al2var-0.0.4/LICENSE
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       17 2022-10-10 23:15:11.000000 al2var-0.0.4/MANIFEST.in
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-04-19 02:48:44.310850 al2var-0.0.4/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     6499 2023-04-19 02:14:41.000000 al2var-0.0.4/README.md
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 02:48:44.309199 al2var-0.0.4/al2var.egg-info/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310     7024 2023-04-19 02:48:44.000000 al2var-0.0.4/al2var.egg-info/PKG-INFO
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      208 2023-04-19 02:48:44.000000 al2var-0.0.4/al2var.egg-info/SOURCES.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-04-19 02:48:44.000000 al2var-0.0.4/al2var.egg-info/dependency_links.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       33 2023-04-19 02:48:44.000000 al2var-0.0.4/al2var.egg-info/requires.txt
+-rw-r--r--   0 hendrixj (1692218720) 1934156310        1 2023-04-19 02:48:44.000000 al2var-0.0.4/al2var.egg-info/top_level.txt
+drwxr-xr-x   0 hendrixj (1692218720) 1934156310        0 2023-04-19 02:48:44.309652 al2var-0.0.4/bin/
+-rw-r--r--   0 hendrixj (1692218720) 1934156310    17784 2023-04-19 02:27:23.000000 al2var-0.0.4/bin/al2var
+-rw-r--r--   0 hendrixj (1692218720) 1934156310       38 2023-04-19 02:48:44.311452 al2var-0.0.4/setup.cfg
+-rw-r--r--   0 hendrixj (1692218720) 1934156310      867 2023-04-19 02:48:26.000000 al2var-0.0.4/setup.py
```

### Comparing `al2var-0.0.3/LICENSE` & `al2var-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `al2var-0.0.3/PKG-INFO` & `al2var-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.3
+Version: 0.0.4
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `al2var-0.0.3/README.md` & `al2var-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `al2var-0.0.3/al2var.egg-info/PKG-INFO` & `al2var-0.0.4/al2var.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: al2var
-Version: 0.0.3
+Version: 0.0.4
 Summary: Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence
 Home-page: https://github.com/jrhendrix/al2var
 Author: Jo Hendrix
 Author-email: jrhendrix36@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `al2var-0.0.3/bin/al2var` & `al2var-0.0.4/bin/al2var`

 * *Files identical despite different names*

### Comparing `al2var-0.0.3/setup.py` & `al2var-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="al2var",
-    version="0.0.3",
+    version="0.0.4",
     author="Jo Hendrix",
     author_email="jrhendrix36@gmail.com",
     description="Identify and calculate find variant rate between a bacterial genome sequence and either paired-end reads or another genome sequence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jrhendrix/al2var",
     scripts=['bin/al2var'],
     packages=setuptools.find_packages(),
     include_package_data=True,
-    install_requires=['bcftools', 'samtools', 'bowtie2', 'mappy'],
+    install_requires=['bcftools', 'xsamtools', 'bowtie2', 'mappy'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
 )
```

