# Comparing `tmp/django_hawk-1.1.1.tar.gz` & `tmp/django_hawk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hawk-1.1.1.tar", max compression
+gzip compressed data, was "django_hawk-1.2.0.tar", max compression
```

## Comparing `django_hawk-1.1.1.tar` & `django_hawk-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1091 2022-11-18 11:48:04.698434 django_hawk-1.1.1/LICENSE
--rw-r--r--   0        0        0     2627 2022-11-18 11:48:04.701767 django_hawk-1.1.1/README.md
--rw-r--r--   0        0        0        0 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/__init__.py
--rw-r--r--   0        0        0     1992 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/authentication.py
--rw-r--r--   0        0        0     1494 2022-11-18 15:02:59.469986 django_hawk-1.1.1/django_hawk/middleware.py
--rw-r--r--   0        0        0        0 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/py.typed
--rw-r--r--   0        0        0     1014 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/settings.py
--rw-r--r--   0        0        0        0 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/tests/__init__.py
--rw-r--r--   0        0        0     1008 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/tests/settings.py
--rw-r--r--   0        0        0     4717 2022-11-18 12:14:30.955072 django_hawk-1.1.1/django_hawk/tests/test_views.py
--rw-r--r--   0        0        0     1101 2022-11-18 15:02:59.469986 django_hawk-1.1.1/django_hawk/tests/test_views_django.py
--rw-r--r--   0        0        0      333 2022-11-18 15:02:59.469986 django_hawk-1.1.1/django_hawk/tests/urls.py
--rw-r--r--   0        0        0      936 2022-11-18 15:02:59.469986 django_hawk-1.1.1/django_hawk/tests/views.py
--rw-r--r--   0        0        0     1011 2022-11-18 11:48:04.701767 django_hawk-1.1.1/django_hawk/utils.py
--rw-r--r--   0        0        0      798 2022-11-18 15:02:59.469986 django_hawk-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3460 1970-01-01 00:00:00.000000 django_hawk-1.1.1/setup.py
--rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 django_hawk-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-15 16:57:39.615067 django_hawk-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2632 2023-04-19 10:07:40.848963 django_hawk-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615449 django_hawk-1.2.0/django_hawk/__init__.py
+-rw-r--r--   0        0        0     1992 2022-11-15 16:58:07.593679 django_hawk-1.2.0/django_hawk/authentication.py
+-rw-r--r--   0        0        0     1494 2023-02-28 10:16:42.657151 django_hawk-1.2.0/django_hawk/middleware.py
+-rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615710 django_hawk-1.2.0/django_hawk/py.typed
+-rw-r--r--   0        0        0     1014 2022-11-15 16:58:07.593989 django_hawk-1.2.0/django_hawk/settings.py
+-rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615896 django_hawk-1.2.0/django_hawk/tests/__init__.py
+-rw-r--r--   0        0        0     1008 2022-11-16 14:11:50.330670 django_hawk-1.2.0/django_hawk/tests/settings.py
+-rw-r--r--   0        0        0     4717 2022-11-16 16:21:34.934697 django_hawk-1.2.0/django_hawk/tests/test_views.py
+-rw-r--r--   0        0        0     1101 2023-02-28 10:16:42.657465 django_hawk-1.2.0/django_hawk/tests/test_views_django.py
+-rw-r--r--   0        0        0      333 2023-02-28 10:16:42.657597 django_hawk-1.2.0/django_hawk/tests/urls.py
+-rw-r--r--   0        0        0      936 2023-02-28 10:16:42.658072 django_hawk-1.2.0/django_hawk/tests/views.py
+-rw-r--r--   0        0        0     1011 2022-11-17 13:21:23.905719 django_hawk-1.2.0/django_hawk/utils.py
+-rw-r--r--   0        0        0      797 2023-04-19 10:12:06.051016 django_hawk-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 django_hawk-1.2.0/PKG-INFO
```

### Comparing `django_hawk-1.1.1/LICENSE` & `django_hawk-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/README.md` & `django_hawk-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,19 @@
 ```
 
 ## Pushing to PyPI
 
 - [PyPI Package](https://pypi.org/project/django-hawk/)
 - [Test PyPI Package](https://test.pypi.org/project/django-hawk/)
 
-Running `make build-package` will build the package into the `dist/` directory
-Running `make push-pypi-test` will push the built package to Test PyPI
-Running `make push-pypi` will push the built package to PyPI
+Running `make build-package` will build the package into the `dist/` directory.
+
+Running `make push-pypi-test` will push the built package to Test PyPI.
+
+Running `make push-pypi` will push the built package to PyPI.
 
 ### Setting up poetry for pushing to PyPI
 
 First you will need to add the test pypy repository to your poetry config:
 
 ```
 poetry config repositories.test-pypi https://test.pypi.org/legacy/
```

### Comparing `django_hawk-1.1.1/django_hawk/authentication.py` & `django_hawk-1.2.0/django_hawk/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/middleware.py` & `django_hawk-1.2.0/django_hawk/middleware.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/settings.py` & `django_hawk-1.2.0/django_hawk/settings.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/tests/settings.py` & `django_hawk-1.2.0/django_hawk/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/tests/test_views.py` & `django_hawk-1.2.0/django_hawk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/tests/test_views_django.py` & `django_hawk-1.2.0/django_hawk/tests/test_views_django.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/tests/views.py` & `django_hawk-1.2.0/django_hawk/tests/views.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/django_hawk/utils.py` & `django_hawk-1.2.0/django_hawk/utils.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.1.1/pyproject.toml` & `django_hawk-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,37 +3,37 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "django-hawk"
-version = "1.1.1"
+version = "1.2.0"
 description = "Authenticate Django Views with HAWK"
 authors = [
     "Cameron Lamb <live.services@digital.trade.gov.uk>"
 ]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "django"
 ]
 homepage = "https://github.com/uktrade/django-hawk"
 
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
-Django = ">=2.2, <4.2"
+python = ">=3.7,<4.0"
+Django = ">=3.2, <4.3"
 mohawk = ">=1.0.0, <2.0"
 
 [tool.poetry.group.testing]
 optional = true
 
 [tool.poetry.group.testing.dependencies]
-tox = "*"
+tox = "^4"
 freezegun = "*"
 coverage = "*"
 
 [tool.poetry.group.utils]
 optional = true
 
 [tool.poetry.group.utils.dependencies]
```

### Comparing `django_hawk-1.1.1/setup.py` & `django_hawk-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,136 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-hawk
+Version: 1.2.0
+Summary: Authenticate Django Views with HAWK
+Home-page: https://github.com/uktrade/django-hawk
+License: MIT
+Keywords: django
+Author: Cameron Lamb
+Author-email: live.services@digital.trade.gov.uk
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=3.2,<4.3)
+Requires-Dist: mohawk (>=1.0.0,<2.0)
+Description-Content-Type: text/markdown
+
+# Django Hawk
+
+This package can be used to help create HAWK Authenticated views.
+
+## Installation
+
+```
+pip install django-hawk
+```
+
+Add the following to your Django Settings:
+
+```python
+DJANGO_HAWK = {
+    "HAWK_INCOMING_ACCESS_KEY": "xxx",
+    "HAWK_INCOMING_SECRET_KEY": "xxx",
+}
+```
 
-packages = \
-['django_hawk', 'django_hawk.tests']
+## Example Usage
 
-package_data = \
-{'': ['*']}
+To use the HAWK Authentication, we need to do 2 things:
 
-install_requires = \
-['Django>=2.2,<4.2', 'mohawk>=1.0.0,<2.0']
-
-setup_kwargs = {
-    'name': 'django-hawk',
-    'version': '1.1.1',
-    'description': 'Authenticate Django Views with HAWK',
-    'long_description': '# Django Hawk\n\nThis package can be used to help create HAWK Authenticated views.\n\n## Installation\n\n```\npip install django-hawk\n```\n\nAdd the following to your Django Settings:\n\n```python\nDJANGO_HAWK = {\n    "HAWK_INCOMING_ACCESS_KEY": "xxx",\n    "HAWK_INCOMING_SECRET_KEY": "xxx",\n}\n```\n\n## Example Usage\n\nTo use the HAWK Authentication, we need to do 2 things:\n\n1. Make sure the `HawkResponseMiddleware` runs\n2. Check the authentication\n\nAdd the `HawkResponseMiddleware` to the `MIDDLEWARE` setting in your project like so:\n\n```\nMIDDLEWARE = [\n    ...\n    "django_hawk.middleware.HawkResponseMiddleware",\n    ...\n]\n```\n\nTo check the authentication you can call `django_hawk.utils.authenticate_request`, if an exception isn\'t raised then you know that the request is authenticated, see below for examples.\n\n```python\nfrom django.http import HttpResponse\n\nfrom django_hawk.utils import DjangoHawkAuthenticationFailed, authenticate_request\n\ndef simple_view(request):\n    # Try to authenticate with HAWK\n    try:\n        authenticate_request(request=request)\n    except DjangoHawkAuthenticationFailed as e:\n        return HttpResponse(status=401)\n\n    # Continue with normal View code...\n    return HttpResponse("This is a simple view")\n```\n\n## Testing\n\nTests belong in the `/django_hawk/tests/` directory. You can run the tests by installing the requirements like so:\n\n```\nmake setup\n```\n\nNow you can run the tests using the following command:\n\n```\npoetry run python manage.py test\n```\n\n### Tox tests\n\nWe use [tox](https://pypi.org/project/tox/) to test compatibility across different Django versions.\n\nTo run these tests with tox, just run the following:\n\n```\nmake tox\n```\n\n## Pushing to PyPI\n\n- [PyPI Package](https://pypi.org/project/django-hawk/)\n- [Test PyPI Package](https://test.pypi.org/project/django-hawk/)\n\nRunning `make build-package` will build the package into the `dist/` directory\nRunning `make push-pypi-test` will push the built package to Test PyPI\nRunning `make push-pypi` will push the built package to PyPI\n\n### Setting up poetry for pushing to PyPI\n\nFirst you will need to add the test pypy repository to your poetry config:\n\n```\npoetry config repositories.test-pypi https://test.pypi.org/legacy/\n```\n\nThen go to https://test.pypi.org/manage/account/token/ and generate a token.\n\nThen add it to your poetry config:\n\n```\npoetry config pypi-token.test-pypi XXXXXXXX\n```\n\nThen you also need to go to https://pypi.org/manage/account/token/ to generate a token for the real PyPI.\n\nThen add it to your poetry config:\n\n```\npoetry config pypi-token.pypi XXXXXXXX\n```\n\nNow the make commands should work as expected.\n',
-    'author': 'Cameron Lamb',
-    'author_email': 'live.services@digital.trade.gov.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/uktrade/django-hawk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<4.0',
-}
+1. Make sure the `HawkResponseMiddleware` runs
+2. Check the authentication
+
+Add the `HawkResponseMiddleware` to the `MIDDLEWARE` setting in your project like so:
+
+```
+MIDDLEWARE = [
+    ...
+    "django_hawk.middleware.HawkResponseMiddleware",
+    ...
+]
+```
+
+To check the authentication you can call `django_hawk.utils.authenticate_request`, if an exception isn't raised then you know that the request is authenticated, see below for examples.
+
+```python
+from django.http import HttpResponse
+
+from django_hawk.utils import DjangoHawkAuthenticationFailed, authenticate_request
+
+def simple_view(request):
+    # Try to authenticate with HAWK
+    try:
+        authenticate_request(request=request)
+    except DjangoHawkAuthenticationFailed as e:
+        return HttpResponse(status=401)
+
+    # Continue with normal View code...
+    return HttpResponse("This is a simple view")
+```
+
+## Testing
+
+Tests belong in the `/django_hawk/tests/` directory. You can run the tests by installing the requirements like so:
+
+```
+make setup
+```
+
+Now you can run the tests using the following command:
+
+```
+poetry run python manage.py test
+```
+
+### Tox tests
+
+We use [tox](https://pypi.org/project/tox/) to test compatibility across different Django versions.
+
+To run these tests with tox, just run the following:
+
+```
+make tox
+```
+
+## Pushing to PyPI
+
+- [PyPI Package](https://pypi.org/project/django-hawk/)
+- [Test PyPI Package](https://test.pypi.org/project/django-hawk/)
+
+Running `make build-package` will build the package into the `dist/` directory.
+
+Running `make push-pypi-test` will push the built package to Test PyPI.
+
+Running `make push-pypi` will push the built package to PyPI.
+
+### Setting up poetry for pushing to PyPI
+
+First you will need to add the test pypy repository to your poetry config:
+
+```
+poetry config repositories.test-pypi https://test.pypi.org/legacy/
+```
+
+Then go to https://test.pypi.org/manage/account/token/ and generate a token.
+
+Then add it to your poetry config:
+
+```
+poetry config pypi-token.test-pypi XXXXXXXX
+```
+
+Then you also need to go to https://pypi.org/manage/account/token/ to generate a token for the real PyPI.
+
+Then add it to your poetry config:
+
+```
+poetry config pypi-token.pypi XXXXXXXX
+```
 
+Now the make commands should work as expected.
 
-setup(**setup_kwargs)
```

