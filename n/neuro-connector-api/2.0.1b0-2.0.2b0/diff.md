# Comparing `tmp/neuro-connector-api-2.0.1b0.tar.gz` & `tmp/neuro-connector-api-2.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro-connector-api-2.0.1b0.tar", last modified: Tue Apr 18 16:13:29 2023, max compression
+gzip compressed data, was "neuro-connector-api-2.0.2b0.tar", last modified: Wed Apr 19 13:21:00 2023, max compression
```

## Comparing `neuro-connector-api-2.0.1b0.tar` & `neuro-connector-api-2.0.2b0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:13:29.953517 neuro-connector-api-2.0.1b0/neuro-connector-api/
--rw-r--r--   0 runner    (1001) docker     (123)    18359 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/neuro-connector-api/NeuroConnector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 16:13:29.000000 neuro-connector-api-2.0.1b0/neuro_connector_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:13:29.957517 neuro-connector-api-2.0.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 16:13:17.000000 neuro-connector-api-2.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/neuro-connector-api/
+-rw-r--r--   0 runner    (1001) docker     (123)    18438 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/neuro-connector-api/NeuroConnector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 13:21:00.000000 neuro-connector-api-2.0.2b0/neuro_connector_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:21:00.945897 neuro-connector-api-2.0.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-19 13:20:47.000000 neuro-connector-api-2.0.2b0/setup.py
```

### Comparing `neuro-connector-api-2.0.1b0/LICENSE` & `neuro-connector-api-2.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuro-connector-api-2.0.1b0/neuro-connector-api/NeuroConnector.py` & `neuro-connector-api-2.0.2b0/neuro-connector-api/NeuroConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,20 @@
     requestWrapper = None
     connectionId = None
     organization = None
     jobName = None
     jobNumber = None
     projectName = None
 
-    def __init__(self, url, organizationId, appToken=None):
+    def __init__(self,url, organizationId, appToken=None):
 
-        assert url, "need neuro base url"
-        self.url = url
+        if url is None:
+            self.url = "https://app.myneuro.ai"
+        else:
+            self.url = url
 
         if appToken:
             token = "Bearer " + appToken
         else:
             token = None
 
         self.requestWrapper = RequestWrapper(token=token,
@@ -363,17 +365,17 @@
     def __init__(self, args):
 
         self.args = args
         self.opts = ["-h", "--func=", "--path=", "--url=", "--org=", "--jobName=", "--jobNum=", "--projKey=", "--vcsProj=",
                 "--branch=", "--commitId=", "--label=", "--env=", "--envType=", "--help"]
 
         self.instructions= '\n-h, --help : Help\n'
-        self.instructions = self.instructions + '\nFunction 1 (sendTestResultsJson)\nNeuroConnector --func 1 --path [filePath] --url [baseUrl] --org [organizationId] --jobName [jobName] --jobNum [jobNumber (optional)]\n'
-        self.instructions = self.instructions + '\nFunction 2 (releaseTrigger)\nNeuroConnector --func 2  --url [baseUrl] --org [organizationId] --projKey [projectKey, e.g jira/management] --vcsProj [vcsProject] --branch [branchName] --commitId [commitId] --label [type label, e.g ms/client]\n'
-        self.instructions = self.instructions + '\nFunction 3 (deploymentTrigger)\nNeuroConnector --func 3 --url [baseUrl] --org [organizationId] --projKey [projectKey, e.g jira/management] --vcsProj [vcsProject] --branch [branchName] --commitId [commitId] --label [type label, e.g ms/client]\n'
+        self.instructions = self.instructions + '\nFunction 1 (sendTestResultsJson)\nNeuroConnector --func 1 --org [organizationId] --path [filePath] --jobName [jobName] --jobNum [jobNumber (optional)] --url [baseUrl (optional)]\n'
+        self.instructions = self.instructions + '\nFunction 2 (releaseTrigger)\nNeuroConnector --func 2 --org [organizationId] --projKey [projectKey, e.g jira/management] --vcsProj [vcsProject] --branch [branchName] --commitId [commitId] --label [type label, e.g ms/client] --url [baseUrl (optional)]\n'
+        self.instructions = self.instructions + '\nFunction 3 (deploymentTrigger)\nNeuroConnector --func 2 --org [organizationId] --projKey [projectKey, e.g jira/management] --vcsProj [vcsProject] --branch [branchName] --commitId [commitId] --label [type label, e.g ms/client] --url [baseUrl (optional)]\n'
 
     def getParameterPairsForArgs(self):
         parameterPairs = {}
         for i, arg in enumerate(self.args):
             for opt in self.opts:
                 if opt[-1] == "=" and opt[:-1] == arg:
                     try:
```

