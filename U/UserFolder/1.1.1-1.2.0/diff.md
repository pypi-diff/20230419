# Comparing `tmp/UserFolder-1.1.1.tar.gz` & `tmp/UserFolder-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UserFolder-1.1.1.tar", last modified: Mon Sep 26 20:55:38 2022, max compression
+gzip compressed data, was "UserFolder-1.2.0.tar", last modified: Wed Apr 19 21:34:13 2023, max compression
```

## Comparing `UserFolder-1.1.1.tar` & `UserFolder-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-26 20:55:38.254190 UserFolder-1.1.1/
--rw-rw-rw-   0        0        0     1077 2022-01-20 21:59:27.000000 UserFolder-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     1699 2022-09-26 20:55:38.255190 UserFolder-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      909 2022-09-26 20:53:56.000000 UserFolder-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-09-26 20:55:38.231190 UserFolder-1.1.1/UserFolder/
--rw-rw-rw-   0        0        0    18205 2022-09-26 20:53:36.000000 UserFolder-1.1.1/UserFolder/User.py
--rw-rw-rw-   0        0        0       79 2022-08-21 23:06:03.000000 UserFolder-1.1.1/UserFolder/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-26 20:55:38.253193 UserFolder-1.1.1/UserFolder.egg-info/
--rw-rw-rw-   0        0        0     1699 2022-09-26 20:55:38.000000 UserFolder-1.1.1/UserFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2022-09-26 20:55:38.000000 UserFolder-1.1.1/UserFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-26 20:55:38.000000 UserFolder-1.1.1/UserFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-09-26 20:55:38.000000 UserFolder-1.1.1/UserFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-09-26 20:55:38.000000 UserFolder-1.1.1/UserFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2022-09-26 20:55:38.257190 UserFolder-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1196 2022-09-26 20:53:46.000000 UserFolder-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:34:13.731317 UserFolder-1.2.0/
+-rw-rw-rw-   0        0        0     1077 2022-01-20 21:59:27.000000 UserFolder-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     3334 2023-04-19 21:34:13.731317 UserFolder-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2541 2023-04-19 21:31:39.000000 UserFolder-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 21:34:13.725315 UserFolder-1.2.0/UserFolder/
+-rw-rw-rw-   0        0        0    30589 2023-04-19 21:22:15.000000 UserFolder-1.2.0/UserFolder/__init__.py
+-rw-rw-rw-   0        0        0     5302 2023-04-18 21:09:17.000000 UserFolder-1.2.0/UserFolder/ctkdialog.py
+-rw-rw-rw-   0        0        0     5135 2023-04-18 21:08:52.000000 UserFolder-1.2.0/UserFolder/dialog.py
+drwxrwxrwx   0        0        0        0 2023-04-19 21:34:13.731317 UserFolder-1.2.0/UserFolder.egg-info/
+-rw-rw-rw-   0        0        0     3334 2023-04-19 21:34:13.000000 UserFolder-1.2.0/UserFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-19 21:34:13.000000 UserFolder-1.2.0/UserFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 21:34:13.000000 UserFolder-1.2.0/UserFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 21:34:13.000000 UserFolder-1.2.0/UserFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 21:34:13.000000 UserFolder-1.2.0/UserFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-04-19 21:34:13.732316 UserFolder-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-04-19 21:24:10.000000 UserFolder-1.2.0/setup.py
```

### Comparing `UserFolder-1.1.1/LICENSE.md` & `UserFolder-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `UserFolder-1.1.1/setup.py` & `UserFolder-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 required_modules = ["requests"]
 
 setuptools.setup(
     name='UserFolder',
-    version='1.1.1',
+    version='1.2.0',
     author='Legopitstop',
     description='This library allows you to write and save files to the users folder. Useful for when you convert this script to a onefile exe program.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/legopitstop/UserFolder/',
     packages=setuptools.find_packages(),
     install_requires=required_modules,
@@ -22,9 +22,9 @@
         'Development Status :: 5 - Production/Stable', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python :: 3.9',
     ],
-    python_requires='>=3.6'
+    python_requires='>=3.11'
 )
```

