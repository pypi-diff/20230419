# Comparing `tmp/raidtoolkit-0.1.0.tar.gz` & `tmp/raidtoolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raidtoolkit-0.1.0.tar", last modified: Sat Mar 19 17:31:46 2022, max compression
+gzip compressed data, was "raidtoolkit-0.2.0.tar", last modified: Wed Apr 19 04:06:03 2023, max compression
```

## Comparing `raidtoolkit-0.1.0.tar` & `raidtoolkit-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 17:31:46.898129 raidtoolkit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-03-19 17:31:46.898129 raidtoolkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-03-19 17:31:46.898129 raidtoolkit-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 17:31:46.894129 raidtoolkit-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 17:31:46.894129 raidtoolkit-0.1.0/src/raidtoolkit/
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/AccountApi.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/PromiseStore.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/RaidToolkit.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/RealtimeApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/RemoteApiClient.py
--rw-r--r--   0 runner    (1001) docker     (121)      818 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/StaticDataApi.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-03-19 17:31:28.000000 raidtoolkit-0.1.0/src/raidtoolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-19 17:31:46.898129 raidtoolkit-0.1.0/src/raidtoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-03-19 17:31:46.000000 raidtoolkit-0.1.0/src/raidtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-03-19 17:31:46.000000 raidtoolkit-0.1.0/src/raidtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-19 17:31:46.000000 raidtoolkit-0.1.0/src/raidtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-19 17:31:46.000000 raidtoolkit-0.1.0/src/raidtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:03.562948 raidtoolkit-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-19 04:06:03.562948 raidtoolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 04:06:03.562948 raidtoolkit-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:03.558948 raidtoolkit-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:03.562948 raidtoolkit-0.2.0/src/raidtoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/Account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/AccountApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/PromiseStore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/RaidToolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/RealtimeApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/RemoteApiClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/StaticDataApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 04:05:48.000000 raidtoolkit-0.2.0/src/raidtoolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 04:06:03.562948 raidtoolkit-0.2.0/src/raidtoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-19 04:06:03.000000 raidtoolkit-0.2.0/src/raidtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 04:06:03.000000 raidtoolkit-0.2.0/src/raidtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 04:06:03.000000 raidtoolkit-0.2.0/src/raidtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 04:06:03.000000 raidtoolkit-0.2.0/src/raidtoolkit.egg-info/top_level.txt
```

### Comparing `raidtoolkit-0.1.0/LICENSE` & `raidtoolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `raidtoolkit-0.1.0/PKG-INFO` & `raidtoolkit-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: raidtoolkit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Client for RaidToolkit API access
 Home-page: https://github.com/raid-toolkit/raid-toolkit-sdk
-Author: dnchattan
-Author-email: dnchattan@gmail.com
-License: UNKNOWN
+Author: raid.toolkit
+Author-email: raid.toolkit@gmail.com
 Project-URL: Bug Tracker, https://github.com/raid-toolkit/raid-toolkit-sdk/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -57,9 +55,7 @@
 | `getAccountDump(accountId)` | Get an account dump for a given `accountId`, in RaidExtractor format. |
 | `getArtifacts(accountId)` | Get all artifacts for a given `accountId` |
 | `getArtifactById(accountId, artifactId)` | Get an artifact by id |
 | `getHeroes(accountId)` | Get all heroes for a given `accountId` |
 | `getHeroById(accountId, heroId)` | Get a hero by id |
 | `getAllResources(accountId)` | Get all resources for a given `accountId` |
 
-
-
```

### Comparing `raidtoolkit-0.1.0/README.md` & `raidtoolkit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `raidtoolkit-0.1.0/setup.cfg` & `raidtoolkit-0.2.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = raidtoolkit
-version = 0.1.0
-author = dnchattan
-author_email = dnchattan@gmail.com
+version = 0.2.0
+author = raid.toolkit
+author_email = raid.toolkit@gmail.com
 description = Client for RaidToolkit API access
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/raid-toolkit/raid-toolkit-sdk
 project_urls = 
 	Bug Tracker = https://github.com/raid-toolkit/raid-toolkit-sdk/issues
 classifiers =
```

### Comparing `raidtoolkit-0.1.0/src/raidtoolkit/AccountApi.py` & `raidtoolkit-0.2.0/src/raidtoolkit/AccountApi.py`

 * *Files identical despite different names*

### Comparing `raidtoolkit-0.1.0/src/raidtoolkit/PromiseStore.py` & `raidtoolkit-0.2.0/src/raidtoolkit/PromiseStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
         self.Promises[id] = DeferredPromise()
         return id
 
     def complete(self, id: str, value: any):
         self.Promises[id].set_result(value)
 
     def fail(self, id: str, error: any):
-        self.Promises[id].set_exception(error)
+        self.Promises[id].set_exception(ValueError(error))
 
     def get(self, id: str):
         return self.Promises[id].promise
```

### Comparing `raidtoolkit-0.1.0/src/raidtoolkit/RemoteApiClient.py` & `raidtoolkit-0.2.0/src/raidtoolkit/RemoteApiClient.py`

 * *Files identical despite different names*

### Comparing `raidtoolkit-0.1.0/src/raidtoolkit/StaticDataApi.py` & `raidtoolkit-0.2.0/src/raidtoolkit/StaticDataApi.py`

 * *Files identical despite different names*

### Comparing `raidtoolkit-0.1.0/src/raidtoolkit.egg-info/PKG-INFO` & `raidtoolkit-0.2.0/src/raidtoolkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: raidtoolkit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Client for RaidToolkit API access
 Home-page: https://github.com/raid-toolkit/raid-toolkit-sdk
-Author: dnchattan
-Author-email: dnchattan@gmail.com
-License: UNKNOWN
+Author: raid.toolkit
+Author-email: raid.toolkit@gmail.com
 Project-URL: Bug Tracker, https://github.com/raid-toolkit/raid-toolkit-sdk/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -57,9 +55,7 @@
 | `getAccountDump(accountId)` | Get an account dump for a given `accountId`, in RaidExtractor format. |
 | `getArtifacts(accountId)` | Get all artifacts for a given `accountId` |
 | `getArtifactById(accountId, artifactId)` | Get an artifact by id |
 | `getHeroes(accountId)` | Get all heroes for a given `accountId` |
 | `getHeroById(accountId, heroId)` | Get a hero by id |
 | `getAllResources(accountId)` | Get all resources for a given `accountId` |
 
-
-
```

