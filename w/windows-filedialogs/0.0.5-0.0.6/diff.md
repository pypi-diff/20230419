# Comparing `tmp/windows_filedialogs-0.0.5.tar.gz` & `tmp/windows_filedialogs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windows_filedialogs-0.0.5.tar", max compression
+gzip compressed data, was "windows_filedialogs-0.0.6.tar", max compression
```

## Comparing `windows_filedialogs-0.0.5.tar` & `windows_filedialogs-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      176 2023-03-30 19:36:42.329294 windows_filedialogs-0.0.5/filedialogs/__init__.py
--rw-r--r--   0        0        0     4602 2023-03-30 19:36:42.329294 windows_filedialogs-0.0.5/filedialogs/filedialogs.py
--rw-r--r--   0        0        0     1090 2023-03-30 19:36:42.329294 windows_filedialogs-0.0.5/LICENSE
--rw-r--r--   0        0        0     2877 2023-03-30 19:36:42.329294 windows_filedialogs-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3853 2023-03-30 19:36:42.329294 windows_filedialogs-0.0.5/README.md
--rw-r--r--   0        0        0     5189 1970-01-01 00:00:00.000000 windows_filedialogs-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      176 2023-04-19 16:54:37.444106 windows_filedialogs-0.0.6/filedialogs/__init__.py
+-rw-r--r--   0        0        0     5352 2023-04-19 16:54:37.444106 windows_filedialogs-0.0.6/filedialogs/filedialogs.py
+-rw-r--r--   0        0        0     1090 2023-04-19 16:54:37.444106 windows_filedialogs-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2878 2023-04-19 16:54:37.444106 windows_filedialogs-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3853 2023-04-19 16:54:37.444106 windows_filedialogs-0.0.6/README.md
+-rw-r--r--   0        0        0     5189 1970-01-01 00:00:00.000000 windows_filedialogs-0.0.6/PKG-INFO
```

### Comparing `windows_filedialogs-0.0.5/filedialogs/filedialogs.py` & `windows_filedialogs-0.0.6/filedialogs/filedialogs.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,26 @@
 
 
 def open_file_dialog(
     title: str = None,
     directory: Optional[str] = None,
     default_name: str = "",
     default_ext: str = "",
-    ext: List[Tuple[str, str]] = None,
+    ext: List[Tuple[str, str | Tuple[str, ...]]] = None,
     multiselect: bool = False,
 ) -> Union[str, List[str], None]:
     """Open a file open dialog at a specified directory.
 
     :param title: Dialog title.
     :param directory: Directory to open file dialog in.
     :param default_name: Default file name.
     :param default_ext: Default file extension. Only letters, no dot.
-    :param ext: List of available extension description + name tuples,
-                e.g. [(JPEG Image, jpg), (PNG Image, png)].
+    :param ext: List of available extension(s) description + name tuples,
+                e.g. [("JPEG Image", "jpg"), ("PNG Image", "png")].
+                or, [("MPEG-4 Variations", ("m4v", "mp4", "m4p")), ("AVI Variations", ("avi", "amv"))]
     :param multiselect: Allow multiple files to be selected.
     :return: Path to a file to open if multiselect=False.
              List of the paths to files, which should be opened if multiselect=True.
              None if file open dialog canceled.
     :raises IOError: File open dialog failed.
     """
 
@@ -46,15 +47,21 @@
     flags = OFN_EXPLORER
     if multiselect:
         flags = flags | OFN_ALLOWMULTISELECT
 
     if ext is None:
         ext = "All Files\0*.*\0"
     else:
-        ext = "".join([f"{name}\0*.{extension}\0" for name, extension in ext])
+        ext_filter = ""
+        for name, extensions in ext:
+            if isinstance(extensions, str):
+                ext_filter += f"{name}\0*.{extensions}\0"
+                continue
+            ext_filter += f"{name}\0" + ";".join(f"*.{extension}" for extension in extensions) + "\0"
+        ext = ext_filter
 
     try:
         file_path, _, _ = GetOpenFileNameW(
             InitialDir=directory,
             File=default_name,
             Flags=flags,
             Title=title,
@@ -82,37 +89,44 @@
 
 
 def save_file_dialog(
     title: str = None,
     directory: Optional[str] = None,
     default_name: str = "",
     default_ext: str = "",
-    ext: List[Tuple[str, str]] = None,
+    ext: List[Tuple[str, str | Tuple[str, ...]]] = None,
 ) -> Optional[str]:
     """Open a file save dialog at a specified directory.
 
     :param title: Dialog title.
     :param directory: Directory to open file dialog in.
     :param default_name: Default file name.
     :param default_ext: Default file extension. Only letters, no dot.
-    :param ext: List of available extension description + name tuples,
-                e.g. [(JPEG Image, jpg), (PNG Image, png)].
+    :param ext: List of available extension(s) description + name tuples,
+                e.g. [("JPEG Image", "jpg"), ("PNG Image", "png")].
+                or, [("MPEG-4 Variations", ("m4v", "mp4", "m4p")), ("AVI Variations", ("avi", "amv"))]
     :return: Path file should be saved to. None if file save dialog canceled.
     :raises IOError: File save dialog failed.
     """
 
     # https://programtalk.com/python-examples/win32gui.GetSaveFileNameW/
 
     if directory is None:
         directory = os.getcwd()
 
     if ext is None:
         ext = "All Files\0*.*\0"
     else:
-        ext = "".join([f"{name}\0*.{extension}\0" for name, extension in ext])
+        ext_filter = ""
+        for name, extensions in ext:
+            if isinstance(extensions, str):
+                ext_filter += f"{name}\0*.{extensions}\0"
+                continue
+            ext_filter += f"{name}\0" + ";".join(f"*.{extension}" for extension in extensions) + "\0"
+        ext = ext_filter
 
     try:
         file_path, _, _ = GetSaveFileNameW(
             InitialDir=directory,
             File=default_name,
             Title=title,
             MaxFile=2**16,
```

### Comparing `windows_filedialogs-0.0.5/LICENSE` & `windows_filedialogs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `windows_filedialogs-0.0.5/pyproject.toml` & `windows_filedialogs-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windows_filedialogs"
-version = "0.0.5"
+version = "0.0.6"
 description = "Simple Windows file dialogs."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "filedialogs" },
 ]
@@ -45,28 +45,28 @@
 "Bug Tracker" = "https://github.com/MrThearMan/filedialogs/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 pywin32 = ">=306"
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.2.2"
+pytest = "7.3.0"
 coverage = "6.5.0"
-pre-commit = "3.2.1"
-tox = "4.4.8"
+pre-commit = "3.2.2"
+tox = "4.4.12"
 tox-gh-actions = "3.1.0"
 coveralls = "3.3.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.4.2"
-pymdown-extensions = "9.10"
+pymdown-extensions = "9.11"
 mkdocs-mermaid2-plugin = "0.6.0"
 
 [tool.poetry.group.lint.dependencies]
-mypy = "1.1.1"
+mypy = "1.2.0"
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 fix = true
 line-length = 120
@@ -130,9 +130,9 @@
     PYTHONPATH = {toxinidir}
 commands =
     poetry install
     poetry run coverage run -m pytest
 """
 
 [build-system]
-requires = ["poetry-core>=1.4.0"]
+requires = ["poetry-core>=1.5.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `windows_filedialogs-0.0.5/README.md` & `windows_filedialogs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `windows_filedialogs-0.0.5/PKG-INFO` & `windows_filedialogs-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windows-filedialogs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple Windows file dialogs.
 Home-page: https://mrthearman.github.io/filedialogs
 License: MIT
 Keywords: file,dialogs,windows,open,save
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.8,<4
```

