# Comparing `tmp/bok_choy-1.1.1.tar.gz` & `tmp/bok_choy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bok_choy-1.1.1.tar", last modified: Fri May  8 19:03:02 2020, max compression
+gzip compressed data, was "bok_choy-2.0.2.tar", last modified: Wed Apr 19 14:08:34 2023, max compression
```

## Comparing `bok_choy-1.1.1.tar` & `bok_choy-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,53 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-05-08 18:58:27.000000 bok_choy-1.1.1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     5215 2020-05-08 19:03:02.000000 bok_choy-1.1.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/bok_choy/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6082 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/promise.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/bok_choy/vendor/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/bok_choy/vendor/google/
--rw-rw-r--   0 travis    (2000) travis    (2000)    81800 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/vendor/google/axs_testing.js
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/bok_choy/vendor/axe-core/
--rw-rw-r--   0 travis    (2000) travis    (2000)   321476 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/vendor/axe-core/axe.min.js
--rw-rw-r--   0 travis    (2000) travis    (2000)    21943 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7937 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/web_app_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/bok_choy/a11y/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6290 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/a11y/a11y_audit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12329 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/a11y/axe_core_ruleset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7024 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/a11y/axs_ruleset.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/a11y/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24636 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/page_object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15201 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/query.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6336 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/javascript.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      313 2020-05-08 18:58:27.000000 bok_choy-1.1.1/bok_choy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      149 2020-05-08 19:03:02.000000 bok_choy-1.1.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2020-05-08 18:58:27.000000 bok_choy-1.1.1/requirements/base.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2020-05-08 18:58:27.000000 bok_choy-1.1.1/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-08 19:03:02.000000 bok_choy-1.1.1/bok_choy.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5215 2020-05-08 19:03:01.000000 bok_choy-1.1.1/bok_choy.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-08 19:03:01.000000 bok_choy-1.1.1/bok_choy.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       23 2020-05-08 19:03:01.000000 bok_choy-1.1.1/bok_choy.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      571 2020-05-08 19:03:01.000000 bok_choy-1.1.1/bok_choy.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-05-08 19:03:01.000000 bok_choy-1.1.1/bok_choy.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2020-05-08 18:58:27.000000 bok_choy-1.1.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      764 2020-05-08 18:58:27.000000 bok_choy-1.1.1/AUTHORS
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.351523 bok_choy-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-04-19 14:08:30.000000 bok_choy-2.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-04-19 14:08:30.000000 bok_choy-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-19 14:08:30.000000 bok_choy-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-19 14:08:30.000000 bok_choy-2.0.2/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4755 2023-04-19 14:08:34.351523 bok_choy-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3807 2023-04-19 14:08:30.000000 bok_choy-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.343523 bok_choy-2.0.2/bok_choy/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.347523 bok_choy-2.0.2/bok_choy/a11y/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/a11y/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6141 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/a11y/a11y_audit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12149 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/a11y/axe_core_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6661 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/a11y/axs_ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21532 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6182 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24542 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/page_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6129 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/promise.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14849 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.339523 bok_choy-2.0.2/bok_choy/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.347523 bok_choy-2.0.2/bok_choy/vendor/axe-core/
+-rw-r--r--   0 runner    (1001) docker     (122)   321476 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/vendor/axe-core/axe.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.347523 bok_choy-2.0.2/bok_choy/vendor/google/
+-rw-r--r--   0 runner    (1001) docker     (122)    81800 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/vendor/google/axs_testing.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7786 2023-04-19 14:08:30.000000 bok_choy-2.0.2/bok_choy/web_app_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.343523 bok_choy-2.0.2/bok_choy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4755 2023-04-19 14:08:34.000000 bok_choy-2.0.2/bok_choy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-19 14:08:34.000000 bok_choy-2.0.2/bok_choy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 14:08:34.000000 bok_choy-2.0.2/bok_choy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-19 14:08:34.000000 bok_choy-2.0.2/bok_choy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-19 14:08:34.000000 bok_choy-2.0.2/bok_choy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.347523 bok_choy-2.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-04-19 14:08:30.000000 bok_choy-2.0.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-04-19 14:08:30.000000 bok_choy-2.0.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-19 14:08:34.351523 bok_choy-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5514 2023-04-19 14:08:30.000000 bok_choy-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 14:08:34.351523 bok_choy-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    14779 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_ajax.py
+-rw-r--r--   0 runner    (1001) docker     (122)      620 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14527 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1138 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_delay.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_focused.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1150 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_javascript.py
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_next_page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5641 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_page_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5885 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2431 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_visible.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1655 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_webapptest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-19 14:08:30.000000 bok_choy-2.0.2/tests/test_xss_exposure.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bok_choy-1.1.1/PKG-INFO` & `bok_choy-2.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,130 +1,137 @@
 Metadata-Version: 2.1
 Name: bok_choy
-Version: 1.1.1
-Summary: UI-level acceptance test framework
-Home-page: http://github.com/edx/bok-choy
+Version: 2.0.2
+Summary: Deprecated UI-level acceptance test framework
+Home-page: http://github.com/openedx/bok-choy
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
-Description: bok-choy
-        ========
-        
-        .. image:: https://img.shields.io/pypi/v/bok_choy.svg
-            :target: https://pypi.python.org/pypi/bok_choy/
-            :alt: PyPI
-        
-        .. image:: https://travis-ci.org/edx/bok-choy.svg?branch=master
-            :target: https://travis-ci.org/edx/bok-choy
-            :alt: Travis
-        
-        .. image:: http://codecov.io/github/edx/bok-choy/coverage.svg?branch=master
-            :target: http://codecov.io/github/edx/bok-choy?branch=master
-            :alt: Codecov
-        
-        .. image:: https://readthedocs.org/projects/bok-choy/badge/?version=latest
-            :target: http://bok-choy.readthedocs.io/en/latest/
-            :alt: Documentation
-        
-        .. image:: https://img.shields.io/pypi/pyversions/bok_choy.svg
-            :target: https://pypi.python.org/pypi/bok_choy/
-            :alt: Supported Python versions
-        
-        .. image:: https://img.shields.io/github/license/edx/bok-choy.svg
-            :target: https://github.com/edx/bok-choy/blob/master/LICENSE.txt
-            :alt: License
-        
-        UI-level acceptance test framework.  `Full documentation available on ReadTheDocs`__.
-        
-        __ http://bok-choy.readthedocs.org/en/latest/
-        
-        
-        Overview
-        --------
-        
-        A Python framework for writing robust Selenium tests.
-        
-        
-        Installation
-        ------------
-        
-        As Bok Choy is a Python framework, you first need to install Python.
-        If you’re running Linux or Mac OS X, you probably already have it installed.
-        We recommend that you use `pip <http://www.pip-installer.org/>`_ to install your Python
-        packages:
-        
-        .. code-block:: bash
-        
-           pip install bok_choy
-        
-        .. Note::
-        
-           On Ubuntu Linux 18.04 you might have to install
-           *firefox-geckodriver* (for Firefox) and/or *chromium-chomedriver* (for Chromium),
-           especially if you hit the following Error when running bok_choy::
-        
-             bok_choy.promise.BrokenPromise: Promise not satisfied: Browser is instantiated successfully.
-        
-        
-        Running Tests
-        -------------
-        
-        To run the test suite for bok-choy itself:
-        
-        * Install Firefox; as of this writing, the current `version 59.0.1 <https://ftp.mozilla.org/pub/firefox/releases/59.0.1/>`_
-          works with the latest selenium Python package (3.11.0)
-        * Install `phantomjs <http://phantomjs.org/download.html>`_
-        * Create a virtualenv which uses Python 2.7, 3.5, or 3.6
-        * With that virtualenv activated, run ``pip install -r requirements/tox.txt`` to
-          install the `tox <http://tox.testrun.org/>`_ testing tool and its
-          dependencies
-        * Run ``tox -e py27`` (or ``tox -e py35``, etc.).  If you want to run the tests in
-          parallel, add the desired number of worker processes like ``tox -e py27 -- -n 5``
-          or ``tox -e py35 -- -n auto``.
-        * To test and build the documentation, run ``tox -e doc``
-        * To run an individual test, run ``py.test tests/<test file>::<test class>::<test name>``
-        
-        
-        License
-        -------
-        
-        The code in this repository is licensed under the Apache License, Version 2.0,
-        unless otherwise noted.
-        
-        Please see ``LICENSE.txt`` for details.
-        
-        
-        How to Contribute
-        -----------------
-        
-        Contributions are very welcome. The easiest way is to fork this repo, and then
-        make a pull request from your fork. The first time you make a pull request, you
-        may be asked to sign a Contributor Agreement.
-        
-        
-        Reporting Security Issues
-        -------------------------
-        
-        Please do not report security issues in public. Please email security@edx.org
-        
-        
-        Mailing List and IRC Channel
-        ----------------------------
-        
-        You can discuss this code on the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_
-        or in the **testing** channel on the `Open edX Slack <https://openedx.slack.com>`_.
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Provides-Extra: visual_diff
+License-File: LICENSE.txt
+License-File: NOTICE.txt
+License-File: AUTHORS
+
+bok-choy
+========
+
+.. image:: https://img.shields.io/pypi/v/bok_choy.svg
+    :target: https://pypi.python.org/pypi/bok_choy/
+    :alt: PyPI
+
+.. image:: https://github.com/openedx/bok-choy/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/bok-choy/actions?query=workflow%3A%22Python+CI%22
+    :alt: Github CI
+
+.. image:: http://codecov.io/github/edx/bok-choy/coverage.svg?branch=master
+    :target: http://codecov.io/github/edx/bok-choy?branch=master
+    :alt: Codecov
+
+.. image:: https://readthedocs.org/projects/bok-choy/badge/?version=latest
+    :target: http://bok-choy.readthedocs.io/en/latest/
+    :alt: Documentation
+
+.. image:: https://img.shields.io/pypi/pyversions/bok_choy.svg
+    :target: https://pypi.python.org/pypi/bok_choy/
+    :alt: Supported Python versions
+
+.. image:: https://img.shields.io/github/license/edx/bok-choy.svg
+    :target: https://github.com/openedx/bok-choy/blob/master/LICENSE.txt
+    :alt: License
+
+UI-level acceptance test framework.  `Full documentation available on ReadTheDocs`__.
+
+__ http://bok-choy.readthedocs.org/en/latest/
+
+⚠️ Deprecation Notice ⚠️
+------------------------
+
+As of 2022-02-18, `bok-choy is deprecated <https://github.com/openedx/public-engineering/issues/13>`_.
+All tests written using bok-choy have either been removed or are slated to be removed soon.
+Please do not write new tests using bok-choy!
+In the near future, this repository will be archived.
+
+Overview
+--------
+
+A Python framework for writing robust Selenium tests.
+
+Installation
+------------
+
+As Bok Choy is a Python framework, you first need to install Python.
+If you’re running Linux or Mac OS X, you probably already have it installed.
+We recommend that you use `pip <http://www.pip-installer.org/>`_ to install your Python
+packages:
+
+.. code-block:: bash
+
+   pip install bok_choy
+
+.. Note::
+
+   On Ubuntu Linux 18.04 you might have to install
+   *firefox-geckodriver* (for Firefox) and/or *chromium-chomedriver* (for Chromium),
+   especially if you hit the following Error when running bok_choy::
+
+     bok_choy.promise.BrokenPromise: Promise not satisfied: Browser is instantiated successfully.
+
+
+Running Tests
+-------------
+
+To run the test suite for bok-choy itself:
+
+* Install Firefox; as of this writing, the current `version 59.0.1 <https://ftp.mozilla.org/pub/firefox/releases/59.0.1/>`_
+  works with the latest selenium Python package (3.11.0)
+* Install `phantomjs <http://phantomjs.org/download.html>`_
+* Create a virtualenv which uses Python 3.8
+* With that virtualenv activated, run ``pip install -r requirements/ci.txt`` to
+  install the `tox <http://tox.testrun.org/>`_ testing tool and its
+  dependencies
+* Run ``tox -e py38``.  If you want to run the tests in
+  parallel, add the desired number of worker processes like ``tox -e py38 -- -n 5``
+  or ``tox -e py38 -- -n auto``.
+* To test and build the documentation, run ``tox -e doc``
+* To run an individual test, run ``py.test tests/<test file>::<test class>::<test name>``
+
+
+License
+-------
+
+The code in this repository is licensed under the Apache License, Version 2.0,
+unless otherwise noted.
+
+Please see ``LICENSE.txt`` for details.
+
+
+How to Contribute
+-----------------
+
+Contributions are very welcome. The easiest way is to fork this repo, and then
+make a pull request from your fork. The first time you make a pull request, you
+may be asked to sign a Contributor Agreement.
+
+
+Reporting Security Issues
+-------------------------
+
+Please do not report security issues in public. Please email security@edx.org
+
+
+Mailing List and IRC Channel
+----------------------------
+
+You can discuss this code on the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_
+or in the **testing** channel on the `Open edX Slack <https://openedx.slack.com>`_.
```

### Comparing `bok_choy-1.1.1/bok_choy/promise.py` & `bok_choy-2.0.2/bok_choy/promise.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Variation on the "promise" design pattern.
 Promises make it easier to handle asynchronous operations correctly.
 """
-from __future__ import absolute_import
 
 import time
 import logging
 
 
 LOGGER = logging.getLogger(__name__)
 
@@ -19,27 +18,28 @@
     def __init__(self, promise):
         """
         Configure the broken promise error.
 
         Args:
             promise (Promise): The promise that was not satisfied.
         """
-        super(BrokenPromise, self).__init__()
+        super().__init__()
         self._promise = promise
 
     def __str__(self):
-        return "Promise not satisfied: {0}".format(self._promise)
+        return f"Promise not satisfied: {self._promise}"
 
 
 class Promise:
     """
     Check that an asynchronous action completed, blocking until it does
     or timeout / try limits are reached.
     """
 
+    # pylint: disable=too-many-arguments
     def __init__(self, check_func, description, try_limit=None, try_interval=0.5, timeout=30):
         """
         Configure the `Promise`.
 
         The `Promise` will poll `check_func()` until either:
             * The promise is satisfied
             * The promise runs out of tries (checks more than `try_limit` times)
@@ -146,15 +146,15 @@
         If `_try_limit` is `None`, always return True.
         """
         if self._try_limit is None:
             return True
         return self._num_tries < self._try_limit
 
 
-class EmptyPromise(Promise):
+class EmptyPromise(Promise):  # pylint: disable=too-few-public-methods
     """
     A promise that has no result value.
     """
 
     def __init__(self, check_func, description, **kwargs):
         """
         Configure the promise.
@@ -173,9 +173,9 @@
             check_func (callable): Function that accepts no arguments and
                 returns a boolean indicating whether the promise is fulfilled.
             description (str): Description of the Promise, used in log messages.
 
         Returns:
             EmptyPromise
         """
-        full_check_func = lambda: (check_func(), None)
-        super(EmptyPromise, self).__init__(full_check_func, description, **kwargs)
+        full_check_func = lambda: (check_func(), None)  # pylint: disable=unnecessary-lambda-assignment
+        super().__init__(full_check_func, description, **kwargs)
```

### Comparing `bok_choy-1.1.1/bok_choy/vendor/google/axs_testing.js` & `bok_choy-2.0.2/bok_choy/vendor/google/axs_testing.js`

 * *Files identical despite different names*

### Comparing `bok_choy-1.1.1/bok_choy/vendor/axe-core/axe.min.js` & `bok_choy-2.0.2/bok_choy/vendor/axe-core/axe.min.js`

 * *Files identical despite different names*

### Comparing `bok_choy-1.1.1/bok_choy/browser.py` & `bok_choy-2.0.2/bok_choy/browser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 Use environment variables to configure Selenium remote WebDriver.
 For use with SauceLabs (via SauceConnect) or local browsers.
 """
-from __future__ import absolute_import, print_function
 
 import errno
 import logging
 import os
-import socket
 from json import dumps
 from shutil import copyfile
 
 try:
     from needle.driver import (
         NeedleChrome as Chrome,
         NeedleFirefox as Firefox,
@@ -93,23 +91,23 @@
     """
     source = driver.page_source
     saved_source_dir = os.environ.get('SAVED_SOURCE_DIR')
     if not saved_source_dir:
         LOGGER.warning('The SAVED_SOURCE_DIR environment variable was not set; not saving page source')
         return
     file_name = os.path.join(saved_source_dir,
-                             '{name}.html'.format(name=name))
+                             f'{name}.html')
 
     try:
         if not os.path.exists(saved_source_dir):
             os.makedirs(saved_source_dir)
         with open(file_name, 'wb') as output_file:
             output_file.write(source.encode('utf-8'))
     except Exception:  # pylint: disable=broad-except
-        msg = u"Could not save the browser page source to {}.".format(file_name)
+        msg = f"Could not save the browser page source to {file_name}."
         LOGGER.warning(msg)
 
 
 def save_screenshot(driver, name):
     """
     Save a screenshot of the browser.
 
@@ -131,19 +129,15 @@
             return
         if not os.path.exists(screenshot_dir):
             os.makedirs(screenshot_dir)
         image_name = os.path.join(screenshot_dir, name + '.png')
         driver.save_screenshot(image_name)
 
     else:
-        msg = (
-            u"Browser does not support screenshots. "
-            u"Could not save screenshot '{name}'"
-        ).format(name=name)
-
+        msg = f"Browser does not support screenshots. Could not save screenshot '{name}'"
         LOGGER.warning(msg)
 
 
 def save_driver_logs(driver, prefix):
     """
     Save the selenium driver logs.
 
@@ -167,33 +161,32 @@
         os.makedirs(log_dir)
     if browser_name == 'firefox':
         # Firefox doesn't yet provide logs to Selenium, but does log to a separate file
         # https://github.com/mozilla/geckodriver/issues/284
         # https://firefox-source-docs.mozilla.org/testing/geckodriver/geckodriver/TraceLogs.html
         log_path = os.path.join(os.getcwd(), 'geckodriver.log')
         if os.path.exists(log_path):
-            dest_path = os.path.join(log_dir, '{}_geckodriver.log'.format(prefix))
+            dest_path = os.path.join(log_dir, f'{prefix}_geckodriver.log')
             copyfile(log_path, dest_path)
         return
 
     log_types = driver.log_types
     for log_type in log_types:
         try:
             log = driver.get_log(log_type)
             file_name = os.path.join(
-                log_dir, '{}_{}.log'.format(prefix, log_type)
+                log_dir, f'{prefix}_{log_type}.log'
             )
-            with open(file_name, 'w') as output_file:
+            with open(file_name, 'w', encoding="utf8") as output_file:
                 for line in log:
                     output_file.write("{}{}".format(dumps(line), '\n'))
         except:  # pylint: disable=bare-except
             msg = (
-                u"Could not save browser log of type '{log_type}'. "
-                u"It may be that the browser does not support it."
-            ).format(log_type=log_type)
+                f"Could not save browser log of type '{log_type}'. It may be that the browser does not support it."
+            )
 
             LOGGER.warning(msg, exc_info=True)
 
 
 def browser(tags=None, proxy=None, other_caps=None):
     """
     Interpret environment variables to configure Selenium.
@@ -283,17 +276,17 @@
             if browser_class == webdriver.Remote:
                 desired_caps = other_caps or {}
                 desired_caps.update(browser_kwargs.get('desired_capabilities', {}))
                 browser_kwargs['desired_capabilities'] = desired_caps
 
             return True, browser_class(*browser_args, **browser_kwargs)
 
-        except (socket.error, WebDriverException) as err:
+        except (OSError, WebDriverException) as err:
             msg = str(err)
-            LOGGER.debug(u'Failed to instantiate browser: %s', msg)
+            LOGGER.debug('Failed to instantiate browser: %s', msg)
             return False, None
 
     browser_instance = Promise(
         # There are cases where selenium takes 30s to return with a failure, so in order to try 3
         # times, we set a long timeout. If there is a hang on the first try, the timeout will
         # be enforced.
         browser_check_func, "Browser is instantiated successfully.", try_limit=3, timeout=95).fulfill()
@@ -312,30 +305,31 @@
 
 
 def _firefox_profile():
     """Configure the Firefox profile, respecting FIREFOX_PROFILE_PATH if set"""
     profile_dir = os.environ.get(FIREFOX_PROFILE_ENV_VAR)
 
     if profile_dir:
-        LOGGER.info(u"Using firefox profile: %s", profile_dir)
+        LOGGER.info("Using firefox profile: %s", profile_dir)
         try:
             firefox_profile = webdriver.FirefoxProfile(profile_dir)
         except OSError as err:
             if err.errno == errno.ENOENT:
                 raise BrowserConfigError(
-                    u"Firefox profile directory {env_var}={profile_dir} does not exist".format(
-                        env_var=FIREFOX_PROFILE_ENV_VAR, profile_dir=profile_dir))
+                    f"Firefox profile directory {FIREFOX_PROFILE_ENV_VAR}={profile_dir} does not exist"
+                ) from err
             if err.errno == errno.EACCES:
                 raise BrowserConfigError(
-                    u"Firefox profile directory {env_var}={profile_dir} has incorrect permissions. It must be \
-                    readable and executable.".format(env_var=FIREFOX_PROFILE_ENV_VAR, profile_dir=profile_dir))
+                    f"Firefox profile directory {FIREFOX_PROFILE_ENV_VAR}={profile_dir} has incorrect permissions. "
+                    f"It must be readable and executable."
+                ) from err
             # Some other OSError:
             raise BrowserConfigError(
-                u"Problem with firefox profile directory {env_var}={profile_dir}: {msg}"
-                .format(env_var=FIREFOX_PROFILE_ENV_VAR, profile_dir=profile_dir, msg=str(err)))
+                f"Problem with firefox profile directory {FIREFOX_PROFILE_ENV_VAR}={profile_dir}: {str(err)}"
+            ) from err
     else:
         LOGGER.info("Using default firefox profile")
         firefox_profile = webdriver.FirefoxProfile()
 
         # Bypasses the security prompt displayed by the browser when it attempts to
         # access a media device (e.g., a webcam)
         firefox_profile.set_preference('media.navigator.permission.disabled', True)
@@ -373,23 +367,24 @@
 
 def _local_browser_class(browser_name):
     """
     Returns class, kwargs, and args needed to instantiate the local browser.
     """
 
     # Log name of local browser
-    LOGGER.info(u"Using local browser: %s [Default is firefox]", browser_name)
+    LOGGER.info("Using local browser: %s [Default is firefox]", browser_name)
 
     # Get class of local browser based on name
     browser_class = BROWSERS.get(browser_name)
     headless = os.environ.get('BOKCHOY_HEADLESS', 'false').lower() == 'true'
     if browser_class is None:
         raise BrowserConfigError(
-            u"Invalid browser name {name}.  Options are: {options}".format(
-                name=browser_name, options=", ".join(list(BROWSERS.keys()))))
+            f"Invalid browser name {browser_name}.  Options are: {', '.join(list(BROWSERS.keys()))}"
+        )
+
     if browser_name == 'firefox':
         # Remove geckodriver log data from previous test cases
         log_path = os.path.join(os.getcwd(), 'geckodriver.log')
         if os.path.exists(log_path):
             os.remove(log_path)
 
         firefox_options = FirefoxOptions()
@@ -450,23 +445,22 @@
     envs = _required_envs(env_vars)
     envs.update(_optional_envs())
 
     # Turn the environment variables into a dictionary of desired capabilities
     caps = _capabilities_dict(envs, tags)
 
     if 'accessKey' in caps:
-        LOGGER.info(u"Using SauceLabs: %s %s %s", caps['platform'], caps['browserName'], caps['version'])
+        LOGGER.info("Using SauceLabs: %s %s %s", caps['platform'], caps['browserName'], caps['version'])
     else:
-        LOGGER.info(u"Using Remote Browser: %s", caps['browserName'])
+        LOGGER.info("Using Remote Browser: %s", caps['browserName'])
 
     # Create and return a new Browser
     # We assume that the WebDriver end-point is running locally (e.g. using
     # SauceConnect)
-    url = u"http://{0}:{1}/wd/hub".format(
-        envs['SELENIUM_HOST'], envs['SELENIUM_PORT'])
+    url = f"http://{envs['SELENIUM_HOST']}:{envs['SELENIUM_PORT']}/wd/hub"
 
     browser_args = []
     browser_kwargs = {
         'command_executor': url,
         'desired_capabilities': caps,
     }
     if caps['browserName'] == 'firefox':
@@ -507,18 +501,18 @@
 def _use_remote_browser(required_vars):
     """
     Returns a boolean indicating whether we should use a remote
     browser.  This means the user has made an attempt to set
     environment variables indicating they want to connect to SauceLabs
     or a remote browser.
     """
-    return all([
+    return all(
         key in os.environ
         for key in required_vars
-    ])
+    )
 
 
 def _required_envs(env_vars):
     """
     Parse environment variables for required values,
     raising a `BrowserConfig` error if they are not found.
 
@@ -529,21 +523,21 @@
         for key in env_vars
     }
 
     # Check for missing keys
     missing = [key for key, val in list(envs.items()) if val is None]
     if missing:
         msg = (
-            u"These environment variables must be set: " + u", ".join(missing)
+            "These environment variables must be set: " + ", ".join(missing)
         )
         raise BrowserConfigError(msg)
 
     # Check that we support this browser
     if envs['SELENIUM_BROWSER'] not in BROWSERS:
-        msg = u"Unsuppported browser: {0}".format(envs['SELENIUM_BROWSER'])
+        msg = f"Unsuppported browser: {envs['SELENIUM_BROWSER']}"
         raise BrowserConfigError(msg)
 
     return envs
 
 
 def _optional_envs():
     """
```

### Comparing `bok_choy-1.1.1/bok_choy/web_app_test.py` & `bok_choy-2.0.2/bok_choy/web_app_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """
 Base class for testing a web application.
 """
-from __future__ import absolute_import
 
 from abc import ABCMeta
 import sys
 from unittest import SkipTest, TestCase
 from uuid import uuid4
 
 try:
     from needle.cases import import_from_string, NeedleTestCase as BaseTestCase
 except ImportError:
     try:
         from unittest2 import TestCase as BaseTestCase
     except ImportError:
         BaseTestCase = TestCase
 from selenium.webdriver import PhantomJS
-import six
 
 from .browser import browser, save_screenshot, save_driver_logs, save_source
 
 
-@six.add_metaclass(ABCMeta)
-class WebAppTest(BaseTestCase):
+class WebAppTest(BaseTestCase, metaclass=ABCMeta):
 
     """
     Base class for testing a web application.
     """
 
     # Execute tests in parallel!
     _multiprocess_can_split_ = True
 
     viewport_width = 1024
     viewport_height = 768
 
     def __init__(self, *args, **kwargs):
-        super(WebAppTest, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         # This allows using the @attr() decorator from nose to set these on a
         # test by test basis
         self.proxy = getattr(self, 'proxy', None)
 
     @classmethod
     def setUpClass(cls):
@@ -62,29 +59,29 @@
             # but instead into our setUp method. This follows our paradigm of starting
             # up a new browser session for each TestCase.
 
             # Now call the super of the NeedleTestCase class, so that we get everything
             # from the setUpClass method of its parent (unittest.TestCase).
             super(BaseTestCase, cls).setUpClass()  # pylint: disable=bad-super-call
         else:
-            super(WebAppTest, cls).setUpClass()
+            super().setUpClass()
 
     @classmethod
     def tearDownClass(cls):
         """
         Override NeedleTestCase's tearDownClass method because it
         would quit the browser. This is not needed as we have already quit the browser
         after each TestCase, by virtue of a cleanup that we add in the setUp method.
         """
         if hasattr(cls, 'engine_class'):
             # We still want to call the super of the NeedleTestCase class, so that we get
             # everything from the tearDownClass method of its parent (unittest.TestCase).
             super(BaseTestCase, cls).tearDownClass()  # pylint: disable=bad-super-call
         else:
-            super(WebAppTest, cls).tearDownClass()
+            super().tearDownClass()
 
     def get_web_driver(self):
         """
         Override NeedleTestCases's get_web_driver class method to return the WebDriver instance
         that is already being used, instead of starting up a new one.
         """
         return self.browser
@@ -108,30 +105,30 @@
         feature. It is particularly useful to predict the size of the resulting screenshots
         when taking fullscreen captures, or to test responsive sites.
         """
         self.driver.set_window_size(width, height)
 
         # Measure the difference between the actual document width and the
         # desired viewport width so we can account for scrollbars:
-        script = u"return {width: document.body.clientWidth, height: document.body.clientHeight};"
+        script = "return {width: document.body.clientWidth, height: document.body.clientHeight};"
         measured = self.driver.execute_script(script)
         delta = width - measured['width']
 
         if delta > 0:
             self.driver.set_window_size(width + delta, height)
 
     def setUp(self):
         """
         Start the browser for use by the test.
         You *must* call this in the `setUp` method of any subclasses before using the browser!
 
         Returns:
             None
         """
-        super(WebAppTest, self).setUp()
+        super().setUp()
 
         # Set up the browser
         # This will start the browser
         # If using SauceLabs, tag the job with test info
         tags = [self.id()]
         self.browser = browser(tags, self.proxy)
 
@@ -150,15 +147,15 @@
     def unique_id(self):
         """
         Helper method to return a uuid.
 
         Returns:
             39-char UUID string
         """
-        return str(uuid4().int)  # pylint: disable=no-member
+        return str(uuid4().int)
 
     def _save_artifacts(self):
         """
         On failure or error save a screenshot, the
         source html, and the selenium driver logs.
         """
         # Get the unittest.TestResult object storing the results for all tests
```

### Comparing `bok_choy-1.1.1/bok_choy/a11y/a11y_audit.py` & `bok_choy-2.0.2/bok_choy/a11y/a11y_audit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 """
 Interface for running accessibility audits on a PageObject.
 """
-from __future__ import absolute_import
 
-import io
 import os
-from abc import abstractmethod, abstractproperty, ABCMeta
-import six
+from abc import abstractmethod, ABCMeta
 
 
 class AccessibilityError(Exception):
     """
     The page violates one or more accessibility rules.
     """
 
 
 class A11yAuditConfigError(Exception):
     """
     An error in A11yAuditConfig.
     """
 
 
-@six.add_metaclass(ABCMeta)
-class A11yAuditConfig:
+class A11yAuditConfig(metaclass=ABCMeta):
     """
     The `A11yAuditConfig` object defines the options available in an
     accessibility ruleset.
     """
 
     def __init__(self, *args, **kwargs):
-        super(A11yAuditConfig, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.rules_file = None
 
     def set_rules_file(self, path=None):
         """
         Sets `self.rules_file` to the passed file.
 
         Args:
@@ -86,16 +82,15 @@
                 specific implementation.
         """
         raise NotImplementedError(
             "The ability to customize the ruleset has not been implemented."
         )
 
 
-@six.add_metaclass(ABCMeta)
-class A11yAudit:
+class A11yAudit(metaclass=ABCMeta):
     """
     Allows auditing of a page for accessibility issues.
 
     The ruleset to use can be specified by the environment variable
     `BOKCHOY_A11Y_RULESET`. Currently, there are two ruleset implemented:
 
     `axe_core`:
@@ -115,32 +110,31 @@
         Sets ruleset to be used.
 
         Args:
             browser: A browser instance
             url: URL of the page to test
             config: (optional) A11yAuditConfig or subclass of A11yAuditConfig
         """
-        super(A11yAudit, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.url = url
         self.browser = browser
         self.config = config or self.default_config
 
     def _get_rules_js(self):
         """
         Checks that the rules file for the enabled ruleset exists
         and returns its contents as string.
 
         Raises: `RuntimeError` if the file isn't found.
         """
         if not os.path.isfile(self.config.rules_file):
-            msg = u'Could not find the accessibility tools JS file: {}'.format(
-                self.config.rules_file)
+            msg = f'Could not find the accessibility tools JS file: {self.config.rules_file}'
             raise RuntimeError(msg)
 
-        with io.open(self.config.rules_file, "r", encoding="utf-8") as rules_file:
+        with open(self.config.rules_file, "r", encoding="utf-8") as rules_file:
             return rules_file.read()
 
     def do_audit(self):
         """
         Audit the page for accessibility problems using the enabled ruleset.
 
         Returns:
@@ -168,15 +162,16 @@
 
             AccessibilityError
         """
         audit_results = self.do_audit()
         if audit_results:
             self.report_errors(audit_results, self.url)
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def default_config(self):
         """
         Return an instance of a subclass of A11yAuditConfig.
         """
         raise NotImplementedError("default_config has not been implemented")
 
     @staticmethod
```

### Comparing `bok_choy-1.1.1/bok_choy/a11y/axe_core_ruleset.py` & `bok_choy-2.0.2/bok_choy/a11y/axe_core_ruleset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """
 Interface for using the axe-core ruleset.
 See: https://github.com/dequelabs/axe-core
 """
-from __future__ import absolute_import
 
 import json
 import os
 
 from textwrap import dedent, fill
 
 from .a11y_audit import A11yAudit, A11yAuditConfig, AccessibilityError, A11yAuditConfigError
 from ..promise import Promise
 
-
 CUR_DIR = os.path.dirname(os.path.abspath(__file__))
 
 
 class AxeCoreAuditConfig(A11yAuditConfig):
     """
     The `AxeCoreAuditConfig` object defines the options available when
     running an `AxeCoreAudit`.
     """
     def __init__(self, *args, **kwargs):
-        super(AxeCoreAuditConfig, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.rules, self.context = None, None
-        self.custom_rules = u"customRules={}"
+        self.custom_rules = "customRules={}"
         self.rules_file = os.path.join(
             os.path.split(CUR_DIR)[0],
             'vendor/axe-core/axe.min.js'
         )
 
         self.set_rules({})
         self.set_scope()
@@ -183,24 +181,24 @@
             to specify the path to the file containing the custom rules.
 
         Documentation for how to write rules:
 
             https://github.com/dequelabs/axe-core/blob/master/doc/developer-guide.md
 
         An example of a custom rules file can be found at
-        https://github.com/edx/bok-choy/tree/master/tests/a11y_custom_rules.js
+        https://github.com/openedx/bok-choy/tree/master/tests/a11y_custom_rules.js
         """
         custom_file = custom_ruleset_file or os.environ.get(
             "BOKCHOY_A11Y_CUSTOM_RULES_FILE"
         )
 
         if not custom_file:
             return
 
-        with open(custom_file, "r") as additional_rules:
+        with open(custom_file, encoding="utf8") as additional_rules:
             custom_rules = additional_rules.read()
 
         if "var customRules" not in custom_rules:
             raise A11yAuditConfigError(
                 "Custom rules file must include \"var customRules\""
             )
 
@@ -239,15 +237,15 @@
         Related documentation:
 
             https://github.com/dequelabs/axe-core/blob/master/doc/API.md#results-object
 
         __Caution__: You probably don't really want to call this method
         directly! It will be used by `AxeCoreAudit.do_audit`.
         """
-        audit_run_script = dedent(u"""
+        audit_run_script = dedent("""
             {rules_js}
             {custom_rules}
             axe.configure(customRules);
             var callback = function(err, results) {{
                 if (err) throw err;
                 window.a11yAuditResults = JSON.stringify(results);
                 window.console.log(window.a11yAuditResults);
@@ -256,15 +254,15 @@
         """).format(
             rules_js=rules_js,
             custom_rules=config.custom_rules,
             context=config.context,
             options=config.rules
         )
 
-        audit_results_script = dedent(u"""
+        audit_results_script = dedent("""
             window.console.log(window.a11yAuditResults);
             return window.a11yAuditResults;
         """)
 
         browser.execute_script(audit_run_script)
 
         def audit_results_check_func():
@@ -347,22 +345,22 @@
                     pass
 
             messages = messages.difference([''])
             return '; '.join(messages)
 
         lines = []
         for error_type in errors:
-            lines.append(u"Severity: {}".format(error_type.get("impact")))
-            lines.append(u"Rule ID: {}".format(error_type.get("id")))
-            lines.append(u"Help URL: {}\n".format(error_type.get('helpUrl')))
+            lines.append(f"Severity: {error_type.get('impact')}")
+            lines.append(f"Rule ID: {error_type.get('id')}")
+            lines.append(f"Help URL: {error_type.get('helpUrl')}\n")
 
             for node in error_type['nodes']:
-                msg = u"Message: {}".format(_get_message(node))
-                html = u"Html: {}".format(node.get('html').encode('utf-8'))
-                target = u"Target: {}".format(node.get('target'))
+                msg = f"Message: {_get_message(node)}"
+                html = f"Html: {node.get('html').encode('utf-8')}"
+                target = f"Target: {node.get('target')}"
                 fill_opts = {
                     'width': 100,
                     'initial_indent': '\t',
                     'subsequent_indent': '\t\t',
                 }
                 lines.append(fill(msg, **fill_opts))
                 lines.append(fill(html, **fill_opts))
@@ -379,13 +377,9 @@
             audit: results of `AxeCoreAudit.do_audit()`.
             url: the url of the page being audited.
 
         Raises: `AccessibilityError`
         """
         errors = AxeCoreAudit.get_errors(audit)
         if errors["total"] > 0:
-            msg = u"URL '{}' has {} errors:\n\n{}".format(
-                url,
-                errors["total"],
-                AxeCoreAudit.format_errors(errors["errors"])
-            )
+            msg = f"URL '{url}' has {errors['total']} errors:\n\n{AxeCoreAudit.format_errors(errors['errors'])}"
             raise AccessibilityError(msg)
```

### Comparing `bok_choy-1.1.1/bok_choy/a11y/axs_ruleset.py` & `bok_choy-2.0.2/bok_choy/a11y/axs_ruleset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Interface for using the google accessibility ruleset.
 See: https://github.com/GoogleChrome/accessibility-developer-tools
 """
-from __future__ import absolute_import
 
 import logging
 import os
 
 from collections import namedtuple
 from textwrap import dedent
 
@@ -19,15 +18,15 @@
 
 class AxsAuditConfig(A11yAuditConfig):
     """
     The `AxsAuditConfig` object defines the options available when
     running an `AxsAudit`.
     """
     def __init__(self, *args, **kwargs):
-        super(AxsAuditConfig, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.rules_file = None
         self.scope, self.rules_to_run, self.rules_to_ignore = None, None, None
         self.rules_file = os.path.join(
             os.path.split(CUR_DIR)[0],
             'vendor/google/axs_testing.js'
         )
         self.set_rules({})
@@ -86,17 +85,15 @@
                 page.a11y_audit.config.set_scope(["div#foo"])
 
             To reset the scope to check the whole document::
 
                 page.a11y_audit.config.set_scope()
         """
         if include:
-            self.scope = u"document.querySelector(\"{}\")".format(
-                u', '.join(include)
-            )
+            self.scope = f"document.querySelector(\"{', '.join(include)}\")"
         else:
             self.scope = "null"
 
         if exclude is not None:
             raise NotImplementedError(
                 "The argument `exclude` has not been implemented in "
                 "AxsAuditConfig.set_scope method."
@@ -156,36 +153,31 @@
             return None
 
         # This line will only be included in the script if rules to check on
         # this page are specified, as the default behavior of the js is to
         # run all rules.
         rules = config.rules_to_run
         if rules:
-            rules_config = u"auditConfig.auditRulesToRun = {rules};".format(
-                rules=rules)
+            rules_config = f"auditConfig.auditRulesToRun = {rules};"
         else:
             rules_config = ""
 
         ignored_rules = config.rules_to_ignore
         if ignored_rules:
-            rules_config += (
-                u"\nauditConfig.auditRulesToIgnore = {rules};".format(
-                    rules=ignored_rules
-                )
-            )
+            rules_config += f"\nauditConfig.auditRulesToIgnore = {ignored_rules};"
 
-        script = dedent(u"""
+        script = dedent(f"""
             {rules_js}
             var auditConfig = new axs.AuditConfiguration();
             {rules_config}
-            auditConfig.scope = {scope};
+            auditConfig.scope = {config.scope};
             var run_results = axs.Audit.run(auditConfig);
             var audit_results = axs.Audit.auditResults(run_results)
             return audit_results;
-        """.format(rules_js=rules_js, rules_config=rules_config, scope=config.scope))
+            """)
 
         result = browser.execute_script(script)
 
         # audit_results is report of accessibility errors for that session
         audit_results = AuditResults(
             errors=result.get('errors_'),
             warnings=result.get('warnings_')
@@ -215,13 +207,9 @@
             audit: results of `AxsAudit.do_audit()`.
             url: the url of the page being audited.
 
         Raises: `AccessibilityError`
         """
         errors = AxsAudit.get_errors(audit)
         if errors:
-            msg = u"URL '{}' has {} errors:\n{}".format(
-                url,
-                len(errors),
-                ', '.join(errors)
-            )
+            msg = f"URL '{url}' has {len(errors)} errors:\n{', '.join(errors)}"
             raise AccessibilityError(msg)
```

### Comparing `bok_choy-1.1.1/bok_choy/page_object.py` & `bok_choy-2.0.2/bok_choy/page_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
 Base implementation of the Page Object pattern.
 See https://github.com/SeleniumHQ/selenium/wiki/PageObjects
 and http://www.seleniumhq.org/docs/06_test_design_considerations.jsp#page-object-design-pattern
 """
-from __future__ import absolute_import
 
-from abc import ABCMeta, abstractmethod, abstractproperty
+from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from functools import wraps
 from contextlib import contextmanager
 import logging
 import os
 import socket
 import re
 from textwrap import dedent
-import six
-from six.moves import urllib_parse
+from urllib import parse
 from lazy import lazy
 
 from selenium.common.exceptions import WebDriverException
 
 from .query import BrowserQuery, no_error
 from .promise import Promise, EmptyPromise, BrokenPromise
 from .a11y import AxeCoreAudit, AxsAudit
@@ -71,22 +69,21 @@
 
     Args:
         func (callable): The function to execute, with retries if an error occurs.
 
     Returns:
         Decorated function
     """
-    def _inner(*args, **kwargs):  # pylint: disable=missing-docstring
+    def _inner(*args, **kwargs):
         try:
             return_val = func(*args, **kwargs)
         except WebDriverException:
-            LOGGER.warning(u'Exception ignored during retry loop:', exc_info=True)
+            LOGGER.warning('Exception ignored during retry loop:', exc_info=True)
             return False
-        else:
-            return return_val
+        return return_val
 
     return _inner
 
 
 def unguarded(method):
     """
     Mark a PageObject method as unguarded.
@@ -111,15 +108,15 @@
     Args:
         method (callable): The method to decorate.
 
     Returns:
         Decorated method
     """
     @wraps(method)
-    def wrapper(self, *args, **kwargs):  # pylint: disable=missing-docstring
+    def wrapper(self, *args, **kwargs):
         self._verify_page()  # pylint: disable=protected-access
         return method(self, *args, **kwargs)
     return wrapper
 
 
 class _PageObjectMetaclass(ABCMeta):
     """
@@ -127,15 +124,15 @@
     so that they call self._verify_page() before executing.
 
     Excludes any methods marked as unguarded with the @unguarded
     decorator, any methods starting with _, or in the list ALWAYS_UNGUARDED.
     """
     ALWAYS_UNGUARDED = ['url', 'is_browser_on_page']
 
-    def __new__(mcs, cls_name, cls_bases, cls_attrs, **kwargs):  # pylint: disable=arguments-differ,unused-argument
+    def __new__(mcs, cls_name, cls_bases, cls_attrs, **kwargs):
         for name, attr in list(cls_attrs.items()):
             # Skip methods marked as unguarded
             if getattr(attr, '_unguarded', False) or name in mcs.ALWAYS_UNGUARDED:
                 continue
 
             # Skip private methods
             if name.startswith('_'):
@@ -162,19 +159,18 @@
                             property_methods[fn_name] = prop_fn
                         else:
                             property_methods[fn_name] = pre_verify(prop_fn)
                 cls_attrs[name] = property(**property_methods)
             else:
                 cls_attrs[name] = pre_verify(attr)
 
-        return super(_PageObjectMetaclass, mcs).__new__(mcs, cls_name, cls_bases, cls_attrs)
+        return super().__new__(mcs, cls_name, cls_bases, cls_attrs)
 
 
-@six.add_metaclass(_PageObjectMetaclass)
-class PageObject:
+class PageObject(metaclass=_PageObjectMetaclass):
     """
     Encapsulates user interactions with a specific part
     of a web application.
 
     The most important thing is this:
     Page objects encapsulate Selenium.
 
@@ -223,15 +219,15 @@
 
         Args:
             browser (selenium.webdriver): The Selenium-controlled browser.
 
         Returns:
             PageObject
         """
-        super(PageObject, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.browser = browser
         a11y_flag = os.environ.get('VERIFY_ACCESSIBILITY', 'False')
         self.verify_accessibility = a11y_flag.lower() == 'true'
         xss_flag = os.environ.get('VERIFY_XSS', 'False')
         self.verify_xss = xss_flag.lower() == 'true'
 
     @lazy
@@ -261,15 +257,16 @@
             3) page headings
 
         Returns:
             A `bool` indicating whether the browser is on the correct page.
         """
         return False
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def url(self):
         """
         Return the URL of the page.  This may be dynamic,
         determined by configuration options passed to the
         page object's constructor.
 
         Some pages may not be directly accessible:
@@ -311,86 +308,88 @@
             PageLoadError: The page did not load successfully.
             NotImplementedError: The page object does not provide a URL to visit.
 
         Returns:
             PageObject
         """
         if self.url is None:
-            raise NotImplementedError(u"Page {} does not provide a URL to visit.".format(self))
+            raise NotImplementedError(f"Page {self} does not provide a URL to visit.")
 
         # Validate the URL
         if not self.validate_url(self.url):
-            raise PageLoadError(u"Invalid URL: '{}'".format(self.url))
+            raise PageLoadError(f"Invalid URL: '{self.url}'")
 
         # Visit the URL
         try:
             self.browser.get(self.url)
-        except (WebDriverException, socket.gaierror):
-            LOGGER.warning(u"Unexpected page load exception:", exc_info=True)
-            raise PageLoadError(u"Could not load page '{!r}' at URL '{}'".format(
-                self, self.url
-            ))
+        except (WebDriverException, socket.gaierror) as err:
+            LOGGER.warning("Unexpected page load exception:", exc_info=True)
+            raise PageLoadError(
+                "Could not load page '{!r}' at URL '{}'".format(  # pylint: disable=consider-using-f-string
+                    self, self.url)
+            ) from err
 
         # Give the browser enough time to get to the page, then return the page object
         # so that the caller can chain the call with an action:
         # Example: FooPage.visit().do_something()
         #
         # A BrokenPromise will be raised if the page object's is_browser_on_page method
         # does not return True before timing out.
         try:
             return self.wait_for_page()
-        except BrokenPromise:
-            raise PageLoadError(u"Timed out waiting to load page '{!r}' at URL '{}'".format(
-                self, self.url
-            ))
+        except BrokenPromise as err:
+            raise PageLoadError(
+                "Timed out waiting to load page '{!r}' at URL '{}'".format(  # pylint: disable=consider-using-f-string
+                    self, self.url
+                )
+            ) from err
 
     @classmethod
     @unguarded
     def validate_url(cls, url):
         """
         Return a boolean indicating whether the URL has a protocol and hostname.
         If a port is specified, ensure it is an integer.
 
         Arguments:
             url (str): The URL to check.
 
         Returns:
             Boolean indicating whether the URL has a protocol and hostname.
         """
-        result = urllib_parse.urlsplit(url)
+        result = parse.urlsplit(url)
 
         # Check that we have a protocol and hostname
         if not result.scheme:
-            LOGGER.warning(u"%s is missing a protocol", url)
+            LOGGER.warning("%s is missing a protocol", url)
             return False
         if not result.netloc:
-            LOGGER.warning(u"%s is missing a hostname", url)
+            LOGGER.warning("%s is missing a hostname", url)
             return False
 
         # Check that the port is an integer
         try:
             if result.port is not None:
                 int(result.port)
             elif result.netloc.endswith(':'):
                 # Valid URLs do not end with colons.
-                LOGGER.warning(u"%s has a colon after the hostname but no port", url)
+                LOGGER.warning("%s has a colon after the hostname but no port", url)
                 return False
         except ValueError:
-            LOGGER.warning(u"%s uses an invalid port", url)
+            LOGGER.warning("%s uses an invalid port", url)
             return False
-        else:
-            return True
+        return True
 
     def _verify_page(self):
         """
         Ask the page object if we're on the right page;
         if not, raise a `WrongPageError`.
         """
         if not self.is_browser_on_page():
-            msg = u"Not on the correct page to use '{!r}' at URL '{}'".format(
+            msg = "Not on the correct page to use '{!r}' at URL '{}'".format(  # pylint: disable=consider-using-f-string
                 self, self.url
             )
             raise WrongPageError(msg)
 
     def _verify_xss_exposure(self):
         """
         Verify that there are no obvious XSS exposures on the page (based on test authors
@@ -406,17 +405,16 @@
         # Check taken from https://www.owasp.org/index.php/XSS_Filter_Evasion_Cheat_Sheet#XSS_Locator.
         all_hits_count = html_source.count(XSS_HTML)
         if all_hits_count > 0:
             safe_hits_count = len(EXPECTED_ATTRIBUTE_FORMAT.findall(html_source))
             if all_hits_count > safe_hits_count:
                 potential_hits = re.findall('<[^<]+<xss', html_source)
                 raise XSSExposureError(
-                    u"{} XSS issue(s) found on page. Potential places are {}".format(
-                        all_hits_count - safe_hits_count, potential_hits
-                    )
+                    f"{all_hits_count - safe_hits_count} XSS issue(s) found on page. "
+                    f"Potential places are {potential_hits}"
                 )
 
     @unguarded
     def wait_for_page(self, timeout=30):
         """
         Block until the page loads, then returns the page.
         Useful for ensuring that we navigate successfully to a particular page.
@@ -447,33 +445,35 @@
             # Wait for page to load completely i.e. for document.readyState to become complete
             EmptyPromise(
                 _is_document_ready,
                 "The document and all sub-resources have finished loading.",
                 timeout=timeout
             ).fulfill()
         except BrokenPromise:
+            # pylint: disable=logging-format-interpolation
             LOGGER.warning(
-                u'document.readyState does not become complete for following url: {}'.format(self.url),
+                'document.readyState does not become complete '  # pylint: disable=consider-using-f-string
+                'for following url: {}'.format(self.url),
                 exc_info=True
             )
             # If document.readyState does not become complete after a specific time relax the
             # condition and check for interactive state
             EmptyPromise(
                 _is_document_interactive,
                 "The document is in interactive mode.",
                 timeout=timeout
             ).fulfill()
 
         result = Promise(
-            lambda: (self.is_browser_on_page(), self), u"loaded page {!r}".format(self),
+            lambda: (self.is_browser_on_page(), self), f"loaded page {self!r}",
             timeout=timeout
         ).fulfill()
 
         if self.verify_accessibility:
-            self.a11y_audit.check_for_accessibility_errors()  # pylint: disable=no-member
+            self.a11y_audit.check_for_accessibility_errors()
 
         return result
 
     @unguarded
     def q(self, **kwargs):  # pylint: disable=invalid-name
         """
         Construct a query on the browser.
@@ -512,18 +512,18 @@
             confirm (bool): Whether to confirm or cancel the alert.
 
         Returns:
             None
         """
 
         # Before executing the `with` block, stub the confirm/alert functions
-        script = dedent(u"""
-            window.confirm = function() {{ return {0}; }};
+        script = dedent(f"""
+            window.confirm = function() {{ return {"true" if confirm else "false"}; }};
             window.alert = function() {{ return; }};
-        """.format("true" if confirm else "false")).strip()
+        """).strip()
         self.browser.execute_script(script)
 
         # Execute the `with` block
         yield
 
     @unguarded
     def wait_for_ajax(self, timeout=30):
@@ -691,13 +691,13 @@
             timeout (float): Maximum number of seconds to wait for the element to be present on the
                 page before timing out.
 
         Raises: BrokenPromise if the element does not exist (and therefore scrolling to it is not possible)
 
         """
         # Ensure element exists
-        msg = u"Element '{element}' is present".format(element=element_selector)
+        msg = f"Element '{element_selector}' is present"
         self.wait_for(lambda: self.q(css=element_selector).present, msg, timeout=timeout)
 
         # Obtain coordinates and use those for JavaScript call
         loc = self.q(css=element_selector).first.results[0].location
-        self.browser.execute_script(u"window.scrollTo({x},{y})".format(x=loc['x'], y=loc['y']))
+        self.browser.execute_script(f"window.scrollTo({loc['x']},{loc['y']})")
```

### Comparing `bok_choy-1.1.1/bok_choy/query.py` & `bok_choy-2.0.2/bok_choy/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Tools for interacting with the DOM inside a browser.
 """
-from __future__ import absolute_import
 
 import logging
 
 from copy import copy
 from collections.abc import Sequence
 from itertools import islice
 from selenium.common.exceptions import WebDriverException
-import six
 from bok_choy.promise import Promise
 
-
+# pylint: disable=duplicate-code, useless-suppression
 LOGGER = logging.getLogger(__name__)
 
 # Mapping of query type to Selenium webdriver query method names
 QUERY_TYPES = {
     'css': 'find_elements_by_css_selector',
     'xpath': 'find_elements_by_xpath',
 }
@@ -35,47 +33,46 @@
 
     Args:
         func (callable): The function to execute, with retries if an error occurs.
 
     Returns:
         Decorated function
     """
-    def _inner(*args, **kwargs):  # pylint: disable=missing-docstring
+    def _inner(*args, **kwargs):
         try:
             return_val = func(*args, **kwargs)
         except WebDriverException:
-            LOGGER.warning(u'Exception ignored during retry loop:', exc_info=True)
+            LOGGER.warning('Exception ignored during retry loop:', exc_info=True)
             return False, None
-        else:
-            return True, return_val
+        return True, return_val
 
     return _inner
 
 
 class Query(Sequence):
     """
     General mechanism for selecting and transforming values.
     """
 
-    def __init__(self, seed_fn, desc=None):  # pylint: disable=super-init-not-called
+    def __init__(self, seed_fn, desc=None):
         """
         Configure the `Query`.
 
         Args:
             seed_fn (callable): Callable with no arguments that produces a list of values.
 
         Keyword Args:
             desc (str): A description of the query, used in log messages.
                 If not provided, defaults to the name of the seed function.
 
         Returns:
             Query
         """
         if desc is None:
-            desc = u'Query({})'.format(getattr(seed_fn, '__name__', ''))
+            desc = f"Query({getattr(seed_fn, '__name__', '')})"
 
         self.seed_fn = seed_fn
         self.transforms = []
         self.desc_stack = []
         self.desc = desc
 
     def replace(self, **kwargs):
@@ -93,15 +90,15 @@
             TypeError: The `Query` does not have the specified attribute.
         """
         clone = copy(self)
 
         clone.transforms = list(clone.transforms)
         for key, value in kwargs.items():
             if not hasattr(clone, key):
-                raise TypeError(u'replace() got an unexpected keyword argument {!r}'.format(key))
+                raise TypeError(f'replace() got an unexpected keyword argument {key!r}')
 
             setattr(clone, key, value)
         return clone
 
     def transform(self, transform, desc=None):
         """
         Create a copy of this query, transformed by `transform`.
@@ -114,15 +111,15 @@
             desc (str): A description of the transform, to use in log messages.
                 Defaults to the name of the `transform` function.
 
         Returns:
             Query
         """
         if desc is None:
-            desc = u'transform({})'.format(getattr(transform, '__name__', ''))
+            desc = f"transform({getattr(transform, '__name__', '')})"
 
         return self.replace(
             transforms=self.transforms + [transform],
             desc_stack=self.desc_stack + [desc]
         )
 
     def map(self, map_fn, desc=None):
@@ -137,15 +134,15 @@
                 Defaults to the name of the map function.
 
         Returns:
             Query
         """
         if desc is None:
             desc = getattr(map_fn, '__name__', '')
-        desc = u'map({})'.format(desc)
+        desc = f'map({desc})'
 
         return self.transform(lambda xs: (map_fn(x) for x in xs), desc=desc)
 
     def filter(self, filter_fn=None, desc=None, **kwargs):
         """
         Return a copy of this query, with some values removed.
 
@@ -176,19 +173,19 @@
         if filter_fn is None and not kwargs:
             raise TypeError('Must supply one of filter_fn or one or more attribute filter parameters to filter().')
 
         if desc is None:
             if filter_fn is not None:
                 desc = getattr(filter_fn, '__name__', '')
             elif kwargs:
-                desc = u", ".join([u"{}={!r}".format(key, value) for key, value in kwargs.items()])
-        desc = u"filter({})".format(desc)
+                desc = ", ".join([f"{key}={value!r}" for key, value in kwargs.items()])
+        desc = f"filter({desc})"
 
         if kwargs:
-            def filter_fn(elem):  # pylint: disable=function-redefined, missing-docstring
+            def filter_fn(elem):  # pylint: disable=function-redefined
                 return all(
                     getattr(elem, filter_key) == filter_value
                     for filter_key, filter_value
                     in kwargs.items()
                 )
 
         return self.transform(lambda xs: (x for x in xs if filter_fn(x)), desc=desc)
@@ -215,15 +212,15 @@
             The transformed results of the query.
 
         Raises:
             BrokenPromise: The query did not execute without a Selenium error after one or more attempts.
         """
         return Promise(
             no_error(self._execute),
-            u"Executing {!r}".format(self),
+            f"Executing {self!r}",
             try_limit=try_limit,
             try_interval=try_interval,
             timeout=timeout,
         ).fulfill()
 
     @property
     def results(self):
@@ -267,17 +264,17 @@
             >> q = Query(lambda: list(range(5)))
             >> q.first.results
             [0]
 
         Returns:
             Query
         """
-        def _transform(xs):  # pylint: disable=missing-docstring, invalid-name
+        def _transform(xs):  # pylint: disable=invalid-name
             try:
-                return [six.next(iter(xs))]
+                return [next(iter(xs))]
             except StopIteration:
                 return []
 
         return self.transform(_transform, 'first')
 
     def nth(self, index):
         """
@@ -294,26 +291,26 @@
 
         Args:
             index (int): The index of the element to select (starts from 0)
 
         Returns:
             Query
         """
-        def _transform(xs):  # pylint: disable=missing-docstring, invalid-name
+        def _transform(xs):  # pylint: disable=invalid-name
             try:
                 return [next(islice(iter(xs), index, None))]
 
             # Gracefully handle (a) running out of elements, and (b) negative indices
             except (StopIteration, ValueError):
                 return []
 
         return self.transform(_transform, 'nth')
 
     def __repr__(self):
-        return u".".join([self.desc] + self.desc_stack)
+        return ".".join([self.desc] + self.desc_stack)
 
 
 class BrowserQuery(Query):
     """
     A Query that operates on a browser.
     """
     def __init__(self, browser, **kwargs):
@@ -338,22 +335,22 @@
 
         if not kwargs:
             raise TypeError('Must pass a query keyword argument to BrowserQuery().')
 
         query_name, query_value = list(kwargs.items())[0]
 
         if query_name not in QUERY_TYPES:
-            raise TypeError(u'{} is not a supported query type for BrowserQuery()'.format(query_name))
+            raise TypeError(f'{query_name} is not a supported query type for BrowserQuery()')
 
-        def query_fn():  # pylint: disable=missing-docstring
+        def query_fn():
             return getattr(browser, QUERY_TYPES[query_name])(query_value)
 
-        super(BrowserQuery, self).__init__(
+        super().__init__(
             query_fn,
-            desc=u"BrowserQuery({}={!r})".format(query_name, query_value),
+            desc=f"BrowserQuery({query_name}={query_value!r})",
         )
         self.browser = browser
 
     def attrs(self, attribute_name):
         """
         Retrieve HTML attribute values from the elements matched by the query.
 
@@ -368,15 +365,15 @@
 
         Args:
             attribute_name (str): The name of the attribute values to retrieve.
 
         Returns:
             A list of attribute values for `attribute_name`.
         """
-        desc = u'attrs({!r})'.format(attribute_name)
+        desc = f'attrs({attribute_name!r})'
         return self.map(lambda el: el.get_attribute(attribute_name), desc).results
 
     @property
     def text(self):
         """
         Retrieve text from each matched element.
 
@@ -496,12 +493,12 @@
 
         Args:
             text (str): The text used to fill the element (usually a text field or text area).
 
         Returns:
             None
         """
-        def _fill(elem):  # pylint: disable=missing-docstring
+        def _fill(elem):
             elem.clear()
             elem.send_keys(text)
 
-        self.map(_fill, u'fill({!r})'.format(text)).execute()
+        self.map(_fill, f'fill({text!r})').execute()
```

### Comparing `bok_choy-1.1.1/bok_choy/javascript.py` & `bok_choy-2.0.2/bok_choy/javascript.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Helpers for dealing with JavaScript synchronization issues.
 """
-from __future__ import absolute_import
 
 import functools
 import json
 from textwrap import dedent
 from selenium.common.exceptions import TimeoutException, WebDriverException
 from .promise import EmptyPromise
 
@@ -51,15 +50,15 @@
         function (callable): Method to decorate.
 
     Returns:
         Decorated method
     """
 
     @functools.wraps(function)
-    def wrapper(*args, **kwargs):  # pylint: disable=missing-docstring
+    def wrapper(*args, **kwargs):
 
         # If not a method, then just call the function
         if len(args) < 1:
             return function(*args, **kwargs)
 
         # Otherwise, retrieve `self` as the first arg
         self = args[0]
@@ -80,15 +79,15 @@
     """
     Return a class decorator that:
 
     1) Defines a new class method, `wait_for_js`
     2) Defines a new class list variable, `store_name` and adds
         `store_values` to the list.
     """
-    def decorator(clz):  # pylint: disable=missing-docstring
+    def decorator(clz):
 
         # Add a `wait_for_js` method to the class
         if not hasattr(clz, 'wait_for_js'):
             setattr(clz, 'wait_for_js', _wait_for_js)  # pylint: disable= literal-used-as-attribute
 
         # Store the RequireJS module names in the class
         if not hasattr(clz, store_name):
@@ -118,42 +117,42 @@
         return
 
     # pylint: disable=protected-access
     # Wait for JavaScript variables to be defined
     if hasattr(self, '_js_vars') and self._js_vars:
         EmptyPromise(
             lambda: _are_js_vars_defined(self.browser, self._js_vars),
-            u"JavaScript variables defined: {0}".format(", ".join(self._js_vars))
+            f"JavaScript variables defined: {', '.join(self._js_vars)}"
         ).fulfill()
 
     # Wait for RequireJS dependencies to load
     if hasattr(self, '_requirejs_deps') and self._requirejs_deps:
         EmptyPromise(
             lambda: _are_requirejs_deps_loaded(self.browser, self._requirejs_deps),
-            u"RequireJS dependencies loaded: {0}".format(", ".join(self._requirejs_deps)),
+            f"RequireJS dependencies loaded: {', '.join(self._requirejs_deps)}",
             try_limit=5
         ).fulfill()
 
 
 def _are_js_vars_defined(browser, js_vars):
     """
     Return a boolean indicating whether all the JavaScript
     variables `js_vars` are defined on the current page.
 
     `browser` is a Selenium webdriver instance.
     """
     # This script will evaluate to True iff all of
     # the required vars are defined.
-    script = u" && ".join([
-        u"!(typeof {0} === 'undefined')".format(var)
+    script = " && ".join([
+        f"!(typeof {var} === 'undefined')"
         for var in js_vars
     ])
 
     try:
-        return browser.execute_script(u"return {}".format(script))
+        return browser.execute_script(f"return {script}")
     except WebDriverException as exc:
         if "is not defined" in exc.msg or "is undefined" in exc.msg:
             return False
         raise
 
 
 def _are_requirejs_deps_loaded(browser, deps):
@@ -170,15 +169,15 @@
     # the browser.  The browser indicates that it wants to return
     # control to us by calling `callback`, which is the last item
     # in the global `arguments` array.
     #
     # We install a RequireJS module with the dependencies we want
     # to ensure are loaded.  When our module loads, we return
     # control to the test suite.
-    script = dedent(u"""
+    script = dedent("""
         // Retrieve the callback function used to return control to the test suite
         var callback = arguments[arguments.length - 1];
 
         // If RequireJS isn't defined, then return immediately
         if (!window.require) {{
             callback("RequireJS not defined");
         }}
```

### Comparing `bok_choy-1.1.1/README.rst` & `bok_choy-2.0.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 bok-choy
 ========
 
 .. image:: https://img.shields.io/pypi/v/bok_choy.svg
     :target: https://pypi.python.org/pypi/bok_choy/
     :alt: PyPI
 
-.. image:: https://travis-ci.org/edx/bok-choy.svg?branch=master
-    :target: https://travis-ci.org/edx/bok-choy
-    :alt: Travis
+.. image:: https://github.com/openedx/bok-choy/workflows/Python%20CI/badge.svg?branch=master
+    :target: https://github.com/openedx/bok-choy/actions?query=workflow%3A%22Python+CI%22
+    :alt: Github CI
 
 .. image:: http://codecov.io/github/edx/bok-choy/coverage.svg?branch=master
     :target: http://codecov.io/github/edx/bok-choy?branch=master
     :alt: Codecov
 
 .. image:: https://readthedocs.org/projects/bok-choy/badge/?version=latest
     :target: http://bok-choy.readthedocs.io/en/latest/
     :alt: Documentation
 
 .. image:: https://img.shields.io/pypi/pyversions/bok_choy.svg
     :target: https://pypi.python.org/pypi/bok_choy/
     :alt: Supported Python versions
 
 .. image:: https://img.shields.io/github/license/edx/bok-choy.svg
-    :target: https://github.com/edx/bok-choy/blob/master/LICENSE.txt
+    :target: https://github.com/openedx/bok-choy/blob/master/LICENSE.txt
     :alt: License
 
 UI-level acceptance test framework.  `Full documentation available on ReadTheDocs`__.
 
 __ http://bok-choy.readthedocs.org/en/latest/
 
+⚠️ Deprecation Notice ⚠️
+------------------------
+
+As of 2022-02-18, `bok-choy is deprecated <https://github.com/openedx/public-engineering/issues/13>`_.
+All tests written using bok-choy have either been removed or are slated to be removed soon.
+Please do not write new tests using bok-choy!
+In the near future, this repository will be archived.
 
 Overview
 --------
 
 A Python framework for writing robust Selenium tests.
 
-
 Installation
 ------------
 
 As Bok Choy is a Python framework, you first need to install Python.
 If you’re running Linux or Mac OS X, you probably already have it installed.
 We recommend that you use `pip <http://www.pip-installer.org/>`_ to install your Python
 packages:
@@ -61,21 +67,21 @@
 -------------
 
 To run the test suite for bok-choy itself:
 
 * Install Firefox; as of this writing, the current `version 59.0.1 <https://ftp.mozilla.org/pub/firefox/releases/59.0.1/>`_
   works with the latest selenium Python package (3.11.0)
 * Install `phantomjs <http://phantomjs.org/download.html>`_
-* Create a virtualenv which uses Python 2.7, 3.5, or 3.6
-* With that virtualenv activated, run ``pip install -r requirements/tox.txt`` to
+* Create a virtualenv which uses Python 3.8
+* With that virtualenv activated, run ``pip install -r requirements/ci.txt`` to
   install the `tox <http://tox.testrun.org/>`_ testing tool and its
   dependencies
-* Run ``tox -e py27`` (or ``tox -e py35``, etc.).  If you want to run the tests in
-  parallel, add the desired number of worker processes like ``tox -e py27 -- -n 5``
-  or ``tox -e py35 -- -n auto``.
+* Run ``tox -e py38``.  If you want to run the tests in
+  parallel, add the desired number of worker processes like ``tox -e py38 -- -n 5``
+  or ``tox -e py38 -- -n auto``.
 * To test and build the documentation, run ``tox -e doc``
 * To run an individual test, run ``py.test tests/<test file>::<test class>::<test name>``
 
 
 License
 -------
```

### Comparing `bok_choy-1.1.1/AUTHORS` & `bok_choy-2.0.2/AUTHORS`

 * *Files identical despite different names*

