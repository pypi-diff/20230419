# Comparing `tmp/lezargus-0.0.1.dev2.tar.gz` & `tmp/lezargus-0.0.1.dev3.tar.gz`

## Comparing `lezargus-0.0.1.dev2.tar` & `lezargus-0.0.1.dev3.tar`

### file list

```diff
@@ -1,26 +1,86 @@
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/SECURITY.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/workspace.code-workspace
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/make.bat
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/.gitignore
--rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/coverage_html.js
--rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/d_42ee850819605eda___init___py.html
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/d_a44f0ac069e85531_test_global_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/favicon_32.png
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/keybd_open.png
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/status.json
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/coverage/style.css
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/source/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/docs/source/index.rst
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/src/lezargus/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/src/lezargus/__version__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/tests/__init__.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/tests/test_global.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/LICENSE.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/README.md
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/SECURITY.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/workspace.code-workspace
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/.nojekyll
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/Makefile
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/index.html
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/make.bat
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.buildinfo
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.nojekyll
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/genindex.html
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/index.html
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/objects.inv
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/py-modindex.html
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/search.html
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/searchindex.js
+-rw-r--r--   0        0        0  6571294 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.doctrees/index.doctree
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.doctrees/code/lezargus.__version__.doctree
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.doctrees/code/lezargus.doctree
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/.doctrees/code/modules.doctree
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_sources/code/lezargus.__version__.rst.txt
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_sources/code/lezargus.rst.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_sources/code/modules.rst.txt
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15715 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/basic.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/doctools.js
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/file.png
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/plus.png
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   135235 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/_static/js/theme.js
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/code/lezargus.__version__.html
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/code/lezargus.html
+-rw-r--r--   0        0        0     5486 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/build/html/code/modules.html
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/.gitignore
+-rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/coverage_html.js
+-rw-r--r--   0        0        0     5428 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/d_42ee850819605eda___init___py.html
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/d_a44f0ac069e85531_test_global_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/favicon_32.png
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/keybd_open.png
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/status.json
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/coverage/style.css
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/source/conf.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/source/index.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/source/code/lezargus.__version__.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/source/code/lezargus.rst
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/docs/source/code/modules.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/src/lezargus/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/src/lezargus/__version__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/tests/__init__.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/tests/test_global.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/LICENSE.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/README.md
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev3/PKG-INFO
```

### Comparing `lezargus-0.0.1.dev2/SECURITY.md` & `lezargus-0.0.1.dev3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/Makefile` & `lezargus-0.0.1.dev3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/make.bat` & `lezargus-0.0.1.dev3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/coverage_html.js` & `lezargus-0.0.1.dev3/docs/coverage/coverage_html.js`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/d_42ee850819605eda___init___py.html` & `lezargus-0.0.1.dev3/docs/coverage/d_42ee850819605eda___init___py.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/d_a44f0ac069e85531___init___py.html` & `lezargus-0.0.1.dev3/docs/coverage/d_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/d_a44f0ac069e85531_test_global_py.html` & `lezargus-0.0.1.dev3/docs/coverage/d_a44f0ac069e85531_test_global_py.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/favicon_32.png` & `lezargus-0.0.1.dev3/docs/coverage/favicon_32.png`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/index.html` & `lezargus-0.0.1.dev3/docs/coverage/index.html`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/keybd_closed.png` & `lezargus-0.0.1.dev3/docs/coverage/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/keybd_open.png` & `lezargus-0.0.1.dev3/docs/coverage/keybd_open.png`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/status.json` & `lezargus-0.0.1.dev3/docs/coverage/status.json`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/coverage/style.css` & `lezargus-0.0.1.dev3/docs/coverage/style.css`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/docs/source/conf.py` & `lezargus-0.0.1.dev3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/.gitignore` & `lezargus-0.0.1.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/LICENSE.txt` & `lezargus-0.0.1.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev2/pyproject.toml` & `lezargus-0.0.1.dev3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "lezargus"
+name = "Lezargus"
 dynamic = ["version"]
 description = "The accompanying data software package to the IRTF SPECTRE Spectrograph."
 readme = "README.md"
 requires-python = ">=3.11"
 license = "MIT"
 keywords = []
 authors = [
@@ -19,30 +19,31 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 
 [project.urls]
-Documentation = "https://github.com/psmd-iberutaru/Lezargus/Lezargus#readme"
-Issues = "https://github.com/psmd-iberutaru/Lezargus/Lezargus/issues"
-Source = "https://github.com/psmd-iberutaru/Lezargus/Lezargus"
+Documentation = "https://github.com/psmd-iberutaru/Lezargus#readme"
+Issues = "https://github.com/psmd-iberutaru/Lezargus/issues"
+Source = "https://github.com/psmd-iberutaru/Lezargus/"
 
 [tool.hatch.version]
 path = "src/lezargus/__version__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
-  "lezargus",
   "coverage[toml]>=6.5",
   "pytest>=7.3.0",
   "black>=23.1.0",
   "mypy>=1.0.0",
   "pylint>=2.17.0",
-  "ruff>=0.0.261"
+  "ruff>=0.0.261",
+  "sphinx>=6.1.0",
+  "sphinx_rtd_theme>=1.2.0",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 typing = "mypy --install-types --non-interactive {args:src/lezargus tests}"
 format = [
   "black {args:.}",
 ]
@@ -56,14 +57,18 @@
 lint = [
   "ruff {args:src}",
   "pylint {args:src}",
 ]
 lintfix = [
   "ruff {args:src} --fix"
 ]
+docs = [
+  "sphinx-apidoc -f -e -P -o ./docs/source/code/ ./src/lezargus/",
+  "sphinx-build -b html ./docs/source/ ./docs/build/html/",
+]
 auxiliary = [
   "typing",
   "lint",
   "lintfix",
   "test",
   "cover",
   "format",
```

### Comparing `lezargus-0.0.1.dev2/PKG-INFO` & `lezargus-0.0.1.dev3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: lezargus
-Version: 0.0.1.dev2
+Name: Lezargus
+Version: 0.0.1.dev3
 Summary: The accompanying data software package to the IRTF SPECTRE Spectrograph.
-Project-URL: Documentation, https://github.com/psmd-iberutaru/Lezargus/Lezargus#readme
-Project-URL: Issues, https://github.com/psmd-iberutaru/Lezargus/Lezargus/issues
-Project-URL: Source, https://github.com/psmd-iberutaru/Lezargus/Lezargus
+Project-URL: Documentation, https://github.com/psmd-iberutaru/Lezargus#readme
+Project-URL: Issues, https://github.com/psmd-iberutaru/Lezargus/issues
+Project-URL: Source, https://github.com/psmd-iberutaru/Lezargus/
 Author-email: Sparrow <psmd.iberutaru@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

