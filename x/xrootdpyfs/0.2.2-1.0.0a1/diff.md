# Comparing `tmp/xrootdpyfs-0.2.2.tar.gz` & `tmp/xrootdpyfs-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xrootdpyfs-0.2.2.tar", last modified: Mon Dec 13 10:02:03 2021, max compression
+gzip compressed data, was "xrootdpyfs-1.0.0a1.tar", last modified: Wed Apr 19 14:37:49 2023, max compression
```

## Comparing `xrootdpyfs-0.2.2.tar` & `xrootdpyfs-1.0.0a1.tar`

### file list

```diff
@@ -1,45 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/CHANGES
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)      471 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/run-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    10160 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7425 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/xrootdpyfs/
--rw-r--r--   0 runner    (1001) docker     (121)     5222 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14709 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/xrdfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    26778 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/fs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/opener.py
--rw-r--r--   0 runner    (1001) docker     (121)     2254 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/xrootdpyfs/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    37319 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_xrdfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_fs_extras.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3425 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_xrdflags.py
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/perf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    25653 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/test_opener.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 10:02:02.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-13 10:02:02.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-13 10:02:02.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4731 2021-12-13 10:02:02.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-12-13 10:02:02.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-12-13 10:02:03.000000 xrootdpyfs-0.2.2/xrootdpyfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3258 2021-12-13 10:01:55.000000 xrootdpyfs-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.918159 xrootdpyfs-1.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      891 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1487 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-19 14:37:49.918159 xrootdpyfs-1.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3718 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7425 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/run-docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      402 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-04-19 14:37:49.918159 xrootdpyfs-1.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      640 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/data/afolder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/afolder/afile.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/tests/data/bfolder/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/bfolder/bfile.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)       10 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/binary.dat
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/multiline.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/data/testa.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2778 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/perf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25647 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_fs_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_opener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2100 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37201 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_xrdfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3366 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/tests/test_xrdflags.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/xrootdpyfs/
+-rw-r--r--   0 runner    (1001) docker     (122)     5188 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/env.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28590 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/fs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1534 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/opener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1631 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14539 2023-04-19 14:37:44.000000 xrootdpyfs-1.0.0a1/xrootdpyfs/xrdfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:37:49.914159 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-19 14:37:49.000000 xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xrootdpyfs-0.2.2/.github/workflows/pypi-publish.yml` & `xrootdpyfs-1.0.0a1/.github/workflows/pypi-publish.yml`

 * *Files 23% similar despite different names*

```diff
@@ -14,20 +14,20 @@
       - v*
 
 jobs:
   Publish:
     runs-on: ubuntu-20.04
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: 3.6
+          python-version: 3.9
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel
 
       - name: Build package
```

### Comparing `xrootdpyfs-0.2.2/.github/workflows/tests.yml` & `xrootdpyfs-1.0.0a1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-0.2.2/CHANGES` & `xrootdpyfs-1.0.0a1/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changes
 =======
 
+Version 1.0.0a1 (released 2023-04-19)
+
+- Upgrade pyfs to version 2.
+- Improve module's files organization and code formatting.
+
 Version 0.2.2 (released 2021-12-13)
 
 - Supports `xrootd@4.12.7`
 - Adds GH publish flow
 - Fixes tests with python 3
 - Adds `__len__` method in `XRootDPyFile`
```

### Comparing `xrootdpyfs-0.2.2/LICENSE` & `xrootdpyfs-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-0.2.2/docs/conf.py` & `xrootdpyfs-1.0.0a1/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,309 +8,305 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import re
-import shlex
-import sys
+from xrootdpyfs import __version__
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.insert(0, os.path.abspath('.'))
+# sys.path.insert(0, os.path.abspath('.'))
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
+    "sphinx.ext.intersphinx",
     # 'sphinx.ext.coverage',
-    'sphinx.ext.viewcode',
+    "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'XRootDPyFS'
-copyright = u'2015, Invenio Collaboration'
-author = u'Invenio Collaboration'
+project = "XRootDPyFS"
+copyright = "2015, Invenio Collaboration"
+author = "Invenio Collaboration"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-# Get the version string. Cannot be done with import!
-with open(os.path.join('..', 'xrootdpyfs', 'version.py'), 'rt') as f:
-    version = re.search(
-        '__version__\s*=\s*"(?P<version>.*)"\n',
-        f.read()
-    ).group('version')
+version = __version__
 
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
-#keep_warnings = False
+# keep_warnings = False
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
-    'description': 'XRootDPyFS is a PyFilesystem interface for XRootD.',
-    'github_user': 'inveniosoftware',
-    'github_repo': 'xrootdpyfs',
-    'github_button': False,
-    'github_banner': True,
-    'show_powered_by': False,
-    'extra_nav_links': {
-        'xrootdpyfs@GitHub': 'http://github.com/inveniosoftware/xrootdpyfs/',
-        'xrootdpyfs@PyPI': 'http://pypi.python.org/pypi/xrootdpyfs/',
-    }
+    "description": "XRootDPyFS is a PyFilesystem interface for XRootD.",
+    "github_user": "inveniosoftware",
+    "github_repo": "xrootdpyfs",
+    "github_button": False,
+    "github_banner": True,
+    "show_powered_by": False,
+    "extra_nav_links": {
+        "xrootdpyfs@GitHub": "http://github.com/inveniosoftware/xrootdpyfs/",
+        "xrootdpyfs@PyPI": "http://pypi.python.org/pypi/xrootdpyfs/",
+    },
 }
 
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+# html_logo = None
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
-#html_extra_path = []
+# html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
 
 # Language to be used for generating the HTML full-text search index.
 # Sphinx supports the following languages:
 #   'da', 'de', 'en', 'es', 'fi', 'fr', 'hu', 'it', 'ja'
 #   'nl', 'no', 'pt', 'ro', 'ru', 'sv', 'tr'
-#html_search_language = 'en'
+# html_search_language = 'en'
 
 # A dictionary with options for the search language support, empty by default.
 # Now only 'ja' uses this config value
-#html_search_options = {'type': 'default'}
+# html_search_options = {'type': 'default'}
 
 # The name of a javascript file (relative to the configuration directory) that
 # implements a search results scorer. If empty, the default will be used.
-#html_search_scorer = 'scorer.js'
+# html_search_scorer = 'scorer.js'
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'XRootDPyFSdoc'
+htmlhelp_basename = "XRootDPyFSdoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
-
-# Latex figure (float) alignment
-#'figure_align': 'htbp',
+    # The paper size ('letterpaper' or 'a4paper').
+    #'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #'preamble': '',
+    # Latex figure (float) alignment
+    #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'XRootDPyFS.tex', u'XRootDPyFS Documentation',
-   u'Invenio Collaboration', 'manual'),
+    (
+        master_doc,
+        "XRootDPyFS.tex",
+        "XRootDPyFS Documentation",
+        "Invenio Collaboration",
+        "manual",
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+# latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+# latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+# latex_show_pagerefs = False
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+# latex_show_urls = False
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'xrootdpyfs', u'XRootDPyFS Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "xrootdpyfs", "XRootDPyFS Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'XRootDPyFS', u'XRootDPyFS Documentation',
-   author, 'XRootDPyFS', 'One line description of project.',
-   'Miscellaneous'),
+    (
+        master_doc,
+        "XRootDPyFS",
+        "XRootDPyFS Documentation",
+        author,
+        "XRootDPyFS",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
-#texinfo_no_detailmenu = False
+# texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/', None),
+    "python": ("https://docs.python.org/", None),
 }
-
```

### Comparing `xrootdpyfs-0.2.2/docs/Makefile` & `xrootdpyfs-1.0.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-0.2.2/docs/index.rst` & `xrootdpyfs-1.0.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xrootdpyfs-0.2.2/xrootdpyfs/__init__.py` & `xrootdpyfs-1.0.0a1/xrootdpyfs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,45 +147,45 @@
     ['test.txt']
 
 Or, alternatively using the PyFilesystem opener (note the first
 ``import xrootdpyfs`` is required to ensure the XRootDPyFS
 opener is registered):
 
     >>> import xrootdpyfs
-    >>> from fs.opener import opener
-    >>> fs, path = opener.parse("root://localhost//tmp/")
+    >>> from fs.opener import open_fs
+    >>> fs = open_fs("root://localhost//tmp/")
     >>> fs.listdir("xrootdpyfs")
     ['test.txt']
 
 Reading files:
 
     >>> f = fs.open("xrootdpyfs/test.txt")
     >>> f.read()
     b'Hello XRootD!\n'
     >>> f.close()
 
-Reading files using the ``getcontents()`` method:
+Reading files using the ``readtext()`` method:
 
-    >>> fs.getcontents("xrootdpyfs/test.txt")
+    >>> fs.readtext("xrootdpyfs/test.txt")
     b'Hello XRootD!\n'
 
 Writing files:
 
     >>> f = fs.open("xrootdpyfs/hello.txt", "w+")
     >>> f.write("World")
     >>> f.close()
 
-Writing files using the ``setcontents()`` method (returns the number of bytes
+Writing files using the ``writetext()`` method (returns the number of bytes
 written):
 
-    >>> fs.setcontents("xrootdpyfs/test.txt", "World")
-    5
+    >>> fs.writetext("xrootdpyfs/test.txt", "World")
+    >>> fs.readtext("xrootdpyfs/test.txt")
+    b'World'
 """
 
-from __future__ import absolute_import, print_function
-
 from .fs import XRootDPyFS
 from .opener import XRootDPyOpener
-from .version import __version__
 from .xrdfile import XRootDPyFile
 
-__all__ = ('__version__', 'XRootDPyFS', 'XRootDPyOpener', 'XRootDPyFile')
+__version__ = "1.0.0a1"
+
+__all__ = ("__version__", "XRootDPyFS", "XRootDPyOpener", "XRootDPyFile")
```

### Comparing `xrootdpyfs-0.2.2/xrootdpyfs/xrdfile.py` & `xrootdpyfs-1.0.0a1/xrootdpyfs/xrdfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,23 @@
 # Copyright (C) 2015, 2016 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """File-like interface for interacting with files over the XRootD protocol."""
 
-from __future__ import absolute_import, print_function
-
 import sys
 
-from fs import SEEK_CUR, SEEK_END, SEEK_SET
-from fs.errors import InvalidPathError, PathError, ResourceNotFoundError, \
-    UnsupportedError
+from fs import Seek
+from fs.errors import InvalidPath, PathError, ResourceNotFound, Unsupported
 from fs.path import basename
 from six import b, binary_type, text_type
 from XRootD.client import File
 
-from .utils import is_valid_path, is_valid_url, spliturl, \
-    translate_file_mode_to_flags
+from .utils import is_valid_path, is_valid_url, spliturl, translate_file_mode_to_flags
 
 
 class XRootDPyFile(object):
     r"""File-like interface for working with files over XRootD protocol.
 
     This class understands and will accept the following mode strings,
     with any additional characters being ignored:
@@ -65,95 +61,101 @@
     :param line_buffering: Unsupported. Anything by False will raise and
         error.
     :param buffer_size: Buffer size used when reading files (defaults to 64K).
         This can likely be optimized to chunks up to 2MB depending on your
         desired memory usage.
     """
 
-    def __init__(self, path, mode='r', buffering=-1, encoding=None,
-                 errors=None, newline=None, line_buffering=False,
-                 buffer_size=None, **kwargs):
+    def __init__(
+        self,
+        path,
+        mode="r",
+        buffering=-1,
+        encoding=None,
+        errors=None,
+        newline=None,
+        line_buffering=False,
+        buffer_size=None,
+        **kwargs
+    ):
         """The XRootDPyFile constructor.
 
         Raises PathError if the given path isn't a valid XRootD URL,
-        and InvalidPathError if it isn't a valid XRootD file path.
+        and InvalidPath if it isn't a valid XRootD file path.
         """
         if not is_valid_url(path):
             raise PathError(path)
 
         xpath = spliturl(path)[1]
 
         if not is_valid_path(xpath):
-            raise InvalidPathError(xpath)
+            raise InvalidPath(xpath)
 
-        if newline not in [None, '', '\n', '\r', '\r\n']:
-            raise UnsupportedError(
-                "Newline character {0} not supported".format(newline))
+        if newline not in [None, "", "\n", "\r", "\r\n"]:
+            raise Unsupported("Newline character {0} not supported".format(newline))
 
         if line_buffering is not False:
-            raise NotImplementedError("Line buffering for writing is not "
-                                      "supported.")
+            raise NotImplementedError("Line buffering for writing is not " "supported.")
 
         buffering = int(buffering)
-        if buffering == 1 and 'b' in mode:
-            raise UnsupportedError(
-                "Line buffering is not supported for "
-                "binary files.")
+        if buffering == 1 and "b" in mode:
+            raise Unsupported("Line buffering is not supported for " "binary files.")
 
         # PyFS attributes
         self.mode = mode
 
         # XRootD attributes & internals
         self.path = path
         self.encoding = encoding or sys.getdefaultencoding()
-        self.errors = errors or 'strict'
+        self.errors = errors or "strict"
         self.buffer_size = buffer_size or 64 * 1024
         self.buffering = buffering
         self._file = File()
         self._ipp = 0
         self._size = -1
         self._iterator = None
         self._newline = newline or b("\n")
-        self._buffer = b('')
+        self._buffer = b("")
         self._buffer_pos = 0
 
         # flag translation
         self._flags = translate_file_mode_to_flags(mode)
 
         statmsg, response = self._file.open(path, flags=self._flags)
 
         if not statmsg.ok:
-            self._raise_status(self.path, statmsg,
-                               "instantiating file ({0})".format(path))
+            self._raise_status(
+                self.path, statmsg, "instantiating file ({0})".format(path)
+            )
 
         # Deal with the modes
-        if 'a' in self.mode:
-            self.seek(self.size, SEEK_SET)
+        if "a" in self.mode:
+            self.seek(self.size, Seek.set)
 
     def _raise_status(self, path, status, source=None):
         """Raise error based on status."""
         if status.errno == 3011:
-            raise ResourceNotFoundError(path)
+            raise ResourceNotFound(path)
         else:
             if source:
                 errstr = "XRootD error {0}file: {1}".format(
-                         source + ' ', status.message)
+                    source + " ", status.message
+                )
             raise IOError(errstr)
 
     def __del__(self):
         """Close file on object deletion."""
         self.close()
 
     def __iter__(self):
         """Initialize the internal iterator."""
         self._next_func = self.read
         self._next_args = ([], dict(sizehint=self.buffer_size))
 
-        if self.buffering == 1 or \
-           (self.buffering == -1 and 'b' not in self.mode):
+        if self.buffering == 1 or (self.buffering == -1 and "b" not in self.mode):
             self._next_func = self.readline
             self._next_args = ([], dict())
         elif self.buffering > 1:
             self._next_args = ([], dict(sizehint=self.buffering))
 
         return self
 
@@ -206,16 +208,15 @@
         )
 
         if not statmsg.ok:
             self._raise_status(self.path, statmsg, "reading")
 
         # Increment internal file pointer.
         self._ipp = min(
-            self._ipp + chunksize,
-            self.size if self.size > self._ipp else self._ipp
+            self._ipp + chunksize, self.size if self.size > self._ipp else self._ipp
         )
 
         return res
 
     def readline(self):
         """Read one entire line from the file.
 
@@ -271,16 +272,16 @@
 
         If the keyword argument 'flushing' is true, it indicates that the
         internal write buffers are being flushed, and *all* the given data
         is expected to be written to the file.
         """
         self._assert_mode("w-")
 
-        if 'a' in self.mode:
-            self.seek(0, SEEK_END)
+        if "a" in self.mode:
+            self.seek(0, Seek.end)
 
         if not isinstance(data, binary_type):
             if isinstance(data, bytearray):
                 data = bytes(data)
             elif isinstance(data, text_type):
                 data = data.encode(self.encoding, self.errors)
 
@@ -295,60 +296,60 @@
             self.flush()
 
     def writelines(self, sequence):
         """Write an sequence of lines to file."""
         for s in sequence:
             self.write(s)
 
-    def seek(self, offset, whence=SEEK_SET):
+    def seek(self, offset, whence=Seek.set):
         """Set the file's internal position pointer, approximately.
 
         The possible values of whence and their meaning are defined
         in the Linux man pages for `lseek()`:
         http://man7.org/linux/man-pages/man2/lseek.2.html
 
-        ``SEEK_SET``
+        ``Seek.set``
             The internal position pointer is set to offset bytes.
-        ``SEEK_CUR``
+        ``Seek.current``
             The ipp is set to its current position plus offset bytes.
-        ``SEEK_END``
+        ``Seek.end``
             The ipp is set to the size of the file plus offset bytes.
         """
         if "-" in self.mode:
             raise IOError("File is not seekable.")
 
         # Convert to integer by rounding down/omitting everything after
         # the decimal point
         offset = int(offset)
 
         # If not in binary mode and seeking from the end, forbid negative
         # offsets
-        if not ('b' in self.mode and whence == SEEK_END) and offset < 0:
+        if not ("b" in self.mode and whence == Seek.end) and offset < 0:
             raise IOError("Invalid argument.")
 
-        if whence == SEEK_SET:
+        if whence == Seek.set:
             self._ipp = offset
-        elif whence == SEEK_CUR:
+        elif whence == Seek.current:
             self._ipp += offset
-        elif whence == SEEK_END:
+        elif whence == Seek.end:
             self._ipp = self.size + offset
         else:
             raise NotImplementedError(whence)
 
     def tell(self):
         """Get the location of the file's internal position pointer."""
         return self._ipp
 
     def truncate(self, size=None):
         """Truncate the file's size to ``size``.
 
         Note that ``size`` will never be None; if it was not specified by the
         user the current file position is used.
         """
-        self._assert_mode('w')
+        self._assert_mode("w")
 
         if size is None:
             size = self.tell()
 
         statmsg = self._file.truncate(size)[0]
 
         if not statmsg.ok:
@@ -372,23 +373,23 @@
         if not self.closed:
             statmsg, dummy = self._file.sync()
             if not statmsg.ok:
                 self._raise_status(self.path, statmsg, "flushing write buffer")
 
     def seekable(self):
         """Check if file is seekable."""
-        return '-' not in self.mode
+        return "-" not in self.mode
 
     def readable(self):
         """Check if file is readable."""
-        return 'r' in self.mode or '+' in self.mode
+        return "r" in self.mode or "+" in self.mode
 
     def writable(self):
         """Check if file is writable."""
-        return 'w' in self.mode or '+' in self.mode or 'a' in self.mode
+        return "w" in self.mode or "+" in self.mode or "a" in self.mode
 
     def isatty(self):
         """Check if file is a TTY (false always).
 
         Added for ``io`` module compatibility.
         """
         return False
@@ -422,17 +423,19 @@
 
     def _assert_mode(self, mode, mstr=None):
         """Check whether the file may be accessed in the given mode."""
         if mstr is None:
             try:
                 mstr = self.mode
             except AttributeError:
-                raise AttributeError("Mode attribute missing -- "
-                                     "was it deleted? "
-                                     "Close and re-open the file.")
+                raise AttributeError(
+                    "Mode attribute missing -- "
+                    "was it deleted? "
+                    "Close and re-open the file."
+                )
         if "+" in mstr:
             return True
         if "-" in mstr and "-" not in mode:
             raise IOError("File does not support seeking.")
         if "r" in mode:
             if "r" not in mstr:
                 raise IOError("File not opened for reading")
```

### Comparing `xrootdpyfs-0.2.2/xrootdpyfs/fs.py` & `xrootdpyfs-1.0.0a1/xrootdpyfs/fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,41 @@
 .
 
 .. note::
    All methods prefixed with ``xrd`` in :py:class:`XRootDPyFS` are specific to
    XRootDPyFS and not supported by other PyFilesystem implementations.
 """
 
-from __future__ import absolute_import, print_function
-
 import re
-from datetime import datetime
 from glob import fnmatch
 
+from fs import ResourceType
 from fs.base import FS
-from fs.errors import DestinationExistsError, DirectoryNotEmptyError, \
-    FSError, InvalidPathError, RemoteConnectionError, ResourceError, \
-    ResourceInvalidError, ResourceNotFoundError, UnsupportedError
-from fs.path import dirname, frombase, normpath, pathcombine, pathjoin
-from six import PY2, PY3, binary_type
+from fs.errors import (
+    DestinationExists,
+    DirectoryNotEmpty,
+    FSError,
+    InvalidPath,
+    RemoteConnectionError,
+    ResourceError,
+    ResourceInvalid,
+    ResourceNotFound,
+    Unsupported,
+)
+from fs.info import Info
+from fs.path import basename, combine, dirname, frombase, isabs, join, normpath, relpath
 from six.moves.urllib.parse import parse_qs, urlencode
 from XRootD.client import CopyProcess, FileSystem
-from XRootD.client.flags import AccessMode, DirListFlags, MkDirFlags, \
-    QueryCode, StatInfoFlags
+from XRootD.client.flags import (
+    AccessMode,
+    DirListFlags,
+    MkDirFlags,
+    QueryCode,
+    StatInfoFlags,
+)
 
 from .utils import is_valid_path, is_valid_url, spliturl
 from .xrdfile import XRootDPyFile
 
 
 class XRootDPyFS(FS):
     """XRootD PyFilesystem interface.
@@ -67,97 +78,114 @@
     :param url: A root URL.
     :param query: Dictionary of key/values to append to the URL query string.
         The contents of the dictionary gets merged with any querystring
         provided in the ``url``.
     :type query: dict
     """
 
+    # https://xrootd.slac.stanford.edu/doc/dev52/ofs_config.htm#_Toc53410373
+    OSS_TYPE_TO_RESOURCE_TYPE = {
+        b"d": ResourceType.directory,
+        b"f": ResourceType.file,
+    }
+
     _meta = {
-        'thread_safe': True,
-        'virtual': False,
-        'read_only': False,
-        'unicode_paths': True,
-        'case_insensitive_paths': False,
-        'network': True,
-        'atomic.move': True,
-        'atomic.copy': True,
-        'atomic.makedir': True,
-        'atomic.rename': True,
-        'atomic.setcontents': False
+        "case_insensitive": False,
+        "network": True,
+        "read_only": False,
+        "supports_rename": True,
     }
 
     def __init__(self, url, query=None):
         """Initialize file system object."""
         if not is_valid_url(url):
-            raise InvalidPathError(path=url)
+            raise InvalidPath(path=url)
 
         root_url, base_path, queryargs = spliturl(url)
 
         if not is_valid_path(base_path):
-            raise InvalidPathError(path=base_path)
+            raise InvalidPath(path=base_path)
 
         if queryargs:
             # Convert query string in URL into a dictionary. Assumes there's no
             # duplication of fields names in query string (such as e.g.
             # '?f1=a&f1=b').
             queryargs = {k: v[0] for (k, v) in parse_qs(queryargs).items()}
 
             # Merge values from kwarg query into the dictionary. Conflicting
             # keys raises an exception.
             for k, v in (query or {}).items():
                 if k in queryargs:
                     raise KeyError(
                         "Query string field {0} conflicts with "
-                        "field in URL {1}".format(k, url))
+                        "field in URL {1}".format(k, url)
+                    )
                 queryargs[k] = v
         else:
             # No query string in URL, use kwarg instead.
             queryargs = query
 
         self.root_url = root_url
         self.base_path = base_path
         self.queryargs = queryargs
         self._client = FileSystem(self.xrd_get_rooturl())
-        super(XRootDPyFS, self).__init__(thread_synchronize=False)
+        super().__init__()
 
-    def _p(self, path, encoding='utf-8'):
-        """Join path to base path."""
-        # fs.path.pathjoin() omits the first '/' in self.base_path.
+    def _p(self, path):
+        """Prepend base path to path."""
+        # fs.path.join() omits the first '/' in self.base_path.
         # It is resolved by adding on an additional '/' to its return value.
-        return '/' + pathjoin(self.base_path, path)
+        _path = path
+        if isabs(path):
+            no_trailing = self.base_path[:-1]
+            one_slash = no_trailing[1:]
+            missing_basepath = not (
+                path.startswith(one_slash) or path.startswith(no_trailing)
+            )
+            if missing_basepath:
+                _path = relpath(path)
+        return "/" + join(self.base_path, _path)
 
     def _raise_status(self, path, status):
         """Raise error based on status."""
         if status.errno in [3006, 17]:
-            raise DestinationExistsError(path=path, details=status)
+            raise DestinationExists(path=path, msg=status)
         elif status.errno == 3005:
             # Unfortunately only way to determine if the error is due to a
             # directory not being empty, or that a resource is not a directory:
             if status.message.strip().endswith("not a directory"):
-                raise ResourceInvalidError(path=path, details=status)
+                raise ResourceInvalid(path=path, msg=status)
             else:
-                raise DirectoryNotEmptyError(path=path, details=status)
+                raise DirectoryNotEmpty(path=path, msg=status)
         elif status.errno == 3011:
-            raise ResourceNotFoundError(path=path, details=status)
+            raise ResourceNotFound(path=path, msg=status)
         else:
-            raise ResourceError(path=path, details=status)
+            raise ResourceError(path=path, msg=status)
 
     def _query(self, flag, arg, parse=True):
         """Query an xrootd server."""
         status, res = self._client.query(flag, arg)
 
         if not status.ok:
             if status.errno == 3013:
-                raise UnsupportedError(opname="calcualte checksum",
-                                       details=status)
-            raise FSError(details=status)
+                raise Unsupported(msg=status)
+            raise FSError(msg=status)
         return parse_qs(res) if parse else res
 
-    def open(self, path, mode='r', buffering=-1, encoding=None, errors=None,
-             newline=None, line_buffering=False, **kwargs):
+    def open(
+        self,
+        path,
+        mode="r",
+        buffering=-1,
+        encoding=None,
+        errors=None,
+        newline=None,
+        line_buffering=False,
+        **kwargs
+    ):
         r"""Open the given path and return a file-like object.
 
         :param path: Path to file that should be opened.
         :type path: str
         :param mode: Mode of file to open, identical to the mode string used
             in 'file' and 'open' builtins.
         :type mode: str
@@ -172,36 +200,38 @@
         :param newline: Newline character to use (either ``\\n``, ``\\r``,
             ``\\r\\n``, ``''`` or ``None``).
         :param line_buffering: Unsupported. Anything by False will raise and
             error.
 
         :returns: A file-like object.
 
-        :raises: `fs.errors.ResourceInvalidError` if an intermediate directory
+        :raises: `fs.errors.ResourceInvalid` if an intermediate directory
             is an file.
-        :raises: `fs.errors.ResourceNotFoundError` if the path is not found.
+        :raises: `fs.errors.ResourceNotFound` if the path is not found.
         """
         return XRootDPyFile(
             self.getpathurl(path, with_querystring=True),
             mode=mode,
             buffering=buffering,
             encoding=encoding,
             errors=errors,
             newline=newline,
             line_buffering=line_buffering,
             **kwargs
         )
 
-    def listdir(self,
-                path="./",
-                wildcard=None,
-                full=False,
-                absolute=False,
-                dirs_only=False,
-                files_only=False):
+    def listdir(
+        self,
+        path="./",
+        wildcard=None,
+        full=False,
+        absolute=False,
+        dirs_only=False,
+        files_only=False,
+    ):
         """List the the files and directories under a given path.
 
         The directory contents are returned as a list of unicode paths.
 
         :param path: Path to list.
         :type path: str
         :param wildcard: Return only paths that matches the wildcard. It can
@@ -215,22 +245,28 @@
         :param dirs_only: If True, return only directories.
         :type dirs_only: bool
         :param files_only: If True, return only files.
         :type files_only: bool
 
         :returns: Iterable of paths.
 
-        :raises: `fs.errors.ResourceInvalidError` if the path exists, but is
+        :raises: `fs.errors.ResourceInvalid` if the path exists, but is
             not a directory.
-        :raises: `fs.errors.ResourceNotFoundError` if the path is not found.
+        :raises: `fs.errors.ResourceNotFound` if the path is not found.
         """
-        return list(self.ilistdir(
-            path=path, wildcard=wildcard, full=full, absolute=absolute,
-            dirs_only=dirs_only, files_only=files_only
-        ))
+        return list(
+            self.ilistdir(
+                path=path,
+                wildcard=wildcard,
+                full=full,
+                absolute=absolute,
+                dirs_only=dirs_only,
+                files_only=files_only,
+            )
+        )
 
     def _stat_flags(self, path):
         """Get status of a path."""
         status, stat = self._client.stat(self._p(path))
 
         if not status.ok:
             raise self._raise_status(path, status)
@@ -242,84 +278,93 @@
         :param path: a path in the filesystem
         :type path: str
 
         :rtype: bool
 
         """
         try:
-            flags = self._stat_flags(path) if _statobj is None \
-                else _statobj.flags
+            flags = self._stat_flags(path) if _statobj is None else _statobj.flags
             return bool(flags & StatInfoFlags.IS_DIR)
-        except ResourceNotFoundError:
+        except ResourceNotFound:
             return False
 
     def isfile(self, path, _statobj=None):
         """Check if a path references a file.
 
         :param path: a path in the filesystem
         :type path: str
 
         :rtype: bool
 
         """
         try:
-            flags = self._stat_flags(path) if _statobj is None \
-                else _statobj.flags
-            return not bool(
-                flags & (StatInfoFlags.IS_DIR | StatInfoFlags.OTHER))
-        except ResourceNotFoundError:
+            flags = self._stat_flags(path) if _statobj is None else _statobj.flags
+            return not bool(flags & (StatInfoFlags.IS_DIR | StatInfoFlags.OTHER))
+        except ResourceNotFound:
             return False
 
     def exists(self, path):
         """Check if a path references a valid resource.
 
         :param path: A path in the filesystem.
         :type path: str
         :rtype: bool
         """
         status, stat = self._client.stat(self._p(path))
         return status.ok
 
-    def makedir(self, path, recursive=False, allow_recreate=False):
+    def makedir(
+        self,
+        path,
+        recursive=False,
+        allow_recreate=False,
+        permissions=None,
+        recreate=False,
+    ):
         """Make a directory on the filesystem.
 
         :param path: Path of directory.
         :type path: str
         :param recursive: If True, any intermediate directories will also be
             created.
         :type recursive: `bool`
         :param allow_recreate: If True, re-creating a directory wont be an
             error.
         :type allow_create: `bool`
 
-        :raises: `fs.errors.DestinationExistsError` if the path is already
+        :raises: `fs.errors.DestinationExists` if the path is already
             existing, and allow_recreate is False.
-        :raises: `fs.errors.ResourceInvalidError` if a containing
+        :raises: `fs.errors.ResourceInvalid` if a containing
             directory is missing and recursive is False or if a path is an
             existing file.
         """
         flags = MkDirFlags.MAKEPATH if recursive else MkDirFlags.NONE
         mode = AccessMode.NONE
 
-        status, res = self._client.mkdir(self._p(path), flags=flags, mode=mode)
+        status, _ = self._client.mkdir(self._p(path), flags=flags, mode=mode)
 
         if not status.ok:
-            if allow_recreate and status.errno == 3006:
+            destination_exists = status.errno == 3006
+            if allow_recreate and destination_exists:
                 return True
             self._raise_status(path, status)
         return True
 
+    def openbin(self, path, mode="r", buffering=-1, **options):
+        """Openbin."""
+        raise NotImplementedError
+
     def remove(self, path):
         """Remove a file from the filesystem.
 
         :param path: Path of the resource to remove.
         :type path: str
 
-        :raises: `fs.errors.ResourceInvalidError` if the path is a directory.
-        :raises: `fs.errors.DirectoryNotEmptyError` if the directory is not
+        :raises: `fs.errors.ResourceInvalid` if the path is a directory.
+        :raises: `fs.errors.DirectoryNotEmpty` if the directory is not
             empty.
         """
         status, res = self._client.rm(self._p(path))
 
         if not status.ok:
             self._raise_status(path, status)
         return True
@@ -334,145 +379,211 @@
         :param force: If True, any directory contents will be removed
             (recursively). Note that this can be very expensive as the xrootd
             protocol does not support recursive deletes - i.e. the library
             will do a full recursive listing of the directory and send a
             network request per file/directory.
         :type force: bool
 
-        :raises: `fs.errors.DirectoryNotEmptyError` if the directory is not
+        :raises: `fs.errors.DirectoryNotEmpty` if the directory is not
             empty and force is `False`.
-        :raises: `fs.errors.ResourceInvalidError` if the path is not a
+        :raises: `fs.errors.ResourceInvalid` if the path is not a
             directory.
-        :raises: `fs.errors.ResourceNotFoundError` if the path does not exist.
+        :raises: `fs.errors.ResourceNotFound` if the path does not exist.
         """
         if recursive:
-            raise UnsupportedError("recursive parameter is not supported.")
+            raise Unsupported("recursive parameter is not supported.")
 
-        status, res = self._client.rmdir(self._p(path))
+        status, _ = self._client.rmdir(self._p(path))
 
         if not status.ok:
-            if force and status.errno == 3005:
+            directory_not_empty_error = status.errno == 3005
+            if directory_not_empty_error and force:
                 # xrootd does not support recursive removal so do we have to
                 # do it ourselves.
-                for d, filenames in self.walk(path, search="depth"):
-                    for filename in filenames:
-                        relpath = pathjoin(d, filename)
-                        status, res = self._client.rm(self._p(relpath))
+                for step in self.walk(path, search="depth"):
+                    for file in step.files:
+                        filepath = join(step.path, file.name)
+                        status, _ = self._client.rm(self._p(filepath))
                         if not status.ok:
-                            self._raise_status(relpath, status)
-                    status, res = self._client.rmdir(self._p(d))
+                            self._raise_status(filepath, status)
+                    status, _ = self._client.rmdir(self._p(step.path))
                     if not status.ok:
                         self._raise_status(path, status)
                 return True
             self._raise_status(path, status)
         return True
 
+    def setinfo(self, path, info):
+        """Set info on a resource."""
+        raise NotImplementedError
+
     def rename(self, src, dst):
         """Rename a file or directory.
 
         :param src: path to rename.
         :type src: str
         :param dst: new name.
         :type dst: str
 
-        :raises: `fs.errors.DestinationExistsError` if destination already
+        :raises: `fs.errors.DestinationExists` if destination already
             exists.
-        :raises: `fs.errors.ResourceNotFoundError` if source does not exists.
+        :raises: `fs.errors.ResourceNotFound` if source does not exists.
         """
         src = self._p(src)
-        dst = self._p(pathjoin(dirname(src), dst))
+        dst = self._p(join(dirname(src), dst))
 
         if not self.exists(src):
-            raise ResourceNotFoundError(src)
+            raise ResourceNotFound(src)
         return self._move(src, dst, overwrite=False)
 
     def getpathurl(self, path, allow_none=False, with_querystring=False):
         """Get URL that corresponds to the given path."""
         if with_querystring and self.queryargs:
             return "{0}{1}?{2}".format(
-                self.root_url, self._p(path), urlencode(self.queryargs))
+                self.root_url, self._p(path), urlencode(self.queryargs)
+            )
         else:
             return "{0}{1}".format(self.root_url, self._p(path))
 
-    def getinfo(self, path):
-        """Return information for a path as a dictionary.
+    def getinfo(self, path, namespaces=None):
+        """Return information for a path as fs.info.Info object.
 
-        The following values can be found in the info dictionary:
+        The extra namespace `xrootd` contains the following:
 
         * ``size`` - Number of bytes used to store the file or directory.
         * ``created_time`` - A datetime object containing the time the
            resource was created.
         * ``modified_time`` - A datetime object containing the time the
            resource was modified.
         * ``accessed_time`` - A datetime object containing the time the
            resource was accessed.
         * ``offline`` - True if file/directory is offline.
         * ``writable`` - True if file/directory is writable.
         * ``readable`` - True if file/directory is readable.
         * ``executable`` - True if file/directory is executable.
 
         :param path: Path to retrieve information about.
+        :namespaces list: Info namespaces to query. The
+            `"basic"` namespace is alway included in the returned
+            info, whatever the value of `namespaces` may be.
         :type path: `string`
-        :rtype: `dict`
+        :rtype: `fs.info.Info`
         """
+        namespaces = namespaces or ()
         fullpath = self._p(path)
-        status, stat = self._client.stat(fullpath)
+        status, statobj = self._client.stat(fullpath)
 
         if not status.ok:
             self._raise_status(path, status)
 
-        info = dict()
-        info['size'] = stat.size
-        info['offline'] = bool(stat.flags & StatInfoFlags.OFFLINE)
-        info['writable'] = bool(stat.flags & StatInfoFlags.IS_WRITABLE)
-        info['readable'] = bool(stat.flags & StatInfoFlags.IS_READABLE)
-        info['executable'] = bool(stat.flags & StatInfoFlags.X_BIT_SET)
-
-        res = self._query(QueryCode.XATTR, fullpath)
-
-        ct = res.get(b'oss.ct', [None])[0]
-        mt = res.get(b'oss.mt', [None])[0]
-        at = res.get(b'oss.at', [None])[0]
+        extended_attr = self._query(QueryCode.XATTR, fullpath)
+
+        is_dir = self.isdir(path, statobj)
+        # `basic` namespace
+        basic = {
+            "name": basename(path),
+            "is_dir": is_dir,
+        }
+
+        # `details` namespace
+        details = {"size": statobj.size, "type": ResourceType.unknown}
+        _type = extended_attr.get(b"oss.type", [None])[0]
+        if _type:
+            details["type"] = self.OSS_TYPE_TO_RESOURCE_TYPE.get(
+                _type, ResourceType.unknown
+            )
 
+        ct = extended_attr.get(b"oss.ct", [None])[0]
+        mt = extended_attr.get(b"oss.mt", [None])[0]
+        at = extended_attr.get(b"oss.at", [None])[0]
         if ct:
-            info['created_time'] = datetime.fromtimestamp(int(ct))
+            details["created"] = int(ct)
         if mt:
-            info['modified_time'] = datetime.fromtimestamp(int(mt))
+            details["modified"] = int(mt)
         if at:
-            info['accessed_time'] = datetime.fromtimestamp(int(at))
-        return info
+            details["accessed"] = int(at)
 
-    def ilistdir(self,
-                 path="./",
-                 wildcard=None,
-                 full=False,
-                 absolute=False,
-                 dirs_only=False,
-                 files_only=False):
+        # optional `access` namespace
+        access = {
+            "permissions": None,  # fs.permissions.Permissions
+        }
+        uid = extended_attr.get(b"oss.u", [None])[0]
+        gid = extended_attr.get(b"oss.u", [None])[0]
+        if uid:
+            access["uid"] = uid
+        if gid:
+            access["gid"] = gid
+
+        # other namespaces
+        xrootd = {
+            "offline": bool(statobj.flags & StatInfoFlags.OFFLINE),
+            "writable": bool(statobj.flags & StatInfoFlags.IS_WRITABLE),
+            "readable": bool(statobj.flags & StatInfoFlags.IS_READABLE),
+            "executable": bool(statobj.flags & StatInfoFlags.X_BIT_SET),
+        }
+
+        info = {
+            "basic": basic,
+        }
+        if "details" in namespaces:
+            info["details"] = details
+        if "stat" in namespaces:
+            info["stat"] = {}
+        if "lstat" in namespaces:
+            info["lstat"] = {}
+        if "link" in namespaces:
+            info["link"] = {}
+        if "access" in namespaces:
+            info["access"] = access
+        if "xrootd" in namespaces:
+            info["xrootd"] = xrootd
+        return Info(info)
+
+    def ilistdir(
+        self,
+        path="./",
+        wildcard=None,
+        full=False,
+        absolute=False,
+        dirs_only=False,
+        files_only=False,
+    ):
         """Generator yielding the files and directories under a given path.
 
         This method behaves identically to `fs.base:FS.listdir` but
         returns an generator instead of a list.
         """
-        flag = DirListFlags.STAT if dirs_only or files_only else \
-            DirListFlags.NONE
+        flag = DirListFlags.STAT if dirs_only or files_only else DirListFlags.NONE
 
         full_path = self._p(path)
         status, entries = self._client.dirlist(full_path, flag)
 
         if not status.ok:
             self._raise_status(path, status)
 
         return self._ilistdir_helper(
-            path, entries, wildcard=wildcard, full=full,
-            absolute=absolute, dirs_only=dirs_only, files_only=files_only
+            path,
+            entries,
+            wildcard=wildcard,
+            full=full,
+            absolute=absolute,
+            dirs_only=dirs_only,
+            files_only=files_only,
         )
 
-    def _ilistdir_helper(self, path, entries, wildcard=None, full=False,
-                         absolute=False, dirs_only=False, files_only=False):
+    def _ilistdir_helper(
+        self,
+        path,
+        entries,
+        wildcard=None,
+        full=False,
+        absolute=False,
+        dirs_only=False,
+        files_only=False,
+    ):
         """A helper method called by ilistdir method that applies filtering.
 
         Given the path to a directory and a list of the names of entries within
         that directory, this method applies the semantics of the ilistdir()
         keyword arguments. An appropriately modified and filtered list of
         directory entries is returned.
         """
@@ -487,84 +598,78 @@
 
                 def wildcard(fn):
                     return bool(wildcard_re.match(fn))
 
             entries = (p for p in entries if wildcard(p.name))
 
         if dirs_only:
-            entries = (
-                p for p in entries if self.isdir(p.name, _statobj=p.statinfo)
-            )
+            entries = (p for p in entries if self.isdir(p.name, _statobj=p.statinfo))
         elif files_only:
-            entries = (
-                p for p in entries if self.isfile(p.name, _statobj=p.statinfo)
-            )
+            entries = (p for p in entries if self.isfile(p.name, _statobj=p.statinfo))
 
         if full:
-            entries = (pathcombine(path, p.name) for p in entries)
+            entries = (combine(path, p.name) for p in entries)
         elif absolute:
             path = self._p(path)
-            entries = ((pathcombine(path, p.name)) for p in entries)
+            entries = ((combine(path, p.name)) for p in entries)
         else:
             entries = (p.name for p in entries)
 
         return entries
 
     def move(self, src, dst, overwrite=False, **kwargs):
         """Move a file from one location to another.
 
         :param src: Source path.
         :type src: str
         :param dst: Destination path.
         :type dst: str
         :param overwrite: When True the destination will be overwritten (if it
-            exists), otherwise a DestinationExistsError will be thrown.
+            exists), otherwise a DestinationExists will be thrown.
         :type overwrite: bool
-        :raise: `fs.errors.DestinationExistsError` if destination exists and
+        :raise: `fs.errors.DestinationExists` if destination exists and
             ``overwrite`` is False.
-        :raise: `fs.errors.ResourceInvalidError` if source is not a file.
-        :raise: `fs.errors.ResourceNotFoundError` if source was not found.
+        :raise: `fs.errors.ResourceInvalid` if source is not a file.
+        :raise: `fs.errors.ResourceNotFound` if source was not found.
         """
         src, dst = self._p(src), self._p(dst)
 
         # isdir/isfile throws an error if file/dir doesn't exists
         if not self.exists(src):
-            raise ResourceNotFoundError(src)
+            raise ResourceNotFound(src)
 
         if not self.isfile(src):
-            raise ResourceInvalidError(
-                src, msg="Source is not a file: %(path)s")
+            raise ResourceInvalid(src, msg="Source is not a file: %(path)s")
 
         return self._move(src, dst, overwrite=overwrite)
 
     def movedir(self, src, dst, overwrite=False, **kwargs):
         """Move a directory from one location to another.
 
         :param src: Source directory path.
         :type src: str
         :param dst: Destination directory path.
         :type dst: str
         :param overwrite: When True the destination will be overwritten (if it
-            exists), otherwise a DestinationExistsError will be thrown.
+            exists), otherwise a DestinationExists will be thrown.
         :type overwrite: bool
-        :raise: `fs.errors.DestinationExistsError` if destination exists and
+        :raise: `fs.errors.DestinationExists` if destination exists and
             `overwrite` is `False`.
-        :raise: `fs.errors.ResourceInvalidError` if source is not a directory.
-        :raise: `fs.errors.ResourceInvalidError` if source is a directory and
+        :raise: `fs.errors.ResourceInvalid` if source is not a directory.
+        :raise: `fs.errors.ResourceInvalid` if source is a directory and
             destination is a file.
-        :raise: `fs.errors.ResourceNotFoundError` if source was not found.
+        :raise: `fs.errors.ResourceNotFound` if source was not found.
         """
         src, dst = self._p(src), self._p(dst)
 
         if not self.exists(src):
-            raise ResourceNotFoundError(src)
+            raise ResourceNotFound(src)
 
         if not self.isdir(src):
-            raise ResourceInvalidError(
-                src, msg="Source is not a directory: %(path)s")
+            raise ResourceInvalid(src, msg="Source is not a directory: %(path)s")
 
         return self._move(src, dst, overwrite=overwrite)
 
     def _move(self, src, dst, overwrite=False):
         """Move source to destination with support for overwriting destination.
 
         Used by ``XRootDPyFS.move()``, ``XRootDPyFS.movedir()`` and
@@ -578,15 +683,15 @@
            If ``overwrite`` is ``True``, this method will first remove any
            destination directory/file if it exists, and then try to move the
            source. Hence, if the source doesn't exists, it will remove the
            destination and then fail.
         """
         if self.exists(dst):
             if not overwrite:
-                raise DestinationExistsError(dst)
+                raise DestinationExists(dst)
 
             if self.isfile(dst):
                 self.remove(dst)
             elif self.isdir(dst):
                 self.removedir(dst, force=True)
 
         status, dummy = self._client.mv(src, dst)
@@ -600,26 +705,25 @@
         """Copy a file from source to destination.
 
         :param src: Source path.
         :type src: str
         :param dst: Destination path.
         :type dst: str
         :param overwrite: If True, then an existing file at the destination may
-            be overwritten; If False then ``DestinationExistsError``
+            be overwritten; If False then ``DestinationExists``
             will be raised.
         :type overwrite: bool
         """
         src, dst = self._p(src), self._p(dst)
 
         # isdir/isfile throws an error if file/dir doesn't exists
         if not self.isfile(src):
             if self.isdir(src):
-                raise ResourceInvalidError(
-                    src, msg="Source is not a file: %(path)s")
-            raise ResourceNotFoundError(src)
+                raise ResourceInvalid(src, msg="Source is not a file: %(path)s")
+            raise ResourceNotFound(src)
 
         if overwrite and self.exists(dst):
             if self.isdir(dst):
                 self.removedir(dst, force=True)
 
         status, dummy = self._client.copy(src, dst, force=overwrite)
 
@@ -643,46 +747,46 @@
             directory will be overwritten.
         :type overwrite: bool
         :param parallel: If True (default), the copy will be done in parallel.
         :type parallel: bool
         """
         if not self.isdir(src):
             if self.isfile(src):
-                raise ResourceInvalidError(
-                    src, msg="Source is not a directory: %(path)s")
-            raise ResourceNotFoundError(src)
+                raise ResourceInvalid(src, msg="Source is not a directory: %(path)s")
+            raise ResourceNotFound(src)
 
         if self.exists(dst):
             if overwrite:
                 if self.isdir(dst):
                     self.removedir(dst, force=True)
                 elif self.isfile(dst):
                     self.remove(dst)
             else:
-                raise DestinationExistsError(dst)
+                raise DestinationExists(dst)
 
         if parallel:
             process = CopyProcess()
 
             def process_copy(src, dst, overwrite=False):
                 process.add_job(src, dst)
 
             copyfile = process_copy
         else:
             copyfile = self.copy
 
         self.makedir(dst, allow_recreate=True)
 
-        for src_dirpath, filenames in self.walk(src):
-            dst_dirpath = pathcombine(dst, frombase(src, src_dirpath))
+        for step in self.walk(src):
+            src_dirpath = relpath(step.path)
+            dst_dirpath = combine(dst, frombase(src, src_dirpath))
             self.makedir(dst_dirpath, allow_recreate=True, recursive=True)
-            for filename in filenames:
-                src_filename = pathjoin(src_dirpath, filename)
-                dst_filename = pathjoin(dst_dirpath, filename)
-                copyfile(src_filename, dst_filename, overwrite=overwrite)
+            for file in step.files:
+                src_filepath = join(src_dirpath, file.name)
+                dst_filepath = join(dst_dirpath, file.name)
+                copyfile(src_filepath, dst_filepath, overwrite=overwrite)
 
         if parallel:
             process.prepare()
             process.run()
 
         return True
 
@@ -711,31 +815,31 @@
         """Get checksum of file from server.
 
         Specific to ``XRootDPyFS``. Note not all XRootD servers support the
         checksum operation (in particular the default local xrootd server).
 
         :param src: File to calculate checksum for.
         :type src: str
-        :raise: `fs.errors.UnsupportedError` if server does not support
+        :raise: `fs.errors.Unsupported` if server does not support
             checksum calculation.
         :raise: `fs.errors.FSError` if you try to get the checksum of e.g. a
             directory.
         """
         if not self.isfile(path, _statobj=_statobj):
-            raise ResourceInvalidError("Path is not a file: %s" % path)
+            raise ResourceInvalid("Path is not a file: %s" % path)
 
         value = self._query(QueryCode.CHECKSUM, self._p(path), parse=False)
-        value = value.decode('ascii').rstrip('\x00')
+        value = value.decode("ascii").rstrip("\x00")
         algorithm, value = value.strip().split(" ")
         return (algorithm, value)
 
     def xrd_ping(self):
         """Ping xrootd server.
 
         Specific to ``XRootDPyFS``.
         """
         status, dummy = self._client.ping()
 
         if not status.ok:
-            raise RemoteConnectionError(opname="ping", details=status)
+            raise RemoteConnectionError(msg=status)
 
         return True
```

### Comparing `xrootdpyfs-0.2.2/xrootdpyfs/utils.py` & `xrootdpyfs-1.0.0a1/xrootdpyfs/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,61 +4,57 @@
 # Copyright (C) 2015 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Helper methods for working with root URLs."""
 
-from __future__ import absolute_import, print_function
-
 import re
 
 from six.moves.urllib.parse import urlparse
 from XRootD.client import URL
 from XRootD.client.flags import OpenFlags
 
 
 def is_valid_url(fs_url):
     """Check if URL is a valid root URL."""
     scheme, netloc, path, params, query, fragment = urlparse(fs_url)
-    return URL(fs_url).is_valid() and scheme in ['root', 'roots']
+    return URL(fs_url).is_valid() and scheme in ["root", "roots"]
 
 
 def is_valid_path(fs_path):
     """Check if path is a valid XRootD compatible path.
 
     Valid paths start with two slashes ('/'), i.e. '//';
     and do not contain any other two adjacent slashes.
     """
     if len(fs_path) > 1:
-        if not re.search(r'^//', fs_path) or re.search(r'//', fs_path[1:]):
+        if not re.search(r"^//", fs_path) or re.search(r"//", fs_path[1:]):
             return False
         else:
             return True
     else:
         return False
 
 
 def spliturl(fs_url):
     """Split XRootD URL in a host and path part."""
     scheme, netloc, path, params, query, fragment = urlparse(fs_url)
 
     pattern = "{scheme}://{netloc}"
 
-    root_url = pattern.format(
-        scheme=scheme, netloc=netloc
-    )
+    root_url = pattern.format(scheme=scheme, netloc=netloc)
 
     return root_url, path, query
 
 
-def translate_file_mode_to_flags(mode='r'):
+def translate_file_mode_to_flags(mode="r"):
     """Translate a PyFS mode string to a combination of XRootD OpenFlags."""
     flags = 0
-    if 'r+' in mode or 'a' in mode:
+    if "r+" in mode or "a" in mode:
         return OpenFlags.UPDATE
-    if 'w' in mode:
+    if "w" in mode:
         return OpenFlags.DELETE
-    if 'r' in mode:
+    if "r" in mode:
         return OpenFlags.READ
 
     return flags
```

### Comparing `xrootdpyfs-0.2.2/xrootdpyfs/env.py` & `xrootdpyfs-1.0.0a1/xrootdpyfs/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,55 +17,53 @@
     * **Connection window**: The time interval during which a single new
       connection will be attempted. Subsequent attempts will not append until
       the next window.
     * **Connection retry**: Number of connection windows to try before
       declaring permanent failure.
 """
 
-from __future__ import absolute_import, print_function
-
 from os import environ
 
 
 def set_timeout(value):
     """Default value for the time after which an error is declared.
 
     This value can be overwritten on case-by-case in
     :py:class:`xrootdpyfs.fs.XRootDPyFS`.
 
     Sets the environment variable ``XRD_REQUESTTIMEOUT``.
     """
-    environ['XRD_REQUESTTIMEOUT'] = str(value)
+    environ["XRD_REQUESTTIMEOUT"] = str(value)
 
 
 def set_timeoutresolution(value):
     """Set resolution for the timeout events.
 
     Ie. timeout events will be processed only every number of seconds.
 
     Sets the environment variable ``XRD_TIMEOUTRESOLUTION``.
     """
-    environ['XRD_TIMEOUTRESOLUTION'] = str(value)
+    environ["XRD_TIMEOUTRESOLUTION"] = str(value)
 
 
 def set_connectionwindow(value):
     """Set time window for the connection establishment.
 
     A connection failure is declared if the connection is not established
     within the time window. If a connection failure happened earlier then
     another connection attempt will only be made at the beginning of the
     next window.
 
     Sets the environment variable ```XRD_CONNECTIONWINDOW``.
     """
-    environ['XRD_CONNECTIONWINDOW'] = str(value)
+    environ["XRD_CONNECTIONWINDOW"] = str(value)
 
 
 def set_connectionretry(value):
     """Number of connection attempts that should be made.
 
     I.e number of available connection windows before declaring a permanent
     failure.
 
     Sets the environment variable ``XRD_CONNECTIONRETRY``.
     """
-    environ['XRD_CONNECTIONRETRY'] = str(value)
+    environ["XRD_CONNECTIONRETRY"] = str(value)
```

### Comparing `xrootdpyfs-0.2.2/tests/test_xrdfile.py` & `xrootdpyfs-1.0.0a1/tests/test_xrdfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,180 +4,177 @@
 # Copyright (C) 2015 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Test of XRootDPyFS."""
 
-from __future__ import absolute_import, print_function
-
 import errno
 import math
-import os
-import sys
 from os.path import join
 
 import fs.path
 import pytest
 from conftest import mkurl
-from fs import SEEK_CUR, SEEK_END, SEEK_SET
-from fs.errors import InvalidPathError, PathError, ResourceNotFoundError, \
-    UnsupportedError
-from fs.opener import fsopendir, opener
+from fs import Seek
+from fs.errors import InvalidPath, PathError, ResourceNotFound, Unsupported
+from fs.opener import open_fs
 from mock import Mock
 from XRootD.client.responses import XRootDStatus
 
 from xrootdpyfs import XRootDPyFile
 from xrootdpyfs.utils import is_valid_path, is_valid_url
 
 
 def _list_str_encode(_list):
     return [el.encode() for el in _list]
 
 
 def test_init_basic(tmppath):
     """Test basic initialization of existing file."""
 
-    fname = 'testa.txt'
-    fpath = 'data/'
-    fcontents = 'testa.txt\n'
+    fname = "testa.txt"
+    fpath = "data/"
+    fcontents = "testa.txt\n"
     full_fpath = join(tmppath, fpath, fname)
     xfile = XRootDPyFile(mkurl(full_fpath))
     assert xfile
     assert type(xfile == XRootDPyFile)
     assert xfile._file
-    assert xfile.mode == 'r'
+    assert xfile.mode == "r"
 
     # Verify that underlying/wrapped file can be read.
     statmsg, res = xfile._file.read()
     assert res == fcontents.encode()
 
 
 def test_init_writemode_basic(tmppath):
     # Non-existing file is created.
-    fn, fp, fc = 'nope', 'data/', ''
+    fn, fp, fc = "nope", "data/", ""
     full_path = join(tmppath, fp, fn)
-    xfile = XRootDPyFile(mkurl(full_path), mode='w+')
+    xfile = XRootDPyFile(mkurl(full_path), mode="w+")
     assert xfile is not None
     assert xfile.read() == fc.encode()
 
     # Existing file is truncated
     fd = get_tsta_file(tmppath)
-    full_path = fd['full_path']
-    xfile = XRootDPyFile(mkurl(full_path), mode='w+')
+    full_path = fd["full_path"]
+    xfile = XRootDPyFile(mkurl(full_path), mode="w+")
     assert xfile is not None
-    assert xfile.read() == b''
+    assert xfile.read() == b""
     assert xfile.size == 0
     assert xfile.tell() == 0
 
 
 def test_init_readmode_basic(tmppath):
     # Non-existing file causes what?
     # Resource not found error.
-    fn, fp, fc = 'nope', 'data/', ''
+    fn, fp, fc = "nope", "data/", ""
     full_path = join(tmppath, fp, fn)
-    pytest.raises(ResourceNotFoundError, XRootDPyFile, mkurl(full_path),
-                  mode='r')
+    pytest.raises(ResourceNotFound, XRootDPyFile, mkurl(full_path), mode="r")
 
     # Existing file can be read?
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(full_path), mode='r')
+    full_path, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(full_path), mode="r")
     assert xfile
     assert xfile.read() == fc.encode()
 
 
 def get_tsta_file(tmppath):
-    fn, fd = 'testa.txt', 'data'
+    fn, fd = "testa.txt", "data"
     return get_file(fn, fd, tmppath)
 
 
 def get_mltl_file(tmppath):
-    fn, fp = 'multiline.txt', 'data'
+    fn, fp = "multiline.txt", "data"
     return get_file(fn, fp, tmppath)
 
 
 def get_bin_testfile(tmppath):
-    fn, fp = 'binary.dat', 'data'
+    fn, fp = "binary.dat", "data"
     return get_file_binary(fn, fp, tmppath)
 
 
 def get_file(fn, fp, tmppath):
-    fpp = join(tmppath, fp, fn)
-    with opener.open(fpp) as f:
+    path = join(tmppath, fp)
+    fpp = join(path, fn)
+    fs = open_fs(path)
+    with fs.open(fn) as f:
         fc = f.read()
-    return {'filename': fn, 'dir': fp, 'contents': fc, 'full_path': fpp}
+    return {"filename": fn, "dir": fp, "contents": fc, "full_path": fpp}
 
 
 def get_file_binary(fn, fp, tmppath):
-    fpp = join(tmppath, fp, fn)
-    with opener.open(fpp, 'rb') as f:
+    path = join(tmppath, fp)
+    fpp = join(path, fn)
+    fs = open_fs(path)
+    with fs.open(fn, "rb") as f:
         fc = f.read()
-    return {'filename': fn, 'dir': fp, 'contents': fc, 'full_path': fpp}
+    return {"filename": fn, "dir": fp, "contents": fc, "full_path": fpp}
 
 
 def copy_file(fn, fp, tmppath):
     path = join(tmppath, fp)
-    fn_new = fn + '_copy'
-    this_fs = fsopendir(path)
+    fn_new = fn + "_copy"
+    this_fs = open_fs(path)
     this_fs.copy(fn, fn_new)
     return fn_new
 
 
 def get_copy_file(arg, binary=False):
     # Would get called with e.g. arg=get_tsta_file(...)
-    fp = fs.path.dirname(arg['full_path'])
-    fn_new = copy_file(arg['filename'], '', fp)
-    return get_file_binary(fn_new, '', fp) if binary else get_file(
-        fn_new, '', fp)
+    fp = fs.path.dirname(arg["full_path"])
+    fn_new = copy_file(arg["filename"], "", fp)
+    return get_file_binary(fn_new, "", fp) if binary else get_file(fn_new, "", fp)
 
 
 def test_open_close(tmppath):
     """Test close() on an open file."""
     fd = get_tsta_file(tmppath)
-    full_path = fd['full_path']
+    full_path = fd["full_path"]
     xfile = XRootDPyFile(mkurl(full_path))
     assert xfile
     assert not xfile.closed
     xfile.close()
     assert xfile.closed
     # Multiple calls to closed do nothing.
     xfile.close()
 
 
 def test_close_error(tmppath):
     """Test error on close()."""
-    xfile = XRootDPyFile(mkurl(get_tsta_file(tmppath)['full_path']))
+    xfile = XRootDPyFile(mkurl(get_tsta_file(tmppath)["full_path"]))
     # Mock error response on close.
     fake_status = {
         "status": 1,
         "code": 3,
         "ok": False,
         "errno": 0,
         "error": True,
-        "message": '[ERROR] Invalid operation',
+        "message": "[ERROR] Invalid operation",
         "fatal": False,
-        "shellcode": 50
+        "shellcode": 50,
     }
     xfile._file.close = Mock(return_value=(XRootDStatus(fake_status), None))
     # Ensure error is raised.
     pytest.raises(IOError, xfile.close)
 
 
 def test_read_existing(tmppath):
     """Test read() on an existing non-empty file."""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
     xfile = XRootDPyFile(mkurl(full_path))
 
     res = xfile.read()
     assert res == fc.encode()
     # After having read the entire file, the file pointer is at the
     # end of the file and consecutive reads return the empty string.
-    assert xfile.read() == b''
+    assert xfile.read() == b""
 
     # reset ipp to start
     xfile.seek(0)
     assert xfile.read(1) == fc[0].encode()
     assert xfile.read(2) == fc[1:3].encode()
     overflow_read = xfile.read(len(fc))
     assert overflow_read == fc[3:].encode()
@@ -185,63 +182,63 @@
     # Mock an error, yayy!
     fake_status = {
         "status": 3,
         "code": 0,
         "ok": False,
         "errno": errno.EREMOTE,
         "error": True,
-        "message": '[FATAL] Remote I/O Error',
+        "message": "[FATAL] Remote I/O Error",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     xfile._file.read = Mock(return_value=(XRootDStatus(fake_status), None))
     pytest.raises(IOError, xfile.read)
 
 
 def test__is_open(tmppath):
     """Test _is_open()"""
     fd = get_tsta_file(tmppath)
-    full_path = fd['full_path']
+    full_path = fd["full_path"]
     xfile = XRootDPyFile(mkurl(full_path))
     assert not xfile.closed
     xfile.close()
     assert xfile.closed
 
 
 def test_size_len(tmppath):
     """Tests for the size and len property."""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
     xfile = XRootDPyFile(mkurl(full_path))
 
     assert xfile.size == len(fc)
     assert len(xfile) == len(fc)
 
     # Length of empty file
-    xfile = XRootDPyFile(mkurl(join(tmppath, fd['dir'], 'whut')), 'w+')
-    assert xfile.size == len('')
-    assert len(xfile) == len('')
+    xfile = XRootDPyFile(mkurl(join(tmppath, fd["dir"], "whut")), "w+")
+    assert xfile.size == len("")
+    assert len(xfile) == len("")
 
     # Length of multiline file
     fd = get_mltl_file(tmppath)
-    fpp, fc = fd['full_path'], fd['contents']
+    fpp, fc = fd["full_path"], fd["contents"]
     xfile = XRootDPyFile(mkurl(fpp))
     assert xfile.size == len(fc)
     assert len(xfile) == len(fc)
 
     # Mock the error
     fake_status = {
         "status": 3,
         "code": 0,
         "ok": False,
         "errno": errno.EREMOTE,
         "error": True,
-        "message": '[FATAL] Remote I/O Error',
+        "message": "[FATAL] Remote I/O Error",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     xfile.close()
     xfile = XRootDPyFile(mkurl(full_path))
     xfile._file.stat = Mock(return_value=(XRootDStatus(fake_status), None))
     try:
         xfile.size
         assert False
@@ -254,41 +251,41 @@
     except IOError:
         assert True
 
 
 def test_seek_and_tell(tmppath):
     """Basic tests for seek() and tell()."""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
     xfile = XRootDPyFile(mkurl(full_path))
     assert xfile.tell() == 0
 
     # Read file, then check the internal position pointer.
     conts = xfile.read()
     assert xfile.tell() == len(fc)
     assert conts == fc.encode()
 
     # Seek to beginning, then verify ipp.
     xfile.seek(0)
     assert xfile.tell() == 0
     assert xfile.read() == fc.encode()
 
-    newpos = len(fc)//2
+    newpos = len(fc) // 2
     xfile.seek(newpos)
     conts2 = xfile.read()
     assert conts2 == conts[newpos:]
     assert xfile.tell() == len(fc)
 
     # # Now with a multiline file!
     fd = get_mltl_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
     xfile = XRootDPyFile(mkurl(full_path))
 
     assert xfile.tell() == 0
-    newpos = len(fc)//3
+    newpos = len(fc) // 3
     xfile.seek(newpos)
     assert xfile.tell() == newpos
     nconts = xfile.read()
     assert xfile.tell() == len(fc)
     assert nconts == fc[newpos:].encode()
 
     # Negative offsets raise an error
@@ -301,223 +298,223 @@
     assert xfile.tell() == 0
 
 
 def test_seek_args(tmppath):
     """Test seek() with a non-default whence argument."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
-    pfile = open(fb['full_path'], 'rb+')
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
+    pfile = open(fb["full_path"], "rb+")
 
     xfile.truncate(3), pfile.truncate(3)
-    xfile.seek(2, SEEK_END), pfile.seek(2, SEEK_END)
+    xfile.seek(2, Seek.end), pfile.seek(2, Seek.end)
     assert xfile.tell() == pfile.tell()
 
-    xfile.seek(3, SEEK_CUR), pfile.seek(3, SEEK_CUR)
+    xfile.seek(3, Seek.current), pfile.seek(3, Seek.current)
     assert xfile.tell() == pfile.tell()
 
-    xfile.seek(8, SEEK_SET), pfile.seek(8, SEEK_SET)
+    xfile.seek(8, Seek.set), pfile.seek(8, Seek.set)
     assert xfile.tell() == pfile.tell()
 
     xfile.truncate(3), pfile.truncate(3)
     xfile.read(), pfile.read()
     assert xfile.tell() == pfile.tell()
-    xfile.seek(8, SEEK_END), pfile.seek(8, SEEK_END)
+    xfile.seek(8, Seek.end), pfile.seek(8, Seek.end)
     assert xfile.tell() == pfile.tell()
 
-    xfile.seek(4, SEEK_CUR), pfile.seek(4, SEEK_CUR)
+    xfile.seek(4, Seek.current), pfile.seek(4, Seek.current)
     assert xfile.tell() == pfile.tell()
 
     pytest.raises(NotImplementedError, xfile.seek, 0, 8)
 
 
 def test_tell_after_open(tmppath):
     """Tests for tell's init values in the various file modes."""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r')
+    xfile = XRootDPyFile(mkurl(full_path), "r")
     assert xfile.tell() == 0
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
     assert xfile.tell() == 0
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r-')
+    xfile = XRootDPyFile(mkurl(full_path), "r-")
     assert xfile.tell() == 0
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'a')
+    xfile = XRootDPyFile(mkurl(full_path), "a")
     assert xfile.tell() == len(fc)
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'a+')
+    xfile = XRootDPyFile(mkurl(full_path), "a+")
     assert xfile.tell() == len(fc)
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'w')
+    xfile = XRootDPyFile(mkurl(full_path), "w")
     assert xfile.tell() == 0
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'w-')
+    xfile = XRootDPyFile(mkurl(full_path), "w-")
     assert xfile.tell() == 0
     xfile.close()
 
 
 def test_truncate1(tmppath):
     """Test truncate(0)."""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
+    full_path, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
     # r+ opens for r/w, and won't truncate the file automatically.
     assert xfile.read() == fc.encode()
     assert xfile.tell() == len(fc)
     xfile.seek(0)  # Reset ipp.
     assert xfile.tell() == 0
 
     # Truncate it to size 0.
     xfile.truncate(0)
     assert xfile.size == 0
     assert xfile.tell() == 0
-    assert xfile.read() == b''
+    assert xfile.read() == b""
     assert xfile.tell() == 0
     xfile.close()
 
     # Re-open same file.
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
     assert xfile.size == 0
-    assert xfile.read() == b''
+    assert xfile.read() == b""
 
     # Truncate it again!
     xfile.truncate(0)
     assert xfile.size == 0
-    assert xfile.read() == b''
+    assert xfile.read() == b""
 
     # Truncate it twice.
     xfile.truncate(0)
     assert xfile.size == 0
-    assert xfile.read() == b''
+    assert xfile.read() == b""
 
     # Truncate to 1.
     xfile.truncate(1)
     assert xfile.tell() == 0
     assert xfile.size == 1
     xfile.seek(0)
-    assert xfile.read() == b'\x00'
+    assert xfile.read() == b"\x00"
     assert xfile.tell() == 1
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
     assert xfile.size == 1
-    assert xfile.read() == b'\x00'
+    assert xfile.read() == b"\x00"
 
     # Mock it.
     fake_status = {
         "status": 3,
         "code": 0,
         "ok": False,
         "errno": errno.EREMOTE,
         "error": True,
-        "message": '[FATAL] Remote I/O Error',
+        "message": "[FATAL] Remote I/O Error",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     xfile._file.truncate = Mock(return_value=(XRootDStatus(fake_status), None))
     pytest.raises(IOError, xfile.truncate, 0)
 
 
 def test_truncate2(tmppath):
     """Test truncate(self._size)."""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
+    full_path, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
     conts = xfile.read()
     assert conts == fc.encode()
 
     newsize = xfile.size
     xfile.truncate(newsize)
     assert xfile.tell() == newsize
     assert xfile.size == len(fc)
     xfile.seek(0)
     assert xfile.read() == conts
 
 
 def test_truncate3(tmppath):
     """Test truncate(0 < size < self._size)."""
     fd = get_mltl_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(full_path), 'r+')
+    full_path, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(full_path), "r+")
 
     initcp = xfile.tell()
 
-    newsiz = len(fc)//2
+    newsiz = len(fc) // 2
     xfile.truncate(newsiz)
     assert xfile.tell() == initcp
     xfile.seek(0)  # reset the internal pointer before reading
     assert xfile.read() == fc[:newsiz].encode()
 
 
 def test_truncate4(tmppath):
     """Verifies that truncate() raises errors on non-truncatable files."""
     fd = get_mltl_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
+    full_path, fc = fd["full_path"], fd["contents"]
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r')
+    xfile = XRootDPyFile(mkurl(full_path), "r")
     pytest.raises(IOError, xfile.truncate, 0)
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(full_path), 'w-')
+    xfile = XRootDPyFile(mkurl(full_path), "w-")
     pytest.raises(IOError, xfile.truncate, 0)
 
 
 def test_truncate5(tmppath):
     """Test truncate() (no arg)."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    xfa = XRootDPyFile(mkurl(fp), 'r+')
-    xfb = XRootDPyFile(mkurl(fp2), 'r+')
+    xfa = XRootDPyFile(mkurl(fp), "r+")
+    xfb = XRootDPyFile(mkurl(fp2), "r+")
 
     acnts = xfa.read()
     assert acnts == xfb.read()
 
     # internal pointer starts at 0 in all 'r' modes.
     xtell = xfa.tell()
     assert xfa.tell() == xfb.tell()
     # f.truncate() and f.truncate(self.tell()) should be equivalent
     xfa.truncate(), xfb.truncate(xfb.tell())
     assert xfa.size == xfb.size
     assert xfa.tell() == xtell
     assert xfb.tell() == xtell
-    assert xfb.read() == b''
-    assert xfa.read() == b''
+    assert xfb.read() == b""
+    assert xfa.read() == b""
 
     xfa.seek(0), xfb.seek(0)
     are = xfa.read()
     assert are == fc.encode()
     assert are == xfb.read()
 
 
 def test_truncate_read_write(tmppath):
     """Tests behaviour of writing after reading after truncating."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    sp = len(fc)//2
+    sp = len(fc) // 2
     wstr = "I am the string"
 
-    pfile = open(fp2, 'r+')
-    xfile = XRootDPyFile(mkurl(fp), 'r+')
+    pfile = open(fp2, "r+")
+    xfile = XRootDPyFile(mkurl(fp), "r+")
 
     xfile.truncate(sp), pfile.truncate(sp)
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
     assert xfile.tell() == pfile.tell()
 
     xfile.write(wstr), pfile.write(wstr)
@@ -527,25 +524,25 @@
     xfile.seek(0), pfile.seek(0)
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
 
 
 def test_truncate_read_write2(tmppath):
     """Tests behaviour of writing after seek(0) after
-       reading after truncating."""
+    reading after truncating."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    sp = len(fc)//2
+    sp = len(fc) // 2
     wstr = "I am the string"
 
-    pfile = open(fp2, 'r+')
-    xfile = XRootDPyFile(mkurl(fp), 'r+')
+    pfile = open(fp2, "r+")
+    xfile = XRootDPyFile(mkurl(fp), "r+")
 
     xfile.truncate(sp), pfile.truncate(sp)
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
     assert xfile.tell() == pfile.tell()
 
     xfile.seek(0), pfile.seek(0)
@@ -559,270 +556,267 @@
     xfile.seek(0), pfile.seek(0)
     assert xfile.read() == pfile.read().encode()
 
 
 def test_write(tmppath):
     """Test write()."""
     # With a new file.
-    xfile = XRootDPyFile(mkurl(join(tmppath, 'data/nuts')), 'w+')
+    xfile = XRootDPyFile(mkurl(join(tmppath, "data/nuts")), "w+")
     assert xfile.size == 0
     conts = xfile.read()
     assert not conts
 
-    nconts = 'Write.'
+    nconts = "Write."
     xfile.write(nconts)
     assert xfile.tell() == len(nconts)
     assert not xfile.closed
     xfile.seek(0)
     assert xfile.size == len(nconts)
     assert xfile.read() == nconts.encode()
     xfile.close()
 
     # Verify persistence after closing.
-    xfile = XRootDPyFile(mkurl(join(tmppath, 'data/nuts')), 'r+')
+    xfile = XRootDPyFile(mkurl(join(tmppath, "data/nuts")), "r+")
     assert xfile.size == len(nconts)
     assert xfile.read() == nconts.encode()
 
     # Seek(x>0) followed by a write
-    nc2 = 'hello'
-    cntr = len(nconts)//2
+    nc2 = "hello"
+    cntr = len(nconts) // 2
     xfile.seek(cntr)
     xfile.write(nc2)
     assert xfile.tell() == len(nc2) + cntr
     xfile.seek(0)
     expected = nconts[:cntr] + nc2
     assert xfile.read() == expected.encode()
     xfile.close()
 
     # Seek(x>0) followed by a write of len < size-x
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(fp), 'r+')
+    fp, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(fp), "r+")
     assert xfile.read() == fc.encode()
     xfile.seek(2)
-    nc = 'yo'
+    nc = "yo"
     xfile.write(nc)
     assert xfile.tell() == len(nc) + 2
-    assert xfile.read() == fc[2+len(nc):].encode()
+    assert xfile.read() == fc[2 + len(nc) :].encode()
 
     # run w/ flushing == true
-    xfile.write('', True)
+    xfile.write("", True)
 
     # Mock an error, yayy!
     fake_status = {
         "status": 3,
         "code": 0,
         "ok": False,
         "errno": errno.EREMOTE,
         "error": True,
-        "message": '[FATAL] Remote I/O Error',
+        "message": "[FATAL] Remote I/O Error",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     xfile._file.write = Mock(return_value=(XRootDStatus(fake_status), None))
-    pytest.raises(IOError, xfile.write, '')
+    pytest.raises(IOError, xfile.write, "")
 
 
 def test_readwrite_diffrent_encodings_fails(tmppath):
     """Test read/write a unicode str in non unicode files."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, dummy = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, dummy = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    unicodestr = u"æøå"
+    unicodestr = "æøå"
 
-    pfile = open(fp2, 'w')  # default encoding is ANSI
+    pfile = open(fp2, "w")  # default encoding is ANSI
     pytest.raises(UnicodeEncodeError, pfile.write, unicodestr)
-    xfile = XRootDPyFile(mkurl(fp), 'w', encoding='ascii')
+    xfile = XRootDPyFile(mkurl(fp), "w", encoding="ascii")
     pytest.raises(UnicodeEncodeError, xfile.write, unicodestr)
     xfile.close()
 
 
 def test_readwrite_unicode(tmppath):
     """Test read/write a unicode str in unicode files."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, dummy = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, dummy = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    unicodestr = u"æøå"
+    unicodestr = "æøå"
 
-    xfile = XRootDPyFile(mkurl(fp), 'w+')  # default encoding is UTF-8
+    xfile = XRootDPyFile(mkurl(fp), "w+")  # default encoding is UTF-8
     xfile.write(unicodestr)
     xfile.flush()
     xfile.seek(0)
-    assert unicodestr.encode('utf8') == xfile.read()
+    assert unicodestr.encode("utf8") == xfile.read()
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(fp), 'w+', encoding='ascii', errors='ignore')
+    xfile = XRootDPyFile(mkurl(fp), "w+", encoding="ascii", errors="ignore")
     xfile.write(unicodestr)
     xfile.flush()
     xfile.seek(0)
-    assert unicodestr.encode('ascii', 'ignore') == xfile.read()
+    assert unicodestr.encode("ascii", "ignore") == xfile.read()
     xfile.close()
 
 
 def test_init_paths(tmppath):
     """Tests how __init__ responds to correct and invalid paths."""
     # Invalid url should raise error
     url = "fee-fyyy-/fooo"
-    assert not is_valid_url(url) \
-        and pytest.raises(PathError, XRootDPyFile, url)
+    assert not is_valid_url(url) and pytest.raises(PathError, XRootDPyFile, url)
 
-    path = '//ARGMEGXXX//\\///'
-    assert not is_valid_path(path) \
-        and pytest.raises(InvalidPathError, XRootDPyFile, mkurl(path))
+    path = "//ARGMEGXXX//\\///"
+    assert not is_valid_path(path) and pytest.raises(
+        InvalidPath, XRootDPyFile, mkurl(path)
+    )
 
 
 def test_init_append(tmppath):
     """Test for files opened 'a'"""
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(fp), 'a')
-    assert xfile.mode == 'a'
+    fp, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(fp), "a")
+    assert xfile.mode == "a"
     pytest.raises(IOError, xfile.read)
     assert xfile.tell() == len(fc)
 
     # Seeking is allowed, but writes still go on the end.
     xfile.seek(0)
     assert xfile.tell() == 0
-    newcont = u'butterflies'
+    newcont = "butterflies"
     xfile.write(newcont)
     assert xfile.tell() == len(fc) + len(newcont)
     # Can't read in this mode.
     xfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'r')
+    xfile = XRootDPyFile(mkurl(fp), "r")
     expected = fc + newcont
     assert xfile.read() == expected.encode()
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'a')
+    xfile = XRootDPyFile(mkurl(fp), "a")
     xfile.write(fc)
     xfile.seek(0)
     pytest.raises(IOError, xfile.read)
 
 
 def test_init_appendread(tmppath):
     """Test for files opened in mode 'a+'."""
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(fp), 'a+')
-    assert xfile.mode == 'a+'
+    fp, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(fp), "a+")
+    assert xfile.mode == "a+"
     assert xfile.tell() == len(fc)
-    assert xfile.read() == b''
+    assert xfile.read() == b""
 
     # Seeking is allowed, but writes still go on the end.
     xfile.seek(0)
     assert xfile.tell() == 0
-    newcont = u'butterflies'
+    newcont = "butterflies"
     xfile.write(newcont)
     assert xfile.tell() == len(fc) + len(newcont)
     xfile.seek(0)
     expected = fc + newcont
     assert xfile.read() == expected.encode()
     xfile.write(fc)
     xfile.seek(0)
     expected = fc + newcont + fc
     xfile.read() == expected.encode()
 
 
 def test_init_writemode(tmppath):
     """Tests for opening files in 'w(+)'"""
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(fp), 'w')
+    fp, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(fp), "w")
     pytest.raises(IOError, xfile.read)
 
     xfile.seek(1)
-    conts = 'what'
+    conts = "what"
     xfile.write(conts)
     assert xfile.tell() == 1 + len(conts)
     assert xfile.size == 1 + len(conts)
     xfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'r')
+    xfile = XRootDPyFile(mkurl(fp), "r")
     fc = xfile.read()
-    expected = '\x00'+conts
+    expected = "\x00" + conts
     assert fc == expected.encode()
     assert not fc == conts
 
 
 def test_init_streammodes(tmppath):
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(fp), 'r-')
+    fp, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(fp), "r-")
     pytest.raises(IOError, xfile.seek, 3)
     assert xfile.size == len(fc)
     assert xfile.tell() == 0
     assert xfile.read() == fc.encode()
     assert xfile.tell() == len(fc)
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'w-')
+    xfile = XRootDPyFile(mkurl(fp), "w-")
     pytest.raises(IOError, xfile.read)
     pytest.raises(IOError, xfile.seek, 3)
     assert xfile.tell() == 0
     assert xfile.size == 0
-    conts = 'hugs are delightful'
+    conts = "hugs are delightful"
     xfile.write(conts)
     assert xfile.tell() == len(conts)
     xfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'r')
+    xfile = XRootDPyFile(mkurl(fp), "r")
     assert xfile.read() == conts.encode()
 
 
 def test_init_newline(tmppath):
     """Tests fs.open() with specified newline parameter."""
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
+    fp, fc = fd["full_path"], fd["contents"]
 
     xfile = XRootDPyFile(mkurl(fp))
-    assert xfile._newline == b'\n'
+    assert xfile._newline == b"\n"
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(fp), newline='\n')
-    assert xfile._newline == '\n'
+    xfile = XRootDPyFile(mkurl(fp), newline="\n")
+    assert xfile._newline == "\n"
     xfile.close()
 
-    pytest.raises(UnsupportedError, XRootDPyFile, mkurl(fp), mode='r',
-                  newline='what')
+    pytest.raises(Unsupported, XRootDPyFile, mkurl(fp), mode="r", newline="what")
 
 
 def test_init_notimplemented(tmppath):
     """Tests that specifying not-implemented args to XRDFile's constructor
-       results in an error."""
+    results in an error."""
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
+    fp, fc = fd["full_path"], fd["contents"]
 
-    pytest.raises(UnsupportedError, XRootDPyFile, mkurl(fp), 'rb',
-                  buffering=1)
-    pytest.raises(NotImplementedError, XRootDPyFile, mkurl(fp),
-                  line_buffering='')
+    pytest.raises(Unsupported, XRootDPyFile, mkurl(fp), "rb", buffering=1)
+    pytest.raises(NotImplementedError, XRootDPyFile, mkurl(fp), line_buffering="")
 
 
 def test_read_errors(tmppath):
     fd = get_tsta_file(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(fp), 'r')
+    fp, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(fp), "r")
     xfile.close()
     pytest.raises(ValueError, xfile.read)
 
 
 def test_read_and_write(tmppath):
     """Tests that the XRDFile behaves like a regular python file."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    seekpoint = len(fc)//2
+    seekpoint = len(fc) // 2
     writestr = "Come what may in May this day says Ray all gay like Jay"
 
-    pfile = open(fp2, 'r+')
-    xfile = XRootDPyFile(mkurl(fp), 'r+')
+    pfile = open(fp2, "r+")
+    xfile = XRootDPyFile(mkurl(fp), "r+")
 
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
     assert xfile.tell() == pfile.tell()
 
     xfile.seek(seekpoint), pfile.seek(seekpoint)
     assert xfile.tell() == pfile.tell()
@@ -835,23 +829,23 @@
     assert xfile.read() == pfile.read().encode()
 
 
 def test_write_and_read(tmppath):
     """Tests that the XRootDPyFile behaves like a regular python file in w+."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
     writestr = "Hello fair mare what fine stairs."
-    seekpoint = len(writestr)//2
+    seekpoint = len(writestr) // 2
     # In 'w' (and variant modes) the file's contents are deleted upon opening.
 
-    pfile = open(fp2, 'w+')
-    xfile = XRootDPyFile(mkurl(fp), 'w+')
+    pfile = open(fp2, "w+")
+    xfile = XRootDPyFile(mkurl(fp), "w+")
 
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
     assert xfile.tell() == pfile.tell()
 
     xfile.write(writestr), pfile.write(writestr)
     assert xfile.tell() == pfile.tell()
@@ -866,428 +860,416 @@
     assert xfile.tell() == pfile.tell()
 
 
 def test_seek_past_eof_rw(tmppath):
     """Tests read/write/truncate behaviour after seeking past the EOF, 'r+'."""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
     wstr = "www"
     eof = len(fc)
-    skpnt = len(fc)+4
+    skpnt = len(fc) + 4
 
-    pfile = open(fp2, 'r+')
-    xfile = XRootDPyFile(mkurl(fp), 'r+')
+    pfile = open(fp2, "r+")
+    xfile = XRootDPyFile(mkurl(fp), "r+")
 
     xfile.seek(skpnt), pfile.seek(skpnt)
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
     assert xfile.tell() == pfile.tell()
     assert xfile.tell() == skpnt
 
     xfile.write(wstr), pfile.write(wstr)
     assert xfile.tell() == pfile.tell()
     xfile.seek(eof), pfile.seek(eof)
-    expected = '\x00'*(skpnt-eof) + wstr
+    expected = "\x00" * (skpnt - eof) + wstr
     assert xfile.read() == pfile.read().encode() == expected.encode()
     assert xfile.tell() == pfile.tell()
 
     xfile.seek(0), pfile.seek(0)
     assert xfile.read() == pfile.read().encode()
 
     xfile.truncate(skpnt), pfile.truncate(skpnt)
     assert xfile.tell() == pfile.tell() == skpnt + len(wstr)
 
     xfile.write(wstr), pfile.write(wstr)
-    expected = fc + '\x00'*(skpnt-eof+len(wstr)) + wstr
+    expected = fc + "\x00" * (skpnt - eof + len(wstr)) + wstr
     xfile.seek(0), pfile.seek(0)
     assert xfile.read() == pfile.read().encode() == expected.encode()
 
 
 def test_seek_past_eof_wr(tmppath):
     """Tests read/write/truncate behaviour after seeking past the EOF, 'w+'"""
     fd = get_tsta_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], u''
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], ""
+    fp2 = fb["full_path"]
 
     wstr = "www"
     eof = len(fc)
-    skpnt = len(fc)+4
+    skpnt = len(fc) + 4
 
-    pfile = open(fp2, 'w+')
-    xfile = XRootDPyFile(mkurl(fp), 'w+')
+    pfile = open(fp2, "w+")
+    xfile = XRootDPyFile(mkurl(fp), "w+")
 
     xfile.seek(skpnt), pfile.seek(skpnt)
     assert xfile.tell() == pfile.tell()
     assert xfile.read() == pfile.read().encode()
     assert xfile.tell() == pfile.tell()
     assert xfile.tell() == skpnt
 
     xfile.write(wstr), pfile.write(wstr)
     assert xfile.tell() == pfile.tell()
     xfile.seek(eof), pfile.seek(eof)
-    expected = '\x00'*(skpnt-eof) + wstr
+    expected = "\x00" * (skpnt - eof) + wstr
     assert xfile.read() == pfile.read().encode() == expected.encode()
     assert xfile.tell() == pfile.tell()
 
     xfile.seek(0), pfile.seek(0)
     assert xfile.read() == pfile.read().encode()
 
     xfile.truncate(skpnt), pfile.truncate(skpnt)
     assert xfile.tell() == pfile.tell() == skpnt + len(wstr)
 
     xfile.write(wstr), pfile.write(wstr)
-    expected = fc + '\x00'*(skpnt-eof+len(wstr)) + wstr
+    expected = fc + "\x00" * (skpnt - eof + len(wstr)) + wstr
     xfile.seek(0), pfile.seek(0)
     assert xfile.read() == pfile.read().encode() == expected.encode()
 
 
 def test_read_binary(tmppath):
     """Tests reading binary data from an existing file."""
     fd = get_bin_testfile(tmppath)
     fb = get_copy_file(fd, binary=True)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
+    fp2 = fb["full_path"]
 
-    pfile = open(fp2, 'rb')
-    xfile = XRootDPyFile(mkurl(fp), 'rb')
+    pfile = open(fp2, "rb")
+    xfile = XRootDPyFile(mkurl(fp), "rb")
 
     assert xfile.read() == pfile.read() == fc
 
 
 def test_write_binary(tmppath):
     """Tests for writing binary data to file."""
     fd = get_bin_testfile(tmppath)
-    fp, fc = fd['full_path'], fd['contents']
+    fp, fc = fd["full_path"], fd["contents"]
 
     # Test w/ confirmed binary data read from a binary file
-    xf_new = XRootDPyFile(mkurl(join(tmppath, 'data/tmp_bin')), 'wb+')
+    xf_new = XRootDPyFile(mkurl(join(tmppath, "data/tmp_bin")), "wb+")
     xf_new.write(fc), xf_new.seek(0)
     assert xf_new.read() == fc
 
     xf_new.close()
     # Verify persistence.
-    xf_new = XRootDPyFile(mkurl(join(tmppath, 'data/tmp_bin')), 'r+')
+    xf_new = XRootDPyFile(mkurl(join(tmppath, "data/tmp_bin")), "r+")
     assert xf_new.read() == fc
 
     # Test truncate
     xf_new.truncate()
     xf_new.seek(0)
     assert xf_new.read() == fc
     xf_new.close()
 
     # Test with bytearray
-    xf_new = XRootDPyFile(mkurl(join(tmppath, 'data/tmp_bin')), 'wb+')
+    xf_new = XRootDPyFile(mkurl(join(tmppath, "data/tmp_bin")), "wb+")
     barr = bytearray(range(0, 5))
     xf_new.write(barr), xf_new.seek(0)
     assert xf_new.read() == barr
     xf_new.close()
 
     # Verify persistence.
-    xf_new = XRootDPyFile(mkurl(join(tmppath, 'data/tmp_bin')), 'r')
+    xf_new = XRootDPyFile(mkurl(join(tmppath, "data/tmp_bin")), "r")
     assert xf_new.read() == barr
     xf_new.close()
 
 
 def test_readline(tmppath):
     """Tests for readline()."""
     fd = get_mltl_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
 
-    xfile, pfile = XRootDPyFile(mkurl(fp), 'r'), opener.open(fp2, 'r')
+    osfs = open_fs(fs.path.dirname(fd["full_path"]))
+    xfile, pfile = XRootDPyFile(mkurl(fp), "r"), osfs.open(fb["filename"], "r")
 
     assert xfile.readline() == pfile.readline().encode()
     assert xfile.readline() == pfile.readline().encode()
     assert xfile.readline() == pfile.readline().encode()
 
     xfile.close(), pfile.close()
-    xfile, pfile = XRootDPyFile(mkurl(fp), 'r'), opener.open(fp2, 'r')
+    xfile, pfile = XRootDPyFile(mkurl(fp), "r"), osfs.open(fb["filename"], "r")
     assert xfile.readline() == pfile.readline().encode()
     xfile.seek(0), pfile.seek(0)
     assert xfile.readline() == pfile.readline().encode()
     assert xfile.tell(), pfile.tell()
 
     xfile.close(), pfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'w+')
+    xfile = XRootDPyFile(mkurl(fp), "w+")
 
-    str1 = 'hello\n'
-    str2 = 'bye\n'
+    str1 = "hello\n"
+    str2 = "bye\n"
 
-    xfile.write(str1+str2)
+    xfile.write(str1 + str2)
     xfile.seek(0)
     assert xfile.readline() == str1.encode()
     assert xfile.readline() == str2.encode()
-    assert xfile.readline() == b''
-    assert xfile.readline() == b''
+    assert xfile.readline() == b""
+    assert xfile.readline() == b""
 
     xfile.seek(100)
-    assert xfile.readline() == b''
+    assert xfile.readline() == b""
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(fp), 'w+')
+    xfile = XRootDPyFile(mkurl(fp), "w+")
 
     xfile.write(str2)
-    xfile.seek(len(str2)+1)
+    xfile.seek(len(str2) + 1)
     xfile.write(str2)
     xfile.seek(0)
-    _value = u'\x00'+str2
+    _value = "\x00" + str2
     assert xfile.readline() == str2.encode()
     assert xfile.readline() == _value.encode()
 
 
 def test_flush(tmppath):
     """Tests for flush()"""
     # Mostly it just ensures calling it doesn't crash the program.
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
-    xfile = XRootDPyFile(mkurl(full_path), 'w')
+    full_path, fc = fd["full_path"], fd["contents"]
+    xfile = XRootDPyFile(mkurl(full_path), "w")
 
-    writestr = 'whut'
+    writestr = "whut"
 
     xfile.flush()
-    xfile.seek(0, SEEK_END)
+    xfile.seek(0, Seek.end)
     xfile.write(writestr)
     xfile.flush()
     xfile.close()
 
-    xfile = XRootDPyFile(mkurl(full_path), 'r')
+    xfile = XRootDPyFile(mkurl(full_path), "r")
     assert xfile.read() == writestr.encode()
 
     # Fake/mock an error response
     fake_status = {
         "status": 3,
         "code": 0,
         "ok": False,
         "errno": errno.EREMOTE,
         "error": True,
-        "message": '[FATAL] Remote I/O Error',
+        "message": "[FATAL] Remote I/O Error",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     # Assign mock return value to the file's sync() function
     # (which is called by flush())
     xfile._file.sync = Mock(return_value=(XRootDStatus(fake_status), None))
     pytest.raises(IOError, xfile.flush)
 
 
 def test__assert_mode(tmppath):
     """Tests for _assert_mode"""
     fd = get_tsta_file(tmppath)
-    full_path, fc = fd['full_path'], fd['contents']
-    mode = 'r'
+    full_path, fc = fd["full_path"], fd["contents"]
+    mode = "r"
     xfile = XRootDPyFile(mkurl(full_path), mode)
 
     assert xfile.mode == mode
     assert xfile._assert_mode(mode)
-    delattr(xfile, 'mode')
+    delattr(xfile, "mode")
     pytest.raises(AttributeError, xfile._assert_mode, mode)
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(full_path), 'r')
-    assert xfile._assert_mode('r')
-    pytest.raises(IOError, xfile._assert_mode, 'w')
+    xfile = XRootDPyFile(mkurl(full_path), "r")
+    assert xfile._assert_mode("r")
+    pytest.raises(IOError, xfile._assert_mode, "w")
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(full_path), 'w-')
-    assert xfile._assert_mode('w-')
-    pytest.raises(IOError, xfile._assert_mode, 'r')
+    xfile = XRootDPyFile(mkurl(full_path), "w-")
+    assert xfile._assert_mode("w-")
+    pytest.raises(IOError, xfile._assert_mode, "r")
 
     xfile.close()
-    xfile = XRootDPyFile(mkurl(full_path), 'a')
-    assert xfile._assert_mode('w')
-    pytest.raises(IOError, xfile._assert_mode, 'r')
+    xfile = XRootDPyFile(mkurl(full_path), "a")
+    assert xfile._assert_mode("w")
+    pytest.raises(IOError, xfile._assert_mode, "r")
 
 
 def test_readlines(tmppath):
     """Tests readlines()"""
     fd = get_mltl_file(tmppath)
     fb = get_copy_file(fd)
-    fp, fc = fd['full_path'], fd['contents']
-    fp2 = fb['full_path']
+    fp, fc = fd["full_path"], fd["contents"]
 
-    xfile, pfile = XRootDPyFile(mkurl(fp), 'r'), open(fp2, 'r')
+    osfs = open_fs(fs.path.dirname(fb["full_path"]))
+    xfile, pfile = XRootDPyFile(mkurl(fp), "r"), osfs.open(fb["filename"], "r")
 
     xfile.seek(0), pfile.seek(0)
     expected = _list_str_encode(pfile.readlines())
     assert xfile.readlines() == expected
 
     xfile.close(), pfile.close()
 
-    xfile, pfile = XRootDPyFile(mkurl(fp), 'w+'), open(fp2, 'w+')
+    xfile, pfile = XRootDPyFile(mkurl(fp), "w+"), osfs.open(fb["filename"], "w+")
     xfile.seek(0), pfile.seek(0)
     expected = _list_str_encode(pfile.readlines())
     assert xfile.readlines() == expected
 
 
 def test_xreadlines(tmppath):
     """Tests xreadlines()"""
-    fp = get_mltl_file(tmppath)['full_path']
+    fp = get_mltl_file(tmppath)["full_path"]
 
-    xfile = XRootDPyFile(mkurl(fp), 'r')
+    xfile = XRootDPyFile(mkurl(fp), "r")
 
     rl = xfile.readlines()
     xfile.seek(0)
     xl = xfile.xreadlines()
     assert xl != rl
     assert list(xl) == rl
 
 
 def test_fileno(tmppath):
     """Test fileno."""
     pytest.raises(
-        IOError,
-        XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), 'r-').fileno
+        IOError, XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r-").fileno
     )
 
 
 def test_name(tmppath):
     """Test name property."""
-    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt"))).name == \
-        'testa.txt'
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt"))).name == "testa.txt"
 
 
 def test_isatty(tmppath):
     """Test isatty()."""
-    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt"))).isatty() is \
-        False
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt"))).isatty() is False
 
 
 def test_writelines(tmppath):
     """Test writelines()."""
-    xfile = XRootDPyFile(mkurl(join(tmppath, "data/multiline.txt")), 'r')
-    yfile = XRootDPyFile(mkurl(join(tmppath, "data/newfile.txt")), 'w+')
+    xfile = XRootDPyFile(mkurl(join(tmppath, "data/multiline.txt")), "r")
+    yfile = XRootDPyFile(mkurl(join(tmppath, "data/newfile.txt")), "w+")
     yfile.writelines(xfile.xreadlines())
     xfile.seek(0), yfile.seek(0)
     assert xfile.readlines() == yfile.readlines()
 
 
 def test_seekable(tmppath):
     """Test seekable."""
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r-').seekable() is False
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r').seekable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w').seekable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w-').seekable() is False
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r+').seekable() is True
+    assert (
+        XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r-").seekable() is False
+    )
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r").seekable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w").seekable() is True
+    assert (
+        XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w-").seekable() is False
+    )
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r+").seekable() is True
 
 
 def test_readable(tmppath):
     """Test seekable."""
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r-').readable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r').readable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w').readable() is False
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r+').readable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w+').readable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w-').readable() is False
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r-").readable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r").readable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w").readable() is False
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r+").readable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w+").readable() is True
+    assert (
+        XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w-").readable() is False
+    )
 
 
 def test_writable(tmppath):
     """Test seekable."""
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r-').writable() is False
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r').writable() is False
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w').writable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'r+').writable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w+').writable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'w-').writable() is True
-    assert XRootDPyFile(
-        mkurl(join(tmppath, "data/testa.txt")), 'a').writable() is True
+    assert (
+        XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r-").writable() is False
+    )
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r").writable() is False
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w").writable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "r+").writable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w+").writable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "w-").writable() is True
+    assert XRootDPyFile(mkurl(join(tmppath, "data/testa.txt")), "a").writable() is True
 
 
 def test_iterator_buffering(tmppath):
     "Test file iteration."
     f = "data/multiline.txt"
-    xfile = XRootDPyFile(mkurl(join(tmppath, f)), 'r')
+    xfile = XRootDPyFile(mkurl(join(tmppath, f)), "r")
     assert len(list(iter(xfile))) == len(open(join(tmppath, f)).readlines())
-    xfile = XRootDPyFile(mkurl(join(tmppath, f)), 'r', buffering=10)
+    xfile = XRootDPyFile(mkurl(join(tmppath, f)), "r", buffering=10)
     assert len(list(iter(xfile))) == int(math.ceil(xfile.size / 10.0))
 
 
 def remove_file(tmppath, file):
     from XRootD import client
+
     myclient = client.FileSystem(tmppath)
     myclient.rm(file)
 
 
 def create_big_file(
     tmppath,
     filename,
     size=2 * 1024 * 1024 * 1024,
     frontfile_content=None,
-    endfile_content=None
+    endfile_content=None,
 ):
-    xfile = XRootDPyFile(mkurl(join(tmppath, filename)), 'w')
+    xfile = XRootDPyFile(mkurl(join(tmppath, filename)), "w")
     if endfile_content:
         endfile_length = len(endfile_content)
     else:
-        endfile_content = '\0'
+        endfile_content = "\0"
         endfile_length = 1
     # Prepare big file for testing
     if frontfile_content:
         xfile.write(frontfile_content)
     xfile.seek(size - endfile_length)
     xfile.write(endfile_content)
     xfile.close()
 
 
 def test_reading_end_of_big_file(tmppath):
     """Tests reading end of big file."""
     f = "data/big_file.txt"
     create_big_file(tmppath, f, endfile_content="test\0")
 
-    xfile = XRootDPyFile(mkurl(join(tmppath, f)), 'r')
+    xfile = XRootDPyFile(mkurl(join(tmppath, f)), "r")
 
-    xfile.seek(xfile.size-10)
+    xfile.seek(xfile.size - 10)
     data = xfile.read()
     assert xfile.size == 2 * 1024 * 1024 * 1024
     assert len(data) == 10
     assert data[-5:-1] == b"test"
     xfile.close()
 
     remove_file(tmppath, f)
 
 
 def test_reading_whole_big_file(tmppath):
     """Tests reading end of big file."""
     f = "data/big_file.txt"
     create_big_file(tmppath, f)
 
-    xfile = XRootDPyFile(mkurl(join(tmppath, f)), 'r')
+    xfile = XRootDPyFile(mkurl(join(tmppath, f)), "r")
 
     pytest.raises(IOError, xfile.read)
     xfile.close()
 
     remove_file(tmppath, f)
 
 
 def test_reading_begining_of_big_file(tmppath):
     """Tests reading end of big file."""
     f = "data/big_file.txt"
     create_big_file(tmppath, f, frontfile_content="test")
 
-    xfile = XRootDPyFile(mkurl(join(tmppath, f)), 'r')
+    xfile = XRootDPyFile(mkurl(join(tmppath, f)), "r")
 
     data = xfile.read(4)
     assert data == b"test"
     xfile.close()
 
     remove_file(tmppath, f)
```

### Comparing `xrootdpyfs-0.2.2/tests/test_env.py` & `xrootdpyfs-1.0.0a1/tests/test_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,37 +4,39 @@
 # Copyright (C) 2015 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Test of environment variables."""
 
-from __future__ import absolute_import, print_function
-
 import os
 
-from xrootdpyfs.env import set_connectionretry, set_connectionwindow, \
-    set_timeout, set_timeoutresolution
+from xrootdpyfs.env import (
+    set_connectionretry,
+    set_connectionwindow,
+    set_timeout,
+    set_timeoutresolution,
+)
 
 
 def test_set_timeout():
     """Test set_timeout."""
     set_timeout(20)
-    assert os.environ['XRD_REQUESTTIMEOUT'] == "20"
+    assert os.environ["XRD_REQUESTTIMEOUT"] == "20"
 
 
 def test_set_timeoutresolution():
     """Test set_timeoutresolution."""
     set_timeoutresolution(2)
-    assert os.environ['XRD_TIMEOUTRESOLUTION'] == "2"
+    assert os.environ["XRD_TIMEOUTRESOLUTION"] == "2"
 
 
 def test_set_connectionretry():
     """Test set_timeoutresolution."""
     set_connectionretry(2)
-    assert os.environ['XRD_CONNECTIONRETRY'] == "2"
+    assert os.environ["XRD_CONNECTIONRETRY"] == "2"
 
 
 def test_set_connectionwindow():
     """Test set_timeoutresolution."""
     set_connectionwindow(10)
-    assert os.environ['XRD_CONNECTIONWINDOW'] == "10"
+    assert os.environ["XRD_CONNECTIONWINDOW"] == "10"
```

### Comparing `xrootdpyfs-0.2.2/tests/test_xrdflags.py` & `xrootdpyfs-1.0.0a1/tests/test_xrdflags.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 # Copyright (C) 2015 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Test of XRootD File Flags."""
 
-from __future__ import absolute_import, print_function
-
 from os.path import join
 
 from conftest import mkurl
 from XRootD import client as xclient
 from XRootD.client.flags import OpenFlags
 
 
 # If "test" is in its name then pytest picks it up.
 def tstfile_a(p):
-    fname = 'data/testa.txt'
+    fname = "data/testa.txt"
     with open(join(p, fname)) as f:
         fconts = f.read()
 
     return fname, fconts
 
 
 def test_READ(tmppath):
@@ -35,23 +33,23 @@
 
     # Can we read?
     statmsg, content = xf.read()
     assert content == fconts.encode()
     assert statmsg.ok
 
     # Can we write?
-    statmsg, res = xf.write('chhhh-eck it')
-    print((statmsg, ))  # Print returned status in case the test fails.
+    statmsg, res = xf.write("chhhh-eck it")
+    print((statmsg,))  # Print returned status in case the test fails.
     assert xf.read()[1] == content
     assert not statmsg.ok
     assert statmsg.error
 
     # Can we truncate?
     statmsg, res = xf.truncate(0)
-    print((statmsg, ))
+    print((statmsg,))
     assert not statmsg.ok
     assert statmsg.error
 
 
 def test_APPEND(tmppath):
     fname, fconts = tstfile_a(tmppath)
     ffpath = join(tmppath, fname)
@@ -61,17 +59,17 @@
 
     # Can we read?
     statmsg, content = xf.read()
     assert content == fconts.encode()
     assert statmsg.ok
 
     # Can we write?
-    statmsg, res = xf.write('chhhh-eck it')
+    statmsg, res = xf.write("chhhh-eck it")
     assert xf.read()[1] == content
-    print((statmsg, ))
+    print((statmsg,))
     assert not statmsg.ok
     assert statmsg.error
 
 
 def test_UPDATE(tmppath):
     fname, fconts = tstfile_a(tmppath)
     ffpath = join(tmppath, fname)
@@ -81,15 +79,15 @@
 
     # Can we read?
     statmsg, content = xf.read()
     assert content == fconts.encode()
     assert statmsg.ok
 
     # Can we write?
-    statmsg, res = xf.write('chhhh-eck it')
+    statmsg, res = xf.write("chhhh-eck it")
     # assert xf.read()[1] == content
     # doesn't truncate file
     print((statmsg, res))
     assert statmsg.ok
     assert not statmsg.error
 
     # Can we truncate?
```

### Comparing `xrootdpyfs-0.2.2/tests/perf.py` & `xrootdpyfs-1.0.0a1/tests/perf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of xrootdpyfs
-# Copyright (C) 2015 CERN.
+# Copyright (C) 2015-2023 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Simple performance test of XRootD PyFilesystem wrapper.
 
 Tests:
@@ -20,55 +20,55 @@
 import pstats
 import shutil
 import tempfile
 import time
 from io import StringIO
 from os.path import join
 
-from fs.opener import opener
+from fs.opener import open_fs
 from XRootD import client
 
-from xrootdpyfs import XRootDPyOpener  # no-qa
-
 
 def teardown(tmppath):
     """Tear down performance test."""
     shutil.rmtree(tmppath)
 
 
 def setup():
     """Setup test files for performance test."""
+    filename = "testfile"
     tmppath = tempfile.mkdtemp()
-    filepath = join(tmppath, "testfile")
+    filepath = join(tmppath, filename)
 
     # Create test file with random data
-    os.system("dd bs=1024 count={1} </dev/urandom >{0}".format(
-        filepath, 1024*10))
+    os.system("dd bs=1024 count={1} </dev/urandom >{0}".format(filepath, 1024 * 10))
 
-    return tmppath, filepath
+    return filename, tmppath, filepath
 
 
 #
 # Test methods
 #
-def read_pyfs_chunks(url, chunksize=2097152, n=100):
+def read_pyfs_chunks(url, filename, mode="rb", chunksize=2097152, n=100):
     """Read a file in chunks."""
     t1 = time.time()
 
+    fs = open_fs(url)
+    assert fs.exists(filename)
     i = 0
     while i < n:
-        fsfile = opener.open(url, 'rb-')
+        fsfile = fs.open(filename, "rb")
         while True:
             data = fsfile.read(chunksize)
             if not data:
                 break
         i += 1
 
     t2 = time.time()
-    return (t2-t1)/n
+    return (t2 - t1) / n
 
 
 def read_pyxrootd_chunks(url, chunksize=2097152, n=100):
     """Read a file in chunks."""
     t1 = time.time()
 
     i = 0
@@ -79,48 +79,49 @@
         for chunk in fsfile.readchunks(offset=0, chunksize=chunksize):
             pass
 
         fsfile.close()
         i += 1
 
     t2 = time.time()
-    return (t2-t1)/n
+    return (t2 - t1) / n
 
 
 def profile_start():
     """Start profiling code."""
     pr = cProfile.Profile()
     pr.enable()
     return pr
 
 
 def profile_end(pr):
     """Write profile output."""
     pr.disable()
-    s = StringIO.StringIO()
-    sortby = 'tottime'
+    s = StringIO()
+    sortby = "tottime"
     ps = pstats.Stats(pr, stream=s).sort_stats(sortby)
     ps.print_stats()
     print(s.getvalue())
 
 
 def main():
     """Main entry point."""
-    tmppath, testfilepath = setup()
+    filename, tmppath, testfilepath = setup()
 
     try:
         n = 10
-        rooturl = 'root://localhost/{0}'.format(testfilepath)
-        osurl = testfilepath
+        rooturl = "root://localhost/{0}".format(testfilepath)
 
-        print("osfs:", osurl, read_pyfs_chunks(osurl, n=n))
+        print("osfs:", testfilepath, read_pyfs_chunks(tmppath, filename, n=n))
         print("pyxrootd:", rooturl, read_pyxrootd_chunks(rooturl, n=n))
 
         pr = profile_start()
-        print("xrootdpyfs:", rooturl, read_pyfs_chunks(rooturl, n=n))
+        print(
+            "xrootdpyfs:", rooturl, read_pyfs_chunks(rooturl, filename, mode="rb-", n=n)
+        )
         profile_end(pr)
     finally:
         teardown(tmppath)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `xrootdpyfs-0.2.2/tests/test_utils.py` & `xrootdpyfs-1.0.0a1/tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 # Copyright (C) 2015 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Test of XRootDPyFS utils."""
 
-from __future__ import absolute_import, print_function
-
 from XRootD.client.flags import OpenFlags
 
-from xrootdpyfs.utils import is_valid_path, spliturl, \
-    translate_file_mode_to_flags
+from xrootdpyfs.utils import is_valid_path, spliturl, translate_file_mode_to_flags
 
 
 def test_spliturl():
     """Test spliturl."""
     root, path, args = spliturl("root://eosuser.cern.ch//eos/user/")
     assert root == "root://eosuser.cern.ch"
     assert path == "//eos/user/"
@@ -46,19 +43,20 @@
     assert not is_valid_path("/")
     assert not is_valid_path("///")
     assert not is_valid_path("//missing//what")
 
 
 def test_translate_file_mode_to_flags():
     """Test mode to xrootd flags translation."""
-    assert translate_file_mode_to_flags('in') == 0
-    assert translate_file_mode_to_flags('r') == OpenFlags.READ
-    assert translate_file_mode_to_flags('r-') == OpenFlags.READ
-    assert bool(translate_file_mode_to_flags('r+') & (
-        OpenFlags.UPDATE | OpenFlags.READ))
-
-    assert translate_file_mode_to_flags('a') == OpenFlags.UPDATE
-    assert translate_file_mode_to_flags('a+') == OpenFlags.UPDATE
-
-    assert translate_file_mode_to_flags('w') == OpenFlags.DELETE
-    assert translate_file_mode_to_flags('w-') == OpenFlags.DELETE
-    assert translate_file_mode_to_flags('w+') == OpenFlags.DELETE
+    assert translate_file_mode_to_flags("in") == 0
+    assert translate_file_mode_to_flags("r") == OpenFlags.READ
+    assert translate_file_mode_to_flags("r-") == OpenFlags.READ
+    assert bool(
+        translate_file_mode_to_flags("r+") & (OpenFlags.UPDATE | OpenFlags.READ)
+    )
+
+    assert translate_file_mode_to_flags("a") == OpenFlags.UPDATE
+    assert translate_file_mode_to_flags("a+") == OpenFlags.UPDATE
+
+    assert translate_file_mode_to_flags("w") == OpenFlags.DELETE
+    assert translate_file_mode_to_flags("w-") == OpenFlags.DELETE
+    assert translate_file_mode_to_flags("w+") == OpenFlags.DELETE
```

### Comparing `xrootdpyfs-0.2.2/tests/test_fs.py` & `xrootdpyfs-1.0.0a1/tests/test_fs.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,28 +4,35 @@
 # Copyright (C) 2015 CERN.
 #
 # xrootdpyfs is free software; you can redistribute it and/or modify it under
 # the terms of the Revised BSD License; see LICENSE file for more details.
 
 """Test of XRootDPyFS."""
 
-from __future__ import absolute_import, print_function
-
 import os
 import types
 from datetime import datetime
 from functools import wraps
 from os.path import exists, join
 
 import pytest
 from conftest import mkurl
-from fs.errors import BackReferenceError, DestinationExistsError, \
-    DirectoryNotEmptyError, FSError, InvalidPathError, RemoteConnectionError, \
-    ResourceError, ResourceInvalidError, ResourceNotFoundError, \
-    UnsupportedError
+from fs import ResourceType
+from fs.errors import (
+    DestinationExists,
+    DirectoryNotEmpty,
+    FSError,
+    IllegalBackReference,
+    InvalidPath,
+    RemoteConnectionError,
+    ResourceError,
+    ResourceInvalid,
+    ResourceNotFound,
+    Unsupported,
+)
 from mock import Mock
 from XRootD.client.responses import XRootDStatus
 
 from xrootdpyfs import XRootDPyFile, XRootDPyFS
 from xrootdpyfs.utils import spliturl
 
 
@@ -35,73 +42,73 @@
     assert fs.xrd_client
     assert fs.base_path == "//tmp/"
     assert fs.root_url == "root://127.0.0.1"
 
     XRootDPyFS("root://user:pw@eosuser.cern.ch//")
     XRootDPyFS("root://eosuser.cern.ch//")
     XRootDPyFS("root://eosuser.cern.ch//")
-    pytest.raises(InvalidPathError, XRootDPyFS, "http://localhost")
-    pytest.raises(InvalidPathError, XRootDPyFS,
-                  "root://eosuser.cern.ch//lhc//")
+    pytest.raises(InvalidPath, XRootDPyFS, "http://localhost")
+    pytest.raises(InvalidPath, XRootDPyFS, "root://eosuser.cern.ch//lhc//")
 
     rooturl = mkurl(tmppath)
     fs = XRootDPyFS(rooturl)
     root_url, base_path, qargs = spliturl(rooturl)
     assert fs.xrd_client
     assert fs.base_path == base_path
     assert fs.root_url == root_url
     assert fs.queryargs is None
 
     qarg = "xrd.wantprot=krb5"
-    fs = XRootDPyFS(rooturl + '?' + qarg)
-    root_url, base_path, qargs = spliturl(rooturl + '?' + qarg)
+    fs = XRootDPyFS(rooturl + "?" + qarg)
+    root_url, base_path, qargs = spliturl(rooturl + "?" + qarg)
     assert fs.base_path == base_path
     assert fs.root_url == root_url
-    assert fs.queryargs == {'xrd.wantprot': 'krb5'}
+    assert fs.queryargs == {"xrd.wantprot": "krb5"}
     assert qargs == qarg
 
     qarg = "xrd.wantprot=krb5"
-    fs = XRootDPyFS(rooturl + '?' + qarg, query={'xrd.k5ccname': '/tmp/krb'})
+    fs = XRootDPyFS(rooturl + "?" + qarg, query={"xrd.k5ccname": "/tmp/krb"})
 
     assert fs.queryargs == {
-        'xrd.wantprot': 'krb5',
-        'xrd.k5ccname': '/tmp/krb',
+        "xrd.wantprot": "krb5",
+        "xrd.k5ccname": "/tmp/krb",
     }
 
     pytest.raises(
-        KeyError,
-        XRootDPyFS,
-        rooturl + '?' + qarg, query={'xrd.wantprot': 'krb5'}
+        KeyError, XRootDPyFS, rooturl + "?" + qarg, query={"xrd.wantprot": "krb5"}
     )
 
 
 def test_p():
     """Test path combine."""
     fs = XRootDPyFS("root://eosuser.cern.ch//eos/user/")
     assert fs._p("./") == "//eos/user"
     assert fs._p("l") == "//eos/user/l"
-    assert fs._p("/eos") == "//eos"
+    assert fs._p("/eos/user") == "//eos/user"
+    assert fs._p("//eos/user") == "//eos/user"
+    assert fs._p("/eos/user/folder") == "//eos/user/folder"
+    assert fs._p("//eos/user/folder") == "//eos/user/folder"
     assert fs._p("../") == "//eos"
     assert fs._p("../project/test") == "//eos/project/test"
     assert fs._p("../project/../test") == "//eos/test"
-    pytest.raises(BackReferenceError, fs._p, "../../../test")
+    pytest.raises(IllegalBackReference, fs._p, "../../../test")
 
 
 def test_query_error(tmppath):
     """Test unknown error from query."""
     fs = XRootDPyFS(mkurl(tmppath))
     fake_status = {
         "status": 3,
         "code": 101,
         "ok": False,
         "errno": 0,
         "error": True,
-        "message": '[FATAL] Invalid address',
+        "message": "[FATAL] Invalid address",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     fs.xrd_client.query = Mock(return_value=(XRootDStatus(fake_status), None))
     pytest.raises(FSError, fs._query, 3, "data/testa.txt")
 
 
 def test_ilistdir(tmppath):
     """Test the ilistdir returns a generator."""
@@ -111,47 +118,41 @@
 
 def test_listdir(tmppath):
     """Test listdir."""
     rooturl = mkurl(tmppath)
 
     dirs = XRootDPyFS(rooturl).listdir()
     assert len(dirs) == 1
-    assert 'data' in dirs
+    assert "data" in dirs
 
     dirs = XRootDPyFS(rooturl).listdir("data")
     assert len(dirs) == 5
 
     dirs = XRootDPyFS(rooturl + "/data").listdir("afolder", full=True)
-    assert 'afolder/afile.txt' in dirs
+    assert "afolder/afile.txt" in dirs
+
+    dirs = XRootDPyFS(rooturl + "/data").listdir("afolder/../bfolder", full=True)
+    assert "bfolder/bfile.txt" in dirs
 
-    dirs = XRootDPyFS(rooturl + "/data").listdir("afolder/../bfolder",
-                                                 full=True)
-    assert 'bfolder/bfile.txt' in dirs
-
-    dirs = XRootDPyFS(rooturl + "/data").listdir(
-        "afolder", absolute=True)
-    assert '/' + tmppath + "/data/afolder/afile.txt" in dirs
-
-    # abosolute/full conflicts - full wins.
-    dirs = XRootDPyFS(rooturl + "/data").listdir(
-        "afolder", absolute=True, full=True)
+    dirs = XRootDPyFS(rooturl + "/data").listdir("afolder", absolute=True)
+    assert "/" + tmppath + "/data/afolder/afile.txt" in dirs
+
+    # absolute/full conflicts - full wins.
+    dirs = XRootDPyFS(rooturl + "/data").listdir("afolder", absolute=True, full=True)
     assert "afolder/afile.txt" in dirs
 
     dirs = XRootDPyFS(rooturl).listdir("data", wildcard="*.txt")
-    assert 'testa.txt' in dirs
-    assert 'afolder' not in dirs
+    assert "testa.txt" in dirs
+    assert "afolder" not in dirs
 
     pytest.raises(
-        ValueError,
-        XRootDPyFS(rooturl).listdir,
-        "data", files_only=True, dirs_only=True
+        ValueError, XRootDPyFS(rooturl).listdir, "data", files_only=True, dirs_only=True
     )
 
-    pytest.raises(ResourceNotFoundError, XRootDPyFS(rooturl).listdir,
-                  "invalid")
+    pytest.raises(ResourceNotFound, XRootDPyFS(rooturl).listdir, "invalid")
 
 
 def test_isfile(tmppath):
     """Test isfile."""
     rooturl = mkurl(tmppath)
     assert XRootDPyFS(rooturl).isfile("data/testa.txt")
     assert not XRootDPyFS(rooturl).isfile("data")
@@ -181,188 +182,180 @@
     # Dir in parent
     assert not XRootDPyFS(rooturl).exists("somedir")
     assert XRootDPyFS(rooturl).makedir("somedir")
     assert XRootDPyFS(rooturl).exists("somedir")
     assert exists(join(tmppath, "somedir"))
 
     # if the path is already a directory, and allow_recreate is False
-    assert pytest.raises(DestinationExistsError, XRootDPyFS(rooturl).makedir,
-                         "data")
+    assert pytest.raises(DestinationExists, XRootDPyFS(rooturl).makedir, "data")
 
     # allow_recreate
     assert XRootDPyFS(rooturl).makedir("data", allow_recreate=True)
 
     # if a containing directory is missing and recursive is False
-    assert pytest.raises(ResourceNotFoundError,
-                         XRootDPyFS(rooturl).makedir, "aa/bb/cc")
+    assert pytest.raises(ResourceNotFound, XRootDPyFS(rooturl).makedir, "aa/bb/cc")
 
     # Recursive
     assert not XRootDPyFS(rooturl).exists("aa/bb/cc")
     assert XRootDPyFS(rooturl).makedir("aa/bb/cc", recursive=True)
     assert XRootDPyFS(rooturl).exists("aa/bb/cc")
 
     # if a path is an existing file
-    assert pytest.raises(DestinationExistsError, XRootDPyFS(rooturl).makedir,
-                         "data/testa.txt")
+    assert pytest.raises(
+        DestinationExists, XRootDPyFS(rooturl).makedir, "data/testa.txt"
+    )
 
 
 def test_unicode_paths(tmppath):
     """Test creation of unicode paths."""
     fs = XRootDPyFS(mkurl(tmppath))
-    d = u'\xe6\xf8\xe5'
+    d = "\xe6\xf8\xe5"
     assert not fs.exists(d)
     assert fs.makedir(d)
     assert fs.exists(d)
-    d = '\xc3\xb8\xc3\xa5\xc3\xa6'
+    d = "\xc3\xb8\xc3\xa5\xc3\xa6"
     assert not fs.exists(d)
     assert fs.makedir(d)
     assert fs.exists(d)
 
 
 def test_remove(tmppath):
     """Test remove."""
     rooturl = mkurl(tmppath)
 
     assert XRootDPyFS(rooturl).exists("data/testa.txt")
     XRootDPyFS(rooturl).remove("data/testa.txt")
     assert not XRootDPyFS(rooturl).exists("data/testa.txt")
 
     # Does not exists
-    assert pytest.raises(ResourceNotFoundError, XRootDPyFS(rooturl).remove,
-                         "a/testa.txt")
+    assert pytest.raises(ResourceNotFound, XRootDPyFS(rooturl).remove, "a/testa.txt")
 
     # Directory not empty
-    assert pytest.raises(DirectoryNotEmptyError, XRootDPyFS(rooturl).remove,
-                         "data")
+    assert pytest.raises(DirectoryNotEmpty, XRootDPyFS(rooturl).remove, "data")
 
     # Remove emptydir
     assert XRootDPyFS(rooturl).makedir("emptydir")
     assert XRootDPyFS(rooturl).remove("emptydir")
 
 
 def test_remove_dir(tmppath):
     """Test removedir."""
     fs = XRootDPyFS(mkurl(tmppath))
 
     # Remove non-empty directory
-    pytest.raises(
-        DirectoryNotEmptyError, fs.removedir, "data/bfolder/")
+    pytest.raises(DirectoryNotEmpty, fs.removedir, "data/bfolder/")
 
     # Use of recursive parameter
-    pytest.raises(
-        UnsupportedError, fs.removedir, "data/bfolder/", recursive=True)
+    pytest.raises(Unsupported, fs.removedir, "data/bfolder/", recursive=True)
 
     # Remove file
-    pytest.raises(
-        ResourceInvalidError, fs.removedir, "data/testa.txt")
+    pytest.raises(ResourceInvalid, fs.removedir, "data/testa.txt")
 
     # Remove empty directory
     fs.makedir("data/tmp")
     assert fs.removedir("data/tmp") and not fs.exists("data/tmp")
 
     # Remove non-empty directory
     assert fs.removedir("data/bfolder/", force=True)
     assert fs.removedir("data/", force=True)
 
 
 def test_remove_dir_mock1(tmppath):
     """Test removedir."""
     fs = XRootDPyFS(mkurl(tmppath))
 
-    status = XRootDStatus({
-        "status": 3,
-        "code": 101,
-        "ok": False,
-        "errno": 0,
-        "error": True,
-        "message": '[FATAL] Invalid address',
-        "fatal": True,
-        "shellcode": 51
-    })
+    status = XRootDStatus(
+        {
+            "status": 3,
+            "code": 101,
+            "ok": False,
+            "errno": 0,
+            "error": True,
+            "message": "[FATAL] Invalid address",
+            "fatal": True,
+            "shellcode": 51,
+        }
+    )
     fs.xrd_client.rm = Mock(return_value=(status, None))
     pytest.raises(ResourceError, fs.removedir, "data/bfolder/", force=True)
 
 
 def test_remove_dir_mock2(tmppath):
     """Test removedir."""
     fs = XRootDPyFS(mkurl(tmppath))
 
-    status = XRootDStatus({
-        "status": 3,
-        "code": 101,
-        "ok": False,
-        "errno": 0,
-        "error": True,
-        "message": '[FATAL] Invalid address',
-        "fatal": True,
-        "shellcode": 51
-    })
+    status = XRootDStatus(
+        {
+            "status": 3,
+            "code": 101,
+            "ok": False,
+            "errno": 0,
+            "error": True,
+            "message": "[FATAL] Invalid address",
+            "fatal": True,
+            "shellcode": 51,
+        }
+    )
 
     def fail(f, fail_on):
         @wraps(f)
         def inner(path, **kwargs):
             if path == fail_on:
                 return (status, None)
             return f(path, **kwargs)
+
         return inner
 
     fs.xrd_client.rmdir = fail(fs.xrd_client.rmdir, fs._p("data/bfolder/"))
     pytest.raises(ResourceError, fs.removedir, "data/", force=True)
 
 
 def test_open(tmppath):
     """Test fs.open()"""
     # Create a file to open.
-    file_name = 'data/testa.txt'
-    expected_content = b'testa.txt\n'
+    file_name = "data/testa.txt"
+    expected_content = b"testa.txt\n"
     xrd_rooturl = mkurl(tmppath)
 
     # Open file w/ xrootd
     xrdfs = XRootDPyFS(xrd_rooturl)
-    xfile = xrdfs.open(file_name, mode='r')
+    xfile = xrdfs.open(file_name, mode="r")
     assert xfile
     assert xfile.path.endswith("data/testa.txt")
     assert type(xfile) == XRootDPyFile
     assert xfile.read() == expected_content
     xfile.close()
 
     # Test passing of querystring.
     xrdfs = XRootDPyFS(xrd_rooturl + "?xrd.wantprot=krb5")
-    xfile = xrdfs.open(file_name, mode='r')
+    xfile = xrdfs.open(file_name, mode="r")
     assert xfile
     assert xfile.path.endswith("data/testa.txt?xrd.wantprot=krb5")
     assert type(xfile) == XRootDPyFile
     assert xfile.read() == expected_content
     xfile.close()
 
 
 def _get_content(fs, path):
-    f = fs.open(path, 'r')
+    f = fs.open(path, "r")
     content = f.read()
     f.close()
     return content
 
 
 def test_rename(tmppath):
     """Test rename."""
     fs = XRootDPyFS(mkurl(tmppath))
 
-    pytest.raises(
-        DestinationExistsError, fs.rename, "data/testa.txt", "multiline.txt")
-    pytest.raises(
-        DestinationExistsError, fs.rename, "data/testa.txt",
-        "afolder/afile.txt")
-    pytest.raises(
-        DestinationExistsError, fs.rename, "data/afolder", "bfolder")
-    pytest.raises(
-        DestinationExistsError, fs.rename, "data/afolder", "bfolder/bfile.txt")
+    pytest.raises(DestinationExists, fs.rename, "data/testa.txt", "multiline.txt")
+    pytest.raises(DestinationExists, fs.rename, "data/testa.txt", "afolder/afile.txt")
+    pytest.raises(DestinationExists, fs.rename, "data/afolder", "bfolder")
+    pytest.raises(DestinationExists, fs.rename, "data/afolder", "bfolder/bfile.txt")
 
-    pytest.raises(
-        ResourceNotFoundError, fs.rename, "data/invalid.txt",
-        "afolder/afile.txt")
+    pytest.raises(ResourceNotFound, fs.rename, "data/invalid.txt", "afolder/afile.txt")
 
     assert fs.exists("data/testa.txt") and not fs.exists("data/testb.txt")
     fs.rename("data/testa.txt", "testb.txt")
     assert fs.exists("data/testb.txt") and not fs.exists("data/testa.txt")
 
     assert fs.exists("data/afolder/") and not fs.exists("data/cfolder/")
     fs.rename("data/afolder/", "cfolder")
@@ -372,113 +365,127 @@
     assert fs.exists("data/a/b/c/test/")
 
 
 def test_getinfo(tmppath):
     """Test getinfo."""
     fs = XRootDPyFS(mkurl(tmppath))
 
+    namespaces = ["details", "stat", "lstat", "link", "access", "xrootd"]
+
     # Info for file
     f = "data/testa.txt"
-    info = fs.getinfo(f)
-    assert info['size'] == os.stat(join(tmppath, f)).st_size
-    assert info['offline'] is False
-    assert info['writable'] is True
-    assert info['readable'] is True
-    assert info['executable'] is False
-    assert isinstance(info['created_time'], datetime)
-    assert isinstance(info['modified_time'], datetime)
-    assert isinstance(info['accessed_time'], datetime)
+    info = fs.getinfo(f, namespaces)
+    assert info.name == "testa.txt"
+    assert info.is_dir is False
+    assert info.size == os.stat(join(tmppath, f)).st_size
+    assert info.type == ResourceType.file
+    assert info.uid == b"*"
+    assert info.gid == b"*"
+    assert info.get("xrootd", "offline") is False
+    assert info.get("xrootd", "writable") is True
+    assert info.get("xrootd", "readable") is True
+    assert info.get("xrootd", "executable") is False
+    assert isinstance(info.created, datetime)
+    assert isinstance(info.modified, datetime)
+    assert isinstance(info.accessed, datetime)
 
     # Info for directory
     f = "data/"
-    info = fs.getinfo(f)
-    assert info['size'] == os.stat(join(tmppath, f)).st_size
-    assert info['offline'] is False
-    assert info['writable'] is True
-    assert info['readable'] is True
-    assert info['executable'] is True
-    assert isinstance(info['created_time'], datetime)
-    assert isinstance(info['modified_time'], datetime)
-    assert isinstance(info['accessed_time'], datetime)
+    info = fs.getinfo(f, namespaces)
+    assert info.name == ""
+    assert info.is_dir is True
+    assert info.size == os.stat(join(tmppath, f)).st_size
+    assert info.type == ResourceType.directory
+    assert info.uid == b"*"
+    assert info.gid == b"*"
+    assert info.get("xrootd", "offline") is False
+    assert info.get("xrootd", "writable") is True
+    assert info.get("xrootd", "readable") is True
+    assert info.get("xrootd", "executable") is True
+    assert isinstance(info.created, datetime)
+    assert isinstance(info.modified, datetime)
+    assert isinstance(info.accessed, datetime)
 
     # Non existing path
-    pytest.raises(ResourceNotFoundError, fs.getinfo, "invalidpath/")
+    pytest.raises(ResourceNotFound, fs.getinfo, "invalidpath/")
 
 
 def test_getpathurl(tmppath):
     """Test getpathurl."""
     fs = XRootDPyFS(mkurl(tmppath))
-    assert fs.getpathurl("data/testa.txt") == \
-        "root://localhost/{0}/{1}".format(tmppath, "data/testa.txt")
+    assert fs.getpathurl("data/testa.txt") == "root://localhost/{0}/{1}".format(
+        tmppath, "data/testa.txt"
+    )
 
-    fs = XRootDPyFS(mkurl(tmppath), query={'xrd.wantprot': 'krb5'})
+    fs = XRootDPyFS(mkurl(tmppath), query={"xrd.wantprot": "krb5"})
 
-    assert fs.getpathurl("data/testa.txt") == \
-        "root://localhost/{0}/{1}".format(tmppath, "data/testa.txt")
+    assert fs.getpathurl("data/testa.txt") == "root://localhost/{0}/{1}".format(
+        tmppath, "data/testa.txt"
+    )
 
-    assert fs.getpathurl("data/testa.txt", with_querystring=True) == \
-        "root://localhost/{0}/{1}?xrd.wantprot=krb5".format(
-            tmppath, "data/testa.txt")
+    assert fs.getpathurl(
+        "data/testa.txt", with_querystring=True
+    ) == "root://localhost/{0}/{1}?xrd.wantprot=krb5".format(tmppath, "data/testa.txt")
 
 
 def test_ping(tmppath):
     """Test ping method."""
     fs = XRootDPyFS(mkurl(tmppath))
     assert fs.xrd_ping()
     fake_status = {
         "status": 3,
         "code": 101,
         "ok": False,
         "errno": 0,
         "error": True,
-        "message": '[FATAL] Invalid address',
+        "message": "[FATAL] Invalid address",
         "fatal": True,
-        "shellcode": 51
+        "shellcode": 51,
     }
     fs.xrd_client.ping = Mock(return_value=(XRootDStatus(fake_status), None))
     pytest.raises(RemoteConnectionError, fs.xrd_ping)
 
 
 def test_checksum(tmppath):
     """Test checksum method."""
     fs = XRootDPyFS(mkurl(tmppath))
 
     # Local xrootd server does not support checksum operation
-    pytest.raises(UnsupportedError, fs.xrd_checksum, "data/testa.txt")
+    pytest.raises(Unsupported, fs.xrd_checksum, "data/testa.txt")
 
     # Let's fake a success response
     fake_status = {
         "status": 0,
         "code": 0,
         "ok": True,
         "errno": 0,
         "error": False,
-        "message": '[SUCCESS] ',
+        "message": "[SUCCESS] ",
         "fatal": False,
-        "shellcode": 0
+        "shellcode": 0,
     }
     fs.xrd_client.query = Mock(
-        return_value=(XRootDStatus(fake_status), b'adler32 3836a69a\x00'))
+        return_value=(XRootDStatus(fake_status), b"adler32 3836a69a\x00")
+    )
     algo, val = fs.xrd_checksum("data/testa.txt")
-    assert algo == 'adler32' and val == "3836a69a"
+    assert algo == "adler32" and val == "3836a69a"
 
     # Fake a bad response (e.g. on directory)
     fake_status = {
         "status": 1,
         "code": 400,
         "ok": False,
         "errno": 3011,
         "error": True,
-        "message": '[ERROR] Server responded with an error: [3011] no such '
-                   'file or directory\n',
+        "message": "[ERROR] Server responded with an error: [3011] no such "
+        "file or directory\n",
         "fatal": False,
-        "shellcode": 54
+        "shellcode": 54,
     }
-    fs.xrd_client.query = Mock(
-        return_value=(XRootDStatus(fake_status), None))
+    fs.xrd_client.query = Mock(return_value=(XRootDStatus(fake_status), None))
     pytest.raises(FSError, fs.xrd_checksum, "data/")
 
 
 def test_move_good(tmppath):
     """Test move file."""
     fs = XRootDPyFS(mkurl(tmppath))
 
@@ -559,32 +566,27 @@
     src_folder_exists = "data/afolder/"
     dst_exists = "data/multiline.txt"
     dst_new = "data/ok.txt"
     dst_folder_exists = "data/bfolder/"
     dst_folder_new = "data/anothernewfolder/"
 
     # Destination exists
-    pytest.raises(
-        DestinationExistsError, fs.move, src_exists, dst_exists)
-    pytest.raises(
-        DestinationExistsError, fs.move, src_exists, src_exists)
-    pytest.raises(
-        DestinationExistsError, fs.move, src_exists, dst_folder_exists)
+    pytest.raises(DestinationExists, fs.move, src_exists, dst_exists)
+    pytest.raises(DestinationExists, fs.move, src_exists, src_exists)
+    pytest.raises(DestinationExists, fs.move, src_exists, dst_folder_exists)
 
     # Cannot move dir
-    pytest.raises(
-        ResourceInvalidError, fs.move, src_folder_exists, dst_new)
-    pytest.raises(
-        ResourceInvalidError, fs.move, src_folder_exists, dst_folder_new)
+    pytest.raises(ResourceInvalid, fs.move, src_folder_exists, dst_new)
+    pytest.raises(ResourceInvalid, fs.move, src_folder_exists, dst_folder_new)
 
     # Source doesn't exists
-    pytest.raises(ResourceNotFoundError, fs.move, src_new, dst_exists)
-    pytest.raises(ResourceNotFoundError, fs.move, src_new, dst_new)
-    pytest.raises(ResourceNotFoundError, fs.move, src_new, dst_folder_exists)
-    pytest.raises(ResourceNotFoundError, fs.move, src_new, dst_folder_new)
+    pytest.raises(ResourceNotFound, fs.move, src_new, dst_exists)
+    pytest.raises(ResourceNotFound, fs.move, src_new, dst_new)
+    pytest.raises(ResourceNotFound, fs.move, src_new, dst_folder_exists)
+    pytest.raises(ResourceNotFound, fs.move, src_new, dst_folder_new)
 
 
 def test_movedir_bad(tmppath):
     """Test move file."""
     fs = XRootDPyFS(mkurl(tmppath))
 
     src_exists = "data/testa.txt"
@@ -593,45 +595,31 @@
     src_folder_new = "data/newfolder/"
     dst_exists = "data/multiline.txt"
     dst_new = "data/ok.txt"
     dst_folder_exists = "data/bfolder/"
     dst_folder_new = "data/anothernewfolder/"
 
     # Destination exists
-    pytest.raises(
-        DestinationExistsError, fs.movedir, src_folder_exists,
-        dst_exists)
-    pytest.raises(
-        DestinationExistsError, fs.movedir, src_folder_exists,
-        dst_folder_exists)
+    pytest.raises(DestinationExists, fs.movedir, src_folder_exists, dst_exists)
+    pytest.raises(DestinationExists, fs.movedir, src_folder_exists, dst_folder_exists)
 
     # Cannot move file
-    pytest.raises(
-        ResourceInvalidError, fs.movedir, src_exists, dst_new)
-    pytest.raises(
-        ResourceInvalidError, fs.movedir, src_exists, dst_folder_new)
+    pytest.raises(ResourceInvalid, fs.movedir, src_exists, dst_new)
+    pytest.raises(ResourceInvalid, fs.movedir, src_exists, dst_folder_new)
 
     # Source doesn't exists
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_new, dst_exists)
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_new, dst_new)
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_new, dst_folder_exists)
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_new, dst_folder_new)
-
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_folder_new, dst_exists)
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_folder_new, dst_new)
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_folder_new, dst_folder_exists)
-    pytest.raises(
-        ResourceNotFoundError, fs.movedir, src_folder_new, dst_folder_new)
+    pytest.raises(ResourceNotFound, fs.movedir, src_new, dst_exists)
+    pytest.raises(ResourceNotFound, fs.movedir, src_new, dst_new)
+    pytest.raises(ResourceNotFound, fs.movedir, src_new, dst_folder_exists)
+    pytest.raises(ResourceNotFound, fs.movedir, src_new, dst_folder_new)
+
+    pytest.raises(ResourceNotFound, fs.movedir, src_folder_new, dst_exists)
+    pytest.raises(ResourceNotFound, fs.movedir, src_folder_new, dst_new)
+    pytest.raises(ResourceNotFound, fs.movedir, src_folder_new, dst_folder_exists)
+    pytest.raises(ResourceNotFound, fs.movedir, src_folder_new, dst_folder_new)
 
 
 def test_copy_good(tmppath):
     """Test move file."""
     fs = XRootDPyFS(mkurl(tmppath))
 
     src_exists = "data/testa.txt"
@@ -670,41 +658,32 @@
     src_folder_exists = "data/afolder/"
     dst_exists = "data/multiline.txt"
     dst_new = "data/ok.txt"
     dst_folder_exists = "data/bfolder/"
     dst_folder_new = "data/anothernewfolder/"
 
     # Destination exists
-    pytest.raises(
-        DestinationExistsError, fs.copy, src_exists, dst_exists)
-    pytest.raises(
-        DestinationExistsError, fs.copy, src_exists, src_exists)
-    pytest.raises(
-        DestinationExistsError, fs.copy, src_exists, dst_folder_exists)
+    pytest.raises(DestinationExists, fs.copy, src_exists, dst_exists)
+    pytest.raises(DestinationExists, fs.copy, src_exists, src_exists)
+    pytest.raises(DestinationExists, fs.copy, src_exists, dst_folder_exists)
 
     # Cannot copy dir
-    pytest.raises(
-        ResourceInvalidError, fs.copy, src_folder_exists, dst_new)
-    pytest.raises(
-        ResourceInvalidError, fs.copy, src_folder_exists, dst_folder_new)
+    pytest.raises(ResourceInvalid, fs.copy, src_folder_exists, dst_new)
+    pytest.raises(ResourceInvalid, fs.copy, src_folder_exists, dst_folder_new)
 
     # Source doesn't exists
-    pytest.raises(ResourceNotFoundError, fs.copy, src_new, dst_exists)
-    pytest.raises(ResourceNotFoundError, fs.copy, src_new, dst_new)
-    pytest.raises(ResourceNotFoundError, fs.copy, src_new, dst_folder_exists)
-    pytest.raises(ResourceNotFoundError, fs.copy, src_new, dst_folder_new)
-
-    pytest.raises(
-        ResourceNotFoundError, fs.copy, src_new, dst_exists)
-    pytest.raises(
-        ResourceNotFoundError, fs.copy, src_new, dst_new)
-    pytest.raises(
-        ResourceNotFoundError, fs.copy, src_new, dst_folder_exists)
-    pytest.raises(
-        ResourceNotFoundError, fs.copy, src_new, dst_folder_new)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_exists)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_new)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_folder_exists)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_folder_new)
+
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_exists)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_new)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_folder_exists)
+    pytest.raises(ResourceNotFound, fs.copy, src_new, dst_folder_new)
 
 
 def test_copydir_good(tmppath):
     """Test copy directory."""
     copydir_good(tmppath, False)
 
 
@@ -735,16 +714,15 @@
     fs.copydir(src_exists, dst_folder_new, parallel=parallel)
     assert fs.exists(src_exists) and fs.exists(dst_folder_new)
 
     fs.copydir(src_exists, dst_exists, overwrite=True, parallel=parallel)
     assert fs.exists(src_exists) and fs.exists(dst_exists)
     assert fs.isdir(dst_exists)
 
-    fs.copydir(
-        src_exists, dst_folder_exists, overwrite=True, parallel=parallel)
+    fs.copydir(src_exists, dst_folder_exists, overwrite=True, parallel=parallel)
     assert fs.exists(src_exists) and fs.exists(dst_folder_exists)
     assert fs.isdir(dst_folder_exists)
 
 
 def test_copydir_bad(tmppath):
     """Test copy directory."""
     copydir_bad(tmppath, False)
@@ -766,50 +744,66 @@
     dst_exists = "data/multiline.txt"
     dst_new = "data/ok.txt"
     dst_folder_exists = "data/bfolder/"
     dst_folder_new = "data/anothernewfolder/"
 
     # Destination exists
     pytest.raises(
-        DestinationExistsError, fs.copydir, src_folder_exists, dst_exists,
-        parallel=parallel)
+        DestinationExists, fs.copydir, src_folder_exists, dst_exists, parallel=parallel
+    )
     pytest.raises(
-        DestinationExistsError, fs.copydir, src_folder_exists,
-        src_folder_exists, parallel=parallel)
+        DestinationExists,
+        fs.copydir,
+        src_folder_exists,
+        src_folder_exists,
+        parallel=parallel,
+    )
     pytest.raises(
-        DestinationExistsError, fs.copydir, src_folder_exists,
-        dst_folder_exists, parallel=parallel)
+        DestinationExists,
+        fs.copydir,
+        src_folder_exists,
+        dst_folder_exists,
+        parallel=parallel,
+    )
 
     # Cannot move file
+    pytest.raises(ResourceInvalid, fs.copydir, src_exists, dst_new, parallel=parallel)
     pytest.raises(
-        ResourceInvalidError, fs.copydir, src_exists, dst_new,
-        parallel=parallel)
-    pytest.raises(
-        ResourceInvalidError, fs.copydir, src_exists, dst_folder_new,
-        parallel=parallel)
+        ResourceInvalid, fs.copydir, src_exists, dst_folder_new, parallel=parallel
+    )
 
     # Source doesn't exists
+    pytest.raises(ResourceNotFound, fs.copydir, src_new, dst_exists, parallel=parallel)
+    pytest.raises(ResourceNotFound, fs.copydir, src_new, dst_new, parallel=parallel)
     pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_new, dst_exists,
-        parallel=parallel)
-    pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_new, dst_new,
-        parallel=parallel)
-    pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_new, dst_folder_exists,
-        parallel=parallel)
+        ResourceNotFound, fs.copydir, src_new, dst_folder_exists, parallel=parallel
+    )
     pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_new, dst_folder_new,
-        parallel=parallel)
+        ResourceNotFound, fs.copydir, src_new, dst_folder_new, parallel=parallel
+    )
 
     pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_folder_new, dst_exists,
-        parallel=parallel)
+        ResourceNotFound, fs.copydir, src_folder_new, dst_exists, parallel=parallel
+    )
     pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_folder_new, dst_new,
-        parallel=parallel)
+        ResourceNotFound, fs.copydir, src_folder_new, dst_new, parallel=parallel
+    )
     pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_folder_new, dst_folder_exists,
-        parallel=parallel)
+        ResourceNotFound,
+        fs.copydir,
+        src_folder_new,
+        dst_folder_exists,
+        parallel=parallel,
+    )
     pytest.raises(
-        ResourceNotFoundError, fs.copydir, src_folder_new, dst_folder_new,
-        parallel=parallel)
+        ResourceNotFound, fs.copydir, src_folder_new, dst_folder_new, parallel=parallel
+    )
+
+
+def test_openbin():
+    """Test openbin."""
+    pytest.raises(NotImplementedError)
+
+
+def test_setinfo():
+    """Test setinfo."""
+    pytest.raises(NotImplementedError)
```

### Comparing `xrootdpyfs-0.2.2/xrootdpyfs.egg-info/SOURCES.txt` & `xrootdpyfs-1.0.0a1/xrootdpyfs.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-.coveragerc
+.dockerignore
+.editorconfig
+.git-blame-ignore-revs
 AUTHORS
 CHANGES
+CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
+run-docker.sh
 run-tests.sh
 setup.cfg
 setup.py
 .github/workflows/pypi-publish.yml
 .github/workflows/tests.yml
 docs/Makefile
 docs/conf.py
@@ -18,20 +22,25 @@
 tests/test_env.py
 tests/test_fs.py
 tests/test_fs_extras.py
 tests/test_opener.py
 tests/test_utils.py
 tests/test_xrdfile.py
 tests/test_xrdflags.py
+tests/data/binary.dat
+tests/data/multiline.txt
+tests/data/testa.txt
+tests/data/afolder/afile.txt
+tests/data/bfolder/bfile.txt
 xrootdpyfs/__init__.py
 xrootdpyfs/env.py
 xrootdpyfs/fs.py
 xrootdpyfs/opener.py
 xrootdpyfs/utils.py
-xrootdpyfs/version.py
 xrootdpyfs/xrdfile.py
 xrootdpyfs.egg-info/PKG-INFO
 xrootdpyfs.egg-info/SOURCES.txt
 xrootdpyfs.egg-info/dependency_links.txt
+xrootdpyfs.egg-info/entry_points.txt
 xrootdpyfs.egg-info/not-zip-safe
 xrootdpyfs.egg-info/requires.txt
 xrootdpyfs.egg-info/top_level.txt
```

### Comparing `xrootdpyfs-0.2.2/README.rst` & `xrootdpyfs-1.0.0a1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -20,24 +20,33 @@
 Further documentation is available on https://xrootdpyfs.readthedocs.io/.
 
 Getting started
 ===============
 
 If you just want to try out the library, the easiest is to use Docker.
 
+Build the image:
+
+.. code-block:: console
+
+   $ docker build --platform linux/amd64 -t xrootd .
+
+Run the container and launch `xrootd`:
+
 .. code-block:: console
 
-   $ docker build -t xrootd .
-   $ docker run -h xrootdpyfs -it xrootd bash
+   $ docker run --platform linux/amd64 -h xrootdpyfs -it xrootd bash
 
-Next, start a XRootD server in the container and fire up an ipython shell:
+You will see the logs in the stdout. Next, in another shell, connect the container
+and fire up an ipython shell:
 
 .. code-block:: console
 
-   [xrootdpyfs@xrootdpyfs code]$ xrootd -b -l /dev/null
+   $ docker ps  # find the container id
+   $ docker exec -it <container-id> bash
    [xrootdpyfs@xrootdpyfs code]$ ipython
 
 
 Quick examples
 --------------
 
 Here is a quick example of a file listing with the xrootd PyFilesystem
@@ -48,59 +57,67 @@
     >>> fs.listdir("xrootdpyfs")
     ['test.txt']
 
 Or, alternatively using the PyFilesystem opener (note the first
 ``import xrootdpyfs`` is required to ensure the XRootDPyFS opener is registered):
 
     >>> import xrootdpyfs
-    >>> from fs.opener import opener
-    >>> fs, path = opener.parse("root://localhost//tmp/")
+    >>> from fs.opener import open_fs
+    >>> fs = open_fs("root://localhost//tmp/")
     >>> fs.listdir("xrootdpyfs")
     ['test.txt']
 
 Reading files:
 
     >>> f = fs.open("xrootdpyfs/test.txt")
     >>> f.read()
     b'Hello XRootD!\n'
     >>> f.close()
 
-Reading files using the ``getcontents()`` method:
+Reading files using the ``readtext()`` method:
 
-    >>> fs.getcontents("xrootdpyfs/test.txt")
+    >>> fs.readtext("xrootdpyfs/test.txt")
     b'Hello XRootD!\n'
 
 Writing files:
 
     >>> f = fs.open("xrootdpyfs/hello.txt", "w+")
     >>> f.write("World")
     >>> f.close()
 
-Writing files using the ``setcontents()`` method:
+Writing files using the ``writetext()`` method:
 
-    >>> fs.setcontents("xrootdpyfs/test.txt", "World")
+    >>> fs.writetext("xrootdpyfs/test.txt", "World")
 
 Development
 ===========
 
 The easiest way to develop is to build the Docker image and mount
 the source code as a volume to test any code modification with a
 running XRootD server:
 
 .. code-block:: console
 
-   $ docker build -t xrootd --progress=plain .
-   $ docker run -h xrootdpyfs -it -v <absolute path to this project>:/code xrootd bash
-   [xrootdpyfs@xrootdpyfs code]$ xrootd -b -l /dev/null
+   $ docker build --platform linux/amd64 -t xrootd --progress=plain .
+   $ docker run --platform linux/amd64 -h xrootdpyfs -it -v <absolute path to this project>:/code xrootd bash
+   [xrootdpyfs@xrootdpyfs code]$ xrootd
+
+In another shell:
+
+.. code-block:: console
+
+   $ docker ps  # find the container id
+   $ docker exec -it <container-id> bash
+   [xrootdpyfs@xrootdpyfs code]$ python -m pytest -vvv tests
 
 If you want to test a specific version of xrootd, run:
 
 .. code-block:: console
 
-   $ docker build --build-arg xrootd_version=4.8.5 -t xrootd --progress=plain .
+   $ docker build --platform linux/amd64 --build-arg xrootd_version=4.12.7 -t xrootd --progress=plain .
 
 Documentation
 =============
 Documentation is available at <http://xrootdpyfs.readthedocs.io/> or can be
 build using Sphinx::
 
     pip install Sphinx
@@ -108,8 +125,8 @@
 
 Testing
 =======
 Running the tests are most easily done using docker:
 
 .. code-block:: console
 
-    $ docker build -t xrootd . && docker run -h xrootdpyfs -it xrootd
+    $ docker build --platform linux/amd64 -t xrootd . && docker run --platform linux/amd64 -h xrootdpyfs -it xrootd
```

