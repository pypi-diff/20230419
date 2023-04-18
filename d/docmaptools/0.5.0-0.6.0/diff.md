# Comparing `tmp/docmaptools-0.5.0.tar.gz` & `tmp/docmaptools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmaptools-0.5.0.tar", last modified: Mon Mar 13 21:18:27 2023, max compression
+gzip compressed data, was "docmaptools-0.6.0.tar", last modified: Tue Apr 18 22:51:52 2023, max compression
```

## Comparing `docmaptools-0.5.0.tar` & `docmaptools-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-03-13 21:18:27.900212 docmaptools-0.5.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-03-13 21:17:54.000000 docmaptools-0.5.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-03-13 21:17:54.000000 docmaptools-0.5.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-03-13 21:18:27.900212 docmaptools-0.5.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-03-13 21:17:54.000000 docmaptools-0.5.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-03-13 21:18:27.900212 docmaptools-0.5.0/docmaptools/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-03-13 21:17:54.000000 docmaptools-0.5.0/docmaptools/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-03-13 21:17:54.000000 docmaptools-0.5.0/docmaptools/convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     4498 2023-03-13 21:17:54.000000 docmaptools-0.5.0/docmaptools/parse.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-03-13 21:18:27.900212 docmaptools-0.5.0/docmaptools.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-03-13 21:18:27.000000 docmaptools-0.5.0/docmaptools.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-03-13 21:18:27.000000 docmaptools-0.5.0/docmaptools.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-03-13 21:18:27.000000 docmaptools-0.5.0/docmaptools.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-03-13 21:18:27.000000 docmaptools-0.5.0/docmaptools.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-03-13 21:18:27.000000 docmaptools-0.5.0/docmaptools.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-03-13 21:17:54.000000 docmaptools-0.5.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-03-13 21:18:27.900212 docmaptools-0.5.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-03-13 21:17:54.000000 docmaptools-0.5.0/setup.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-03-13 21:18:27.900212 docmaptools-0.5.0/tests/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-03-13 21:17:54.000000 docmaptools-0.5.0/tests/test_convert.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-03-13 21:17:54.000000 docmaptools-0.5.0/tests/test_init.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    18512 2023-03-13 21:17:54.000000 docmaptools-0.5.0/tests/test_parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1088 2023-04-18 22:51:22.000000 docmaptools-0.6.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2023-04-18 22:51:22.000000 docmaptools-0.6.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-18 22:51:52.379190 docmaptools-0.6.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       90 2023-04-18 22:51:22.000000 docmaptools-0.6.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/docmaptools/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      543 2023-04-18 22:51:22.000000 docmaptools-0.6.0/docmaptools/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     4796 2023-04-18 22:51:22.000000 docmaptools-0.6.0/docmaptools/convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     5293 2023-04-18 22:51:22.000000 docmaptools-0.6.0/docmaptools/parse.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/docmaptools.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      643 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      358 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       20 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       12 2023-04-18 22:51:52.000000 docmaptools-0.6.0/docmaptools.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       78 2023-04-18 22:51:22.000000 docmaptools-0.6.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2023-04-18 22:51:52.379190 docmaptools-0.6.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      840 2023-04-18 22:51:22.000000 docmaptools-0.6.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2023-04-18 22:51:52.379190 docmaptools-0.6.0/tests/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     8341 2023-04-18 22:51:22.000000 docmaptools-0.6.0/tests/test_convert.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      710 2023-04-18 22:51:22.000000 docmaptools-0.6.0/tests/test_init.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    24022 2023-04-18 22:51:22.000000 docmaptools-0.6.0/tests/test_parse.py
```

### Comparing `docmaptools-0.5.0/LICENSE` & `docmaptools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docmaptools-0.5.0/PKG-INFO` & `docmaptools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.5.0/docmaptools/__init__.py` & `docmaptools-0.6.0/docmaptools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
 
 
 def configure_logging(filename, level=logging.INFO, format_string=None):
```

### Comparing `docmaptools-0.5.0/docmaptools/convert.py` & `docmaptools-0.6.0/docmaptools/convert.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.5.0/docmaptools/parse.py` & `docmaptools-0.6.0/docmaptools/parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,14 +54,36 @@
             outputs = action_outputs(action)
             for output in outputs:
                 if output.get("type") == "preprint":
                     return output
     return {}
 
 
+def docmap_latest_preprint(d_json):
+    "find the most recent preprint in the docmap"
+    step = docmap_first_step(d_json)
+    most_recent_output = {}
+    if step and step.get("inputs"):
+        # assume the preprint data is the first step first inputs value
+        most_recent_output = step_inputs(step)[0]
+    # continue to search
+    step = next_step(d_json, step)
+    while step:
+        actions = step_actions(step)
+        for action in actions:
+            outputs = action_outputs(action)
+            for output in outputs:
+                if output.get("type") == "preprint":
+                    # remember this value
+                    most_recent_output = output
+        # search the next step
+        step = next_step(d_json, step)
+    return most_recent_output
+
+
 def step_actions(step_json):
     "return the actions of the step"
     return step_json.get("actions")
 
 
 def action_outputs(action_json):
     "return the outputs of an action"
@@ -89,24 +111,26 @@
     # look at the first item in the list for now
     return output_content(outputs[0])
 
 
 def content_step(d_json):
     "find the step which includes peer review content data"
     step = docmap_first_step(d_json)
+    step_previous = None
     while step:
         actions = step_actions(step)
         for action in actions:
             outputs = action_outputs(action)
             for output in outputs:
                 if output.get("type") == "review-article":
-                    # return the first step found which has review-article content
-                    return step
+                    # remember this step
+                    step_previous = step
         # search the next step
         step = next_step(d_json, step)
+    return step_previous
 
 
 def docmap_content(d_json):
     "abbreviated and simplified data for content outputs"
     content = []
     # the step from which to get the data
     step = content_step(d_json)
```

### Comparing `docmaptools-0.5.0/docmaptools.egg-info/PKG-INFO` & `docmaptools-0.6.0/docmaptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmaptools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Use DocMap content, generate JATS XML from it, and other utility functions.
 Home-page: https://github.com/elifesciences/docmap-tools
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `docmaptools-0.5.0/setup.py` & `docmaptools-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.5.0/tests/test_convert.py` & `docmaptools-0.6.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.5.0/tests/test_init.py` & `docmaptools-0.6.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `docmaptools-0.5.0/tests/test_parse.py` & `docmaptools-0.6.0/tests/test_parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,14 +80,141 @@
         docmap_string = read_fixture("2022.10.17.512253.docmap.json", mode="r")
         result = parse.docmap_json(docmap_string)
         # some simple assertions
         self.assertEqual(result.get("first-step"), "_:b0")
         self.assertEqual(len(result.get("steps")), 3)
 
 
+class TestDocmapSteps85111Sample(unittest.TestCase):
+    def setUp(self):
+        docmap_string = read_fixture("sample_docmap_for_85111.json", mode="r")
+        self.d_json = json.loads(docmap_string)
+
+    def test_docmap_steps(self):
+        "get the steps of the docmap"
+        result = parse.docmap_steps(self.d_json)
+        self.assertEqual(len(result), 5)
+
+    def test_docmap_first_step(self):
+        "get the first step according to the first-step value"
+        result = parse.docmap_first_step(self.d_json)
+
+        self.assertEqual(len(result), 4)
+        self.assertEqual(
+            sorted(result.keys()), ["actions", "assertions", "inputs", "next-step"]
+        )
+
+    def test_step_inputs(self):
+        "get inputs from the first step"
+        first_step = parse.docmap_first_step(self.d_json)
+        result = parse.step_inputs(first_step)
+        self.assertEqual(len(result), 0)
+        # step _:b1
+        step_1 = parse.next_step(self.d_json, first_step)
+        result = parse.step_inputs(step_1)
+        self.assertEqual(len(result), 1)
+        # step _:b2
+        step_2 = parse.next_step(self.d_json, step_1)
+        result = parse.step_inputs(step_2)
+        self.assertEqual(len(result), 1)
+        # step _:b3
+        step_3 = parse.next_step(self.d_json, step_2)
+        result = parse.step_inputs(step_3)
+        self.assertEqual(len(result), 0)
+        # step _:b4
+        step_4 = parse.next_step(self.d_json, step_3)
+        result = parse.step_inputs(step_4)
+        self.assertEqual(len(result), 5)
+        self.assertEqual(step_4.get("next-step"), None)
+
+    def test_docmap_preprint(self):
+        "preprint data from the first step inputs"
+        result = parse.docmap_preprint(self.d_json)
+        self.assertDictEqual(
+            result,
+            {
+                "type": "preprint",
+                "doi": "10.1101/2022.11.08.515698",
+                "url": "https://www.biorxiv.org/content/10.1101/2022.11.08.515698v2",
+                "published": "2022-11-22",
+                "versionIdentifier": "2",
+                "_tdmPath": "s3://transfers-elife/biorxiv_Current_Content/November_2022/23_Nov_22_Batch_1444/b0f4d90b-6c92-1014-9a2e-aae015926ab4.meca",
+            },
+        )
+
+    def test_docmap_latest_preprint(self):
+        "preprint data from the most recent step inputs"
+        result = parse.docmap_latest_preprint(self.d_json)
+        self.assertDictEqual(
+            result,
+            {
+                "type": "preprint",
+                "identifier": "85111",
+                "versionIdentifier": "2",
+                "doi": "10.7554/eLife.85111.2",
+            },
+        )
+
+    def test_step_actions(self):
+        "get actions from the last step"
+        step_2 = parse.next_step(
+            self.d_json,
+            parse.next_step(self.d_json, parse.docmap_first_step(self.d_json)),
+        )
+        result = parse.step_actions(step_2)
+        self.assertEqual(len(result), 4)
+
+    def test_action_outputs(self):
+        "outputs from a step action"
+        first_step = parse.docmap_first_step(self.d_json)
+        first_action = parse.step_actions(first_step)[0]
+        result = parse.action_outputs(first_action)
+        self.assertEqual(len(result), 1)
+
+    def test_docmap_content(self):
+        "test parsing docmap JSON into docmap content structure"
+        result = parse.docmap_content(self.d_json)
+        expected = [
+            OrderedDict(
+                [("type", "preprint"), ("published", None), ("web-content", None)]
+            ),
+            OrderedDict(
+                [
+                    ("type", "review-article"),
+                    ("published", "2023-04-14T13:42:24.130023+00:00"),
+                    (
+                        "web-content",
+                        "https://sciety.org/evaluations/hypothesis:L_wlTNrKEe25pKupBGTeqA/content",
+                    ),
+                ]
+            ),
+            OrderedDict(
+                [
+                    ("type", "review-article"),
+                    ("published", "2023-04-14T13:42:24.975810+00:00"),
+                    (
+                        "web-content",
+                        "https://sciety.org/evaluations/hypothesis:MHuA2trKEe2NmT9GM4xGlw/content",
+                    ),
+                ]
+            ),
+            OrderedDict(
+                [
+                    ("type", "evaluation-summary"),
+                    ("published", "2023-04-14T13:42:25.781585+00:00"),
+                    (
+                        "web-content",
+                        "https://sciety.org/evaluations/hypothesis:MPYp6NrKEe2anmsrxlBg-w/content",
+                    ),
+                ]
+            ),
+        ]
+        self.assertEqual(result, expected)
+
+
 class TestDocmapPreprint(unittest.TestCase):
     def test_docmap_preprint(self):
         "test case for when there is empty input"
         self.assertEqual(parse.docmap_preprint({}), {})
 
 
 class TestDocmapSteps446694(unittest.TestCase):
@@ -119,14 +246,25 @@
             result,
             {
                 "doi": "10.1101/2021.06.02.446694",
                 "url": "https://doi.org/10.1101/2021.06.02.446694",
             },
         )
 
+    def test_docmap_latest_preprint(self):
+        "preprint data from the most recent step inputs"
+        result = parse.docmap_latest_preprint(self.d_json)
+        self.assertDictEqual(
+            result,
+            {
+                "doi": "10.1101/2021.06.02.446694",
+                "url": "https://doi.org/10.1101/2021.06.02.446694",
+            },
+        )
+
     def test_step_actions(self):
         "get actions from the first step"
         first_step = parse.docmap_first_step(self.d_json)
         result = parse.step_actions(first_step)
         self.assertEqual(len(result), 5)
 
     def test_action_outputs(self):
@@ -290,14 +428,27 @@
                 "url": "https://www.biorxiv.org/content/10.1101/2022.10.17.512253v1",
                 "published": "2022-10-17",
                 "versionIdentifier": "1",
                 "_tdmPath": "s3://transfers-elife/biorxiv_Current_Content/October_2022/18_Oct_22_Batch_1408/a6575018-6cfe-1014-94b3-ca3c122c1e09.meca",
             },
         )
 
+    def test_docmap_latest_preprint(self):
+        "preprint data from the most recent step inputs"
+        result = parse.docmap_latest_preprint(self.d_json)
+        self.assertDictEqual(
+            result,
+            {
+                "identifier": "84364",
+                "versionIdentifier": "",
+                "type": "preprint",
+                "doi": "10.7554/eLife.84364",
+            },
+        )
+
     def test_step_actions(self):
         "get actions from the last step"
         step_2 = parse.next_step(
             self.d_json,
             parse.next_step(self.d_json, parse.docmap_first_step(self.d_json)),
         )
         result = parse.step_actions(step_2)
```

