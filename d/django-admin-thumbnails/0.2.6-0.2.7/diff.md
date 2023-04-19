# Comparing `tmp/django-admin-thumbnails-0.2.6.tar.gz` & `tmp/django-admin-thumbnails-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-admin-thumbnails-0.2.6.tar", last modified: Thu Jun 17 14:09:08 2021, max compression
+gzip compressed data, was "dist/django-admin-thumbnails-0.2.7.tar", last modified: Wed Apr 19 12:00:30 2023, max compression
```

## Comparing `django-admin-thumbnails-0.2.6.tar` & `django-admin-thumbnails-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     8871 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/PKG-INFO
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8871 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-07 12:40:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/not-zip-safe
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      404 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       93 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       58 2019-04-07 10:23:12.000000 django-admin-thumbnails-0.2.6/MANIFEST.in
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/admin_thumbnails/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3483 2019-04-16 19:36:33.000000 django-admin-thumbnails-0.2.6/admin_thumbnails/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      248 2019-10-10 09:50:06.000000 django-admin-thumbnails-0.2.6/admin_thumbnails/utils.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1300 2019-04-16 19:16:08.000000 django-admin-thumbnails-0.2.6/admin_thumbnails/settings.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6387 2021-06-17 14:04:49.000000 django-admin-thumbnails-0.2.6/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2191 2021-06-17 13:58:13.000000 django-admin-thumbnails-0.2.6/setup.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       79 2021-06-17 14:09:08.000000 django-admin-thumbnails-0.2.6/setup.cfg
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10127 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/PKG-INFO
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    10127 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/PKG-INFO
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-07 12:40:08.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/not-zip-safe
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      404 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/SOURCES.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       93 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/requires.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       17 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/top_level.txt
+-rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       58 2019-04-07 10:23:12.000000 django-admin-thumbnails-0.2.7/MANIFEST.in
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4739 2023-04-19 11:27:10.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      248 2019-10-10 09:50:06.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1300 2019-04-16 19:16:08.000000 django-admin-thumbnails-0.2.7/admin_thumbnails/settings.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7443 2023-04-19 11:54:42.000000 django-admin-thumbnails-0.2.7/README.md
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2196 2023-04-19 11:58:42.000000 django-admin-thumbnails-0.2.7/setup.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       79 2023-04-19 12:00:31.000000 django-admin-thumbnails-0.2.7/setup.cfg
```

### Comparing `django-admin-thumbnails-0.2.6/PKG-INFO` & `django-admin-thumbnails-0.2.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-thumbnails
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Django app for DRY thumbnails in admin list views and forms.
 Home-page: http://github.com/BigglesZX/django-admin-thumbnails
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Description: # django-admin-thumbnails
         
@@ -14,31 +14,34 @@
         
         When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
         
         ## Compatibility
         
         I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
         
-        |                | Django 1.10   | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 |
-        |---------------:|:-------------:|:----:|:---:|:---:|:---:|:---:|:---:|:---:|
-        | **Python** 2.7 | ✔             | ✔    |     |     |     |     |     |     |
-        | 3.6            | ✔             | ✔    | ✔   | ✔   | ✔   | ✔   | ✔   | ✔   |
+        |                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
+        | -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
+        | **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
+        |            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
+        |         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
         
         ## Installation
         
         ```
         $ pip install django-admin-thumbnails
         ```
         
         ## Usage
         
         The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
         
         `django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
         
+        ### Basic usage
+        
         To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
         
         Assuming a model like the following:
         
         ```python
         class Person(models.Model):
             name = models.CharField('Name', max_length=100)
@@ -81,25 +84,47 @@
             fieldsets = (
                 (None, {
                     'fields': ('name', 'image_thumbnail'),
                 }),
             )
         ```
         
+        ### Using thumbnails in the list view only
+        
         By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
         
         ```python
         @admin.register(models.Person)
         @admin_thumbnails.thumbnail('image', append=False)
         class PersonAdmin(admin.ModelAdmin):
             list_display = ('name', 'image_thumbnail')
         ```
         
         This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
         
+        ### Using a property on the model as the thumbnail source
+        
+        As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
+        
+        ```python
+        class Person(models.Model):
+            # ...
+            @property
+            def primary_image(self):
+                if self.images.count():
+                    return self.images.first().image
+                return None
+        ```
+        
+        Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
+        
+        This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
+        
+        ### Adding a background to displayed thumbnails
+        
         If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
         
         ```python
         @admin_thumbnails.thumbnail('image', background=True)
         ```
         
         If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
@@ -136,29 +161,29 @@
         
         ### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
         
         **Default:** `{'background': '#000'}`
         
         A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
         
-        ## Development Installation
+        ## Development installation
         
         If working locally on the package you can install the development tools via `pip`:
         
         ```shell
         $ pip install -e .[dev]
         ```
         
         To lint with `flake8`:
         
         ```shell
         $ flake8
         ```
         
-        ## Issues, Suggestions, Contributions
+        ## Issues, suggestions, contributions
         
         ...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
         
 Keywords: django
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-admin-thumbnails-0.2.6/django_admin_thumbnails.egg-info/PKG-INFO` & `django-admin-thumbnails-0.2.7/django_admin_thumbnails.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-thumbnails
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Django app for DRY thumbnails in admin list views and forms.
 Home-page: http://github.com/BigglesZX/django-admin-thumbnails
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Description: # django-admin-thumbnails
         
@@ -14,31 +14,34 @@
         
         When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
         
         ## Compatibility
         
         I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
         
-        |                | Django 1.10   | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 |
-        |---------------:|:-------------:|:----:|:---:|:---:|:---:|:---:|:---:|:---:|
-        | **Python** 2.7 | ✔             | ✔    |     |     |     |     |     |     |
-        | 3.6            | ✔             | ✔    | ✔   | ✔   | ✔   | ✔   | ✔   | ✔   |
+        |                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
+        | -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
+        | **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
+        |            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
+        |         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
         
         ## Installation
         
         ```
         $ pip install django-admin-thumbnails
         ```
         
         ## Usage
         
         The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
         
         `django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
         
+        ### Basic usage
+        
         To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
         
         Assuming a model like the following:
         
         ```python
         class Person(models.Model):
             name = models.CharField('Name', max_length=100)
@@ -81,25 +84,47 @@
             fieldsets = (
                 (None, {
                     'fields': ('name', 'image_thumbnail'),
                 }),
             )
         ```
         
+        ### Using thumbnails in the list view only
+        
         By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
         
         ```python
         @admin.register(models.Person)
         @admin_thumbnails.thumbnail('image', append=False)
         class PersonAdmin(admin.ModelAdmin):
             list_display = ('name', 'image_thumbnail')
         ```
         
         This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
         
+        ### Using a property on the model as the thumbnail source
+        
+        As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
+        
+        ```python
+        class Person(models.Model):
+            # ...
+            @property
+            def primary_image(self):
+                if self.images.count():
+                    return self.images.first().image
+                return None
+        ```
+        
+        Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
+        
+        This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
+        
+        ### Adding a background to displayed thumbnails
+        
         If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
         
         ```python
         @admin_thumbnails.thumbnail('image', background=True)
         ```
         
         If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
@@ -136,29 +161,29 @@
         
         ### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
         
         **Default:** `{'background': '#000'}`
         
         A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
         
-        ## Development Installation
+        ## Development installation
         
         If working locally on the package you can install the development tools via `pip`:
         
         ```shell
         $ pip install -e .[dev]
         ```
         
         To lint with `flake8`:
         
         ```shell
         $ flake8
         ```
         
-        ## Issues, Suggestions, Contributions
+        ## Issues, suggestions, contributions
         
         ...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
         
 Keywords: django
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-admin-thumbnails-0.2.6/admin_thumbnails/__init__.py` & `django-admin-thumbnails-0.2.7/admin_thumbnails/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 from django.contrib.admin.options import BaseModelAdmin
 from django.db.models import FileField
+from django.db.models.fields.files import FieldFile
+from django.utils.functional import cached_property
 from django.utils.safestring import mark_safe
 
 from .settings import (ADMIN_THUMBNAIL_BACKGROUND_STYLE,
                        ADMIN_THUMBNAIL_DEFAULT_LABEL,
                        ADMIN_THUMBNAIL_FIELD_SUFFIX,
                        ADMIN_THUMBNAIL_STYLE,
                        ADMIN_THUMBNAIL_THUMBNAIL_ALIAS)
@@ -43,16 +45,35 @@
             raise ValueError(
                 'admin_thumbnails: Wrapped class must be a subclass of '
                 'django.contrib.admin.options.BaseModelAdmin'
             )
 
         ''' define the thumbnail field method using the above configuration '''
         def thumbnail_field(self, obj):
-            field = obj._meta.get_field(field_name)
-            field_value = getattr(obj, field_name)
+            if isinstance(getattr(type(obj), field_name, None), property) or isinstance(getattr(type(obj), field_name, None), cached_property):  # noqa: E501
+                ''' the supplied field_name is a property of the of model '''
+                value = getattr(obj, field_name)
+                if not isinstance(value, FieldFile):
+                    raise TypeError(
+                        'admin_thumbnails: Found a model property matching the'
+                        ' supplied field name, but it did not return an '
+                        'instance of `FieldFile` or a descendent. If using a '
+                        'property as the thumbnail source, it must return a '
+                        'value from a field that is an instance of Django’s '
+                        '`ImageField`, `FileField` or easy_thumbnails’ '
+                        '`ThumbnailerImageField` (received: {0})'.format(
+                            type(value))
+                    )
+                field = value.field
+                field_value = value
+            else:
+                ''' default: access field_name as a field on the model '''
+                field = obj._meta.get_field(field_name)
+                field_value = getattr(obj, field_name)
+
             if not field_value:
                 return ''
 
             ''' determine the image url based on the field type - in the case
                 of `ThumbnailerImageField` instances, check the alias given
                 against the list of available aliases from `easy_thumbnails`
             '''
```

### Comparing `django-admin-thumbnails-0.2.6/admin_thumbnails/settings.py` & `django-admin-thumbnails-0.2.7/admin_thumbnails/settings.py`

 * *Files identical despite different names*

### Comparing `django-admin-thumbnails-0.2.6/README.md` & `django-admin-thumbnails-0.2.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,31 +6,34 @@
 
 When working with models that include `ImageField`s, `FileField`s or when using `ThumbnailerImageField` from `easy_thumbnails`, it can often be desirable to include a thumbnail preview of the field as part of the admin form, fieldset or in list views. Various methods to achieve this exist but all seem to involve a degree of duplication. I've made a few attempts to DRY out such code over the years and this library represents my most recent solution. So, please enjoy!
 
 ## Compatibility
 
 I've not exhaustively tested all the below combinations, however I believe this table to be accurate.
 
-|                | Django 1.10   | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 |
-|---------------:|:-------------:|:----:|:---:|:---:|:---:|:---:|:---:|:---:|
-| **Python** 2.7 | ✔             | ✔    |     |     |     |     |     |     |
-| 3.6            | ✔             | ✔    | ✔   | ✔   | ✔   | ✔   | ✔   | ✔   |
+|                | Django 1.10 | 1.11 | 2.0 | 2.1 | 2.2 | 3.0 | 3.1 | 3.2 | 4.0 | 4.1 | 4.2 |
+| -------------: | :---------: | :--: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
+| **Python** 2.7 |      ✔      |  ✔   |     |     |     |     |     |     |     |     |     |
+|            3.6 |      ✔      |  ✔   |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |     |     |     |
+|         >= 3.8 |             |      |     |     |     |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |  ✔  |
 
 ## Installation
 
 ```
 $ pip install django-admin-thumbnails
 ```
 
 ## Usage
 
 The app adds fields to your `ModelAdmin` or `*Inline` class; one for each thumbnail you want to display. These are appended to the class's `readonly_fields` tuple (unless you specify otherwise) so they will be displayed at the bottom of your admin form, or you can include them by name in your `fieldsets` or `list_display` definitions.
 
 `django-admin-thumbnails` will handle `ImageField`, `FileField` (so you can use SVG, for example) and (if `easy_thumbnails` is installed) `ThumbnailerImageField`. In the latter case a thumbnail alias will be used, which you can specify in settings.
 
+### Basic usage
+
 To create an admin thumbnail field, decorate your `ModelAdmin` or `*Inline` class and optionally specify what to do with the newly created field.
 
 Assuming a model like the following:
 
 ```python
 class Person(models.Model):
     name = models.CharField('Name', max_length=100)
@@ -73,25 +76,47 @@
     fieldsets = (
         (None, {
             'fields': ('name', 'image_thumbnail'),
         }),
     )
 ```
 
+### Using thumbnails in the list view only
+
 By default the new field will be appended to the `readonly_fields` tuple – if this is undesirable (e.g. if you want to include the thumbnail in the list view but _not_ in the default form fields), pass `append=False` to the decorator:
 
 ```python
 @admin.register(models.Person)
 @admin_thumbnails.thumbnail('image', append=False)
 class PersonAdmin(admin.ModelAdmin):
     list_display = ('name', 'image_thumbnail')
 ```
 
 This isn't necessary if you're using `fieldsets`, as by doing so you will control the inclusion (or omission) and position of the thumbnail field.
 
+### Using a property on the model as the thumbnail source
+
+As of version 0.2.7, the name passed to the `thumbnail` decorator can refer to a property on the model rather than a field. For example:
+
+```python
+class Person(models.Model):
+    # ...
+    @property
+    def primary_image(self):
+        if self.images.count():
+            return self.images.first().image
+        return None
+```
+
+Provided the specified property returns an instance of a `FieldFile` (i.e. a file stored in a field that is an instance of Django's `ImageField`, `FileField`, or `easy_thumbnails`' `ThumbnailerImageField`), this will work as normal.
+
+This also works with Django's [`cached_property`](https://docs.djangoproject.com/en/dev/ref/utils/#django.utils.functional.cached_property) decorator.
+
+### Adding a background to displayed thumbnails
+
 If your field contains images that are designed to be shown on a dark background, you can supply `background=True` to the decorator to add one to the thumbnail (via CSS) when displayed:
 
 ```python
 @admin_thumbnails.thumbnail('image', background=True)
 ```
 
 If you're using `easy_thumbnails` and want to override the alias used to generate your thumbnail on a per-field basis (as opposed to using the `ADMIN_THUMBNAIL_THUMBNAIL_ALIAS` setting; see below), you can use the `alias` argument to the decorator:
@@ -128,24 +153,24 @@
 
 ### `ADMIN_THUMBNAIL_BACKGROUND_STYLE`
 
 **Default:** `{'background': '#000'}`
 
 A dictionary of CSS property/value pairs added when the `background=True` option is used (see **Usage** above). Override to supply your own styles. Note that these styles are used _in addition_ to any defined in `ADMIN_THUMBNAIL_STYLE`.
 
-## Development Installation
+## Development installation
 
 If working locally on the package you can install the development tools via `pip`:
 
 ```shell
 $ pip install -e .[dev]
 ```
 
 To lint with `flake8`:
 
 ```shell
 $ flake8
 ```
 
-## Issues, Suggestions, Contributions
+## Issues, suggestions, contributions
 
 ...are welcome on GitHub. Thanks for your interest in `django-admin-thumbnails`!
```

### Comparing `django-admin-thumbnails-0.2.6/setup.py` & `django-admin-thumbnails-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python
 
 ''' XXX: allow dist building on vagrant
     source: http://bugs.python.org/issue8876
+'''
+import os
+del os.link
+
+from setuptools import setup, find_packages  # noqa: E402
+
+
+''' To make a new release:
 
-    To make a new release:
     1. Bump version number in setup.py
     2. Update CHANGELOG
     3. $ git commit ...
     4. $ git tag -a x.x.x  # see `git tags` for latest
     5. $ git push origin master
     6. $ git push --tags
     7. $ python setup.py register sdist
     8. $ twine upload dist/*
 '''
-import os
-del os.link
-
-from setuptools import setup, find_packages  # noqa: E402
-
 
-VERSION = '.'.join(('0', '2', '6'))
+VERSION = '.'.join(('0', '2', '7'))
 
 DESCRIPTION = 'A Django app for DRY thumbnails in admin list views and forms.'
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
```

