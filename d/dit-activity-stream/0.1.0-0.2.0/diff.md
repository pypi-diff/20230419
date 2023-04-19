# Comparing `tmp/dit_activity_stream-0.1.0.tar.gz` & `tmp/dit_activity_stream-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dit_activity_stream-0.1.0.tar", max compression
+gzip compressed data, was "dit_activity_stream-0.2.0.tar", max compression
```

## Comparing `dit_activity_stream-0.1.0.tar` & `dit_activity_stream-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1091 2022-11-17 16:47:15.957768 dit_activity_stream-0.1.0/LICENSE
--rw-r--r--   0        0        0     2678 2022-11-21 11:56:33.916206 dit_activity_stream-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958280 dit_activity_stream-0.1.0/dit_activity_stream/__init__.py
--rw-r--r--   0        0        0     5272 2022-11-17 16:47:15.958448 dit_activity_stream-0.1.0/dit_activity_stream/client.py
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958505 dit_activity_stream-0.1.0/dit_activity_stream/py.typed
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958646 dit_activity_stream-0.1.0/dit_activity_stream/test_app/__init__.py
--rw-r--r--   0        0        0      257 2022-11-17 16:47:15.958783 dit_activity_stream-0.1.0/dit_activity_stream/test_app/apps.py
--rw-r--r--   0        0        0     1118 2022-11-17 16:47:15.958923 dit_activity_stream-0.1.0/dit_activity_stream/test_app/client.py
--rw-r--r--   0        0        0      321 2022-11-17 16:47:15.959043 dit_activity_stream-0.1.0/dit_activity_stream/test_app/factories.py
--rw-r--r--   0        0        0      336 2022-11-17 16:47:15.959163 dit_activity_stream-0.1.0/dit_activity_stream/test_app/models.py
--rw-r--r--   0        0        0     1398 2022-11-17 16:47:15.959307 dit_activity_stream-0.1.0/dit_activity_stream/test_app/settings.py
--rw-r--r--   0        0        0      128 2022-11-17 16:47:15.959434 dit_activity_stream-0.1.0/dit_activity_stream/test_app/urls.py
--rw-r--r--   0        0        0     1218 2022-11-17 16:47:15.959555 dit_activity_stream-0.1.0/dit_activity_stream/test_app/utils.py
--rw-r--r--   0        0        0        0 2022-11-17 16:47:15.959678 dit_activity_stream-0.1.0/dit_activity_stream/tests/__init__.py
--rw-r--r--   0        0        0      634 2022-11-17 16:47:15.959809 dit_activity_stream-0.1.0/dit_activity_stream/tests/test_client.py
--rw-r--r--   0        0        0     3869 2022-11-17 16:47:15.959944 dit_activity_stream-0.1.0/dit_activity_stream/tests/test_views.py
--rw-r--r--   0        0        0      168 2022-11-17 16:47:15.960056 dit_activity_stream-0.1.0/dit_activity_stream/urls.py
--rw-r--r--   0        0        0     1374 2022-11-18 13:29:28.471899 dit_activity_stream-0.1.0/dit_activity_stream/views.py
--rw-r--r--   0        0        0      789 2022-11-21 12:15:43.649409 dit_activity_stream-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 dit_activity_stream-0.1.0/setup.py
--rw-r--r--   0        0        0     3432 1970-01-01 00:00:00.000000 dit_activity_stream-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-17 16:47:15.957768 dit_activity_stream-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2678 2022-11-21 11:56:33.916206 dit_activity_stream-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958280 dit_activity_stream-0.2.0/dit_activity_stream/__init__.py
+-rw-r--r--   0        0        0     5272 2022-11-17 16:47:15.958448 dit_activity_stream-0.2.0/dit_activity_stream/client.py
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958505 dit_activity_stream-0.2.0/dit_activity_stream/py.typed
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.958646 dit_activity_stream-0.2.0/dit_activity_stream/test_app/__init__.py
+-rw-r--r--   0        0        0      257 2022-11-17 16:47:15.958783 dit_activity_stream-0.2.0/dit_activity_stream/test_app/apps.py
+-rw-r--r--   0        0        0     1118 2022-11-17 16:47:15.958923 dit_activity_stream-0.2.0/dit_activity_stream/test_app/client.py
+-rw-r--r--   0        0        0      321 2022-11-17 16:47:15.959043 dit_activity_stream-0.2.0/dit_activity_stream/test_app/factories.py
+-rw-r--r--   0        0        0      336 2022-11-17 16:47:15.959163 dit_activity_stream-0.2.0/dit_activity_stream/test_app/models.py
+-rw-r--r--   0        0        0     1398 2022-11-17 16:47:15.959307 dit_activity_stream-0.2.0/dit_activity_stream/test_app/settings.py
+-rw-r--r--   0        0        0      128 2022-11-17 16:47:15.959434 dit_activity_stream-0.2.0/dit_activity_stream/test_app/urls.py
+-rw-r--r--   0        0        0     1218 2022-11-17 16:47:15.959555 dit_activity_stream-0.2.0/dit_activity_stream/test_app/utils.py
+-rw-r--r--   0        0        0        0 2022-11-17 16:47:15.959678 dit_activity_stream-0.2.0/dit_activity_stream/tests/__init__.py
+-rw-r--r--   0        0        0      634 2022-11-17 16:47:15.959809 dit_activity_stream-0.2.0/dit_activity_stream/tests/test_client.py
+-rw-r--r--   0        0        0     3869 2022-11-17 16:47:15.959944 dit_activity_stream-0.2.0/dit_activity_stream/tests/test_views.py
+-rw-r--r--   0        0        0      168 2022-11-17 16:47:15.960056 dit_activity_stream-0.2.0/dit_activity_stream/urls.py
+-rw-r--r--   0        0        0     1374 2022-11-18 13:29:28.471899 dit_activity_stream-0.2.0/dit_activity_stream/views.py
+-rw-r--r--   0        0        0      788 2023-04-19 10:28:56.039099 dit_activity_stream-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 dit_activity_stream-0.2.0/PKG-INFO
```

### Comparing `dit_activity_stream-0.1.0/LICENSE` & `dit_activity_stream-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/README.md` & `dit_activity_stream-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/client.py` & `dit_activity_stream-0.2.0/dit_activity_stream/client.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/test_app/client.py` & `dit_activity_stream-0.2.0/dit_activity_stream/test_app/client.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/test_app/settings.py` & `dit_activity_stream-0.2.0/dit_activity_stream/test_app/settings.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/test_app/utils.py` & `dit_activity_stream-0.2.0/dit_activity_stream/test_app/utils.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/tests/test_client.py` & `dit_activity_stream-0.2.0/dit_activity_stream/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/tests/test_views.py` & `dit_activity_stream-0.2.0/dit_activity_stream/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/dit_activity_stream/views.py` & `dit_activity_stream-0.2.0/dit_activity_stream/views.py`

 * *Files identical despite different names*

### Comparing `dit_activity_stream-0.1.0/pyproject.toml` & `dit_activity_stream-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,36 +3,36 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "dit-activity-stream"
-version = "0.1.0"
+version = "0.2.0"
 description = "DIT Activity Stream"
 authors = [
     "Cameron Lamb <live.services@digital.trade.gov.uk>"
 ]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "django"
 ]
 homepage = "https://github.com/uktrade/dit-activity-stream"
 
 [tool.poetry.dependencies]
-python = "^3.6.3"
-Django = ">=2.2, <4.2"
-django-hawk = "^1.1.1"
+python = "^3.7"
+Django = ">=3.2, <4.2"
+django-hawk = "^1.2.0"
 
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

### Comparing `dit_activity_stream-0.1.0/setup.py` & `dit_activity_stream-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,118 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dit-activity-stream
+Version: 0.2.0
+Summary: DIT Activity Stream
+Home-page: https://github.com/uktrade/dit-activity-stream
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
+Requires-Dist: Django (>=3.2,<4.2)
+Requires-Dist: django-hawk (>=1.2.0,<2.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['dit_activity_stream',
- 'dit_activity_stream.test_app',
- 'dit_activity_stream.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Django>=2.2,<4.2', 'django-hawk>=1.1.1,<2.0.0']
-
-setup_kwargs = {
-    'name': 'dit-activity-stream',
-    'version': '0.1.0',
-    'description': 'DIT Activity Stream',
-    'long_description': '# DIT Activity Stream\n\n## Installation\n\nRead the [Django Hawk installation](https://github.com/uktrade/django-hawk/#installation) documentation.\n\nAdd the package to your `urls.py` file.\n\n```python\nfrom django.urls import include, path\n\nurlpatterns = [\n    ...\n    path("dit-activity-stream/", include("dit_activity_stream.urls")),\n    ...\n]\n```\n\n## How to implement?\n\nWrite your custom client, here is an example client for returning all users:\n\n```python\nfrom typing import Any, Dict\n\nfrom django.contrib.auth import get_user_model\nfrom django.db.models import QuerySet\nfrom django.http import HttpRequest\n\nfrom dit_activity_stream.client import ActivityStreamClient\n\nUser = get_user_model()\n\n\nclass ActivityStreamUserClient(ActivityStreamClient):\n    object_uuid_field: str = "user_id"\n    object_last_modified_field: str = "last_modified"\n\n    def get_queryset(self, request: HttpRequest) -> QuerySet:\n        return User.objects.all()\n\n    def render_object(self, object: User) -> Dict:\n        return {\n            "id": object.id,\n            "username": object.username,\n            "first_name": object.first_name,\n            "last_name": object.last_name,\n        }\n```\n\nWhere the following attributes:\n- `object_uuid_field` is a field on the Object that is a Unique Identifier for the object.\n  - This will be output in the URL GET parameter so it should be a UUID.\n- `object_last_modified_field` us a field on the Object that holds a datetime value of when the object was last modified.\n  - This will be output in the URL GET parameter.\n\nSet `DIT_ACTIVITY_STREAM_CLIENT_CLASS` in your django settings file:\n\n```python\nDIT_ACTIVITY_STREAM_CLIENT_CLASS = "package.client.ActivityStreamUserClient"\n```\n\n## Pushing to PyPI\n\n- [PyPI Package](https://pypi.org/project/dit-activity-stream/)\n- [Test PyPI Package](https://test.pypi.org/project/dit-activity-stream/)\n\nRunning `make build` will build the package into the `dist/` directory.\nRunning `make push-pypi-test` will push the built package to Test PyPI.\nRunning `make push-pypi` will push the built package to PyPI.\n\n### Setting up poetry for pushing to PyPI\n\nFirst you will need to add the test pypy repository to your poetry config:\n\n```\npoetry config repositories.test-pypi https://test.pypi.org/legacy/\n```\n\nThen go to https://test.pypi.org/manage/account/token/ and generate a token.\n\nThen add it to your poetry config:\n\n```\npoetry config pypi-token.test-pypi XXXXXXXX\n```\n\nThen you also need to go to https://pypi.org/manage/account/token/ to generate a token for the real PyPI.\n\nThen add it to your poetry config:\n\n```\npoetry config pypi-token.pypi XXXXXXXX\n```\n\nNow the make commands should work as expected.\n',
-    'author': 'Cameron Lamb',
-    'author_email': 'live.services@digital.trade.gov.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/uktrade/dit-activity-stream',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.3,<4.0.0',
-}
+# DIT Activity Stream
 
+## Installation
+
+Read the [Django Hawk installation](https://github.com/uktrade/django-hawk/#installation) documentation.
+
+Add the package to your `urls.py` file.
+
+```python
+from django.urls import include, path
+
+urlpatterns = [
+    ...
+    path("dit-activity-stream/", include("dit_activity_stream.urls")),
+    ...
+]
+```
+
+## How to implement?
+
+Write your custom client, here is an example client for returning all users:
+
+```python
+from typing import Any, Dict
+
+from django.contrib.auth import get_user_model
+from django.db.models import QuerySet
+from django.http import HttpRequest
+
+from dit_activity_stream.client import ActivityStreamClient
+
+User = get_user_model()
+
+
+class ActivityStreamUserClient(ActivityStreamClient):
+    object_uuid_field: str = "user_id"
+    object_last_modified_field: str = "last_modified"
+
+    def get_queryset(self, request: HttpRequest) -> QuerySet:
+        return User.objects.all()
+
+    def render_object(self, object: User) -> Dict:
+        return {
+            "id": object.id,
+            "username": object.username,
+            "first_name": object.first_name,
+            "last_name": object.last_name,
+        }
+```
+
+Where the following attributes:
+- `object_uuid_field` is a field on the Object that is a Unique Identifier for the object.
+  - This will be output in the URL GET parameter so it should be a UUID.
+- `object_last_modified_field` us a field on the Object that holds a datetime value of when the object was last modified.
+  - This will be output in the URL GET parameter.
+
+Set `DIT_ACTIVITY_STREAM_CLIENT_CLASS` in your django settings file:
+
+```python
+DIT_ACTIVITY_STREAM_CLIENT_CLASS = "package.client.ActivityStreamUserClient"
+```
+
+## Pushing to PyPI
+
+- [PyPI Package](https://pypi.org/project/dit-activity-stream/)
+- [Test PyPI Package](https://test.pypi.org/project/dit-activity-stream/)
+
+Running `make build` will build the package into the `dist/` directory.
+Running `make push-pypi-test` will push the built package to Test PyPI.
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
+
+Now the make commands should work as expected.
 
-setup(**setup_kwargs)
```

