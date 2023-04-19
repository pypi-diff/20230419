# Comparing `tmp/segment-geospatial-0.0.3.tar.gz` & `tmp/segment-geospatial-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.0.3.tar", last modified: Wed Apr 19 03:45:58 2023, max compression
+gzip compressed data, was "segment-geospatial-0.1.0.tar", last modified: Wed Apr 19 20:24:43 2023, max compression
```

## Comparing `segment-geospatial-0.0.3.tar` & `segment-geospatial-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:43.742399 segment-geospatial-0.1.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 20:24:43.000000 segment-geospatial-0.1.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 20:24:43.746399 segment-geospatial-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-19 20:24:33.000000 segment-geospatial-0.1.0/setup.py
```

### Comparing `segment-geospatial-0.0.3/LICENSE` & `segment-geospatial-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.0.3/setup.py` & `segment-geospatial-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # get the dependencies and installs
 with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
     all_reqs = f.read().split("\n")
 
 install_requires = [x.strip() for x in all_reqs if "git+" not in x]
 dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
 
-requirements = [ ]
+requirements = []
 
-setup_requirements = [ ]
+setup_requirements = []
 
-test_requirements = [ ]
+test_requirements = []
 
 setup(
     author="Qiusheng Wu",
     author_email='giswqs@gmail.com',
     python_requires='>=3.8',
     classifiers=[
         'Intended Audience :: Developers',
@@ -48,10 +48,10 @@
     keywords='samgeo',
     name='segment-geospatial',
     packages=find_packages(include=['samgeo', 'samgeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/segment-geospatial',
-    version='0.0.3',
+    version='0.1.0',
     zip_safe=False,
 )
```

