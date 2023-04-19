# Comparing `tmp/cfscanner-1.3.6.tar.gz` & `tmp/cfscanner-1.3.7.tar.gz`

## Comparing `cfscanner-1.3.6.tar` & `cfscanner-1.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.6/.vscode/settings.json
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/__main__.py
--rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/cfscanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/args/__init__.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/args/parser.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/args/testconfig.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/report/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/report/colors.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/report/print.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/report/result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/speedtest/__init__.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/speedtest/conduct.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/speedtest/download.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/speedtest/fronting.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/speedtest/tools.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/speedtest/upload.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/subnets/__init__.py
--rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/subnets/cidr.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/subnets/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/utils/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/utils/decorators.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/utils/exceptions.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/utils/os.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/utils/requests.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/utils/socket.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/xray/__init__.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/xray/binary.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/xray/config.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/xray/service.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.6/cfscanner/xray/templates.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.6/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.6/LICENSE
--rw-r--r--   0        0        0     8789 2020-02-02 00:00:00.000000 cfscanner-1.3.6/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cfscanner-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     9538 2020-02-02 00:00:00.000000 cfscanner-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.7/.vscode/settings.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/__main__.py
+-rw-r--r--   0        0        0    10940 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/args/__init__.py
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/args/parser.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/args/testconfig.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/report/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/report/colors.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/report/print.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/report/result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/speedtest/__init__.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/speedtest/conduct.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/speedtest/download.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/speedtest/fronting.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/speedtest/tools.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/speedtest/upload.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/subnets/__init__.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/subnets/cidr.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/subnets/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/utils/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/utils/decorators.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/utils/exceptions.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/utils/os.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/utils/requests.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/utils/socket.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/xray/__init__.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/xray/binary.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/xray/config.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/xray/service.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.7/cfscanner/xray/templates.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.7/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.7/LICENSE
+-rw-r--r--   0        0        0     8832 2020-02-02 00:00:00.000000 cfscanner-1.3.7/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cfscanner-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 cfscanner-1.3.7/PKG-INFO
```

### Comparing `cfscanner-1.3.6/cfscanner/cfscanner.py` & `cfscanner-1.3.7/cfscanner/main.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/args/parser.py` & `cfscanner-1.3.7/cfscanner/args/parser.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/args/testconfig.py` & `cfscanner-1.3.7/cfscanner/args/testconfig.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/report/print.py` & `cfscanner-1.3.7/cfscanner/report/print.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/report/result.py` & `cfscanner-1.3.7/cfscanner/report/result.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/speedtest/conduct.py` & `cfscanner-1.3.7/cfscanner/speedtest/conduct.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/speedtest/download.py` & `cfscanner-1.3.7/cfscanner/speedtest/download.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/speedtest/fronting.py` & `cfscanner-1.3.7/cfscanner/speedtest/fronting.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/speedtest/upload.py` & `cfscanner-1.3.7/cfscanner/speedtest/upload.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/subnets/cidr.py` & `cfscanner-1.3.7/cfscanner/subnets/cidr.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/utils/decorators.py` & `cfscanner-1.3.7/cfscanner/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/utils/exceptions.py` & `cfscanner-1.3.7/cfscanner/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/utils/os.py` & `cfscanner-1.3.7/cfscanner/utils/os.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/utils/requests.py` & `cfscanner-1.3.7/cfscanner/utils/requests.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/utils/socket.py` & `cfscanner-1.3.7/cfscanner/utils/socket.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/xray/__init__.py` & `cfscanner-1.3.7/cfscanner/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/xray/binary.py` & `cfscanner-1.3.7/cfscanner/xray/binary.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/xray/config.py` & `cfscanner-1.3.7/cfscanner/xray/config.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/xray/service.py` & `cfscanner-1.3.7/cfscanner/xray/service.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/cfscanner/xray/templates.py` & `cfscanner-1.3.7/cfscanner/xray/templates.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/.gitignore` & `cfscanner-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/LICENSE` & `cfscanner-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.6/README.md` & `cfscanner-1.3.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -236,10 +236,12 @@
   * fixed an issue with packaging
 * 1.3.4
   * change the structure to improve module names in the logs
 * 1.3.5
   * fixed a bug
 * 1.3.6
   * another bug!
+* 1.3.7
+  * fixed a bug in the config file
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.3.0-blue
```

### Comparing `cfscanner-1.3.6/pyproject.toml` & `cfscanner-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfscanner"
-version = "1.3.6"
+version = "1.3.7"
 authors = [
   { name="tempookian", email="tempookian@gmail.com" },
   { name="Morteza Bashsiz", email="morteza.bashsiz@gmail.com"}
 ]
 description = "Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `cfscanner-1.3.6/PKG-INFO` & `cfscanner-1.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfscanner
-Version: 1.3.6
+Version: 1.3.7
 Summary: Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray
 Project-URL: Homepage, https://github.com/MortezaBashsiz/CFScanner/tree/main/python
 Project-URL: Bug Tracker, https://github.com/MortezaBashsiz/CFScanner/issues
 Author-email: tempookian <tempookian@gmail.com>, Morteza Bashsiz <morteza.bashsiz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -253,10 +253,12 @@
   * fixed an issue with packaging
 * 1.3.4
   * change the structure to improve module names in the logs
 * 1.3.5
   * fixed a bug
 * 1.3.6
   * another bug!
+* 1.3.7
+  * fixed a bug in the config file
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
 [version]: https://img.shields.io/badge/Version-1.3.0-blue
```

