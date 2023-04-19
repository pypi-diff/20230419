# Comparing `tmp/reportbro_lib-3.0.5.tar.gz` & `tmp/reportbro_lib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportbro_lib-3.0.5.tar", max compression
+gzip compressed data, was "reportbro_lib-3.1.0.tar", max compression
```

## Comparing `reportbro_lib-3.0.5.tar` & `reportbro_lib-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0    34520 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/LICENSE
--rw-r--r--   0        0        0     1805 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/README.rst
--rw-r--r--   0        0        0     1327 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/pyproject.toml
--rw-r--r--   0        0        0      122 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/__init__.py
--rw-r--r--   0        0        0     7046 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/barcode128.py
--rw-r--r--   0        0        0    10728 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/containers.py
--rw-r--r--   0        0        0    15158 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/context.py
--rw-r--r--   0        0        0        0 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/data/__init__.py
--rw-r--r--   0        0        0    10193 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/data/logo_watermark.png
--rw-r--r--   0        0        0     5928 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/docelement.py
--rw-r--r--   0        0        0    80444 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/elements.py
--rw-r--r--   0        0        0     1143 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/enums.py
--rw-r--r--   0        0        0      698 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/errors.py
--rw-r--r--   0        0        0    13346 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/rendering.py
--rw-r--r--   0        0        0    45714 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/reportbro.py
--rw-r--r--   0        0        0     7085 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/structs.py
--rw-r--r--   0        0        0     1515 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/utils.py
--rw-r--r--   0        0        0       22 2022-12-30 11:03:41.945384 reportbro_lib-3.0.5/reportbro/version.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 reportbro_lib-3.0.5/setup.py
--rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 reportbro_lib-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1805 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/README.rst
+-rw-r--r--   0        0        0     1327 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/__init__.py
+-rw-r--r--   0        0        0     7046 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/barcode128.py
+-rw-r--r--   0        0        0    10728 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/containers.py
+-rw-r--r--   0        0        0    15158 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/context.py
+-rw-r--r--   0        0        0        0 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/data/__init__.py
+-rw-r--r--   0        0        0    10193 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/data/logo_watermark.png
+-rw-r--r--   0        0        0     5928 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/docelement.py
+-rw-r--r--   0        0        0    80968 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/elements.py
+-rw-r--r--   0        0        0     1143 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/enums.py
+-rw-r--r--   0        0        0      698 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/errors.py
+-rw-r--r--   0        0        0    13346 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/rendering.py
+-rw-r--r--   0        0        0    46361 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/reportbro.py
+-rw-r--r--   0        0        0     7085 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/structs.py
+-rw-r--r--   0        0        0     1515 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/utils.py
+-rw-r--r--   0        0        0       22 2023-04-19 09:20:51.618879 reportbro_lib-3.1.0/reportbro/version.py
+-rw-r--r--   0        0        0     3367 1970-01-01 00:00:00.000000 reportbro_lib-3.1.0/PKG-INFO
```

### Comparing `reportbro_lib-3.0.5/LICENSE` & `reportbro_lib-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/README.rst` & `reportbro_lib-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/pyproject.toml` & `reportbro_lib-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reportbro-lib"
-version = "3.0.5"
+version = "3.1.0"
 description = "Generate PDF and Excel reports from visually designed templates"
 authors = ["jobsta <alex@reportbro.com>"]
 license = "AGPL-3.0"
 readme = "README.rst"
 
 homepage = "https://www.reportbro.com"
 repository = "https://github.com/jobsta/reportbro-lib"
```

### Comparing `reportbro_lib-3.0.5/reportbro/barcode128.py` & `reportbro_lib-3.1.0/reportbro/barcode128.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/containers.py` & `reportbro_lib-3.1.0/reportbro/containers.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/context.py` & `reportbro_lib-3.1.0/reportbro/context.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/data/logo_watermark.png` & `reportbro_lib-3.1.0/reportbro/data/logo_watermark.png`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/docelement.py` & `reportbro_lib-3.1.0/reportbro/docelement.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/elements.py` & `reportbro_lib-3.1.0/reportbro/elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -937,25 +937,25 @@
                         content_row.set_parameter_range(parameter=self.data_source_parameter, ctx=ctx, clear=True)
 
                         render_element.add_band(content_row, row_index=self.row_index)
                         if not content_row.rendering_complete:
                             ctx.pop_context()
                             return render_element, False
 
+                        content_row.postprocess(row_index=self.row_index)
+
                         # only perform page break after content if this is not the last row
                         if content_row.page_break and not content_row.before_group and\
                                 self.row_index < (self.row_count - 1):
                             self.content_row_index += 1
                             ctx.pop_context()
                             return render_element, False
                     else:
                         content_row.rendering_complete = True
 
-                content_row.update_group_changed_row_indices()
-
                 self.content_row_index += 1
             ctx.pop_context()
 
             self.row_index += 1
             first_row_on_page = False
 
         if self.row_index >= self.row_count and self.print_footer:
@@ -1041,14 +1041,16 @@
                 content_row.prepare(ctx=ctx, row_index=self.row_index)
                 if content_row.is_printed(ctx=ctx):
                     if columns == 0:
                         # get column count from first printed content row if there is no header
                         columns = len(content_row.printed_cells)
                     row, _ = content_row.render_spreadsheet(
                         row, col, ctx, renderer, row_index=self.row_index)
+                    content_row.postprocess(row_index=self.row_index)
+
             ctx.pop_context()
             self.row_index += 1
 
         if self.footer:
             row, _ = self.footer.render_spreadsheet(row, col, ctx, renderer)
 
         if self.spreadsheet_add_empty_row:
@@ -1173,24 +1175,14 @@
             if self.before_group:
                 if self.group_expr_result != self.prev_group_expr_result:
                     self.group_changed_row_indices.append(row_index)
             else:
                 if self.group_expr_result != self.next_group_expr_result:
                     self.group_changed_row_indices.append(row_index)
 
-    def update_group_changed_row_indices(self):
-        """
-        The internal array of changed row indices for groups is updated in
-        case a group row was currently rendered.
-
-        Must be called after the row was processed.
-        """
-        if self.rendering_complete and self.group_changed:
-            self.group_changed_row_indices.pop(0)
-
     def prepare(self, ctx, row_index=None):
         if self.group_expression:
             self.group_changed = False
             if self.group_changed_row_indices and self.group_changed_row_indices[0] == row_index:
                 # the group expression has changed for this row index -> group band will be printed
                 self.group_changed = True
                 # now set index range which is used for function parameters like sum/avg
@@ -1204,14 +1196,26 @@
                     self.group_row_index_start = self.group_row_index_end
                     self.group_row_index_end = self.group_changed_row_indices[0] + 1
 
         if self.print_if:
             self.print_if_result = ctx.evaluate_expression(
                 self.print_if, self.id, field='printIf')
 
+    def postprocess(self, row_index):
+        """
+        Must be called after a row was processed for this band.
+
+        The internal array of changed row indices for groups is updated in
+        case a group row was currently rendered.
+
+        :param row_index: current row index when the band was processed.
+        """
+        if self.group_changed_row_indices and self.group_changed_row_indices[0] == row_index:
+            self.group_changed_row_indices.pop(0)
+
     def set_parameter_range(self, parameter, ctx, clear=False):
         """
         Set start and end row index for the given parameter which is used when evaluating a parameter
         function (e.g. sum or avg).
 
         :param parameter: data source parameter of table
         :param ctx: current context
@@ -1321,14 +1325,15 @@
         DocElement.__init__(self, report, data)
         from .containers import Frame
         self.background_color = Color(data.get('backgroundColor'))
         self.border_style = BorderStyle(data)
         self.print_if = get_str_value(data, 'printIf')
         self.remove_empty_element = bool(data.get('removeEmptyElement'))
         self.shrink_to_content_height = bool(data.get('shrinkToContentHeight'))
+        self.align_to_page_bottom = bool(data.get('alignToPageBottom'))
         self.spreadsheet_hide = bool(data.get('spreadsheet_hide'))
         self.spreadsheet_column = get_int_value(data, 'spreadsheet_column')
         self.spreadsheet_add_empty_row = bool(data.get('spreadsheet_addEmptyRow'))
 
         # rendering_complete status for next page, in case rendering was not started on first page.
         self.next_page_rendering_complete = False
         # container content height of previous page, in case rendering was not started on first page
@@ -1376,14 +1381,19 @@
                 container_top + offset_y, content_height, ctx, pdf_doc)
 
             needed_height = self.get_render_bottom()
 
             if rendering_complete and needed_height <= available_height:
                 # rendering is complete and all elements of frame fit on current page
                 self.rendering_complete = True
+                if self.align_to_page_bottom:
+                    spacer = available_height - needed_height
+                    render_element.render_y += spacer
+                    self.render_y += spacer
+                    needed_height = available_height
                 self.render_bottom = offset_y + needed_height
                 self.render_element_type = RenderElementType.complete
                 render_element.add_elements(self.container, self.render_element_type, needed_height)
                 return render_element, True
             else:
                 if offset_y == 0:
                     # rendering of frame elements does not fit on current page but
```

### Comparing `reportbro_lib-3.0.5/reportbro/enums.py` & `reportbro_lib-3.1.0/reportbro/enums.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/errors.py` & `reportbro_lib-3.1.0/reportbro/errors.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/rendering.py` & `reportbro_lib-3.1.0/reportbro/rendering.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/reportbro.py` & `reportbro_lib-3.1.0/reportbro/reportbro.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 import base64
 import fpdf
 import importlib.resources
 import re
 import os
 import xlsxwriter
+from copy import deepcopy
+from babel import Locale
 from io import BufferedReader, IOBase
 
 from .containers import ReportBand
 from .elements import *
 from .enums import *
 from .errors import Error, ReportBroError, ReportBroInternalError
 from .structs import Parameter, TextStyle
@@ -258,14 +260,23 @@
         self.margin_top = get_int_value(data, 'marginTop')
         self.margin_right = get_int_value(data, 'marginRight')
         self.margin_bottom = get_int_value(data, 'marginBottom')
         self.pattern_locale = data.get('patternLocale', '')
         self.pattern_currency_symbol = data.get('patternCurrencySymbol', '')
         if self.pattern_locale not in ('de', 'en', 'es', 'fr', 'it'):
             raise ReportBroInternalError('invalid pattern_locale', log_error=False)
+        self.pattern_number_group_symbol = data.get('patternNumberGroupSymbol', '')
+        if self.pattern_number_group_symbol and len(self.pattern_number_group_symbol) > 1:
+            raise ReportBroInternalError('invalid pattern_number_group_symbol', log_error=False)
+
+        if self.pattern_number_group_symbol:
+            rbro_locale = Locale(self.pattern_locale)
+            rbro_locale.number_symbols  # ensure instance has been populated
+            self.pattern_locale = deepcopy(rbro_locale)
+            self.pattern_locale.number_symbols['group'] = self.pattern_number_group_symbol
 
         self.header = bool(data.get('header'))
         if self.header:
             self.header_display = BandDisplay[data.get('headerDisplay')]
             self.header_size = get_int_value(data, 'headerSize')
         else:
             self.header_display = BandDisplay.never
```

### Comparing `reportbro_lib-3.0.5/reportbro/structs.py` & `reportbro_lib-3.1.0/reportbro/structs.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/reportbro/utils.py` & `reportbro_lib-3.1.0/reportbro/utils.py`

 * *Files identical despite different names*

### Comparing `reportbro_lib-3.0.5/PKG-INFO` & `reportbro_lib-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reportbro-lib
-Version: 3.0.5
+Version: 3.1.0
 Summary: Generate PDF and Excel reports from visually designed templates
 Home-page: https://www.reportbro.com
 License: AGPL-3.0
 Keywords: pdf,excel,report,generate,create,web,template,layout
 Author: jobsta
 Author-email: alex@reportbro.com
 Requires-Python: >=3.7,<4.0
```

