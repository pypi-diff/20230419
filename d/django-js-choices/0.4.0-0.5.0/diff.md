# Comparing `tmp/django-js-choices-0.4.0.tar.gz` & `tmp/django_js_choices-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-js-choices-0.4.0.tar", max compression
+gzip compressed data, was "django_js_choices-0.5.0.tar", max compression
```

## Comparing `django-js-choices-0.4.0.tar` & `django_js_choices-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1075 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/LICENSE
--rw-r--r--   0        0        0     6600 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/README.rst
--rw-r--r--   0        0        0        0 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/__init__.py
--rw-r--r--   0        0        0     3628 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/core.py
--rw-r--r--   0        0        0       72 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/js_choices_settings.py
--rw-r--r--   0        0        0        0 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/management/commands/__init__.py
--rw-r--r--   0        0        0     1013 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/management/commands/collectstatic_js_choices.py
--rw-r--r--   0        0        0        0 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/models.py
--rw-r--r--   0        0        0      983 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/templates/django_js_choices/choices_js.tpl
--rw-r--r--   0        0        0        0 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/templatetags/__init__.py
--rw-r--r--   0        0        0      517 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/templatetags/js_choices.py
--rw-r--r--   0        0        0      285 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/django_js_choices/views.py
--rw-r--r--   0        0        0     1191 2022-07-31 08:57:58.680410 django-js-choices-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7798 2022-07-31 08:58:47.621398 django-js-choices-0.4.0/setup.py
--rw-r--r--   0        0        0     7598 2022-07-31 08:58:47.621918 django-js-choices-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6600 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/README.rst
+-rw-r--r--   0        0        0        0 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/__init__.py
+-rw-r--r--   0        0        0     3624 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/core.py
+-rw-r--r--   0        0        0       72 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/js_choices_settings.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/management/commands/__init__.py
+-rw-r--r--   0        0        0     1013 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/management/commands/collectstatic_js_choices.py
+-rw-r--r--   0        0        0        0 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/models.py
+-rw-r--r--   0        0        0      983 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/templates/django_js_choices/choices_js.tpl
+-rw-r--r--   0        0        0        0 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/templatetags/__init__.py
+-rw-r--r--   0        0        0      517 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/templatetags/js_choices.py
+-rw-r--r--   0        0        0      285 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/django_js_choices/views.py
+-rw-r--r--   0        0        0     1187 2023-04-19 18:54:05.660472 django_js_choices-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7543 1970-01-01 00:00:00.000000 django_js_choices-0.5.0/PKG-INFO
```

### Comparing `django-js-choices-0.4.0/LICENSE` & `django_js_choices-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-js-choices-0.4.0/README.rst` & `django_js_choices-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-js-choices-0.4.0/django_js_choices/core.py` & `django_js_choices-0.5.0/django_js_choices/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 
 from django.apps import apps
 from django.conf import settings
 from django.template import loader
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 from django.utils.translation import activate, deactivate
 
 from . import js_choices_settings as default_settings
 
 
 def prepare_choices(choices):
     new_choices = []
     for choice in choices:
         if len(choice) != 2:
             continue
         try:
             json.dumps(choice[0])
-            new_choices.append((choice[0], force_text(choice[1])))
+            new_choices.append((choice[0], force_str(choice[1])))
         except TypeError:
-            new_choices.append((force_text(choice[0]), force_text(choice[1])))
+            new_choices.append((force_str(choice[0]), force_str(choice[1])))
     return new_choices
 
 
 class ExternalChoices:
     def __init__(self):
         self.choices = []
```

### Comparing `django-js-choices-0.4.0/django_js_choices/management/commands/collectstatic_js_choices.py` & `django_js_choices-0.5.0/django_js_choices/management/commands/collectstatic_js_choices.py`

 * *Files identical despite different names*

### Comparing `django-js-choices-0.4.0/django_js_choices/templates/django_js_choices/choices_js.tpl` & `django_js_choices-0.5.0/django_js_choices/templates/django_js_choices/choices_js.tpl`

 * *Files identical despite different names*

### Comparing `django-js-choices-0.4.0/django_js_choices/templatetags/js_choices.py` & `django_js_choices-0.5.0/django_js_choices/templatetags/js_choices.py`

 * *Files identical despite different names*

### Comparing `django-js-choices-0.4.0/pyproject.toml` & `django_js_choices-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "django-js-choices"
-version = "0.4.0"
+version = "0.5.0"
 description = "Javascript model field choices handling for Django."
 license = "MIT"
 authors = ["Lorenzo Peña <lorinkoz@gmail.com>"]
 readme = "README.rst"
 repository = "https://github.com/lorinkoz/django-js-choices"
 keywords = ["django", "choices", "javascript"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Django",
-    "Framework :: Django :: 2.2",
-    "Framework :: Django :: 3.1",
-    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
-django = ">=2.2,<=3.2,!=3.0"
+python = "^3.8.1"
+django = ">=4.0,<=4.2"
 rjsmin = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
-coverage = {extras = ["toml"], version = "^5.1"}
+black = "^23.3.0"
+coverage = {extras = ["toml"], version = "^6.3"}
 django-multiselectfield = "^0.1.12"
-dukpy = "^0.2.3"
-flake8 = "^3.8.4"
-flake8-bugbear = "^20.11.1"
-flake8-comprehensions = "^3.3.1"
-flake8-no-types = "^1.1.1"
-flake8-tidy-imports = "^4.2.1"
-isort = "^5.6.4"
+dukpy = "^0.3.0"
+flake8 = "^6.0.0"
+flake8-bugbear = "^23.3.23"
+flake8-comprehensions = "^3.12.0"
+flake8-no-types = "^1.5.1"
+flake8-tidy-imports = "^4.8.0"
+isort = "^5.12.0"
 dj-inmemorystorage = "^2.1.0"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 atomic = true
```

### Comparing `django-js-choices-0.4.0/PKG-INFO` & `django_js_choices-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: django-js-choices
-Version: 0.4.0
+Version: 0.5.0
 Summary: Javascript model field choices handling for Django.
 Home-page: https://github.com/lorinkoz/django-js-choices
 License: MIT
 Keywords: django,choices,javascript
 Author: Lorenzo Peña
 Author-email: lorinkoz@gmail.com
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: django (>=2.2,<=3.2,!=3.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django (>=4.0,<=4.2)
 Requires-Dist: rjsmin (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/lorinkoz/django-js-choices
 Description-Content-Type: text/x-rst
 
 django-js-choices
 =================
```

