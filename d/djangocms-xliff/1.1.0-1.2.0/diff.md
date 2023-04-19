# Comparing `tmp/djangocms_xliff-1.1.0.tar.gz` & `tmp/djangocms_xliff-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms_xliff-1.1.0.tar", max compression
+gzip compressed data, was "djangocms_xliff-1.2.0.tar", max compression
```

## Comparing `djangocms_xliff-1.1.0.tar` & `djangocms_xliff-1.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1073 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/LICENSE
--rw-r--r--   0        0        0     6356 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/README.md
--rw-r--r--   0        0        0       22 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/djangocms_xliff/__init__.py
--rw-r--r--   0        0        0      216 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/djangocms_xliff/apps.py
--rw-r--r--   0        0        0     1885 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/djangocms_xliff/cms_toolbars.py
--rw-r--r--   0        0        0      186 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/djangocms_xliff/exceptions.py
--rw-r--r--   0        0        0     1166 2023-04-06 11:16:57.480252 djangocms_xliff-1.1.0/djangocms_xliff/exports.py
--rw-r--r--   0        0        0     5792 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/extractors.py
--rw-r--r--   0        0        0      801 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/forms.py
--rw-r--r--   0        0        0     3596 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/imports.py
--rw-r--r--   0        0        0     4022 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5560 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/management/commands/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/management/commands/xliff_export.py
--rw-r--r--   0        0        0     1657 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/management/commands/xliff_import.py
--rw-r--r--   0        0        0     1515 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/management/commands/xliff_page_plugins.py
--rw-r--r--   0        0        0     3648 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/parsers.py
--rw-r--r--   0        0        0     1148 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/renderer.py
--rw-r--r--   0        0        0     1071 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/settings.py
--rw-r--r--   0        0        0      193 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/base.html
--rw-r--r--   0        0        0      151 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/error.html
--rw-r--r--   0        0        0      522 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/export/index.html
--rw-r--r--   0        0        0     1005 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
--rw-r--r--   0        0        0     1389 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html
--rw-r--r--   0        0        0     1116 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/import/success.html
--rw-r--r--   0        0        0      447 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/import/upload.html
--rw-r--r--   0        0        0     1769 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/types.py
--rw-r--r--   0        0        0      526 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/urls.py
--rw-r--r--   0        0        0     2437 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/utils.py
--rw-r--r--   0        0        0     6694 2023-04-06 11:16:57.484252 djangocms_xliff-1.1.0/djangocms_xliff/views.py
--rw-r--r--   0        0        0     1364 2023-04-06 11:16:57.488252 djangocms_xliff-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     7623 1970-01-01 00:00:00.000000 djangocms_xliff-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/LICENSE
+-rw-r--r--   0        0        0     7132 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/apps.py
+-rw-r--r--   0        0        0     2186 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/cms_toolbars.py
+-rw-r--r--   0        0        0      186 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/exceptions.py
+-rw-r--r--   0        0        0     1276 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/exports.py
+-rw-r--r--   0        0        0     7317 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/extractors.py
+-rw-r--r--   0        0        0      801 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/forms.py
+-rw-r--r--   0        0        0     3642 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/imports.py
+-rw-r--r--   0        0        0     4022 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5560 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/__init__.py
+-rw-r--r--   0        0        0     1804 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_export.py
+-rw-r--r--   0        0        0     1704 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_import.py
+-rw-r--r--   0        0        0     1623 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_page_plugins.py
+-rw-r--r--   0        0        0     5662 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/parsers.py
+-rw-r--r--   0        0        0     1148 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/renderer.py
+-rw-r--r--   0        0        0     1494 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/settings.py
+-rw-r--r--   0        0        0      193 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/base.html
+-rw-r--r--   0        0        0      151 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/error.html
+-rw-r--r--   0        0        0      522 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/index.html
+-rw-r--r--   0        0        0     1000 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/v1.2.xliff
+-rw-r--r--   0        0        0     1389 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html
+-rw-r--r--   0        0        0     1116 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/success.html
+-rw-r--r--   0        0        0      447 2023-04-19 12:17:15.943159 djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/upload.html
+-rw-r--r--   0        0        0     2152 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/types.py
+-rw-r--r--   0        0        0      589 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/urls.py
+-rw-r--r--   0        0        0     3652 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/utils.py
+-rw-r--r--   0        0        0     6931 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/djangocms_xliff/views.py
+-rw-r--r--   0        0        0     1364 2023-04-19 12:17:15.947160 djangocms_xliff-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8399 1970-01-01 00:00:00.000000 djangocms_xliff-1.2.0/PKG-INFO
```

### Comparing `djangocms_xliff-1.1.0/LICENSE` & `djangocms_xliff-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/README.md` & `djangocms_xliff-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -105,15 +105,16 @@
 
 ![Preview](docs/screenshots/preview.png)
 
 The translations are now imported, and you can publish the page.
 
 ## Settings
 
-By default, djangocms-xliff searches for the following django model fields: `CharField, TextField, URLField` in your
+By default, djangocms-xliff searches for the following django model fields: `CharField, SlugField, TextField, URLField`
+in your
 plugins.
 The texts from these fields will be used for the XLIFF import and export.
 
 If you want to add additional or 3rd party app fields, you can define the following settings in your `settings.py`,
 to integrate them into the XLIFF package:
 
 ```python
@@ -173,13 +174,42 @@
 
 # The signature of the validator function must be the following:
 def is_not_background(field: django.db.models.Field, instance: CMSPlugin) -> bool:
     # example:
     return field.name != "background"
 ```
 
+## Placeholders Outside the CMS
+
+Add a toolbar for your own Django model:
+
+```python
+from cms.toolbar_pool import toolbar_pool
+from djangocms_xliff.cms_toolbars import XliffModelToolbar
+
+from magazine.models import Article
+
+
+@toolbar_pool.register
+class ArticleXliffToolbar(XliffModelToolbar):
+    pass
+
+```
+
+This package does not handle translatability at database level. There are various packages for that. We recommend the
+use of django-modeltranslation. Because this way import and export of XLIFF works out-of-the-box.
+
+```python
+# By default all fields on a model get exported. You can exclude fields like this:
+DJANGOCMS_XLIFF_MODEL_METADATA_FIELDS = {
+    'magazine.models.Article': {
+        'exclude': ["slug", "og_title", "og_description"]
+    }
+}
+```
+
 ## Contribute
 
 Issues and pull requests are welcomed.
 
 You can find a documentation on how to set up your project
 in [here](docs/contribute.md)
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/exports.py` & `djangocms_xliff-1.2.0/djangocms_xliff/exports.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from cms.models import Page
+from django.contrib.contenttypes.models import ContentType
 
-from djangocms_xliff.extractors import extract_units_from_page
+from djangocms_xliff.extractors import extract_units_from_obj
 from djangocms_xliff.renderer import render_xliff_document
-from djangocms_xliff.types import ExportPage, XliffContext
+from djangocms_xliff.types import ExportPage, XliffContext, XliffObj
 from djangocms_xliff.utils import (
-    get_draft_page,
+    get_path,
     get_xliff_export_file_name,
     get_xliff_version,
 )
 
 
-def convert_page_to_xliff_context(page: Page, source_language: str, target_language: str) -> XliffContext:
+def convert_obj_to_xliff_context(obj: XliffObj, source_language: str, target_language: str) -> XliffContext:
+    content_type_id = ContentType.objects.get_for_model(obj).pk
     return XliffContext(
         source_language=source_language,
         target_language=target_language,
-        page_id=page.pk,
-        page_path=page.get_path(target_language),
-        units=extract_units_from_page(page, target_language),
+        content_type_id=content_type_id,
+        obj_id=obj.id,
+        path=get_path(obj=obj, language=target_language),
+        units=extract_units_from_obj(obj, target_language),
     )
 
 
-def export_page_as_xliff(
-    page_id: int,
+def export_content_as_xliff(
+    obj: XliffObj,
     source_language: str,
     target_language: str,
     version: str = "1.2",
 ) -> ExportPage:
     xliff_version = get_xliff_version(version)
-    page = get_draft_page(page_id)
-    context = convert_page_to_xliff_context(page, source_language, target_language)
+    context = convert_obj_to_xliff_context(obj, source_language, target_language)
     content = render_xliff_document(xliff_version, context)
-    file_name = get_xliff_export_file_name(page=page, target_language=target_language)
+    file_name = get_xliff_export_file_name(obj=obj, target_language=target_language)
     return content, file_name
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/extractors.py` & `djangocms_xliff-1.2.0/djangocms_xliff/extractors.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 import logging
 from functools import partial
-from typing import Generator, List
+from typing import Generator, List, Tuple, Type
 
-from cms.models import CMSPlugin, Page, Placeholder, StaticPlaceholder
-from django.db.models import CharField, Field, SlugField, TextField, URLField
+from cms.models import CMSPlugin, Page, Placeholder, PlaceholderField, StaticPlaceholder
+from django.db.models import (
+    CharField,
+    Field,
+    Model,
+    OneToOneField,
+    SlugField,
+    TextField,
+    URLField,
+)
+from django.utils import translation
 from django.utils.translation import gettext as _
 
 from djangocms_xliff.exceptions import XliffExportError
 from djangocms_xliff.settings import (
     FIELD_EXTRACTORS,
     FIELDS,
+    MODEL_METADATA_FIELDS,
+    TITLE_METADATA_FIELDS,
     UNIT_ID_METADATA_ID,
     VALIDATORS,
 )
-from djangocms_xliff.types import Unit
+from djangocms_xliff.types import Unit, XliffObj
 from djangocms_xliff.utils import get_type_with_path
 
 logger = logging.getLogger(__name__)
 
 
 def has_translatable_type(field: Field) -> bool:
     return type(field) in [CharField, TextField, URLField, SlugField, *FIELDS]
@@ -44,15 +55,15 @@
 def extract_units_from_plugin_instance(instance: CMSPlugin) -> List[Unit]:
     units = []
 
     for field in instance._meta.fields:
         if not is_field_to_translate(field, instance):
             continue
 
-        source = getattr(instance, field.name, None)
+        source = field.value_from_object(instance)
         if not source:
             continue
 
         field_type = type(field)
         if field_type in FIELD_EXTRACTORS:
             units.extend(FIELD_EXTRACTORS[field_type](instance=instance, field=field, source=source))
         else:
@@ -106,66 +117,98 @@
     for declared_placeholders_slot in declared_placeholders_slots:
         yield page.placeholders.get(slot=declared_placeholders_slot)
 
     for declared_static_placeholder in declared_static_placeholders:
         yield StaticPlaceholder.objects.get(code=declared_static_placeholder).draft
 
 
-def extract_page_metadata(page: Page, language: str) -> List[Unit]:
-    metadata_fields = {
-        "title": _("Title"),
-        "slug": _("Slug"),
-        "menu_title": _("Menu Title"),
-        "page_title": _("Page Title"),
-        "meta_description": _("Description meta tag"),
-    }
-
-    page_unit = partial(
-        Unit, plugin_id=UNIT_ID_METADATA_ID, plugin_type=UNIT_ID_METADATA_ID, plugin_name=UNIT_ID_METADATA_ID
-    )
+def get_model_placeholders(obj: Type[Model]):
+    placeholders = []
+    for field in obj._meta.fields:
+        field_type = type(field)
 
-    title = page.get_title_obj(language=language)
+        if field_type == PlaceholderField or (field_type == OneToOneField and field.related_model == StaticPlaceholder):
+            placeholder = getattr(obj, field.name)
+            if placeholder:
+                placeholders.append(placeholder.draft)
+    return placeholders
 
-    units = []
-    for metadata_field, metadata_field_description in metadata_fields.items():
-        title_field = title._meta.get_field(metadata_field)
 
-        if not is_field_to_translate(title_field, title):
-            continue
+def get_placeholders(obj: XliffObj):
+    if type(obj) == Page:
+        return get_declared_page_placeholders(obj)
+    else:
+        return get_model_placeholders(obj)
 
-        title_field_name = title_field.name
 
-        source = getattr(title, title_field_name, None)
-        if not source:
-            continue
+def get_metadata_fields(obj: XliffObj) -> Tuple[XliffObj, dict]:
+    obj_type = type(obj)
 
-        units.append(
-            page_unit(
-                field_name=title_field_name,
-                field_type=get_type_with_path(title_field),
-                field_verbose_name=metadata_field_description,
-                source=source,
-                max_length=title_field.max_length,
-            )
+    if obj_type == Page:
+        fields = TITLE_METADATA_FIELDS
+        target_obj = obj.get_title_obj()
+    else:
+        fields = {f.name: f.verbose_name for f in obj._meta.fields}
+        target_obj = obj
+
+    excluded_fields = MODEL_METADATA_FIELDS.get(obj_type, {}).get("exclude", [])
+    for excluded_field in excluded_fields:
+        fields.pop(excluded_field, None)
+
+    return target_obj, fields
+
+
+def extract_metadata_from_obj(obj: XliffObj, language: str) -> List[Unit]:
+    with translation.override(language):
+        target_obj, fields = get_metadata_fields(obj)
+
+        model_unit = partial(
+            Unit, plugin_id=UNIT_ID_METADATA_ID, plugin_type=UNIT_ID_METADATA_ID, plugin_name=UNIT_ID_METADATA_ID
         )
 
-    return units
+        units = []
+        for field_name, field_verbose_name in fields.items():
+            target_obj_field = target_obj._meta.get_field(field_name)
+
+            if not is_field_to_translate(target_obj_field, target_obj):
+                continue
+
+            source = target_obj_field.value_from_object(target_obj)
+            if not source:
+                continue
+
+            target_obj_field_type = type(target_obj_field)
+            if target_obj_field_type in FIELD_EXTRACTORS:
+                units.extend(
+                    FIELD_EXTRACTORS[target_obj_field_type](instance=target_obj, field=target_obj_field, source=source)
+                )
+            else:
+                units.append(
+                    model_unit(
+                        field_name=target_obj_field.name,
+                        field_type=get_type_with_path(target_obj_field),
+                        field_verbose_name=field_verbose_name,
+                        source=target_obj_field.value_from_object(target_obj),
+                        max_length=target_obj_field.max_length,
+                    )
+                )
+        return units
 
 
-def extract_units_from_page(page: Page, language: str, include_metadata: bool = True) -> List[Unit]:
+def extract_units_from_obj(obj: XliffObj, language: str, include_metadata=True) -> List[Unit]:
     plugin_units = []
 
-    for placeholder in get_declared_page_placeholders(page):
+    for placeholder in get_placeholders(obj):
         logger.debug(
             f"Placeholder: {placeholder.pk}, is_static={placeholder.is_static}, "
             f"is_editable={placeholder.is_editable}, label={placeholder.get_label()}"
         )
         plugin_units.extend(extract_units_from_placeholder(placeholder, language))
 
     if len(plugin_units) == 0:
         raise XliffExportError(_("No plugins found. You need to copy plugins from an existing page"))
 
-    page_units = []
+    metadata_units = []
     if include_metadata:
-        page_units.extend(extract_page_metadata(page, language))
+        metadata_units.extend(extract_metadata_from_obj(obj, language))
 
-    return [*page_units, *plugin_units]
+    return [*metadata_units, *plugin_units]
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/forms.py` & `djangocms_xliff-1.2.0/djangocms_xliff/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/imports.py` & `djangocms_xliff-1.2.0/djangocms_xliff/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import logging
 from typing import List
 
-from cms.models import CMSPlugin, Page, Title
+from cms.models import CMSPlugin, Page
+from django.utils import translation
 from django.utils.translation import gettext as _
 
 from djangocms_xliff.exceptions import XliffImportError
 from djangocms_xliff.settings import FIELD_IMPORTERS, UNIT_ID_METADATA_ID
-from djangocms_xliff.types import Unit, XliffContext
+from djangocms_xliff.types import Unit, XliffContext, XliffObj
 from djangocms_xliff.utils import get_lang_name
 
 logger = logging.getLogger(__name__)
 
 
-def save_xliff_units_for_page(units: List[Unit], target_title_obj: Title) -> None:
-    for unit in units:
-        field_name = unit.field_name
-        target = unit.target
+def save_xliff_units_for_metadata(units: List[Unit], obj: XliffObj, target_language: str) -> None:
+    with translation.override(target_language):
+        if type(obj) == Page:
+            obj = obj.get_title_obj()
+
+        for unit in units:
+            field_name = unit.field_name
+            target = unit.target
 
-        setattr(target_title_obj, field_name, target)
+            setattr(obj, field_name, target)
 
-    target_title_obj.save()
+        obj.save()
 
 
-def save_xliff_units_for_cms_plugins(units: List[Unit], plugin_id: str) -> None:
+def save_xliff_units_for_cms_plugin(units: List[Unit], plugin_id: str) -> None:
     try:
         cms_plugin = CMSPlugin.objects.get(pk=plugin_id)
     except CMSPlugin.DoesNotExist:
         logger.debug(f"Found plugin with id: {plugin_id} in xliff, but not in database")
         return
 
     instance, plugin = cms_plugin.get_plugin_instance()
@@ -40,33 +45,27 @@
         else:
             setattr(instance, field_name, target)
 
     instance.save()
 
 
 def save_xliff_context(xliff_context: XliffContext) -> None:
-    page = xliff_context.page
-    target_title_obj = page.get_title_obj(language=xliff_context.target_language)
-
     for plugin_id, units in xliff_context.grouped_units:
         if plugin_id == UNIT_ID_METADATA_ID:
-            save_xliff_units_for_page(units, target_title_obj)
+            save_xliff_units_for_metadata(units, xliff_context.obj, xliff_context.target_language)
         else:
-            save_xliff_units_for_cms_plugins(units, plugin_id)
+            save_xliff_units_for_cms_plugin(units, plugin_id)
 
 
-def validate_page_with_xliff_context(page: Page, xliff_context: XliffContext, current_language: str):
-    page_id = page.pk
-    xliff_page_id = xliff_context.page_id
-    if page_id != xliff_page_id:
-        error_message = _('Selected page id: "%(page_id)s" is not the same as xliff page id: "%(xliff_page_id)s"')
-        error_params = {
-            "page_id": page_id,
-            "xliff_page_id": xliff_page_id,
-        }
+def validate_page_with_xliff_context(obj: XliffObj, xliff_context: XliffContext, current_language: str):
+    obj_id = obj.id
+    xliff_obj_id = xliff_context.obj_id
+    if obj_id != xliff_obj_id:
+        error_message = _('Selected page id: "%(obj_id)s" is not the same as xliff page id: "%(xliff_obj_id)s"')
+        error_params = {"obj_id": obj_id, "xliff_obj_id": xliff_obj_id}
         raise XliffImportError(error_message % error_params)
 
     xliff_target_language = xliff_context.target_language
     if xliff_target_language != current_language:
         error_message = _(
             'Current page language: "%(page_language)s" is not the same as '
             'xliff target language: "%(xliff_target_language)s"'
@@ -90,10 +89,10 @@
                 "target": unit.target,
                 "max_length": unit.max_length,
                 "target_length": unit.target_length,
             }
             raise XliffImportError(error_message % error_params)
 
 
-def validate_xliff(page: Page, xliff_context: XliffContext, current_language: str) -> None:
+def validate_xliff(obj: XliffObj, xliff_context: XliffContext, current_language: str) -> None:
     validate_units_max_lengths(xliff_context.units)
-    validate_page_with_xliff_context(page, xliff_context, current_language)
+    validate_page_with_xliff_context(obj, xliff_context, current_language)
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo` & `djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po` & `djangocms_xliff-1.2.0/djangocms_xliff/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/management/commands/xliff_export.py` & `djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_export.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from pathlib import Path
 
 from django.conf import settings
 from django.core.management import BaseCommand, CommandError
 
 from djangocms_xliff.exceptions import XliffError
-from djangocms_xliff.exports import export_page_as_xliff
+from djangocms_xliff.exports import export_content_as_xliff
+from djangocms_xliff.utils import get_obj
 
 
 class Command(BaseCommand):
     def add_arguments(self, parser):
-        parser.add_argument("page_id", type=int)
+        parser.add_argument("content_type_id", type=int)
+        parser.add_argument("obj_id", type=int)
         parser.add_argument(
             "xliff_source_language",
             type=str,
             choices=[code for code, language in settings.LANGUAGES],
         )
         parser.add_argument(
             "target_language",
             type=str,
             choices=[code for code, language in settings.LANGUAGES],
         )
 
     def handle(self, *args, **options):
         try:
-            page_id = options["page_id"]
+            content_type_id = options["content_type_id"]
+            obj_id = options["obj_id"]
             xliff_source_language = options["xliff_source_language"]
             target_language = options["target_language"]
 
             if xliff_source_language == target_language:
                 raise CommandError("xliff source language and current language should not be the same")
 
-            xliff_str, file_name = export_page_as_xliff(
-                page_id=page_id,
+            obj = get_obj(content_type_id, obj_id)
+            xliff_str, file_name = export_content_as_xliff(
+                obj=obj,
                 source_language=xliff_source_language,
                 target_language=target_language,
             )
 
             exported_file = Path(file_name)
             with exported_file.open("w") as translation_file:
                 translation_file.write(xliff_str)
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/management/commands/xliff_import.py` & `djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,18 @@
                 )
                 if wants_to_continue == "y":
                     save_xliff_context(xliff_context)
 
                     self.stdout.write(
                         self.style.SUCCESS(
                             f"Successfully imported {len(xliff_context.units)} units for "
-                            f"page with id: {xliff_context.page_id} "
+                            f"obj with id: {xliff_context.obj_id}, content_type_id: {xliff_context.content_type_id} "
                             f"and language: {xliff_context.target_language}"
                         )
                     )
                     self.stdout.write(
-                        f"Path to page: {xliff_context.page.get_absolute_url(xliff_context.target_language)}"
+                        f"Path to page: {xliff_context.obj.get_absolute_url(xliff_context.target_language)}"
                     )
                 else:
                     raise CommandError("Aborted.")
         except XliffError as e:
             raise CommandError(e)
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/management/commands/xliff_page_plugins.py` & `djangocms_xliff-1.2.0/djangocms_xliff/management/commands/xliff_page_plugins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import pprint
 
 from django.conf import settings
 from django.core.management import BaseCommand, CommandError
 
 from djangocms_xliff.exceptions import XliffError
-from djangocms_xliff.extractors import extract_units_from_page
-from djangocms_xliff.utils import get_draft_page, group_units_by_plugin_id
+from djangocms_xliff.extractors import extract_units_from_obj
+from djangocms_xliff.utils import get_obj, group_units_by_plugin_id
 
 
 class Command(BaseCommand):
     def add_arguments(self, parser):
-        parser.add_argument("page_id", type=int)
+        parser.add_argument("content_type_id", type=int)
+        parser.add_argument("obj_id", type=int)
         parser.add_argument(
             "current_language",
             nargs="?",
             type=str,
             choices=[code for code, language in settings.LANGUAGES],
             default="de",
         )
 
     def handle(self, *args, **options):
         try:
-            page_id = options["page_id"]
+            content_type_id = options["content_type_id"]
+            obj_id = options["obj_id"]
             current_language = options["current_language"]
 
-            page = get_draft_page(page_id)
-            units = extract_units_from_page(page, current_language)
+            obj = get_obj(content_type_id, obj_id)
+            units = extract_units_from_obj(obj, current_language)
 
             self.stdout.write(
                 self.style.SUCCESS(
-                    f"Found {len(units)} xliff units on page with id: {page.pk} and language: {current_language}"
+                    f"Found {len(units)} xliff units on page with id: {obj.id} and language: {current_language}"
                 )
             )
             self.stdout.write()
 
             for plugin_id, units in group_units_by_plugin_id(units):
                 self.stdout.write(f"Plugin: {plugin_id}")
                 self.stdout.write()
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/parsers.py` & `djangocms_xliff-1.2.0/djangocms_xliff/parsers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,146 @@
+import abc
 from html import unescape
-from xml.etree.ElementTree import Element, ParseError
+from typing import Optional, Tuple, Union
+from xml.etree import ElementTree as ET
 
+from cms.models import Page
 from defusedxml.ElementTree import parse
+from django.contrib.contenttypes.models import ContentType
 from django.utils.translation import gettext as _
 
 from djangocms_xliff.exceptions import XliffConfigurationError, XliffError
 from djangocms_xliff.settings import UNIT_ID_DELIMITER, XliffVersion
 from djangocms_xliff.types import Unit, XliffContext
 from djangocms_xliff.utils import get_xliff_namespaces, get_xliff_version
 
 
-def _parse_xliff_units_version_1_2(xml_namespaces: dict, body_element: Element):
-    units = []
-    for trans_unit in body_element.findall("trans-unit", namespaces=xml_namespaces):
-        unit_id = trans_unit.attrib["id"]
-        plugin_id, field_name = unit_id.split(UNIT_ID_DELIMITER, 1)
-
-        field_type = trans_unit.attrib["extype"]
-
-        max_length = trans_unit.attrib.get("maxwidth")
-
-        source_element = trans_unit.find("source", namespaces=xml_namespaces)
-        if source_element is None:
-            raise XliffError("XLIFF Error: Missing <source> in <trans-unit>")
-
-        target_element = trans_unit.find("target", namespaces=xml_namespaces)
-        if target_element is None:
-            raise XliffError("XLIFF Error: Missing <target> in <trans-unit>")
-
-        source = unescape(source_element.text if source_element.text else "")
-        target = unescape(target_element.text if target_element.text else source)
-
-        notes = trans_unit.iterfind("note", namespaces=xml_namespaces)
-        plugin_type = next(notes).text
-        plugin_name = next(notes).text
-        field_verbose_name = next(notes).text
-
-        unit = Unit(
-            plugin_id=plugin_id,
-            plugin_type=plugin_type if plugin_type else "",
-            plugin_name=plugin_name if plugin_name else "",
-            field_name=field_name,
-            field_type=field_type,
-            field_verbose_name=field_verbose_name,
-            source=source,
-            target=target,
-            max_length=int(max_length) if max_length else None,
+class VersionParser(abc.ABC):
+    def __init__(self, xliff_element: ET.Element, xml_namespaces: dict):
+        self.xliff_element = xliff_element
+        self.xml_namespaces = xml_namespaces
+
+    @abc.abstractmethod
+    def parse(self) -> XliffContext:
+        raise NotImplementedError()
+
+
+class Version12(VersionParser):
+    def __init__(self, xliff_element: ET.Element, xml_namespaces: dict):
+        super().__init__(xliff_element, xml_namespaces)
+
+        file_element = xliff_element.find("file", namespaces=self.xml_namespaces)
+        if file_element is None:
+            raise XliffError("XLIFF Error: Missing file tag")
+
+        body_element = file_element.find("body", namespaces=self.xml_namespaces)
+        if body_element is None:
+            raise XliffError("XLIFF Error: Missing <body> in <file>")
+
+        self.file_element: ET.Element = file_element
+        self.body_element: ET.Element = body_element
+
+    def parse_file_element(self) -> Tuple[str, str, str]:
+        file_element = self.xliff_element.find("file", namespaces=self.xml_namespaces)
+        if file_element is None:
+            raise XliffError("XLIFF Error: Missing file tag")
+
+        source_language = file_element.attrib["source-language"]
+        target_language = file_element.attrib["target-language"]
+        path = file_element.attrib["original"]
+
+        tool_element = file_element.find("tool", namespaces=self.xml_namespaces)
+        if tool_element is None:
+            raise XliffError("XLIFF Error: Missing <tool> in <file>")
+
+        return source_language, target_language, path
+
+    def parse_tool_element(self) -> Tuple[int, int]:
+        tool_element = self.file_element.find("tool", namespaces=self.xml_namespaces)
+        if tool_element is None:
+            raise XliffError("XLIFF Error: Missing <tool> in <file>")
+
+        content_type_id: Union[str, int]
+        try:
+            content_type_id, obj_id = tool_element.attrib["tool-id"].split(UNIT_ID_DELIMITER)
+        except ValueError:
+            # For backwards compatibility, if there are existing xliff files
+            # with just the page_id as the tool-id
+            obj_id = tool_element.attrib["tool-id"]
+            content_type_id = ContentType.objects.get_for_model(Page).id
+
+        return int(content_type_id), int(obj_id)
+
+    def parse_body_element(self):
+        units = []
+        for trans_unit in self.body_element.findall("trans-unit", namespaces=self.xml_namespaces):
+            unit_id = trans_unit.attrib["id"]
+            plugin_id, field_name = unit_id.split(UNIT_ID_DELIMITER, 1)
+
+            field_type = trans_unit.attrib["extype"]
+
+            max_length = trans_unit.attrib.get("maxwidth")
+
+            source_element = trans_unit.find("source", namespaces=self.xml_namespaces)
+            if source_element is None:
+                raise XliffError("XLIFF Error: Missing <source> in <trans-unit>")
+
+            target_element = trans_unit.find("target", namespaces=self.xml_namespaces)
+            if target_element is None:
+                raise XliffError("XLIFF Error: Missing <target> in <trans-unit>")
+
+            source = unescape(source_element.text if source_element.text else "")
+            target = unescape(target_element.text if target_element.text else source)
+
+            notes = trans_unit.iterfind("note", namespaces=self.xml_namespaces)
+            plugin_type = next(notes).text
+            plugin_name = next(notes).text
+            field_verbose_name = next(notes).text
+
+            unit = Unit(
+                plugin_id=plugin_id,
+                plugin_type=plugin_type if plugin_type else "",
+                plugin_name=plugin_name if plugin_name else "",
+                field_name=field_name,
+                field_type=field_type,
+                field_verbose_name=field_verbose_name,
+                source=source,
+                target=target,
+                max_length=int(max_length) if max_length else None,
+            )
+            units.append(unit)
+        return units
+
+    def parse(self) -> XliffContext:
+        source_language, target_language, path = self.parse_file_element()
+        content_type_id, obj_id = self.parse_tool_element()
+        units = self.parse_body_element()
+
+        return XliffContext(
+            source_language=source_language,
+            target_language=target_language,
+            content_type_id=content_type_id,
+            obj_id=obj_id,
+            path=path,
+            units=units,
         )
-        units.append(unit)
-    return units
-
-
-def parse_xliff_version_1_2(version: XliffVersion, xliff_element: Element) -> XliffContext:
-    xml_namespaces = get_xliff_namespaces(version)
-
-    file_element = xliff_element.find("file", namespaces=xml_namespaces)
-    if file_element is None:
-        raise XliffError("XLIFF Error: Missing file tag")
-
-    source_language = file_element.attrib["source-language"]
-    target_language = file_element.attrib["target-language"]
-    page_path = file_element.attrib["original"]
-
-    tool_element = file_element.find("tool", namespaces=xml_namespaces)
-    if tool_element is None:
-        raise XliffError("XLIFF Error: Missing <tool> in <file>")
-
-    page_id = tool_element.attrib["tool-id"]
-
-    body_element = file_element.find("body", namespaces=xml_namespaces)
-    if body_element is None:
-        raise XliffError("XLIFF Error: Missing <body> in <file>")
-
-    units = _parse_xliff_units_version_1_2(xml_namespaces, body_element)
-
-    return XliffContext(
-        source_language=source_language,
-        target_language=target_language,
-        page_id=int(page_id),
-        page_path=page_path,
-        units=units,
-    )
 
 
 def parse_xliff_document(file) -> XliffContext:
     try:
         doc = parse(file)
-    except ParseError:
+    except ET.ParseError:
         raise XliffError(_("Invalid xml"))
 
     xliff_element = doc.getroot()
 
     found_version = get_xliff_version(xliff_element.attrib["version"])
+    xml_namespaces = get_xliff_namespaces(found_version)
 
+    parser: Optional[VersionParser] = None
     if found_version == XliffVersion.V1_2:
-        return parse_xliff_version_1_2(found_version, xliff_element)
+        parser = Version12(xliff_element, xml_namespaces)
+
+    if parser is None:
+        raise XliffConfigurationError(f"Missing VersionParser for version: {found_version.value}")
 
-    raise XliffConfigurationError(f"Missing parser function for version: {found_version.value}")
+    return parser.parse()
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/renderer.py` & `djangocms_xliff-1.2.0/djangocms_xliff/renderer.py`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/export/index.html` & `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/export/index.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html` & `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/preview.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/templates/djangocms_xliff/import/success.html` & `djangocms_xliff-1.2.0/djangocms_xliff/templates/djangocms_xliff/import/success.html`

 * *Files identical despite different names*

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/types.py` & `djangocms_xliff-1.2.0/djangocms_xliff/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from dataclasses import dataclass
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, TypeVar, Union
 
-from cms.models import Page
+from cms.models import Page, Title
+from django.db.models import Model
 from django.utils.translation import gettext as _
 
-from djangocms_xliff.settings import UNIT_ID_DELIMITER
-
 ExportContent = str
 ExportFileName = str
 ExportPage = Tuple[ExportContent, ExportFileName]
 
+DjangoModelType = TypeVar("DjangoModelType", bound=Model)
+XliffObj = Union[Page, Title, DjangoModelType]
+
 
 @dataclass
 class Unit:
     plugin_id: str
     plugin_type: str
     plugin_name: str
 
@@ -24,14 +26,16 @@
     target: str = ""
 
     field_verbose_name: Optional[str] = None
     max_length: Optional[int] = None
 
     @property
     def id(self):
+        from djangocms_xliff.settings import UNIT_ID_DELIMITER
+
         return f"{self.plugin_id}{UNIT_ID_DELIMITER}{self.field_name}"
 
     @property
     def notes(self) -> List[Optional[str]]:
         notes = [
             self.plugin_type,
             self.plugin_name,
@@ -53,22 +57,29 @@
         return self.target_length > self.max_length
 
 
 @dataclass
 class XliffContext:
     source_language: str
     target_language: str
-    page_id: int
-    page_path: str
+    content_type_id: int
+    obj_id: int
+    path: str
     units: List[Unit]
 
     @property
     def grouped_units(self) -> List[Tuple[str, List[Unit]]]:
         from djangocms_xliff.utils import group_units_by_plugin_id
 
         return group_units_by_plugin_id(self.units)
 
     @property
-    def page(self) -> Page:
-        from djangocms_xliff.utils import get_draft_page
+    def obj(self) -> XliffObj:
+        from djangocms_xliff.utils import get_obj
+
+        return get_obj(self.content_type_id, self.obj_id)
+
+    @property
+    def tool_id(self) -> str:
+        from djangocms_xliff.settings import UNIT_ID_DELIMITER
 
-        return get_draft_page(self.page_id)
+        return f"{self.content_type_id}{UNIT_ID_DELIMITER}{self.obj_id}"
```

### Comparing `djangocms_xliff-1.1.0/djangocms_xliff/views.py` & `djangocms_xliff-1.2.0/djangocms_xliff/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import json
 from dataclasses import asdict
 from typing import Type
 
-from cms.models import Page
 from django.contrib.admin import site
 from django.contrib.admin.views.decorators import staff_member_required
 from django.forms import Form
 from django.http import HttpResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.translation import gettext as _
 from django.views import View
 
 from djangocms_xliff.exceptions import XliffError
-from djangocms_xliff.exports import export_page_as_xliff
+from djangocms_xliff.exports import export_content_as_xliff
 from djangocms_xliff.forms import ExportForm, UploadFileForm
 from djangocms_xliff.imports import save_xliff_context, validate_xliff
 from djangocms_xliff.parsers import parse_xliff_document
 from djangocms_xliff.settings import (
     TEMPLATES_FOLDER,
     TEMPLATES_FOLDER_EXPORT,
     TEMPLATES_FOLDER_IMPORT,
 )
 from djangocms_xliff.types import Unit, XliffContext
-from djangocms_xliff.utils import get_draft_page, get_lang_name
+from djangocms_xliff.utils import get_lang_name, get_obj
 
 
 class XliffView(View):
     template: str
     form_class: Type[Form]
 
     def error_response(self, message):
@@ -40,26 +39,27 @@
 
 
 @method_decorator(staff_member_required, name="dispatch")
 class ExportView(XliffView):
     template = f"{TEMPLATES_FOLDER_EXPORT}/index.html"
     form_class: Type[ExportForm] = ExportForm
 
-    def get(self, request, page_id: int, current_language: str, *args, **kwargs):
+    def get(self, request, current_language: str, *args, **kwargs):
         form = self.form_class(current_language)
         return self.render_template(form, current_language)
 
-    def post(self, request, page_id: int, current_language: str, *args, **kwargs):
+    def post(self, request, content_type_id: int, obj_id: int, current_language: str, *args, **kwargs):
         form = self.form_class(current_language, request.POST)
         if not form.is_valid():
             return self.render_template(form, current_language)
 
+        obj = get_obj(content_type_id, obj_id)
         try:
-            xliff_str, file_name = export_page_as_xliff(
-                page_id=page_id,
+            xliff_str, file_name = export_content_as_xliff(
+                obj=obj,
                 source_language=form.cleaned_data["source_language"],
                 target_language=current_language,
             )
         except XliffError as e:
             return self.error_response(e)
 
         return HttpResponse(
@@ -95,29 +95,29 @@
 
 @method_decorator(staff_member_required, name="dispatch")
 class UploadView(XliffView):
     template = f"{TEMPLATES_FOLDER_IMPORT}/upload.html"
     template_success = f"{TEMPLATES_FOLDER_IMPORT}/preview.html"
     form_class: Type[UploadFileForm] = UploadFileForm
 
-    def get(self, request, page_id, current_language: str, *args, **kwargs):
+    def get(self, request, current_language: str, *args, **kwargs):
         form = self.form_class()
         return self.render_template(form, current_language)
 
-    def post(self, request, page_id, current_language, *args, **kwargs):
+    def post(self, request, content_type_id: int, obj_id: int, current_language: str, *args, **kwargs):
         form = self.form_class(request.POST, request.FILES)
         if not form.is_valid():
             return self.render_template(form, current_language)
 
         try:
             uploaded_file = form.cleaned_data["file"]
             xliff_context = parse_xliff_document(uploaded_file)
 
-            page = get_draft_page(page_id)
-            validate_xliff(page, xliff_context, current_language)
+            obj = get_obj(content_type_id, obj_id)
+            validate_xliff(obj, xliff_context, current_language)
 
             return self.render_template_success(uploaded_file.name, xliff_context)
         except XliffError as e:
             return self.error_response(e)
 
     def render_template(self, form: Form, current_language: str):
         lead_params = {"language": get_lang_name(current_language)}
@@ -146,31 +146,34 @@
 
         context = {
             "description": description,
             "note": note,
             "action_url": reverse(
                 "djangocms_xliff:import",
                 kwargs={
-                    "page_id": xliff_context.page_id,
+                    "content_type_id": xliff_context.content_type_id,
+                    "obj_id": xliff_context.obj_id,
                     "current_language": xliff_context.target_language,
                 },
             ),
             "xliff": xliff_context,
             "xliff_json": json.dumps(asdict(xliff_context)),
         }
         return render(self.request, self.template_success, context)
 
 
 @method_decorator(staff_member_required, name="dispatch")
 class ImportView(XliffView):
-    def post(self, request, page_id, current_language, *args, **kwargs):
+    def post(self, request, content_type_id: int, obj_id: int, *args, **kwargs):
         try:
             data = json.loads(request.POST["xliff_json"])
             units = data.pop("units", [])
 
             xliff_context = XliffContext(**data, units=[Unit(**u) for u in units])
             save_xliff_context(xliff_context)
 
-            admin = site._registry[Page]
-            return admin.response_change(request, xliff_context.page)
+            # Determine the HttpResponse for the change_view stage.
+            obj = get_obj(content_type_id, obj_id)
+            admin = site._registry[obj._meta.model]
+            return admin.response_change(request, obj)
         except XliffError as e:
             return self.error_response(e)
```

### Comparing `djangocms_xliff-1.1.0/pyproject.toml` & `djangocms_xliff-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms-xliff"
-version = "1.1.0"
+version = "1.2.0"
 description = "XLIFF Import and Export for the Django CMS"
 authors = ["Energie 360 <onlineservice@energie360.ch>"]
 maintainers = ["Energie 360 <onlineservice@energie360.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://energie360.ch"
 repository = "https://github.com/energie360/djangocms-xliff"
```

### Comparing `djangocms_xliff-1.1.0/PKG-INFO` & `djangocms_xliff-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-xliff
-Version: 1.1.0
+Version: 1.2.0
 Summary: XLIFF Import and Export for the Django CMS
 Home-page: https://energie360.ch
 License: MIT
 Keywords: django,django-cms,xliff,import,export
 Author: Energie 360
 Author-email: onlineservice@energie360.ch
 Maintainer: Energie 360
@@ -138,15 +138,16 @@
 
 ![Preview](docs/screenshots/preview.png)
 
 The translations are now imported, and you can publish the page.
 
 ## Settings
 
-By default, djangocms-xliff searches for the following django model fields: `CharField, TextField, URLField` in your
+By default, djangocms-xliff searches for the following django model fields: `CharField, SlugField, TextField, URLField`
+in your
 plugins.
 The texts from these fields will be used for the XLIFF import and export.
 
 If you want to add additional or 3rd party app fields, you can define the following settings in your `settings.py`,
 to integrate them into the XLIFF package:
 
 ```python
@@ -206,14 +207,43 @@
 
 # The signature of the validator function must be the following:
 def is_not_background(field: django.db.models.Field, instance: CMSPlugin) -> bool:
     # example:
     return field.name != "background"
 ```
 
+## Placeholders Outside the CMS
+
+Add a toolbar for your own Django model:
+
+```python
+from cms.toolbar_pool import toolbar_pool
+from djangocms_xliff.cms_toolbars import XliffModelToolbar
+
+from magazine.models import Article
+
+
+@toolbar_pool.register
+class ArticleXliffToolbar(XliffModelToolbar):
+    pass
+
+```
+
+This package does not handle translatability at database level. There are various packages for that. We recommend the
+use of django-modeltranslation. Because this way import and export of XLIFF works out-of-the-box.
+
+```python
+# By default all fields on a model get exported. You can exclude fields like this:
+DJANGOCMS_XLIFF_MODEL_METADATA_FIELDS = {
+    'magazine.models.Article': {
+        'exclude': ["slug", "og_title", "og_description"]
+    }
+}
+```
+
 ## Contribute
 
 Issues and pull requests are welcomed.
 
 You can find a documentation on how to set up your project
 in [here](docs/contribute.md)
```

