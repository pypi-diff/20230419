# Comparing `tmp/metadata_utils-0.1.3.tar.gz` & `tmp/metadata_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metadata_utils-0.1.3.tar", last modified: Fri Mar 26 16:12:03 2021, max compression
+gzip compressed data, was "metadata_utils-0.2.0.tar", last modified: Wed Apr 19 16:45:05 2023, max compression
```

## Comparing `metadata_utils-0.1.3.tar` & `metadata_utils-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/
--rw-r--r--   0 jvanasco   (501) admin       (80)      309 2021-03-26 16:10:04.000000 metadata_utils-0.1.3/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1105 2013-10-22 19:00:17.000000 metadata_utils-0.1.3/LICENSE
--rw-r--r--   0 jvanasco   (501) admin       (80)      179 2021-03-26 16:10:32.000000 metadata_utils-0.1.3/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     1072 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-14 19:40:51.000000 metadata_utils-0.1.3/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)      400 2020-10-20 21:33:43.000000 metadata_utils-0.1.3/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       69 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1529 2021-03-26 16:09:25.000000 metadata_utils-0.1.3/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils/
--rw-r--r--   0 jvanasco   (501) admin       (80)      886 2021-03-26 16:11:16.000000 metadata_utils-0.1.3/src/metadata_utils/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:10:54.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     1072 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       22 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      401 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       15 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/src/metadata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:12:03.000000 metadata_utils-0.1.3/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:10:41.000000 metadata_utils-0.1.3/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1991 2019-09-19 21:35:12.000000 metadata_utils-0.1.3/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2020-10-13 00:24:20.000000 metadata_utils-0.1.3/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.836947 metadata_utils-0.2.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      368 2023-04-19 16:18:53.000000 metadata_utils-0.2.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1105 2013-10-22 19:00:17.000000 metadata_utils-0.2.0/LICENSE
+-rw-r--r--   0 jvanasco   (501) admin       (80)      179 2021-03-26 16:10:32.000000 metadata_utils-0.2.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1236 2023-04-19 16:45:05.837327 metadata_utils-0.2.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      400 2020-10-20 21:33:43.000000 metadata_utils-0.2.0/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-04-19 15:50:34.000000 metadata_utils-0.2.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)       69 2023-04-19 16:45:05.838847 metadata_utils-0.2.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1847 2023-04-19 16:44:40.000000 metadata_utils-0.2.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.808022 metadata_utils-0.2.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.820179 metadata_utils-0.2.0/src/metadata_utils/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      957 2023-04-19 15:55:35.000000 metadata_utils-0.2.0/src/metadata_utils/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.833011 metadata_utils-0.2.0/src/metadata_utils.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1236 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      401 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:10:54.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       18 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       15 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.836148 metadata_utils-0.2.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:10:41.000000 metadata_utils-0.2.0/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-04-19 16:35:27.000000 metadata_utils-0.2.0/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-04-19 16:17:53.000000 metadata_utils-0.2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `metadata_utils-0.1.3/LICENSE` & `metadata_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata_utils-0.1.3/PKG-INFO` & `metadata_utils-0.2.0/src/metadata_utils.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 Metadata-Version: 2.1
-Name: metadata_utils
-Version: 0.1.3
+Name: metadata-utils
+Version: 0.2.0
 Summary: Lightweight Metadata Support
 Home-page: https://github.com/jvanasco/metadata_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
-Description: ![Python package](https://github.com/jvanasco/metadata_utils/workflows/Python%20package/badge.svg)
-        
-        metadata_utils
-        ==============
-        
-        This package offers lightweight tools for dealing with metadata in HTML.
-        
-        The following functions are made available to streamline dealing with html encodings:
-        
-        * `html_attribute_escape`
-        * `html_attribute_unescape`
-        * `force_clean_ascii_NFKD`
-        * `force_clean_ascii_NFKC`
-        
 Keywords: web
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+![Python package](https://github.com/jvanasco/metadata_utils/workflows/Python%20package/badge.svg)
+
+metadata_utils
+==============
+
+This package offers lightweight tools for dealing with metadata in HTML.
+
+The following functions are made available to streamline dealing with html encodings:
+
+* `html_attribute_escape`
+* `html_attribute_unescape`
+* `force_clean_ascii_NFKD`
+* `force_clean_ascii_NFKC`
```

### Comparing `metadata_utils-0.1.3/setup.py` & `metadata_utils-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,43 +13,49 @@
 
 # store version in the init.py
 with open(os.path.join(HERE, "src", "metadata_utils", "__init__.py")) as v_file:
     VERSION = re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
 
 requires = []
 tests_require = [
-    "six",
     "pytest",
 ]
 testing_extras = tests_require + []
 
 setup(
     name="metadata_utils",
     description="Lightweight Metadata Support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=VERSION,
     url="https://github.com/jvanasco/metadata_utils",
     author="Jonathan Vanasco",
     author_email="jonathan@findmeon.com",
     zip_safe=False,
+    python_requires=">=3.6",
     keywords="web",
     install_requires=requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
     test_suite="tests",
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"metadata_utils": ["py.typed"]},
     include_package_data=True,
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     license="MIT",
 )
```

### Comparing `metadata_utils-0.1.3/src/metadata_utils/__init__.py` & `metadata_utils-0.2.0/src/metadata_utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
+# stdlib
 import unicodedata
-
 from xml.sax.saxutils import escape, unescape
 
-__VERSION__ = "0.1.3"
+__VERSION__ = "0.2.0"
 
 
 # ==============================================================================
 
 
 # https://wiki.python.org/moin/EscapingHtml
-# escape() and unescape() takes care of "&" , "<" and ">" - we need to handle quotes, so we don't break things
-html_attribute_escape_table = {'"': "&quot;", "'": "&apos;"}
-
-
-html_attribute_unescape_table = {v: k for (k, v) in html_attribute_escape_table.items()}
+# escape() and unescape() takes care of "&" , "<" and ">"
+# we need to handle quotes, so we don't break things
+html_attribute_escape_table: dict = {'"': "&quot;", "'": "&apos;"}
+html_attribute_unescape_table: dict = {
+    v: k for (k, v) in html_attribute_escape_table.items()
+}
 
 
-def html_attribute_escape(text):
+def html_attribute_escape(text: str) -> str:
     return escape(text, html_attribute_escape_table)
 
 
-def html_attribute_unescape(text):
+def html_attribute_unescape(text: str) -> str:
     return unescape(text, html_attribute_unescape_table)
 
 
-##
-
-
-def force_clean_ascii_NFKD(text):
+def force_clean_ascii_NFKD(text: str) -> bytes:
     return unicodedata.normalize("NFKD", text).encode("ascii", "ignore")
 
 
-def force_clean_ascii_NFKC(text):
+def force_clean_ascii_NFKC(text: str) -> bytes:
     return unicodedata.normalize("NFKC", text).encode("ascii", "ignore")
```

### Comparing `metadata_utils-0.1.3/tests/test_core.py` & `metadata_utils-0.2.0/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import unittest
 import metadata_utils
 
-import six
-
 
 # ==============================================================================
 
 
 class TestEscaping(unittest.TestCase):
     text_raw = """foo "' bar"""
     text_escaped = "foo &quot;&apos; bar"
@@ -30,27 +28,19 @@
         self.assertEqual(escaped, self.text_escaped)
         unescaped = metadata_utils.html_attribute_unescape(escaped)
         self.assertEqual(unescaped, self.text_raw)
 
 
 class TestCleanAscii(unittest.TestCase):
     def test_NFKD(self):
-        text_unicode = u"El Ni\xf1o"  # u needed for 2/3 compat
+        text_unicode = "El Ni\xf1o"
         text_clean_a = "El Nino"  # downgrades
         escaped = metadata_utils.force_clean_ascii_NFKD(text_unicode)
-        if six.PY2:
-            # py2 is a string
-            self.assertEqual(escaped, text_clean_a)
-        else:
-            # py3 is a bytes
-            self.assertEqual(escaped, text_clean_a.encode())
+        # py3 is a bytes
+        self.assertEqual(escaped, text_clean_a.encode())
 
     def test_NFKC(self):
-        text_unicode = u"El Ni\xf1o"  # u needed for 2/3 compat
+        text_unicode = "El Ni\xf1o"
         text_clean_a = "El Nio"  # strips
         escaped = metadata_utils.force_clean_ascii_NFKC(text_unicode)
-        if six.PY2:
-            # py2 is a string
-            self.assertEqual(escaped, text_clean_a)
-        else:
-            # py3 is a bytes
-            self.assertEqual(escaped, text_clean_a.encode())
+        # py3 is a bytes
+        self.assertEqual(escaped, text_clean_a.encode())
```

