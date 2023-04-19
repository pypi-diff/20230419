# Comparing `tmp/lezargus-0.0.1.dev1.tar.gz` & `tmp/lezargus-0.0.1.dev2.tar.gz`

## Comparing `lezargus-0.0.1.dev1.tar` & `lezargus-0.0.1.dev2.tar`

### file list

```diff
@@ -1,15 +1,26 @@
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/SECURITY.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/workspace.code-workspace
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/make.bat
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/source/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/source/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/src/lezargus/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/src/lezargus/__version__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/tests/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/tests/test_global.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/LICENSE.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/README.md
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/SECURITY.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/workspace.code-workspace
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/make.bat
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/.gitignore
+-rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/d_42ee850819605eda___init___py.html
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/d_a44f0ac069e85531_test_global_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/favicon_32.png
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/keybd_open.png
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/status.json
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/style.css
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/source/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/source/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/src/lezargus/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/src/lezargus/__version__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/tests/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/tests/test_global.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/LICENSE.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/PKG-INFO
```

### Comparing `lezargus-0.0.1.dev1/SECURITY.md` & `lezargus-0.0.1.dev2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev1/docs/Makefile` & `lezargus-0.0.1.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev1/docs/make.bat` & `lezargus-0.0.1.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev1/docs/source/conf.py` & `lezargus-0.0.1.dev2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev1/.gitignore` & `lezargus-0.0.1.dev2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
-build/
+./build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
```

### Comparing `lezargus-0.0.1.dev1/LICENSE.txt` & `lezargus-0.0.1.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev1/pyproject.toml` & `lezargus-0.0.1.dev2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,16 @@
 format = [
   "black {args:.}",
 ]
 cover = [
   "coverage run -m pytest {args:tests}",
   "- coverage combine",
   "coverage report",
+  "coverage html",
+  "coverage erase",
 ]
 lint = [
   "ruff {args:src}",
   "pylint {args:src}",
 ]
 lintfix = [
   "ruff {args:src} --fix"
@@ -62,19 +64,28 @@
   "typing",
   "lint",
   "lintfix",
   "test",
   "cover",
   "format",
 ]
+aux = "auxiliary"
 
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.11"]
 
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "src",
+]
+testpaths = [
+  "tests"
+]
+
 [tool.black]
 target-version = ["py311"]
 line-length = 80
 
 [tool.ruff]
 target-version = "py311"
 line-length = 80
@@ -126,7 +137,11 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.coverage.html]
+title = "Lezargus Code Coverage Report"
+directory = "./docs/coverage/"
```

### Comparing `lezargus-0.0.1.dev1/PKG-INFO` & `lezargus-0.0.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lezargus
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: The accompanying data software package to the IRTF SPECTRE Spectrograph.
 Project-URL: Documentation, https://github.com/psmd-iberutaru/Lezargus/Lezargus#readme
 Project-URL: Issues, https://github.com/psmd-iberutaru/Lezargus/Lezargus/issues
 Project-URL: Source, https://github.com/psmd-iberutaru/Lezargus/Lezargus
 Author-email: Sparrow <psmd.iberutaru@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

