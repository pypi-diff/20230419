# Comparing `tmp/excelcolumnizer-0.0.6.tar.gz` & `tmp/excelcolumnizer-0.0.7.tar.gz`

## Comparing `excelcolumnizer-0.0.6.tar` & `excelcolumnizer-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/updatePackage.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/src/excelcolumnizer/__init__.py
--rw-r--r--   0        0        0    11929 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/src/excelcolumnizer/_excelColumnizer.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/updatePackage.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/src/excelcolumnizer/__init__.py
+-rw-r--r--   0        0        0    11929 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/src/excelcolumnizer/_excelColumnizer.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.7/PKG-INFO
```

### Comparing `excelcolumnizer-0.0.6/updatePackage.txt` & `excelcolumnizer-0.0.7/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.6/src/excelcolumnizer/_excelColumnizer.py` & `excelcolumnizer-0.0.7/src/excelcolumnizer/_excelColumnizer.py`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.6/LICENSE.txt` & `excelcolumnizer-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.6/README.md` & `excelcolumnizer-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.6</li>
+<li>Version 0.0.7</li>
 <ul><li>Added some help:</li>
 <ol><li>When a column is all None, it will be deleted without any notice.</li>
 <li>Rows in a pattern that takes place at the least number of rows will be highlighted.</li>
 <li>The first row of the rows will be selected and is ready for next action. This selection is only a hint and should not be followed unless otherwise.</li></ol></ul>
 
 
 <br>
 
 <li>Version 0.0.5</li>
-<ul><li>Disabled some bindings that belong to tksheet package.<ul>
+<ul><li>Disabled some bindings that belong to tksheet package.</li></ul>
 <br>
 
 <li>Version 0.0.4</li>
 
 ```python
 
 import excelcolumnizer as xl
```

#### html2text {}

```diff
@@ -1,60 +1,52 @@
 # excelcolumnizer ## What is it? A package that helps you recover columns of
 Excel data converted from PDF files. ## Where to get it
 pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.6
+    * Version 0.0.7
           o Added some help:
                1. When a column is all None, it will be deleted without any
                   notice.
                2. Rows in a pattern that takes place at the least number of
                   rows will be highlighted.
                3. The first row of the rows will be selected and is ready for
                   next action. This selection is only a hint and should not be
                   followed unless otherwise.
     *
     * Version 0.0.5
           o Disabled some bindings that belong to tksheet package.
-                #
-                # Version 0.0.4
-                # ```python import excelcolumnizer as xl xlpath='(excel file
-                  name with extension)' xl.sheet(xlpath) ```
-                      # A tksheet window will be opened with the contents of
-                        excel file.
-                      # Here are recommending orders of actions to try:
-                           1. Remove unwanted rows (F7)
-                           2. Remove unwanted columns (F7) or combine columns
-                              (F5)
-                           3. Click a cell to insert (F1) or delete the cell
-                              (F3)
-                      #
-                      # If the same pattern or kind of selected rows/columns is
-                        found at other locations, the same action is repeated
-                        for the found rows/columns.
-                            # Thus, it would better try one action at the top
-                            # To remove rows, click the row names.
-                            # To remove or combine columns, click the column
-                              names.
-                      #
-                      # After every action, the contents will be saved to a
-                        file that is the original name with a string
-                        "_cleaned".
-                      # When a cell is inserted, all the cells at right will be
-                        shifted to the right and an extra column will be
-                        created with empty for all other rows that are not
-                        changed.
-                      # When a cell is deleted, all the cells at right will be
-                        shifted to the left and the cell at the last column
-                        will be empty.
-                      # If one action is done by mistake, press function-key
-                        F12 to restore the the data before he last action
-                #
-                      # After each action is completed,
-                            # the number of columns and rows and the number of
-                              patterns of rows will be displayed
-                            # either a few columns or muliple rows are
-                              highlighted, which are indicative of ok to be
-                              deleted.
+    *
+    * Version 0.0.4
+    * ```python import excelcolumnizer as xl xlpath='(excel file name with
+      extension)' xl.sheet(xlpath) ```
+          o A tksheet window will be opened with the contents of excel file.
+          o Here are recommending orders of actions to try:
+               1. Remove unwanted rows (F7)
+               2. Remove unwanted columns (F7) or combine columns (F5)
+               3. Click a cell to insert (F1) or delete the cell (F3)
+          o
+          o If the same pattern or kind of selected rows/columns is found at
+            other locations, the same action is repeated for the found rows/
+            columns.
+                # Thus, it would better try one action at the top
+                # To remove rows, click the row names.
+                # To remove or combine columns, click the column names.
+          o
+          o After every action, the contents will be saved to a file that is
+            the original name with a string "_cleaned".
+          o When a cell is inserted, all the cells at right will be shifted to
+            the right and an extra column will be created with empty for all
+            other rows that are not changed.
+          o When a cell is deleted, all the cells at right will be shifted to
+            the left and the cell at the last column will be empty.
+          o If one action is done by mistake, press function-key F12 to restore
+            the the data before he last action
+    *
+          o After each action is completed,
+                # the number of columns and rows and the number of patterns of
+                  rows will be displayed
+                # either a few columns or muliple rows are highlighted, which
+                  are indicative of ok to be deleted.
```

### Comparing `excelcolumnizer-0.0.6/pyproject.toml` & `excelcolumnizer-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excelcolumnizer"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `excelcolumnizer-0.0.6/PKG-INFO` & `excelcolumnizer-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excelcolumnizer
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -30,25 +30,25 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.6</li>
+<li>Version 0.0.7</li>
 <ul><li>Added some help:</li>
 <ol><li>When a column is all None, it will be deleted without any notice.</li>
 <li>Rows in a pattern that takes place at the least number of rows will be highlighted.</li>
 <li>The first row of the rows will be selected and is ready for next action. This selection is only a hint and should not be followed unless otherwise.</li></ol></ul>
 
 
 <br>
 
 <li>Version 0.0.5</li>
-<ul><li>Disabled some bindings that belong to tksheet package.<ul>
+<ul><li>Disabled some bindings that belong to tksheet package.</li></ul>
 <br>
 
 <li>Version 0.0.4</li>
 
 ```python
 
 import excelcolumnizer as xl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.6 Summary: A small
+Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.7 Summary: A small
 packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -13,60 +13,52 @@
 markdown # excelcolumnizer ## What is it? A package that helps you recover
 columns of Excel data converted from PDF files. ## Where to get it
 pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.6
+    * Version 0.0.7
           o Added some help:
                1. When a column is all None, it will be deleted without any
                   notice.
                2. Rows in a pattern that takes place at the least number of
                   rows will be highlighted.
                3. The first row of the rows will be selected and is ready for
                   next action. This selection is only a hint and should not be
                   followed unless otherwise.
     *
     * Version 0.0.5
           o Disabled some bindings that belong to tksheet package.
-                #
-                # Version 0.0.4
-                # ```python import excelcolumnizer as xl xlpath='(excel file
-                  name with extension)' xl.sheet(xlpath) ```
-                      # A tksheet window will be opened with the contents of
-                        excel file.
-                      # Here are recommending orders of actions to try:
-                           1. Remove unwanted rows (F7)
-                           2. Remove unwanted columns (F7) or combine columns
-                              (F5)
-                           3. Click a cell to insert (F1) or delete the cell
-                              (F3)
-                      #
-                      # If the same pattern or kind of selected rows/columns is
-                        found at other locations, the same action is repeated
-                        for the found rows/columns.
-                            # Thus, it would better try one action at the top
-                            # To remove rows, click the row names.
-                            # To remove or combine columns, click the column
-                              names.
-                      #
-                      # After every action, the contents will be saved to a
-                        file that is the original name with a string
-                        "_cleaned".
-                      # When a cell is inserted, all the cells at right will be
-                        shifted to the right and an extra column will be
-                        created with empty for all other rows that are not
-                        changed.
-                      # When a cell is deleted, all the cells at right will be
-                        shifted to the left and the cell at the last column
-                        will be empty.
-                      # If one action is done by mistake, press function-key
-                        F12 to restore the the data before he last action
-                #
-                      # After each action is completed,
-                            # the number of columns and rows and the number of
-                              patterns of rows will be displayed
-                            # either a few columns or muliple rows are
-                              highlighted, which are indicative of ok to be
-                              deleted.
+    *
+    * Version 0.0.4
+    * ```python import excelcolumnizer as xl xlpath='(excel file name with
+      extension)' xl.sheet(xlpath) ```
+          o A tksheet window will be opened with the contents of excel file.
+          o Here are recommending orders of actions to try:
+               1. Remove unwanted rows (F7)
+               2. Remove unwanted columns (F7) or combine columns (F5)
+               3. Click a cell to insert (F1) or delete the cell (F3)
+          o
+          o If the same pattern or kind of selected rows/columns is found at
+            other locations, the same action is repeated for the found rows/
+            columns.
+                # Thus, it would better try one action at the top
+                # To remove rows, click the row names.
+                # To remove or combine columns, click the column names.
+          o
+          o After every action, the contents will be saved to a file that is
+            the original name with a string "_cleaned".
+          o When a cell is inserted, all the cells at right will be shifted to
+            the right and an extra column will be created with empty for all
+            other rows that are not changed.
+          o When a cell is deleted, all the cells at right will be shifted to
+            the left and the cell at the last column will be empty.
+          o If one action is done by mistake, press function-key F12 to restore
+            the the data before he last action
+    *
+          o After each action is completed,
+                # the number of columns and rows and the number of patterns of
+                  rows will be displayed
+                # either a few columns or muliple rows are highlighted, which
+                  are indicative of ok to be deleted.
```

