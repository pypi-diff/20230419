# Comparing `tmp/djdantic-0.0.7.tar.gz` & `tmp/djdantic-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djdantic-0.0.7.tar", last modified: Wed Apr 19 12:08:33 2023, max compression
+gzip compressed data, was "djdantic-0.0.8.tar", last modified: Wed Apr 19 12:21:16 2023, max compression
```

## Comparing `djdantic-0.0.7.tar` & `djdantic-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.141977 djdantic-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    26022 2023-04-19 12:08:23.000000 djdantic-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-19 12:08:23.000000 djdantic-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 12:08:33.141977 djdantic-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-19 12:08:23.000000 djdantic-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.137977 djdantic-0.0.7/djdantic/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.141977 djdantic-0.0.7/djdantic/context/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/context/access.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.141977 djdantic-0.0.7/djdantic/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/schemas/access.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/schemas/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/schemas/price.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.141977 djdantic-0.0.7/djdantic/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.141977 djdantic-0.0.7/djdantic/utils/pydantic_django/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic_django/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic_django/django_to_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic_django/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic_django/pydantic_to_django.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/pydantic_django/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 12:08:23.000000 djdantic-0.0.7/djdantic/utils/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:08:33.141977 djdantic-0.0.7/djdantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 12:08:33.000000 djdantic-0.0.7/djdantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 12:08:33.000000 djdantic-0.0.7/djdantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:08:33.000000 djdantic-0.0.7/djdantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:08:33.000000 djdantic-0.0.7/djdantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 12:08:33.000000 djdantic-0.0.7/djdantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 12:08:33.000000 djdantic-0.0.7/djdantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-19 12:08:33.141977 djdantic-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:08:23.000000 djdantic-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    26022 2023-04-19 12:21:11.000000 djdantic-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-19 12:21:11.000000 djdantic-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 12:21:16.812976 djdantic-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-19 12:21:11.000000 djdantic-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.808976 djdantic-0.0.8/djdantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/context/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/context/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/schemas/price.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic/utils/pydantic_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/django_to_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14557 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic_to_django.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/pydantic_django/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 12:21:11.000000 djdantic-0.0.8/djdantic/utils/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:21:16.812976 djdantic-0.0.8/djdantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 12:21:16.000000 djdantic-0.0.8/djdantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-19 12:21:16.812976 djdantic-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:21:11.000000 djdantic-0.0.8/setup.py
```

### Comparing `djdantic-0.0.7/LICENSE` & `djdantic-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/PKG-INFO` & `djdantic-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdantic
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities to use pydantic with the django orm
 Home-page: https://github.com/Voltane-EU/djdantic
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djdantic-0.0.7/README.md` & `djdantic-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/fields.py` & `djdantic-0.0.8/djdantic/fields.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/models.py` & `djdantic-0.0.8/djdantic/models.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/schemas/access.py` & `djdantic-0.0.8/djdantic/schemas/access.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/utils/pydantic.py` & `djdantic-0.0.8/djdantic/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/utils/pydantic_django/checks.py` & `djdantic-0.0.8/djdantic/utils/pydantic_django/checks.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/utils/pydantic_django/django_to_pydantic.py` & `djdantic-0.0.8/djdantic/utils/pydantic_django/django_to_pydantic.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/utils/pydantic_django/pydantic.py` & `djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic.py`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/djdantic/utils/pydantic_django/pydantic_to_django.py` & `djdantic-0.0.8/djdantic/utils/pydantic_django/pydantic_to_django.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 from enum import Enum
 from pydantic import BaseModel, validate_model, SecretStr
 from pydantic.fields import SHAPE_SINGLETON, SHAPE_LIST, Undefined
 from django.db import models
 from django.db.models.fields import Field as DjangoField
 from django.db.models.fields.related_descriptors import ManyToManyDescriptor, ReverseManyToOneDescriptor
 from django.db.transaction import atomic
-from dirtyfields import DirtyFieldsMixin
 from sentry_tools.decorators import instrument_span
 from sentry_tools.span import set_tag, set_data
 from async_tools import is_async, sync_to_async
 from ...schemas import Access
 from ..pydantic import Reference, get_orm_field_attr, is_orm_field_set
 from .checks import check_field_access
 
 try:
+    from dirtyfields import DirtyFieldsMixin
+
+except ImportError:
+    class DirtyFieldsMixin:
+        pass
+
+try:
     from fastapi.exceptions import RequestValidationError
 
 except ImportError:
     from pydantic import ValidationError as RequestValidationError
 
 
 class TransferAction(Enum):
```

### Comparing `djdantic-0.0.7/djdantic.egg-info/PKG-INFO` & `djdantic-0.0.8/djdantic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djdantic
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities to use pydantic with the django orm
 Home-page: https://github.com/Voltane-EU/djdantic
 Author: Manuel Stingl
 Author-email: opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djdantic-0.0.7/djdantic.egg-info/SOURCES.txt` & `djdantic-0.0.8/djdantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djdantic-0.0.7/setup.cfg` & `djdantic-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djdantic
-version = 0.0.7
+version = 0.0.8
 author = Manuel Stingl
 author_email = opensource@voltane.eu
 description = Utilities to use pydantic with the django orm
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```

