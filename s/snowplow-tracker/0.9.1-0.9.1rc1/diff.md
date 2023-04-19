# Comparing `tmp/snowplow-tracker-0.9.1.tar.gz` & `tmp/snowplow-tracker-0.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowplow-tracker-0.9.1.tar", last modified: Tue Oct 26 09:55:09 2021, max compression
+gzip compressed data, was "dist/snowplow-tracker-0.9.1rc1.tar", last modified: Tue Oct 26 09:07:55 2021, max compression
```

## Comparing `snowplow-tracker-0.9.1.tar` & `snowplow-tracker-0.9.1rc1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     7511 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4897 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/snowplow_tracker/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/snowplow_tracker/celery/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/celery/celery_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)    14167 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/emitters.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/payload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/snowplow_tracker/redis/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2610 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/redis/redis_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2784 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/redis/redis_worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/self_describing_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/subject.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/snowplow_tracker/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    30565 2021-10-26 09:55:04.000000 snowplow-tracker-0.9.1/snowplow_tracker/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:55:09.248815 snowplow-tracker-0.9.1/snowplow_tracker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6013 2021-10-26 09:55:09.000000 snowplow-tracker-0.9.1/snowplow_tracker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      710 2021-10-26 09:55:09.000000 snowplow-tracker-0.9.1/snowplow_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 09:55:09.000000 snowplow-tracker-0.9.1/snowplow_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-26 09:55:09.000000 snowplow-tracker-0.9.1/snowplow_tracker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-26 09:55:09.000000 snowplow-tracker-0.9.1/snowplow_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3013 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2792 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/celery_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14167 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/emitters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3366 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30565 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5113 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/subject.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)      474 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2784 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/redis_worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2610 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/redis_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/snowplow_tracker/self_describing_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7511 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6733 2021-10-26 09:07:55.000000 snowplow-tracker-0.9.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4897 2021-10-26 09:07:48.000000 snowplow-tracker-0.9.1rc1/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `snowplow-tracker-0.9.1/CHANGES.txt` & `snowplow-tracker-0.9.1rc1/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/PKG-INFO` & `snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,107 @@
 Metadata-Version: 2.1
 Name: snowplow-tracker
-Version: 0.9.1
+Version: 0.9.1rc1
 Summary: Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
 Home-page: http://snowplowanalytics.com
 Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock
 Author-email: support@snowplowanalytics.com
 License: Apache License 2.0
+Description: ======================================================
+        Python Analytics for Snowplow
+        ======================================================
+        .. image:: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC
+            :alt: Early Release
+            :target: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
+        .. image:: https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg
+            :alt: Build Status
+            :target: https://github.com/snowplow/snowplow-python-tracker/actions
+        .. image:: https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker
+            :alt: Test Coverage
+            :target: https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master
+        .. image:: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
+            :target: http://www.apache.org/licenses/LICENSE-2.0
+        
+        |
+        
+        .. image:: https://img.shields.io/pypi/v/snowplow-tracker
+            :alt: Pypi Snowplow Tracker
+            :target: https://pypi.org/project/snowplow-tracker/
+        .. image:: https://img.shields.io/pypi/pyversions/snowplow-tracker
+            :alt: Python Versions
+            :target: https://pypi.org/project/snowplow-tracker/
+        .. image:: https://img.shields.io/pypi/dm/snowplow-tracker
+            :alt: Monthly Downloads
+            :target: https://pypi.org/project/snowplow-tracker/
+        
+        
+        Overview
+        ########
+        
+        Add analytics to your Python apps and Python games with the Snowplow_ event tracker for Python_.
+        
+        .. _Snowplow: http://snowplowanalytics.com
+        .. _Python: http://python.org
+        
+        With this tracker you can collect event data from your Python-based applications, games or Python web servers/frameworks.
+        
+        Find out more
+        #############
+        
+        +---------------------------------+---------------------------+-----------------------------------+
+        | Technical Docs                  | Setup Guide               | Contributing                      |
+        +=================================+===========================+===================================+
+        | |techdocs|_                     | |setup|_                  | |contributing|                    |
+        +---------------------------------+---------------------------+-----------------------------------+
+        | `Technical Docs`_               | `Setup Guide`_            | `Contributing`_                   |
+        +---------------------------------+---------------------------+-----------------------------------+
+        
+        .. |techdocs| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
+        .. |setup| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
+        .. |contributing| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
+        
+        .. _techdocs: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
+        .. _setup: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
+        
+        .. _`Technical Docs`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
+        .. _`Setup Guide`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
+        .. _`Contributing`: https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md
+        
+        Maintainer Quickstart
+        #######################
+        
+        Assuming pyenv_ is installed
+        
+        ::
+        
+           host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
+           host$ cd snowplow-python-tracker
+           host$ pyenv install 2.7.18 && pyenv install 3.5.10 && pyenv install 3.6.14 && pyenv install 3.7.11 && pyenv install 3.8.11 && pyenv install 3.9.6
+           host$ ./run-tests.sh deploy
+           host$ ./run-tests.sh test
+        
+        .. _pyenv: https://github.com/pyenv/pyenv
+        
+        Copyright and license
+        #####################
+        
+        The Snowplow Python Tracker is copyright 2013-2021 Snowplow Analytics Ltd.
+        
+        Licensed under the `Apache License, Version 2.0`_ (the "License");
+        you may not use this software except in compliance with the License.
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+        
+        .. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -19,102 +111,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 Provides-Extra: celery
 Provides-Extra: redis
-License-File: LICENSE
-
-======================================================
-Python Analytics for Snowplow
-======================================================
-.. image:: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC
-    :alt: Early Release
-    :target: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
-.. image:: https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg
-    :alt: Build Status
-    :target: https://github.com/snowplow/snowplow-python-tracker/actions
-.. image:: https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker
-    :alt: Test Coverage
-    :target: https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master
-.. image:: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
-    :target: http://www.apache.org/licenses/LICENSE-2.0
-
-|
-
-.. image:: https://img.shields.io/pypi/v/snowplow-tracker
-    :alt: Pypi Snowplow Tracker
-    :target: https://pypi.org/project/snowplow-tracker/
-.. image:: https://img.shields.io/pypi/pyversions/snowplow-tracker
-    :alt: Python Versions
-    :target: https://pypi.org/project/snowplow-tracker/
-.. image:: https://img.shields.io/pypi/dm/snowplow-tracker
-    :alt: Monthly Downloads
-    :target: https://pypi.org/project/snowplow-tracker/
-
-
-Overview
-########
-
-Add analytics to your Python apps and Python games with the Snowplow_ event tracker for Python_.
-
-.. _Snowplow: http://snowplowanalytics.com
-.. _Python: http://python.org
-
-With this tracker you can collect event data from your Python-based applications, games or Python web servers/frameworks.
-
-Find out more
-#############
-
-+---------------------------------+---------------------------+-----------------------------------+
-| Technical Docs                  | Setup Guide               | Contributing                      |
-+=================================+===========================+===================================+
-| |techdocs|_                     | |setup|_                  | |contributing|                    |
-+---------------------------------+---------------------------+-----------------------------------+
-| `Technical Docs`_               | `Setup Guide`_            | `Contributing`_                   |
-+---------------------------------+---------------------------+-----------------------------------+
-
-.. |techdocs| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
-.. |setup| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
-.. |contributing| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
-
-.. _techdocs: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-.. _setup: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-
-.. _`Technical Docs`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-.. _`Setup Guide`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-.. _`Contributing`: https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md
-
-Maintainer Quickstart
-#######################
-
-Assuming pyenv_ is installed
-
-::
-
-   host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
-   host$ cd snowplow-python-tracker
-   host$ pyenv install 2.7.18 && pyenv install 3.5.10 && pyenv install 3.6.14 && pyenv install 3.7.11 && pyenv install 3.8.11 && pyenv install 3.9.6
-   host$ ./run-tests.sh deploy
-   host$ ./run-tests.sh test
-
-.. _pyenv: https://github.com/pyenv/pyenv
-
-Copyright and license
-#####################
-
-The Snowplow Python Tracker is copyright 2013-2021 Snowplow Analytics Ltd.
-
-Licensed under the `Apache License, Version 2.0`_ (the "License");
-you may not use this software except in compliance with the License.
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-
-
-.. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
-
-
```

### Comparing `snowplow-tracker-0.9.1/README.rst` & `snowplow-tracker-0.9.1rc1/README.rst`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/setup.py` & `snowplow-tracker-0.9.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 authors_email_list = [
     'support@snowplowanalytics.com',
     ]
 authors_email_str = ', '.join(authors_email_list)
 
 setup(
     name='snowplow-tracker',
-    version='0.9.1',
+    version='0.9.1rc1',
     author=authors_str,
     author_email=authors_email_str,
     packages=['snowplow_tracker', 'snowplow_tracker.test', 'snowplow_tracker.redis', 'snowplow_tracker.celery'],
     url='http://snowplowanalytics.com',
     license='Apache License 2.0',
     description='Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games',
     long_description=open('README.rst').read(),
```

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/_version.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
     Authors: Anuj More, Alex Dean, Fred Blundun, Paul Boocock
     Copyright: Copyright (c) 2013-2021 Snowplow Analytics Ltd
     License: Apache License Version 2.0
 """
 
 
-__version_info__ = (0, 9, 1)
+__version_info__ = (0, 9, '1rc1')
 __version__ = ".".join(str(x) for x in __version_info__)
 __build_version__ = __version__ + ''
```

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/celery/celery_emitter.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/celery/celery_emitter.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/emitters.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/emitters.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/payload.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/payload.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/redis/redis_emitter.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/redis_emitter.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/redis/redis_worker.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/redis/redis_worker.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/self_describing_json.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/self_describing_json.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/subject.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/subject.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker/tracker.py` & `snowplow-tracker-0.9.1rc1/snowplow_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker.egg-info/PKG-INFO` & `snowplow-tracker-0.9.1rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,107 @@
 Metadata-Version: 2.1
 Name: snowplow-tracker
-Version: 0.9.1
+Version: 0.9.1rc1
 Summary: Snowplow event tracker for Python. Add analytics to your Python and Django apps, webapps and games
 Home-page: http://snowplowanalytics.com
 Author: Anuj More, Alexander Dean, Fred Blundun, Paul Boocock
 Author-email: support@snowplowanalytics.com
 License: Apache License 2.0
+Description: ======================================================
+        Python Analytics for Snowplow
+        ======================================================
+        .. image:: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC
+            :alt: Early Release
+            :target: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
+        .. image:: https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg
+            :alt: Build Status
+            :target: https://github.com/snowplow/snowplow-python-tracker/actions
+        .. image:: https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker
+            :alt: Test Coverage
+            :target: https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master
+        .. image:: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
+            :target: http://www.apache.org/licenses/LICENSE-2.0
+        
+        |
+        
+        .. image:: https://img.shields.io/pypi/v/snowplow-tracker
+            :alt: Pypi Snowplow Tracker
+            :target: https://pypi.org/project/snowplow-tracker/
+        .. image:: https://img.shields.io/pypi/pyversions/snowplow-tracker
+            :alt: Python Versions
+            :target: https://pypi.org/project/snowplow-tracker/
+        .. image:: https://img.shields.io/pypi/dm/snowplow-tracker
+            :alt: Monthly Downloads
+            :target: https://pypi.org/project/snowplow-tracker/
+        
+        
+        Overview
+        ########
+        
+        Add analytics to your Python apps and Python games with the Snowplow_ event tracker for Python_.
+        
+        .. _Snowplow: http://snowplowanalytics.com
+        .. _Python: http://python.org
+        
+        With this tracker you can collect event data from your Python-based applications, games or Python web servers/frameworks.
+        
+        Find out more
+        #############
+        
+        +---------------------------------+---------------------------+-----------------------------------+
+        | Technical Docs                  | Setup Guide               | Contributing                      |
+        +=================================+===========================+===================================+
+        | |techdocs|_                     | |setup|_                  | |contributing|                    |
+        +---------------------------------+---------------------------+-----------------------------------+
+        | `Technical Docs`_               | `Setup Guide`_            | `Contributing`_                   |
+        +---------------------------------+---------------------------+-----------------------------------+
+        
+        .. |techdocs| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
+        .. |setup| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
+        .. |contributing| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
+        
+        .. _techdocs: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
+        .. _setup: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
+        
+        .. _`Technical Docs`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
+        .. _`Setup Guide`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
+        .. _`Contributing`: https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md
+        
+        Maintainer Quickstart
+        #######################
+        
+        Assuming pyenv_ is installed
+        
+        ::
+        
+           host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
+           host$ cd snowplow-python-tracker
+           host$ pyenv install 2.7.18 && pyenv install 3.5.10 && pyenv install 3.6.14 && pyenv install 3.7.11 && pyenv install 3.8.11 && pyenv install 3.9.6
+           host$ ./run-tests.sh deploy
+           host$ ./run-tests.sh test
+        
+        .. _pyenv: https://github.com/pyenv/pyenv
+        
+        Copyright and license
+        #####################
+        
+        The Snowplow Python Tracker is copyright 2013-2021 Snowplow Analytics Ltd.
+        
+        Licensed under the `Apache License, Version 2.0`_ (the "License");
+        you may not use this software except in compliance with the License.
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+        
+        .. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
@@ -19,102 +111,7 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
 Provides-Extra: celery
 Provides-Extra: redis
-License-File: LICENSE
-
-======================================================
-Python Analytics for Snowplow
-======================================================
-.. image:: https://img.shields.io/static/v1?style=flat&label=Snowplow&message=Early%20Release&color=014477&labelColor=9ba0aa&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAMAAAAoLQ9TAAAAeFBMVEVMaXGXANeYANeXANZbAJmXANeUANSQAM+XANeMAMpaAJhZAJeZANiXANaXANaOAM2WANVnAKWXANZ9ALtmAKVaAJmXANZaAJlXAJZdAJxaAJlZAJdbAJlbAJmQAM+UANKZANhhAJ+EAL+BAL9oAKZnAKVjAKF1ALNBd8J1AAAAKHRSTlMAa1hWXyteBTQJIEwRgUh2JjJon21wcBgNfmc+JlOBQjwezWF2l5dXzkW3/wAAAHpJREFUeNokhQOCA1EAxTL85hi7dXv/E5YPCYBq5DeN4pcqV1XbtW/xTVMIMAZE0cBHEaZhBmIQwCFofeprPUHqjmD/+7peztd62dWQRkvrQayXkn01f/gWp2CrxfjY7rcZ5V7DEMDQgmEozFpZqLUYDsNwOqbnMLwPAJEwCopZxKttAAAAAElFTkSuQmCC
-    :alt: Early Release
-    :target: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/tracker-maintenance-classification/
-.. image:: https://github.com/snowplow/snowplow-python-tracker/actions/workflows/ci.yml/badge.svg
-    :alt: Build Status
-    :target: https://github.com/snowplow/snowplow-python-tracker/actions
-.. image:: https://img.shields.io/coveralls/github/snowplow/snowplow-python-tracker
-    :alt: Test Coverage
-    :target: https://coveralls.io/github/snowplow/snowplow-python-tracker?branch=master
-.. image:: http://img.shields.io/badge/license-Apache--2-blue.svg?style=flat
-    :target: http://www.apache.org/licenses/LICENSE-2.0
-
-|
-
-.. image:: https://img.shields.io/pypi/v/snowplow-tracker
-    :alt: Pypi Snowplow Tracker
-    :target: https://pypi.org/project/snowplow-tracker/
-.. image:: https://img.shields.io/pypi/pyversions/snowplow-tracker
-    :alt: Python Versions
-    :target: https://pypi.org/project/snowplow-tracker/
-.. image:: https://img.shields.io/pypi/dm/snowplow-tracker
-    :alt: Monthly Downloads
-    :target: https://pypi.org/project/snowplow-tracker/
-
-
-Overview
-########
-
-Add analytics to your Python apps and Python games with the Snowplow_ event tracker for Python_.
-
-.. _Snowplow: http://snowplowanalytics.com
-.. _Python: http://python.org
-
-With this tracker you can collect event data from your Python-based applications, games or Python web servers/frameworks.
-
-Find out more
-#############
-
-+---------------------------------+---------------------------+-----------------------------------+
-| Technical Docs                  | Setup Guide               | Contributing                      |
-+=================================+===========================+===================================+
-| |techdocs|_                     | |setup|_                  | |contributing|                    |
-+---------------------------------+---------------------------+-----------------------------------+
-| `Technical Docs`_               | `Setup Guide`_            | `Contributing`_                   |
-+---------------------------------+---------------------------+-----------------------------------+
-
-.. |techdocs| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
-.. |setup| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
-.. |contributing| image:: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png
-
-.. _techdocs: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-.. _setup: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-
-.. _`Technical Docs`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/
-.. _`Setup Guide`: https://docs.snowplowanalytics.com/docs/collecting-data/collecting-from-own-applications/python-tracker/setup/
-.. _`Contributing`: https://github.com/snowplow/snowplow-python-tracker/blob/master/CONTRIBUTING.md
-
-Maintainer Quickstart
-#######################
-
-Assuming pyenv_ is installed
-
-::
-
-   host$ git clone git@github.com:snowplow/snowplow-python-tracker.git
-   host$ cd snowplow-python-tracker
-   host$ pyenv install 2.7.18 && pyenv install 3.5.10 && pyenv install 3.6.14 && pyenv install 3.7.11 && pyenv install 3.8.11 && pyenv install 3.9.6
-   host$ ./run-tests.sh deploy
-   host$ ./run-tests.sh test
-
-.. _pyenv: https://github.com/pyenv/pyenv
-
-Copyright and license
-#####################
-
-The Snowplow Python Tracker is copyright 2013-2021 Snowplow Analytics Ltd.
-
-Licensed under the `Apache License, Version 2.0`_ (the "License");
-you may not use this software except in compliance with the License.
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-
-
-.. _Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
-
-
```

### Comparing `snowplow-tracker-0.9.1/snowplow_tracker.egg-info/SOURCES.txt` & `snowplow-tracker-0.9.1rc1/snowplow_tracker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 CHANGES.txt
-LICENSE
 MANIFEST.in
 README.rst
 requirements-test.txt
 setup.py
 snowplow_tracker/__init__.py
 snowplow_tracker/_version.py
 snowplow_tracker/emitters.py
```

