# Comparing `tmp/hcf-backend-0.5.2.1.tar.gz` & `tmp/hcf-backend-0.5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcf-backend-0.5.2.1.tar", last modified: Mon Apr 17 02:31:52 2023, max compression
+gzip compressed data, was "hcf-backend-0.5.2.2.tar", last modified: Wed Apr 19 11:52:16 2023, max compression
```

## Comparing `hcf-backend-0.5.2.1.tar` & `hcf-backend-0.5.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.518352 hcf-backend-0.5.2.1/hcf_backend/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       48 2023-04-17 02:30:13.000000 hcf-backend-0.5.2.1/hcf_backend/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2.1/hcf_backend/backend.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4529 2023-04-13 17:18:18.000000 hcf-backend-0.5.2.1/hcf_backend/manager.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/hcf_backend/utils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2.1/hcf_backend/utils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4003 2023-04-17 02:24:22.000000 hcf-backend-0.5.2.1/hcf_backend/utils/crawlmanager.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13380 2023-04-13 16:12:38.000000 hcf-backend-0.5.2.1/hcf_backend/utils/hcfpal.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-17 02:31:52.518352 hcf-backend-0.5.2.1/hcf_backend.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-17 02:31:52.000000 hcf-backend-0.5.2.1/hcf_backend.egg-info/top_level.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-17 02:31:52.522353 hcf-backend-0.5.2.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1014 2023-04-17 02:30:02.000000 hcf-backend-0.5.2.1/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)     1478 2019-01-31 18:02:16.000000 hcf-backend-0.5.2.2/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2067 2023-04-11 20:57:08.000000 hcf-backend-0.5.2.2/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.835138 hcf-backend-0.5.2.2/hcf_backend/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       48 2023-04-19 11:51:45.000000 hcf-backend-0.5.2.2/hcf_backend/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    14039 2023-04-13 16:11:52.000000 hcf-backend-0.5.2.2/hcf_backend/backend.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4529 2023-04-13 17:18:18.000000 hcf-backend-0.5.2.2/hcf_backend/manager.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/hcf_backend/utils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1566 2023-04-11 21:18:45.000000 hcf-backend-0.5.2.2/hcf_backend/utils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4003 2023-04-17 02:24:22.000000 hcf-backend-0.5.2.2/hcf_backend/utils/crawlmanager.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    13590 2023-04-19 11:51:04.000000 hcf-backend-0.5.2.2/hcf_backend/utils/hcfpal.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/hcf_backend.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2688 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      377 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      107 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       12 2023-04-19 11:52:16.000000 hcf-backend-0.5.2.2/hcf_backend.egg-info/top_level.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2021-07-13 00:16:34.000000 hcf-backend-0.5.2.2/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-04-19 11:52:16.839138 hcf-backend-0.5.2.2/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1014 2023-04-19 11:51:36.000000 hcf-backend-0.5.2.2/setup.py
```

### Comparing `hcf-backend-0.5.2.1/LICENSE` & `hcf-backend-0.5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.1/PKG-INFO` & `hcf-backend-0.5.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.2.1
+Version: 0.5.2.2
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.2.1/README.md` & `hcf-backend-0.5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.1/hcf_backend/backend.py` & `hcf-backend-0.5.2.2/hcf_backend/backend.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.1/hcf_backend/manager.py` & `hcf-backend-0.5.2.2/hcf_backend/manager.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.1/hcf_backend/utils/__init__.py` & `hcf-backend-0.5.2.2/hcf_backend/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.1/hcf_backend/utils/crawlmanager.py` & `hcf-backend-0.5.2.2/hcf_backend/utils/crawlmanager.py`

 * *Files identical despite different names*

### Comparing `hcf-backend-0.5.2.1/hcf_backend/utils/hcfpal.py` & `hcf-backend-0.5.2.2/hcf_backend/utils/hcfpal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import re
 import pprint
 from itertools import cycle, groupby
 from operator import itemgetter
-from typing import Optional
+from typing import Optional, TypedDict, Dict
 
 import humanize
 import requests
 from requests.auth import HTTPBasicAuth
 from shub_workflow.script import BaseScript, SCProjectClass
 from shub_workflow.utils import dash_retry_decorator
 
 from hcf_backend.utils import assign_slotno
 
 
+class SlotsInfo(TypedDict):
+    slots: Dict[str, int]
+    total: int
+    not_empty_slots: int
+
+
 class HCFPal(SCProjectClass):
 
     HCF_API_URLS = {
         "count": "https://storage.scrapinghub.com/hcf/{pid}/{frontier}/s/{slot}/q/count",
         "list_frontiers": "https://storage.scrapinghub.com/hcf/{pid}/list",
         "list_slots": "https://storage.scrapinghub.com/hcf/{pid}/{frontier}/list",
     }
@@ -67,31 +73,31 @@
             data = self._get_json(next_url)
             total += int(data.get("count"))
             nextstart = data.get("nextstart", "")
             if not nextstart:
                 break
         return total
 
-    def get_slots_count(self, frontier, prefix, num_slots=None, regex=""):
-        result = {"slots": {}}
+    def get_slots_count(self, frontier, prefix, num_slots: Optional[int] = None, regex: str = "") -> SlotsInfo:
+        result: SlotsInfo = {"slots": {}, "total": 0, "not_empty_slots": 0}
         total = 0
         not_empty_slots = 0
         slots = ["{}{}".format(prefix, slot) for slot in range(num_slots)] if num_slots else self.get_slots(frontier)
         for slot in slots:
             if not slot.startswith(prefix):
                 continue
             if not re.search(regex, slot):
                 continue
             cnt = self.get_slot_count(frontier, slot)
             if cnt:
                 not_empty_slots += 1
             total += cnt
             result["slots"][slot] = cnt
         result["total"] = total
-        result["not empty slots"] = not_empty_slots
+        result["not_empty_slots"] = not_empty_slots
         return result
 
     def dump_slot(self, frontier, slot, max_requests):
         count = 0
         for batch in self.project.frontier.read(frontier, slot, max_requests):
             for request in batch["requests"]:
                 yield batch["id"], request
@@ -105,15 +111,15 @@
 
     flow_id_required = False
 
     def __init__(self):
         super().__init__()
         hsc = self.client._hsclient
         self.hsp = hsc.get_project(self.project_id)
-        self.hcf = HCFPal()
+        self.hcf = HCFPal(self.project_id)
 
     @property
     def description(self):
         return "Helper script for accessing HubCrawlFrontier."
 
     def add_argparser_options(self):
         super().add_argparser_options()
@@ -235,15 +241,15 @@
         )
         result = self.hcf.get_slots_count(self.args.frontier, self.args.prefix, self.args.num_slots, self.args.regex)
         for slot in sorted(result["slots"].keys()):
             cnt_text = "\t{}: {}".format(slot, result["slots"][slot])
             print(cnt_text)
         print("\t" + "-" * 25)
         print("\tTotal count: {}".format(humanize.intcomma(result["total"])))
-        print("\tNot-empty slots: {}".format(result["not empty slots"]))
+        print("\tNot-empty slots: {}".format(result["not_empty_slots"]))
 
     def dump_slot(self):
         print(
             "Dumping next {} requests from slot {}, frontier {}, pid {}:".format(
                 self.args.num_requests, self.args.slot, self.args.frontier, self.project_id,
             )
         )
```

### Comparing `hcf-backend-0.5.2.1/hcf_backend.egg-info/PKG-INFO` & `hcf-backend-0.5.2.2/hcf_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcf-backend
-Version: 0.5.2.1
+Version: 0.5.2.2
 Summary: ScrapyCloud HubStorage frontier backend for Frontera
 Home-page: https://github.com/scrapinghub/hcf-backend
 Maintainer: Scrapinghub
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hcf-backend-0.5.2.1/setup.py` & `hcf-backend-0.5.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name="hcf-backend",
-    version="0.5.2.1",
+    version="0.5.2.2",
     description="ScrapyCloud HubStorage frontier backend for Frontera",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/scrapinghub/hcf-backend",
     maintainer="Scrapinghub",
     packages=find_packages(),
```

