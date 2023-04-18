# Comparing `tmp/multiuserfilelock-0.0.5.tar.gz` & `tmp/multiuserfilelock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multiuserfilelock-0.0.5.tar", last modified: Tue Nov 23 23:34:09 2021, max compression
+gzip compressed data, was "multiuserfilelock-0.0.7.tar", last modified: Tue Apr 18 23:03:29 2023, max compression
```

## Comparing `multiuserfilelock-0.0.5.tar` & `multiuserfilelock-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1521 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/multiuserfilelock/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3257 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/multiuserfilelock/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/multiuserfilelock/_version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/multiuserfilelock/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/multiuserfilelock/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      640 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/multiuserfilelock/tests/test_acquire.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/multiuserfilelock.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2021-11-23 23:34:08.000000 multiuserfilelock-0.0.5/multiuserfilelock.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-11-23 23:34:08.000000 multiuserfilelock-0.0.5/multiuserfilelock.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-23 23:34:08.000000 multiuserfilelock-0.0.5/multiuserfilelock.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-11-23 23:34:08.000000 multiuserfilelock-0.0.5/multiuserfilelock.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2021-11-23 23:34:08.000000 multiuserfilelock-0.0.5/multiuserfilelock.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      337 2021-11-23 23:34:09.000000 multiuserfilelock-0.0.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      531 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80044 2021-11-23 23:33:36.000000 multiuserfilelock-0.0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:03:29.205746 multiuserfilelock-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 23:03:29.205746 multiuserfilelock-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:03:29.205746 multiuserfilelock-0.0.7/multiuserfilelock/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/multiuserfilelock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 23:03:29.205746 multiuserfilelock-0.0.7/multiuserfilelock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:03:29.205746 multiuserfilelock-0.0.7/multiuserfilelock/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/multiuserfilelock/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/multiuserfilelock/tests/test_acquire.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:03:29.201746 multiuserfilelock-0.0.7/multiuserfilelock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 23:03:29.000000 multiuserfilelock-0.0.7/multiuserfilelock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-18 23:03:29.000000 multiuserfilelock-0.0.7/multiuserfilelock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:03:29.000000 multiuserfilelock-0.0.7/multiuserfilelock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 23:03:29.000000 multiuserfilelock-0.0.7/multiuserfilelock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 23:03:29.000000 multiuserfilelock-0.0.7/multiuserfilelock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-18 23:03:29.205746 multiuserfilelock-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-04-18 23:03:20.000000 multiuserfilelock-0.0.7/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `multiuserfilelock-0.0.5/LICENSE` & `multiuserfilelock-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multiuserfilelock-0.0.5/multiuserfilelock/__init__.py` & `multiuserfilelock-0.0.7/multiuserfilelock/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 __version__ = _version.get_versions()['version']
 
 from filelock import FileLock, Timeout
 import os
 import shutil
 import tempfile
 from pathlib import Path
+import filelock
+from packaging.version import Version
 
 # Creating the locks directly in the /tmp dir on linux causes
 # many problems since the `/tmp` dir has the sticky bit enabled.
 # The sticky bit stops an other user from deleting your file.
 # It seems that this stops some other user from opening a file for
 #
 # We tried to use `SoftFileLock` and while it worked,
@@ -33,18 +35,22 @@
         if os.name == 'nt':
             self._user = None
             self._group = None
         else:
             self._user = user
             self._group = group
         self._chmod = chmod
+
+        if Version(filelock.__version__) >= Version('3.12.0'):
+            kwargs['thread_local'] = False
+
         # Will create a ._lock_file object
         # but will not create the files on the file system
         super().__init__(*args, **kwargs)
-        self._lock_file_path = Path(self._lock_file)
+        self._lock_file_path = Path(self.lock_file)
         parent = self._lock_file_path.parent
         # Even though the "other write" permissions are enabled
         # it seems that the operating systems disables that for the /tmp dir
         parent.mkdir(mode=0o777, parents=True, exist_ok=True)
 
         if self._group is not None and parent.group() != self._group:
             shutil.chown(parent, group=self._group)
```

### Comparing `multiuserfilelock-0.0.5/setup.py` & `multiuserfilelock-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from setuptools import find_packages, setup
 import versioneer
 
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
 
 setup(
     name='multiuserfilelock',
     version=versioneer.get_version(),
     url='https://github.com/ramonaoptics/python-multiuserfilelock',
     author='Ramona Optics, Inc.',
     author_email='info@ramonaoptics.com',
     description='A lock to share resources between users based on filelock.',
+    long_description=readme,
+    long_description_content_type='text/markdown',
     license='BSD',
     python_requires='>=3.7',
     install_requires=[
-        'filelock',
+        'filelock!=3.11.0',
     ],
     packages=find_packages(),
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `multiuserfilelock-0.0.5/versioneer.py` & `multiuserfilelock-0.0.7/versioneer.py`

 * *Files identical despite different names*

