# Comparing `tmp/aws-cdk.cli-lib-alpha-2.75.0a0.tar.gz` & `tmp/aws-cdk.cli-lib-alpha-2.75.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/codebuild/output/src418252965/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.75.0a0.tar", last modified: Mon Apr 17 22:39:12 2023, max compression
+gzip compressed data, was "/codebuild/output/src905434118/src/packages/@aws-cdk/cli-lib-alpha/dist/python/aws-cdk.cli-lib-alpha-2.75.1a0.tar", last modified: Tue Apr 18 23:36:02 2023, max compression
```

## Comparing `aws-cdk.cli-lib-alpha-2.75.0a0.tar` & `aws-cdk.cli-lib-alpha-2.75.1a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/
--rw-r--r--   0 root         (0) root         (0)    11391 2023-04-17 22:39:01.000000 aws-cdk.cli-lib-alpha-2.75.0a0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      726 2023-04-17 22:39:02.000000 aws-cdk.cli-lib-alpha-2.75.0a0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4179 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3192 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1766 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/
--rw-r--r--   0 root         (0) root         (0)   189502 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/_jsii/
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  3641728 2023-04-17 22:39:01.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.75.0-alpha.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 22:39:06.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4179 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      491 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-17 22:39:12.000000 aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/
+-rw-r--r--   0 root         (0) root         (0)    11391 2023-04-18 23:35:42.000000 aws-cdk.cli-lib-alpha-2.75.1a0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      726 2023-04-18 23:35:44.000000 aws-cdk.cli-lib-alpha-2.75.1a0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/README.md
+-rw-r--r--   0 root         (0) root         (0)      234 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/
+-rw-r--r--   0 root         (0) root         (0)   189502 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  3641727 2023-04-18 23:35:42.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.75.1-alpha.0.jsii.tgz
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 23:35:49.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-18 23:36:02.000000 aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/top_level.txt
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/LICENSE` & `aws-cdk.cli-lib-alpha-2.75.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/NOTICE` & `aws-cdk.cli-lib-alpha-2.75.1a0/NOTICE`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.75.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.75.0a0
+Version: 2.75.1a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/README.md` & `aws-cdk.cli-lib-alpha-2.75.1a0/README.md`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/setup.py` & `aws-cdk.cli-lib-alpha-2.75.1a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-cdk.cli-lib-alpha",
-    "version": "2.75.0.a0",
+    "version": "2.75.1.a0",
     "description": "AWS CDK Programmatic CLI library",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-cdk",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_cdk.cli_lib_alpha",
         "aws_cdk.cli_lib_alpha._jsii"
     ],
     "package_data": {
         "aws_cdk.cli_lib_alpha._jsii": [
-            "cli-lib-alpha@2.75.0-alpha.0.jsii.tgz"
+            "cli-lib-alpha@2.75.1-alpha.0.jsii.tgz"
         ],
         "aws_cdk.cli_lib_alpha": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/__init__.py` & `aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.75.0-alpha.0.jsii.tgz` & `aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk/cli_lib_alpha/_jsii/cli-lib-alpha@2.75.1-alpha.0.jsii.tgz`

 * *Files 7% similar despite different names*

#### Comparing `cli-lib-alpha@2.75.0-alpha.0.jsii.tgz-content` & `cli-lib-alpha@2.75.1-alpha.0.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'2.75.1-alpha.0'"}*

```diff
@@ -1420,9 +1420,9 @@
                         "primitive": "boolean"
                     }
                 }
             ],
             "symbolId": "lib/commands/synth:SynthOptions"
         }
     },
-    "version": "2.75.0-alpha.0"
+    "version": "2.75.1-alpha.0"
 }
```

##### package/lib/main.js

###### js-beautify {}

```diff
@@ -1017431,15 +1017431,15 @@
     }
 });
 var require_package3 = __commonJS({
     "../../aws-cdk/package.json"(exports, module2) {
         module2.exports = {
             name: "aws-cdk",
             description: "CDK Toolkit, the command line tool for CDK apps",
-            version: "2.75.0",
+            version: "2.75.1",
             bin: {
                 cdk: "bin/cdk"
             },
             scripts: {
                 build: "cdk-build",
                 watch: "cdk-watch",
                 lint: "cdk-lint",
@@ -1017480,15 +1017480,15 @@
             author: {
                 name: "Amazon Web Services",
                 url: "https://aws.amazon.com",
                 organization: true
             },
             license: "Apache-2.0",
             devDependencies: {
-                "aws-cdk-lib": "2.75.0",
+                "aws-cdk-lib": "2.75.1",
                 "@octokit/rest": "^18.12.0",
                 "@types/archiver": "^5.3.1",
                 "@types/fs-extra": "^9.0.13",
                 "@types/glob": "^7.2.0",
                 "@types/jest": "^27.5.2",
                 "@types/minimatch": "^3.0.5",
                 "@types/mockery": "^1.4.30",
@@ -1017497,39 +1017497,39 @@
                 "@types/sinon": "^9.0.11",
                 "@types/source-map-support": "^0.5.6",
                 "@types/table": "^6.0.0",
                 "@types/uuid": "^8.3.4",
                 "@types/wrap-ansi": "^3.0.0",
                 "@types/yargs": "^15.0.15",
                 "aws-sdk-mock": "5.6.0",
-                "@aws-cdk/cdk-build-tools": "2.75.0-alpha.0",
+                "@aws-cdk/cdk-build-tools": "2.75.1-alpha.0",
                 jest: "^27.5.1",
                 madge: "^5.0.2",
                 constructs: "^10.0.0",
                 "make-runnable": "^1.4.1",
                 mockery: "^2.1.0",
                 nock: "^13.3.0",
-                "@aws-cdk/pkglint": "2.75.0-alpha.0",
+                "@aws-cdk/pkglint": "2.75.1-alpha.0",
                 sinon: "^9.2.4",
                 "ts-jest": "^27.1.5",
                 "ts-mock-imports": "^1.3.8",
                 "xml-js": "^1.6.11",
                 axios: "^0.27.2",
                 "fast-check": "^2.25.0"
             },
             dependencies: {
-                "@aws-cdk/cloud-assembly-schema": "2.75.0",
-                "@aws-cdk/cloudformation-diff": "2.75.0",
-                "@aws-cdk/cx-api": "2.75.0",
-                "@aws-cdk/region-info": "2.75.0",
+                "@aws-cdk/cloud-assembly-schema": "2.75.1",
+                "@aws-cdk/cloudformation-diff": "2.75.1",
+                "@aws-cdk/cx-api": "2.75.1",
+                "@aws-cdk/region-info": "2.75.1",
                 "@jsii/check-node": "1.78.1",
                 archiver: "^5.3.1",
                 "aws-sdk": "^2.1329.0",
                 camelcase: "^6.3.0",
-                "cdk-assets": "2.75.0-alpha.0",
+                "cdk-assets": "2.75.1-alpha.0",
                 chokidar: "^3.5.3",
                 chalk: "^4",
                 decamelize: "^5.0.1",
                 "fs-extra": "^9.1.0",
                 glob: "^7.2.3",
                 "json-diff": "^0.10.0",
                 minimatch: ">=3.1",
```

##### package/build-info.json

###### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'comment'": "'Generated at 2023-04-18T22:51:46Z by generate.sh'", "'commit'": "'aa30a30'"}*

```diff
@@ -1,4 +1,4 @@
 {
-    "comment": "Generated at 2023-04-17T21:53:15Z by generate.sh",
-    "commit": "37c53d6"
+    "comment": "Generated at 2023-04-18T22:51:46Z by generate.sh",
+    "commit": "aa30a30"
 }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9759615384615384%*

 * *Differences: {"'devDependencies'": "{'@aws-cdk/cdk-build-tools': '2.75.1-alpha.0', 'aws-cdk-lib': '2.75.1', "*

 * *                      "'@aws-cdk/pkglint': '2.75.1-alpha.0', 'aws-cdk': '2.75.1'}",*

 * * "'version'": "'2.75.1-alpha.0'"}*

```diff
@@ -21,19 +21,19 @@
             "cp ../../../node_modules/vm2/lib/bridge.js ../../../node_modules/vm2/lib/setup-sandbox.js ./lib",
             "yarn bundle"
         ]
     },
     "dependencies": {},
     "description": "AWS CDK Programmatic CLI library",
     "devDependencies": {
-        "@aws-cdk/cdk-build-tools": "2.75.0-alpha.0",
-        "@aws-cdk/pkglint": "2.75.0-alpha.0",
+        "@aws-cdk/cdk-build-tools": "2.75.1-alpha.0",
+        "@aws-cdk/pkglint": "2.75.1-alpha.0",
         "@types/jest": "^27.5.2",
-        "aws-cdk": "2.75.0",
-        "aws-cdk-lib": "2.75.0",
+        "aws-cdk": "2.75.1",
+        "aws-cdk-lib": "2.75.1",
         "constructs": "^10.0.0",
         "jest": "^27.5.1",
         "ts-node": "^10.9.1"
     },
     "engines": {
         "node": ">= 14.15.0"
     },
@@ -119,9 +119,9 @@
     },
     "separate-module": true,
     "stability": "experimental",
     "types": "lib/index.d.ts",
     "ubergen": {
         "exclude": true
     },
-    "version": "2.75.0-alpha.0"
+    "version": "2.75.1-alpha.0"
 }
```

### Comparing `aws-cdk.cli-lib-alpha-2.75.0a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO` & `aws-cdk.cli-lib-alpha-2.75.1a0/src/aws_cdk.cli_lib_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk.cli-lib-alpha
-Version: 2.75.0a0
+Version: 2.75.1a0
 Summary: AWS CDK Programmatic CLI library
 Home-page: https://github.com/aws/aws-cdk
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-cdk.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

