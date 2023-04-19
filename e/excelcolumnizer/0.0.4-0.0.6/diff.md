# Comparing `tmp/excelcolumnizer-0.0.4.tar.gz` & `tmp/excelcolumnizer-0.0.6.tar.gz`

## Comparing `excelcolumnizer-0.0.4.tar` & `excelcolumnizer-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/updatePackage.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/src/excelcolumnizer/__init__.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/src/excelcolumnizer/_excelColumnizer.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/updatePackage.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/src/excelcolumnizer/__init__.py
+-rw-r--r--   0        0        0    11929 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/src/excelcolumnizer/_excelColumnizer.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.6/PKG-INFO
```

### Comparing `excelcolumnizer-0.0.4/updatePackage.txt` & `excelcolumnizer-0.0.6/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.4/src/excelcolumnizer/_excelColumnizer.py` & `excelcolumnizer-0.0.6/src/excelcolumnizer/_excelColumnizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,24 +220,31 @@
 
             indicesJ =[j for j, p in enumerate(patt) if p == 'none']
             for v in copy.deepcopy(indices0):
                 if v not in indicesJ: indices0.remove(v)
 
         self.shtL.dehighlight_all()
         if indices0:
-            self.shtL.highlight_columns(columns = indices0, bg = colors[0], redraw = True)
+            #print('deleting column of  ', indices0[-1])
+            self.shtL.select_column(column=indices0[-1], redraw=True)
+            self.delRowsColumns()
         else:
             indices = [j+1 for j, kind in enumerate(kinds) if kind == list(patterns.keys())[0]]
             self.shtL.highlight_rows(rows = indices, bg = colors[2], redraw = True)
+            self.shtL.select_row(row=indices[0], redraw=True)
+            self.shtL.see(row=indices[0])
+                
             
         self.saveCleanedData()
+        rows = self.shtL.get_sheet_data()
         if self.hL['fg'] == 'green':
             self.hL.config(text=f'총 항목 수: {len(rows[0])}×{len(rows)}   총 줄-패턴 종류 수: {len(patterns)}')
 
 
+
     @staticmethod
     def getType(a):
         if isinstance(a, str):
             if a.isnumeric() or ('.' in a and a.replace('.','').isnumeric()): return 'num'
             else: return 'str'
         elif isinstance(a, int):
             return 'int'
@@ -266,33 +273,43 @@
             wb=load_workbook(xlpath, data_only=True)
             data = [[f.value for f in row] for row in wb.worksheets[0].rows]
             self.data=[row for row in data if row != [None for _ in range(len(data[0]))]]
         
         self.hw=tk.Tk()
         self.hw.option_add('*Font', ('Palatino Linotype',12))
         self.hw.geometry('1000x850')
-        self.hw.title(self.title+' '*10+'F1: add cells, F3: subtract cells, F5: combine cells, F7: delete cells, F9: save, F12: restore')
+        self.hw.title(self.title+' '*10+'F1: insert cell, F3: delete cell, F5: combine columns/rows, F7: delete columns/row, F9: save, F12: restore')
         self.hw.bind('<F1>', self.addCells)
         self.hw.bind('<F3>', self.subCells)
         self.hw.bind('<F5>', self.combineRowsColumns)
         self.hw.bind('<F7>', self.delRowsColumns)
         self.hw.bind('<F9>', self.saveCleanedData)
         self.hw.bind('<F12>', self.restore)
         
         self.hL=tk.Label(self.hw, text='...')
         self.hL.pack(pady=2)
 
         self.shtL = tksheet.Sheet(self.hw)
         self.shtL.pack(expand=1, fill='both')
         self.shtL.enable_bindings()
+        self.shtL.disable_bindings(['rc_delete_row', 'rc_delete_column'])
+
+        self.shtL.popup_menu_add_command("선택한 cell에 빈 칸 추가 - 오른쪽으로 이동 (F1)", self.addCells)
+        self.shtL.popup_menu_add_command("선택한 cell 삭제 - 왼쪽으로 이동 (F3)", self.subCells)
+        self.shtL.popup_menu_add_command("행/열 합치기 (F5)", self.combineRowsColumns)
+        self.shtL.popup_menu_add_command("행/열 삭제 (F7)", self.delRowsColumns)
+        self.shtL.popup_menu_add_command("방금 전 작업 복원 (F12)", self.restore)
 
         self.shtL.set_sheet_data(self.data)
         self.shtL.set_all_cell_sizes_to_text(redraw = True)
 
         self.hL.config(text=f'총 항목 수: {len(self.data[0])}×{len(self.data)}')
         self.hw.mainloop()        
     
 
 
 if __name__ == '__main__':
-    path=r'D:/Dropbox/POS/testing/JC-OSI007413.xlsx'
+    #path=r'D:/Dropbox/POS/testing/JC-OSI007413.xlsx'
+    #path=r'../ATE-207.xlsx'
+    #path=r'../KC_80968.xlsx'
+    path=r'../AJ-SO007558.xlsx'
     sheet(path)
```

### Comparing `excelcolumnizer-0.0.4/LICENSE.txt` & `excelcolumnizer-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.4/README.md` & `excelcolumnizer-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,38 +11,54 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
+<li>Version 0.0.6</li>
+<ul><li>Added some help:</li>
+<ol><li>When a column is all None, it will be deleted without any notice.</li>
+<li>Rows in a pattern that takes place at the least number of rows will be highlighted.</li>
+<li>The first row of the rows will be selected and is ready for next action. This selection is only a hint and should not be followed unless otherwise.</li></ol></ul>
+
+
+<br>
+
+<li>Version 0.0.5</li>
+<ul><li>Disabled some bindings that belong to tksheet package.<ul>
+<br>
+
 <li>Version 0.0.4</li>
 
 ```python
 
 import excelcolumnizer as xl
 
-xlpath='<full name of your excel file including extension>'
+xlpath='(excel file name with extension)'
 xl.sheet(xlpath)
 
 ```
 
-<ul><li>A GUI with tksheet will be opened with the contents of excel file.</li>
-<li>Here is a recommending set of actions to try:</li>
+<ul><li>A tksheet window will be opened with the contents of excel file.</li>
+<li>Here are recommending orders of actions to try:</li>
 <ol><li>Remove unwanted rows (F7)</li>
 <li>Remove unwanted columns (F7) or combine columns (F5)</li>
   <li>Click a cell to insert (F1) or delete the cell (F3)</li></ol>
 <br>
 
-<li>All action is repeated if the same kind of selected rows/columns is found at other locations.</li>
-  <ul><li>Thus, try one action at the top</li></ul>
+<li>If the same pattern or kind of selected rows/columns is found at other locations, the same action is repeated for the found rows/columns.</li>
+  <ul><li>Thus, it would better try one action at the top</li>
+  <li>To remove rows, click the row names.</li>
+    <li>To remove or combine columns, click the column names.</li></ul>
+  <br>
 <li>After every action, the contents will be saved to a file that is the original name with a string "_cleaned".</li>
-<li>When a cell is inserted, all the cells at right will be shifted to the right</li>
+<li>When a cell is inserted, all the cells at right will be shifted to the right and an extra column will be created with empty for all other rows that are not changed.</li>
 <li>When a cell is deleted, all the cells at right will be shifted to the left and the cell at the last column will be empty.</li>
-  <li>If the action is done by mistake, press function-key F12 to restore the last action</li></ul>
+  <li>If one action is done by mistake, press function-key F12 to restore the the data before he last action</li></ul>
   <br>
-<ul><li>To aid your step, some highlights take places</li>
-  <ul><li>Some rows will be highlighted in redish, indicating that the rows are least occurance among "patterns". It does not mean you need to delete the rows, but it might be one of them you want to delete.</li>
-    <li>When columns are highlighted, the columns are all empty. Thus, you can certainly delete the columns</li></ul>
-    
+<ul><li>After each action is completed,</li>
+<ul><li>the number of columns and rows and the number of patterns of rows will be displayed</li>
+<li>either a few columns or muliple rows are highlighted, which are indicative of ok to be deleted.</li></ul>
 </ul>
-<br>
+</ul>
+<br>
```

#### html2text {}

```diff
@@ -1,35 +1,60 @@
 # excelcolumnizer ## What is it? A package that helps you recover columns of
 Excel data converted from PDF files. ## Where to get it
 pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.4
-    * ```python import excelcolumnizer as xl xlpath='' xl.sheet(xlpath) ```
-          o A GUI with tksheet will be opened with the contents of excel file.
-          o Here is a recommending set of actions to try:
-               1. Remove unwanted rows (F7)
-               2. Remove unwanted columns (F7) or combine columns (F5)
-               3. Click a cell to insert (F1) or delete the cell (F3)
-          o
-          o All action is repeated if the same kind of selected rows/columns is
-            found at other locations.
-                # Thus, try one action at the top
-          o After every action, the contents will be saved to a file that is
-            the original name with a string "_cleaned".
-          o When a cell is inserted, all the cells at right will be shifted to
-            the right
-          o When a cell is deleted, all the cells at right will be shifted to
-            the left and the cell at the last column will be empty.
-          o If the action is done by mistake, press function-key F12 to restore
-            the last action
-    *
-          o To aid your step, some highlights take places
-                # Some rows will be highlighted in redish, indicating that the
-                  rows are least occurance among "patterns". It does not mean
-                  you need to delete the rows, but it might be one of them you
-                  want to delete.
-                # When columns are highlighted, the columns are all empty.
-                  Thus, you can certainly delete the columns
+    * Version 0.0.6
+          o Added some help:
+               1. When a column is all None, it will be deleted without any
+                  notice.
+               2. Rows in a pattern that takes place at the least number of
+                  rows will be highlighted.
+               3. The first row of the rows will be selected and is ready for
+                  next action. This selection is only a hint and should not be
+                  followed unless otherwise.
     *
+    * Version 0.0.5
+          o Disabled some bindings that belong to tksheet package.
+                #
+                # Version 0.0.4
+                # ```python import excelcolumnizer as xl xlpath='(excel file
+                  name with extension)' xl.sheet(xlpath) ```
+                      # A tksheet window will be opened with the contents of
+                        excel file.
+                      # Here are recommending orders of actions to try:
+                           1. Remove unwanted rows (F7)
+                           2. Remove unwanted columns (F7) or combine columns
+                              (F5)
+                           3. Click a cell to insert (F1) or delete the cell
+                              (F3)
+                      #
+                      # If the same pattern or kind of selected rows/columns is
+                        found at other locations, the same action is repeated
+                        for the found rows/columns.
+                            # Thus, it would better try one action at the top
+                            # To remove rows, click the row names.
+                            # To remove or combine columns, click the column
+                              names.
+                      #
+                      # After every action, the contents will be saved to a
+                        file that is the original name with a string
+                        "_cleaned".
+                      # When a cell is inserted, all the cells at right will be
+                        shifted to the right and an extra column will be
+                        created with empty for all other rows that are not
+                        changed.
+                      # When a cell is deleted, all the cells at right will be
+                        shifted to the left and the cell at the last column
+                        will be empty.
+                      # If one action is done by mistake, press function-key
+                        F12 to restore the the data before he last action
+                #
+                      # After each action is completed,
+                            # the number of columns and rows and the number of
+                              patterns of rows will be displayed
+                            # either a few columns or muliple rows are
+                              highlighted, which are indicative of ok to be
+                              deleted.
+
```

### Comparing `excelcolumnizer-0.0.4/pyproject.toml` & `excelcolumnizer-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excelcolumnizer"
-version = "0.0.4"
+version = "0.0.6"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `excelcolumnizer-0.0.4/PKG-INFO` & `excelcolumnizer-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excelcolumnizer
-Version: 0.0.4
+Version: 0.0.6
 Summary: A small packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -30,38 +30,54 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
+<li>Version 0.0.6</li>
+<ul><li>Added some help:</li>
+<ol><li>When a column is all None, it will be deleted without any notice.</li>
+<li>Rows in a pattern that takes place at the least number of rows will be highlighted.</li>
+<li>The first row of the rows will be selected and is ready for next action. This selection is only a hint and should not be followed unless otherwise.</li></ol></ul>
+
+
+<br>
+
+<li>Version 0.0.5</li>
+<ul><li>Disabled some bindings that belong to tksheet package.<ul>
+<br>
+
 <li>Version 0.0.4</li>
 
 ```python
 
 import excelcolumnizer as xl
 
-xlpath='<full name of your excel file including extension>'
+xlpath='(excel file name with extension)'
 xl.sheet(xlpath)
 
 ```
 
-<ul><li>A GUI with tksheet will be opened with the contents of excel file.</li>
-<li>Here is a recommending set of actions to try:</li>
+<ul><li>A tksheet window will be opened with the contents of excel file.</li>
+<li>Here are recommending orders of actions to try:</li>
 <ol><li>Remove unwanted rows (F7)</li>
 <li>Remove unwanted columns (F7) or combine columns (F5)</li>
   <li>Click a cell to insert (F1) or delete the cell (F3)</li></ol>
 <br>
 
-<li>All action is repeated if the same kind of selected rows/columns is found at other locations.</li>
-  <ul><li>Thus, try one action at the top</li></ul>
+<li>If the same pattern or kind of selected rows/columns is found at other locations, the same action is repeated for the found rows/columns.</li>
+  <ul><li>Thus, it would better try one action at the top</li>
+  <li>To remove rows, click the row names.</li>
+    <li>To remove or combine columns, click the column names.</li></ul>
+  <br>
 <li>After every action, the contents will be saved to a file that is the original name with a string "_cleaned".</li>
-<li>When a cell is inserted, all the cells at right will be shifted to the right</li>
+<li>When a cell is inserted, all the cells at right will be shifted to the right and an extra column will be created with empty for all other rows that are not changed.</li>
 <li>When a cell is deleted, all the cells at right will be shifted to the left and the cell at the last column will be empty.</li>
-  <li>If the action is done by mistake, press function-key F12 to restore the last action</li></ul>
+  <li>If one action is done by mistake, press function-key F12 to restore the the data before he last action</li></ul>
   <br>
-<ul><li>To aid your step, some highlights take places</li>
-  <ul><li>Some rows will be highlighted in redish, indicating that the rows are least occurance among "patterns". It does not mean you need to delete the rows, but it might be one of them you want to delete.</li>
-    <li>When columns are highlighted, the columns are all empty. Thus, you can certainly delete the columns</li></ul>
-    
+<ul><li>After each action is completed,</li>
+<ul><li>the number of columns and rows and the number of patterns of rows will be displayed</li>
+<li>either a few columns or muliple rows are highlighted, which are indicative of ok to be deleted.</li></ul>
 </ul>
-<br>
+</ul>
+<br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.4 Summary: A small
+Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.6 Summary: A small
 packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -13,35 +13,60 @@
 markdown # excelcolumnizer ## What is it? A package that helps you recover
 columns of Excel data converted from PDF files. ## Where to get it
 pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.4
-    * ```python import excelcolumnizer as xl xlpath='' xl.sheet(xlpath) ```
-          o A GUI with tksheet will be opened with the contents of excel file.
-          o Here is a recommending set of actions to try:
-               1. Remove unwanted rows (F7)
-               2. Remove unwanted columns (F7) or combine columns (F5)
-               3. Click a cell to insert (F1) or delete the cell (F3)
-          o
-          o All action is repeated if the same kind of selected rows/columns is
-            found at other locations.
-                # Thus, try one action at the top
-          o After every action, the contents will be saved to a file that is
-            the original name with a string "_cleaned".
-          o When a cell is inserted, all the cells at right will be shifted to
-            the right
-          o When a cell is deleted, all the cells at right will be shifted to
-            the left and the cell at the last column will be empty.
-          o If the action is done by mistake, press function-key F12 to restore
-            the last action
-    *
-          o To aid your step, some highlights take places
-                # Some rows will be highlighted in redish, indicating that the
-                  rows are least occurance among "patterns". It does not mean
-                  you need to delete the rows, but it might be one of them you
-                  want to delete.
-                # When columns are highlighted, the columns are all empty.
-                  Thus, you can certainly delete the columns
+    * Version 0.0.6
+          o Added some help:
+               1. When a column is all None, it will be deleted without any
+                  notice.
+               2. Rows in a pattern that takes place at the least number of
+                  rows will be highlighted.
+               3. The first row of the rows will be selected and is ready for
+                  next action. This selection is only a hint and should not be
+                  followed unless otherwise.
     *
+    * Version 0.0.5
+          o Disabled some bindings that belong to tksheet package.
+                #
+                # Version 0.0.4
+                # ```python import excelcolumnizer as xl xlpath='(excel file
+                  name with extension)' xl.sheet(xlpath) ```
+                      # A tksheet window will be opened with the contents of
+                        excel file.
+                      # Here are recommending orders of actions to try:
+                           1. Remove unwanted rows (F7)
+                           2. Remove unwanted columns (F7) or combine columns
+                              (F5)
+                           3. Click a cell to insert (F1) or delete the cell
+                              (F3)
+                      #
+                      # If the same pattern or kind of selected rows/columns is
+                        found at other locations, the same action is repeated
+                        for the found rows/columns.
+                            # Thus, it would better try one action at the top
+                            # To remove rows, click the row names.
+                            # To remove or combine columns, click the column
+                              names.
+                      #
+                      # After every action, the contents will be saved to a
+                        file that is the original name with a string
+                        "_cleaned".
+                      # When a cell is inserted, all the cells at right will be
+                        shifted to the right and an extra column will be
+                        created with empty for all other rows that are not
+                        changed.
+                      # When a cell is deleted, all the cells at right will be
+                        shifted to the left and the cell at the last column
+                        will be empty.
+                      # If one action is done by mistake, press function-key
+                        F12 to restore the the data before he last action
+                #
+                      # After each action is completed,
+                            # the number of columns and rows and the number of
+                              patterns of rows will be displayed
+                            # either a few columns or muliple rows are
+                              highlighted, which are indicative of ok to be
+                              deleted.
+
```

