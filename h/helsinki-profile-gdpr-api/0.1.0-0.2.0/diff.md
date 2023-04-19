# Comparing `tmp/helsinki-profile-gdpr-api-0.1.0.tar.gz` & `tmp/helsinki-profile-gdpr-api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helsinki-profile-gdpr-api-0.1.0.tar", last modified: Mon Mar 15 11:08:01 2021, max compression
+gzip compressed data, was "helsinki-profile-gdpr-api-0.2.0.tar", last modified: Wed Apr 19 06:07:25 2023, max compression
```

## Comparing `helsinki-profile-gdpr-api-0.1.0.tar` & `helsinki-profile-gdpr-api-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 11:08:01.125474 helsinki-profile-gdpr-api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2021-03-15 11:08:01.125474 helsinki-profile-gdpr-api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1746 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 11:08:01.125474 helsinki-profile-gdpr-api-0.1.0/helsinki_gdpr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_gdpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4214 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_gdpr/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_gdpr/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3554 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_gdpr/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-15 11:08:01.125474 helsinki-profile-gdpr-api-0.1.0/helsinki_profile_gdpr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2021-03-15 11:08:01.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_profile_gdpr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      402 2021-03-15 11:08:01.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_profile_gdpr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-15 11:08:01.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_profile_gdpr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-03-15 11:08:01.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_profile_gdpr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-03-15 11:08:01.000000 helsinki-profile-gdpr-api-0.1.0/helsinki_profile_gdpr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-03-15 11:08:01.125474 helsinki-profile-gdpr-api-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-15 11:07:51.000000 helsinki-profile-gdpr-api-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:07:25.065729 helsinki-profile-gdpr-api-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-19 06:07:25.065729 helsinki-profile-gdpr-api-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:07:25.065729 helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:07:25.065729 helsinki-profile-gdpr-api-0.2.0/helsinki_profile_gdpr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-19 06:07:25.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_profile_gdpr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 06:07:25.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_profile_gdpr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:07:25.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_profile_gdpr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 06:07:25.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_profile_gdpr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 06:07:25.000000 helsinki-profile-gdpr-api-0.2.0/helsinki_profile_gdpr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-19 06:07:25.065729 helsinki-profile-gdpr-api-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:07:25.065729 helsinki-profile-gdpr-api-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/tests/test_gdpr_api_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/tests/test_gdpr_api_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 06:07:15.000000 helsinki-profile-gdpr-api-0.2.0/tests/test_models.py
```

### Comparing `helsinki-profile-gdpr-api-0.1.0/LICENSE` & `helsinki-profile-gdpr-api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helsinki-profile-gdpr-api-0.1.0/helsinki_gdpr/models.py` & `helsinki-profile-gdpr-api-0.2.0/helsinki_gdpr/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,49 +71,61 @@
             ]
 
     class Meta:
         abstract = True
 
     objects = SerializableManager()
 
-    def _resolve_field(self, model, field):
-        def _resolve_value(data, field):
-            if "accessor" in field:
+    def _resolve_field(self, model, field_description):
+        field_name = field_description.get("name")
+
+        def _resolve_value():
+            value = getattr(model, field_name)
+
+            if "accessor" in field_description:
                 # call the accessor with value as an argument
-                return field["accessor"](getattr(data, field.get("name")))
-            else:
-                # no accessor, return the value
-                return getattr(data, field.get("name"))
+                value = field_description["accessor"](value)
+
+            return value
 
         related_types = {item.name: type(item) for item in model._meta.related_objects}
-        if field.get("name") in related_types.keys():
+        if field_name in related_types.keys():
             value = (
-                getattr(model, field.get("name")).serialize()
-                if hasattr(model, field.get("name"))
-                and hasattr(getattr(model, field.get("name")), "serialize")
+                getattr(model, field_name).serialize()
+                if hasattr(model, field_name)
+                and hasattr(getattr(model, field_name), "serialize")
                 else None
             )
             # field is a related object, let's serialize more
-            if related_types[field.get("name")] == OneToOneRel:
+            if related_types[field_name] == OneToOneRel:
                 # do not wrap one-to-one relations into list
                 return value
             else:
                 return {
-                    "key": field.get("name").upper(),
+                    "key": field_name.upper(),
                     "children": value,
                 }
         else:
-            # concrete field, let's just add the value
+            # concrete field
+            value = _resolve_value()
+
+            if hasattr(value, "serialize"):
+                return value.serialize()
+
             return {
-                "key": field.get("name").upper(),
-                "value": _resolve_value(model, field),
+                "key": field_name.upper(),
+                "value": value,
             }
 
     def serialize(self):
         return {
             "key": self._meta.model_name.upper(),
-            "children": [
-                self._resolve_field(self, field)
-                for field in self.serialize_fields
-                if self._resolve_field(self, field) is not None
-            ],
+            "children": list(
+                filter(
+                    lambda x: x is not None,
+                    [
+                        self._resolve_field(self, field_description)
+                        for field_description in self.serialize_fields
+                    ],
+                )
+            ),
         }
```

### Comparing `helsinki-profile-gdpr-api-0.1.0/setup.cfg` & `helsinki-profile-gdpr-api-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = helsinki-profile-gdpr-api
-version = 0.1.0
+version = 0.2.0
 author = City of Helsinki
 author_email = dev@hel.fi
 description = Django app for implementing Helsinki profile GDPR API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/City-of-Helsinki/helsinki-profile-gdpr-api
@@ -15,31 +15,30 @@
 	Framework :: Django
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 include_package_data = True
 install_requires = 
 	Django
 	djangorestframework
 	django-helusers
-	drf-oidc-auth<1.0.0
+	drf-oidc-auth
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
 
 [pep8]
@@ -49,15 +48,16 @@
 
 [flake8]
 max-line-length = 120
 exclude = *migrations*
 max-complexity = 10
 
 [tool:pytest]
-django_settings_module = tests.settings
+pythonpath = .
+DJANGO_SETTINGS_MODULE = tests.settings
 norecursedirs = .git .idea venv*
 doctest_optionflags = NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL ALLOW_UNICODE
 
 [coverage:run]
 branch = True
 omit = *migrations*,*site-packages*,*venv*,*tests*
```

