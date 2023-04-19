# Comparing `tmp/ai21-1.0.4.tar.gz` & `tmp/ai21-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ai21-1.0.4.tar", last modified: Mon Apr 10 09:45:55 2023, max compression
+gzip compressed data, was "ai21-1.0.5.tar", last modified: Wed Apr 19 09:59:09 2023, max compression
```

## Comparing `ai21-1.0.4.tar` & `ai21-1.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-04-10 09:45:55.000000 ai21-1.0.4/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2600 2023-04-10 09:05:28.000000 ai21-1.0.4/README.md
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      576 2023-03-27 12:47:23.000000 ai21-1.0.4/setup.py
--rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      107 2023-04-10 09:45:55.000000 ai21-1.0.4/setup.cfg
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/ai21_object.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-04-10 09:39:56.000000 ai21-1.0.4/ai21/version.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3868 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/http_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      104 2023-04-10 09:05:28.000000 ai21-1.0.4/ai21/constants.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      751 2023-04-10 09:33:18.000000 ai21-1.0.4/ai21/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2590 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/ai21_studio_client.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2100 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/SM_utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/api_resources.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1875 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/utils.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2823 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/errors.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21/modules/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      771 2023-04-10 09:33:08.000000 ai21-1.0.4/ai21/modules/question_answering.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1375 2023-04-10 09:05:28.000000 ai21-1.0.4/ai21/modules/completion.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1823 2023-04-10 09:18:41.000000 ai21-1.0.4/ai21/modules/experimantal.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/custom_model.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21/modules/resources/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1208 2023-04-10 09:05:28.000000 ai21-1.0.4/ai21/modules/resources/nlp_task.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/listable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/creatable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/retrievable_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/upload_resource.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/resources/ai21_module.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/__init__.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      461 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/tokenization.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      678 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/improvements.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      795 2023-04-10 09:35:40.000000 ai21-1.0.4/ai21/modules/summarize.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      536 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/gec.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/dataset.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/paraphrase.py
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      611 2023-03-25 06:53:34.000000 ai21-1.0.4/ai21/modules/segmentation.py
-drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-10 09:45:55.000000 ai21-1.0.4/ai21.egg-info/
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/PKG-INFO
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)      968 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/SOURCES.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)       21 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/requires.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/top_level.txt
--rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-04-10 09:45:54.000000 ai21-1.0.4/ai21.egg-info/dependency_links.txt
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-19 09:59:09.655881 ai21-1.0.5/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-04-19 09:59:09.655985 ai21-1.0.5/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2600 2023-04-10 09:05:28.000000 ai21-1.0.5/README.md
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-19 09:59:09.645835 ai21-1.0.5/ai21/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2100 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/SM_utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      751 2023-04-19 09:02:11.000000 ai21-1.0.5/ai21/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      971 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/ai21_object.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2590 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/ai21_studio_client.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      473 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/api_resources.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      104 2023-04-10 09:05:28.000000 ai21-1.0.5/ai21/constants.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2823 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/errors.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     3868 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/http_client.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-19 09:59:09.651899 ai21-1.0.5/ai21/modules/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1375 2023-04-10 09:05:28.000000 ai21-1.0.5/ai21/modules/completion.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      856 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/custom_model.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      646 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/dataset.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     2167 2023-04-19 09:07:47.000000 ai21-1.0.5/ai21/modules/experimental.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      650 2023-04-19 09:13:33.000000 ai21-1.0.5/ai21/modules/gec.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      654 2023-04-19 09:13:40.000000 ai21-1.0.5/ai21/modules/improvements.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      664 2023-04-19 09:12:58.000000 ai21-1.0.5/ai21/modules/paraphrase.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      771 2023-04-19 08:57:55.000000 ai21-1.0.5/ai21/modules/question_answering.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-19 09:59:09.655666 ai21-1.0.5/ai21/modules/resources/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        0 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/resources/__init__.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      585 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/resources/ai21_module.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      371 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/resources/creatable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      352 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/resources/listable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1208 2023-04-10 09:05:28.000000 ai21-1.0.5/ai21/modules/resources/nlp_task.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      387 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/resources/retrievable_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      476 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/resources/upload_resource.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      611 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/segmentation.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      795 2023-04-10 09:35:40.000000 ai21-1.0.5/ai21/modules/summarize.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      461 2023-03-25 06:53:34.000000 ai21-1.0.5/ai21/modules/tokenization.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)     1875 2023-04-19 09:08:00.000000 ai21-1.0.5/ai21/utils.py
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       22 2023-04-19 09:59:04.000000 ai21-1.0.5/ai21/version.py
+drwxr-xr-x   0 amirkoblyansky   (501) staff       (20)        0 2023-04-19 09:59:09.647325 ai21-1.0.5/ai21.egg-info/
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      204 2023-04-19 09:59:09.000000 ai21-1.0.5/ai21.egg-info/PKG-INFO
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)      968 2023-04-19 09:59:09.000000 ai21-1.0.5/ai21.egg-info/SOURCES.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        1 2023-04-19 09:59:09.000000 ai21-1.0.5/ai21.egg-info/dependency_links.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)       21 2023-04-19 09:59:09.000000 ai21-1.0.5/ai21.egg-info/requires.txt
+-rw-r--r--   0 amirkoblyansky   (501) staff       (20)        5 2023-04-19 09:59:09.000000 ai21-1.0.5/ai21.egg-info/top_level.txt
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      107 2023-04-19 09:59:09.656304 ai21-1.0.5/setup.cfg
+-rwxr-xr-x   0 amirkoblyansky   (501) staff       (20)      576 2023-03-27 12:47:23.000000 ai21-1.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ai21-1.0.4/README.md` & `ai21-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/setup.py` & `ai21-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/ai21_object.py` & `ai21-1.0.5/ai21/ai21_object.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/http_client.py` & `ai21-1.0.5/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/__init__.py` & `ai21-1.0.5/ai21/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ai21.constants import STUDIO_HOST, DEFAULT_API_VERSION
 from ai21.modules.completion import Completion
 from ai21.modules.dataset import Dataset
 from ai21.modules.tokenization import Tokenization
 from ai21.modules.custom_model import CustomModel
-from ai21.modules.experimantal import Experimental
+from ai21.modules.experimental import Experimental
 from ai21.modules.paraphrase import Paraphrase
 from ai21.modules.summarize import Summarize
 from ai21.modules.segmentation import Segmentation
 from ai21.modules.improvements import Improvements
 from ai21.modules.question_answering import Answer
 from ai21.modules.gec import GEC
```

### Comparing `ai21-1.0.4/ai21/ai21_studio_client.py` & `ai21-1.0.5/ai21/ai21_studio_client.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/SM_utils.py` & `ai21-1.0.5/ai21/SM_utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/utils.py` & `ai21-1.0.5/ai21/utils.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/errors.py` & `ai21-1.0.5/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/question_answering.py` & `ai21-1.0.5/ai21/modules/question_answering.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/completion.py` & `ai21-1.0.5/ai21/modules/completion.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/experimantal.py` & `ai21-1.0.5/ai21/modules/experimental.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from ai21 import Completion
 from ai21.constants import SAGEMAKER_ENDPOINT_KEY
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
 class Experimental(NLPTask):
@@ -22,14 +24,21 @@
     def summarize(cls, **params):
         validate_mandatory_field(key='text', call_name="summarize_experimental", params=params, validate_type=True, expected_type=str)
         url = cls.get_base_url(**params)
         url = f'{url}/experimental/summarize'
         return super().execute(task_url=url, **params)
 
     @classmethod
+    def embed(cls, **params):
+        validate_mandatory_field(key='texts', call_name="embed_experimental", params=params, validate_type=True, expected_type=list)
+        url = cls.get_base_url(**params)
+        url = f'{url}/experimental/embed'
+        return super().execute(task_url=url, **params)
+
+    @classmethod
     def j1_grande_instruct(cls, **params):
         params["model"] = "j1-grande-instruct"
         return Completion.execute(experimental_mode=True, **params)
 
     @classmethod
     def answer(cls, **params):
         validate_mandatory_field(key='context', call_name="answer_experimental", params=params, validate_type=True, expected_type=str)
```

### Comparing `ai21-1.0.4/ai21/modules/custom_model.py` & `ai21-1.0.5/ai21/modules/custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/resources/nlp_task.py` & `ai21-1.0.5/ai21/modules/resources/nlp_task.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/resources/ai21_module.py` & `ai21-1.0.5/ai21/modules/resources/ai21_module.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/improvements.py` & `ai21-1.0.5/ai21/modules/improvements.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List
 
 from ai21.errors import EmptyMandatoryListException
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
 class Improvements(NLPTask):
```

### Comparing `ai21-1.0.4/ai21/modules/summarize.py` & `ai21-1.0.5/ai21/modules/summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/gec.py` & `ai21-1.0.5/ai21/modules/segmentation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-from typing import List
-
-from ai21.errors import EmptyMandatoryListException
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class GEC(NLPTask):
-    MODULE_NAME = 'gec'
+class Segmentation(NLPTask):
+    MODULE_NAME = 'segmentation'
 
     @classmethod
     def execute(cls, **params):
-        validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
+        validate_mandatory_field(key='sourceType', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
+        validate_mandatory_field(key='source', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
         return super().execute(task_url=url, **params)
```

### Comparing `ai21-1.0.4/ai21/modules/dataset.py` & `ai21-1.0.5/ai21/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-1.0.4/ai21/modules/segmentation.py` & `ai21-1.0.5/ai21/modules/gec.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from ai21.constants import SAGEMAKER_ENDPOINT_KEY
+
 from ai21.modules.resources.nlp_task import NLPTask
 from ai21.utils import validate_mandatory_field
 
 
-class Segmentation(NLPTask):
-    MODULE_NAME = 'segmentation'
+class GEC(NLPTask):
+    MODULE_NAME = 'gec'
 
     @classmethod
     def execute(cls, **params):
-        validate_mandatory_field(key='sourceType', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
-        validate_mandatory_field(key='source', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
+        validate_mandatory_field(key='text', call_name=cls.MODULE_NAME, params=params, validate_type=True, expected_type=str)
+        use_sm_endpoint = SAGEMAKER_ENDPOINT_KEY in params
+        if use_sm_endpoint:
+            return cls.execute_sm_endpoint(**params)
         url = cls.get_base_url(**params)
         url = f'{url}/{cls.MODULE_NAME}'
         return super().execute(task_url=url, **params)
```

### Comparing `ai21-1.0.4/ai21.egg-info/SOURCES.txt` & `ai21-1.0.5/ai21.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ai21.egg-info/dependency_links.txt
 ai21.egg-info/requires.txt
 ai21.egg-info/top_level.txt
 ai21/modules/__init__.py
 ai21/modules/completion.py
 ai21/modules/custom_model.py
 ai21/modules/dataset.py
-ai21/modules/experimantal.py
+ai21/modules/experimental.py
 ai21/modules/gec.py
 ai21/modules/improvements.py
 ai21/modules/paraphrase.py
 ai21/modules/question_answering.py
 ai21/modules/segmentation.py
 ai21/modules/summarize.py
 ai21/modules/tokenization.py
```

