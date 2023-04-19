# Comparing `tmp/e-models-1.1.tar.gz` & `tmp/e-models-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.1.tar", last modified: Tue Apr 18 18:43:32 2023, max compression
+gzip compressed data, was "e-models-1.1.1.tar", last modified: Wed Apr 19 14:04:04 2023, max compression
```

## Comparing `e-models-1.1.tar` & `e-models-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.362634 e-models-1.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3550 2023-04-18 18:43:32.362634 e-models-1.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3012 2023-04-18 18:35:24.000000 e-models-1.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.358634 e-models-1.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3550 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      447 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       17 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-04-18 18:43:32.000000 e-models-1.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.358634 e-models-1.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-04-18 18:42:20.000000 e-models-1.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.362634 e-models-1.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34179 2023-04-05 19:57:01.000000 e-models-1.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.1/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6870 2023-04-18 18:32:52.000000 e-models-1.1/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-18 18:43:32.362634 e-models-1.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      926 2023-04-18 18:42:11.000000 e-models-1.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-18 18:43:32.362634 e-models-1.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7875 2023-04-18 18:32:24.000000 e-models-1.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.703922 e-models-1.1.1/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.1.1/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-04-19 14:04:04.703922 e-models-1.1.1/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.1.1/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.699922 e-models-1.1.1/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3270 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      447 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       17 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-04-19 14:04:04.000000 e-models-1.1.1/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.699922 e-models-1.1.1/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-04-19 14:03:03.000000 e-models-1.1.1/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.1.1/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.703922 e-models-1.1.1/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34187 2023-04-19 14:01:20.000000 e-models-1.1.1/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3841 2023-04-01 19:54:46.000000 e-models-1.1.1/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.1.1/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.1.1/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.1.1/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.1.1/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7028 2023-04-19 13:53:58.000000 e-models-1.1.1/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.1.1/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-19 14:04:04.703922 e-models-1.1.1/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      928 2023-04-19 14:02:56.000000 e-models-1.1.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 14:04:04.703922 e-models-1.1.1/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7946 2023-04-19 14:00:24.000000 e-models-1.1.1/tests/test_scrapyutils.py
```

### Comparing `e-models-1.1/LICENSE` & `e-models-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.1/PKG-INFO` & `e-models-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.1
+Version: 1.1.1
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -52,11 +52,8 @@
 In addition, in order to have your dataset well ordered, you should choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
 schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. At
 the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
 So, even if you didn't train the transformer to extract a specific item class, it will do great if you trained it to extract its fields, if it already learned to extract same fields from
 other item classes. You only need to ask the correct question. For example, given an html page as a context, you can ask the model: `which is the phone number?`. You don't need to specify
 which kind of data (a business? a person? an organization?) you expect to find there.
 
-**Important Note**: Usage of the methods introduced by ExtractItemLoader (`add_text_re()` and `add_text_re_as_html()`) will have an impact in the performance of the spiders you use it, so the
-recommendation is to use them in spiders that don't extract more than few hundred items.
-
 (WIP...)
```

### Comparing `e-models-1.1/README.md` & `e-models-1.1.1/e_models.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: e-models
+Version: 1.1.1
+Summary: Tools for helping build of extraction models with scrapy spiders.
+Home-page: https://github.com/kalessin/emodels
+Author: Martin Olveyra
+Author-email: molveyra@gmail.com
+License: BSD
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 e-models
 ========
 
 
 Suite of tools to assist in the build of extraction models with scrapy spiders
 
 Installation:
@@ -36,11 +52,8 @@
 In addition, in order to have your dataset well ordered, you should choose the same item class name for same item schema, even accross multiple projects. And avoid to repeat it among items with different
 schema. However, in general you will use extraction data from all classes of items at same time in order to train a transformer model, as this is the way how transformers learn to generalize. At
 the end you will have a transformer model that is suited to extract any kind of item, as they are trained not to extract "data from x item" but instead to recognize and extract based on fields.
 So, even if you didn't train the transformer to extract a specific item class, it will do great if you trained it to extract its fields, if it already learned to extract same fields from
 other item classes. You only need to ask the correct question. For example, given an html page as a context, you can ask the model: `which is the phone number?`. You don't need to specify
 which kind of data (a business? a person? an organization?) you expect to find there.
 
-**Important Note**: Usage of the methods introduced by ExtractItemLoader (`add_text_re()` and `add_text_re_as_html()`) will have an impact in the performance of the spiders you use it, so the
-recommendation is to use them in spiders that don't extract more than few hundred items.
-
 (WIP...)
```

### Comparing `e-models-1.1/emodels/html2text/__init__.py` & `e-models-1.1.1/emodels/html2text/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
     def handle_starttag(self, tag: str, attrs: List[Tuple[str, Optional[str]]]) -> None:
         attrid = dict(attrs).get("itemprop", "")
         if not attrid:
             attrid = dict(attrs).get("id", "")
         self.current_id.append(attrid)
 
-        attrclass = dict(attrs).get("class", "")
+        attrclass = dict(attrs).get("class", "").strip()
         self.current_class.append(attrclass)
 
         self.handle_tag(tag, dict(attrs), start=True)
 
     def handle_endtag(self, tag: str) -> None:
         if self.current_id:
             self.current_id.pop()
```

### Comparing `e-models-1.1/emodels/html2text/config.py` & `e-models-1.1.1/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.1/emodels/html2text/utils.py` & `e-models-1.1.1/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.1/emodels/scrapyutils.py` & `e-models-1.1.1/emodels/scrapyutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,25 +82,27 @@
     def text_re(
         self,
         reg: str = "(.+?)",
         tid: Optional[str] = None,
         flags: int = 0,
         skip_prefix: str = DEFAULT_SKIP_PREFIX,
         strict_tid: bool = False,
+        optimize: bool = False,
     ):
-        if strict_tid:
+        if tid and strict_tid:
             reg = f"(?:.*<!--.+-->)?{reg}"
         reg = f"{skip_prefix}{reg}"
         markdown = self.markdown
         if tid:
-            reg += fr"\s+<!--{tid}-->"
             if tid.startswith("#"):
                 markdown = self.markdown_ids
             elif tid.startswith("."):
+                tid = "\\" + tid
                 markdown = self.markdown_classes
+            reg += fr"\s+<!--{tid}-->"
         result = []
         for m in re.finditer(reg, markdown, flags):
             if m.groups():
                 extracted = m.groups()[0]
                 start = m.start(1)
                 end = m.end(1)
             else:
@@ -118,14 +120,16 @@
                     accum = 0
                     for m in COMMENT_RE.finditer(markdown[:start]):
                         comment_len = m.end() - m.start()
                         accum += comment_len
                     start -= accum
                     end -= accum
                 result.append((extracted, start, end))
+                if optimize:
+                    break
         return result
 
 
 ExtractDict = NewType("ExtractDict", Dict[str, Tuple[int, int]])
 
 
 class ExtractItemLoader(ItemLoader):
@@ -155,24 +159,24 @@
         flags: int = 0,
         skip_prefix: str = DEFAULT_SKIP_PREFIX,
         strict_tid: bool = False,
         *processors,
         **kw,
     ):
         extracted = self.context["response"].text_re(
-            reg=reg, tid=tid, flags=flags, skip_prefix=skip_prefix, strict_tid=strict_tid
+            reg=reg, tid=tid, flags=flags, skip_prefix=skip_prefix, strict_tid=strict_tid, optimize=True
         )
         if extracted:
             t, s, e = extracted[0]
             if attr not in self.extract_indexes:
                 self.extract_indexes[attr] = (s, e)
                 self.add_value(attr, t, *processors, **kw)
 
     def add_text_re_as_html(self, attr: str, reg: str, flags: int = 0, *processors, **kw):
-        extracted = self.context["response"].text_re(reg, flags=flags)
+        extracted = self.context["response"].text_re(reg, flags=flags, optimize=True)
         if extracted:
             t, s, e = extracted[0]
             if attr not in self.extract_indexes:
                 cleaned = self._mconverter.convert(t).strip()
                 self.add_value(attr, cleaned, *processors, **kw)
                 self.extract_indexes[attr] = (s, e)
```

### Comparing `e-models-1.1/setup.py` & `e-models-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.1',
+    version      = '1.1.1',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.1/tests/test_scrapyutils.py` & `e-models-1.1.1/tests/test_scrapyutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         )
         self.assertEqual(data["markdown"][slice(*data["indexes"]["job_id"])], "492556")
         self.assertEqual(data["markdown"][slice(*data["indexes"]["employment_type"])], "Full-time Staff")
 
         self.assertEqual(data["markdown"][slice(*data["indexes"]["description"])], item["description"])
         self.assertEqual(data["markdown"][slice(*data["indexes"]["description_as_html"])], item["description"])
 
+        self.assertTrue(response.text_re(tid=".job-field job-title"))
+
     def test_example_two(self):
         sample_file = os.path.join(SAMPLES_DIR, "yell.html")
         body = open(sample_file).read().encode("utf8")
         response = ExtractTextResponse(url="https://yell.com/result.html", body=body, status=200)
 
         for r in response.css_split(".businessCapsule--mainRow"):
             loader = BusinessSearchItemLoader(response=r)
```

