# Comparing `tmp/ortelius-cli-9.3.232.tar.gz` & `tmp/ortelius-cli-9.3.233.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.232.tar", last modified: Tue Apr  4 17:07:10 2023, max compression
+gzip compressed data, was "ortelius-cli-9.3.233.tar", last modified: Tue Apr 18 23:21:59 2023, max compression
```

## Comparing `ortelius-cli-9.3.232.tar` & `ortelius-cli-9.3.233.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-04 17:07:10.454635 ortelius-cli-9.3.232/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-03-09 18:41:03.000000 ortelius-cli-9.3.232/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2021-05-26 22:33:09.000000 ortelius-cli-9.3.232/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    11080 2023-04-04 17:07:10.453950 ortelius-cli-9.3.232/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-03-09 18:39:10.000000 ortelius-cli-9.3.232/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-04 17:07:10.444943 ortelius-cli-9.3.232/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    69517 2023-04-04 17:06:51.000000 ortelius-cli-9.3.232/bin/dh
--rwxr-xr-x   0 steve      (502) staff       (20)     3038 2023-03-23 17:39:44.000000 ortelius-cli-9.3.232/bin/helminfo.sh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-04 17:07:10.446478 ortelius-cli-9.3.232/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2023-04-04 17:06:51.000000 ortelius-cli-9.3.232/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    74480 2023-03-23 17:39:44.000000 ortelius-cli-9.3.232/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-04 17:07:10.450323 ortelius-cli-9.3.232/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23766 2023-03-23 17:39:44.000000 ortelius-cli-9.3.232/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    10508 2023-03-23 17:40:27.000000 ortelius-cli-9.3.232/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-04 17:07:10.453439 ortelius-cli-9.3.232/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    11080 2023-04-04 17:07:10.000000 ortelius-cli-9.3.232/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      308 2023-04-04 17:07:10.000000 ortelius-cli-9.3.232/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2023-04-04 17:07:10.000000 ortelius-cli-9.3.232/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2023-04-04 17:07:10.000000 ortelius-cli-9.3.232/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2023-04-04 17:07:10.000000 ortelius-cli-9.3.232/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2023-04-04 17:07:10.454764 ortelius-cli-9.3.232/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1007 2023-04-04 17:06:51.000000 ortelius-cli-9.3.232/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.747339 ortelius-cli-9.3.233/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-03-09 18:41:03.000000 ortelius-cli-9.3.233/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2021-05-26 22:33:09.000000 ortelius-cli-9.3.233/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    11080 2023-04-18 23:21:59.744175 ortelius-cli-9.3.233/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-03-09 18:39:10.000000 ortelius-cli-9.3.233/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.732319 ortelius-cli-9.3.233/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    70590 2023-04-18 23:21:37.000000 ortelius-cli-9.3.233/bin/dh
+-rwxr-xr-x   0 steve      (502) staff       (20)     3038 2023-03-23 17:39:44.000000 ortelius-cli-9.3.233/bin/helminfo.sh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.736856 ortelius-cli-9.3.233/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2023-04-18 23:21:37.000000 ortelius-cli-9.3.233/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    74485 2023-04-18 23:20:46.000000 ortelius-cli-9.3.233/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.739018 ortelius-cli-9.3.233/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23766 2023-03-23 17:39:44.000000 ortelius-cli-9.3.233/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    10508 2023-03-23 17:40:27.000000 ortelius-cli-9.3.233/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2023-04-18 23:21:59.743387 ortelius-cli-9.3.233/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    11080 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      308 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       68 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2023-04-18 23:21:59.000000 ortelius-cli-9.3.233/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2023-04-18 23:21:59.747614 ortelius-cli-9.3.233/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1007 2023-04-18 23:21:37.000000 ortelius-cli-9.3.233/setup.py
```

### Comparing `ortelius-cli-9.3.232/LICENSE` & `ortelius-cli-9.3.233/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.232/PKG-INFO` & `ortelius-cli-9.3.233/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.232
+Version: 9.3.233
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.232/README.md` & `ortelius-cli-9.3.233/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.232/bin/dh` & `ortelius-cli-9.3.233/bin/dh`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.232"
+__version__ = "9.3.233"
 
 import json
 import os
 from pathlib import Path
 import re
 import stat
 import subprocess
@@ -229,14 +229,15 @@
 @click.option("--compversion", help="Component Version", envvar="COMPONENT_VERSION")
 @click.option("--compautoinc", help="Component Auto Increment Version", envvar="COMPONENT_AUTOINC")
 @click.option("--deploydatasave", help="Name of the json file to save the new component and application versions names to")
 @click.option("--kvconfig", help="Directory containing the json and properties file", envvar="KVCONFIG")
 @click.option("--crdatasource", help="Change Request Data Source for the Component", envvar="CR_DATASOURCE")
 @click.option("--changerequest", help="Change Request for Component, use multiple time for each Change Request Id", multiple=True)
 @click.option("--deploydata", help="The json file that contains the application, environment and log details", envvar="DEPLOY_DATA")
+@click.option("--namespace", help="The Kubernetes namespace to map a image tag to an application version")
 @click.option("--from_domain", help="Move from domain")
 @click.option("--task", help="Task to use for move")
 @click.option("--envvars", help="Env Variables TOML file")
 @click.option("--envvars_sh", help="Env Variables Output sh file")
 @click.option("--docker", "kind", flag_value="docker", default=True, help="Component Item Type")
 @click.option("--file", "kind", flag_value="file")
 @click.option("--compattr", help="Component Attributes, use multiple time for each attr", multiple=True)
@@ -288,14 +289,15 @@
     msbranch,
     deppkg,
     logdeployment,
     consumes,
     provides,
     rsp,
     cert,
+    namespace,
 ):
     """
     ACTION: deploy, updatecomp, approve, move, envscript, kv, cluster, export or import for the type of action to perform.
 
         deploy: deploy the application to the evironment\n
         approve: approve the application version\n
         move: move the application version using the supplied task\n
@@ -528,14 +530,33 @@
             with open(deploydata, mode="r", encoding="utf-8") as fin_data:
                 payload = fin_data.read()
 
             data = {}
             if dhapi.is_not_empty(payload):
                 data = json.loads(payload)
 
+            if dhapi.is_not_empty(namespace):
+                data['imagetags'] = []
+                pid = subprocess.Popen("kubectl get pods -A -o json", shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                payload = ""
+                for line in pid.stdout.readlines():
+                    payload = payload + line.decode("utf-8").strip()
+
+                if dhapi.is_not_empty(payload):
+                    cluster_json = json.loads(payload)
+                    items = cluster_json.get('items', [])
+                    for item in items:
+                        if (item['metadata']['namespace'] == namespace):
+                            containers = item['spec']['containers']
+                            imagetag = ""
+                            for img in containers:
+                                imagetag = img['image']
+                            data['imagetags'].append(imagetag)
+                            
+
             if dhapi.is_empty(appname):
                 appname = data.get("application", "")
             else:
                 data["application"] = appname
 
             if dhapi.is_empty(appversion):
                 appversion = data.get("appversion", "")
```

### Comparing `ortelius-cli-9.3.232/bin/helminfo.sh` & `ortelius-cli-9.3.233/bin/helminfo.sh`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.232/deployhub/dhapi.py` & `ortelius-cli-9.3.233/deployhub/dhapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         cookies (string) - login cookies
 
     Returns:
         string: The json string.
 
     """
     try:
-        res = requests.get(url, cookies=cookies, timeout=30)
+        res = requests.get(url, cookies=cookies, timeout=300)
         if res is None:
             return None
         if res.status_code != 200:
             return None
         return res.json()
     except requests.exceptions.ConnectionError as conn_error:
         print(str(conn_error))
@@ -91,15 +91,15 @@
         payload (string): json payload to post
         cookies (string): login cookies
 
     Returns:
         string: The json string.
     """
     try:
-        res = requests.post(url, data=payload, cookies=cookies, headers={"Content-Type": "application/json"}, timeout=30)
+        res = requests.post(url, data=payload, cookies=cookies, headers={"Content-Type": "application/json"}, timeout=300)
         if res is None:
             return None
         if res.status_code != 200:
             return None
         return res.json()
     except requests.exceptions.ConnectionError as conn_error:
         print(str(conn_error))
@@ -151,15 +151,15 @@
         my_string = str(my_string)
 
     return bool(my_string and my_string.strip())
 
 
 def sslcerts(dhurl, customcert):
     try:
-        requests.get(dhurl, timeout=30)
+        requests.get(dhurl, timeout=300)
     except requests.exceptions.SSLError:
         print("Adding custom certs to certifi store...")
         cafile = certifi.where()
         with open(customcert, "rb") as infile:
             customca = infile.read()
         with open(cafile, "rb") as infile:
             ca = infile.read()
@@ -179,15 +179,15 @@
         password (string): password for login
         errors (list): list to return any errors back to the caller
 
     Returns:
         string: the cookies to be used in subsequent API calls.
     """
     try:
-        result = requests.post(dhurl + "/dmadminweb/API/login", data={"user": user, "pass": password}, timeout=30)
+        result = requests.post(dhurl + "/dmadminweb/API/login", data={"user": user, "pass": password}, timeout=300)
         cookies = result.cookies
         if result.status_code == 200:
             data = result.json()
             if not data.get("success", False):
                 errors.append(data.get("error", ""))
                 return None
             return cookies
@@ -2199,7 +2199,8 @@
 def run_git(cmd):
     pid = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     retval = ""
     for line in pid.stdout.readlines():
         retval = line.decode("utf-8").strip()
         break
     return retval
+
```

### Comparing `ortelius-cli-9.3.232/doc/deployhub.md` & `ortelius-cli-9.3.233/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.232/doc/dh.md` & `ortelius-cli-9.3.233/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.232/ortelius_cli.egg-info/PKG-INFO` & `ortelius-cli-9.3.233/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.232
+Version: 9.3.233
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.232/setup.py` & `ortelius-cli-9.3.233/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.232",
+    version="9.3.233",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh", "bin/helminfo.sh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
```

