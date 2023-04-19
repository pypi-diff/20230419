# Comparing `tmp/cli-aws-mfa-0.0.2.tar.gz` & `tmp/cli-aws-mfa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-aws-mfa-0.0.2.tar", last modified: Wed Apr 19 06:29:50 2023, max compression
+gzip compressed data, was "cli-aws-mfa-0.0.3.tar", last modified: Wed Apr 19 06:32:44 2023, max compression
```

## Comparing `cli-aws-mfa-0.0.2.tar` & `cli-aws-mfa-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 06:29:50.901426 cli-aws-mfa-0.0.2/
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 06:29:50.900110 cli-aws-mfa-0.0.2/MFA/
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 05:43:29.000000 cli-aws-mfa-0.0.2/MFA/__init__.py
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     2649 2023-04-19 05:48:10.000000 cli-aws-mfa-0.0.2/MFA/mfa.py
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1214 2023-04-19 06:29:50.901213 cli-aws-mfa-0.0.2/PKG-INFO
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      992 2023-04-19 05:56:14.000000 cli-aws-mfa-0.0.2/README.md
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 06:29:50.901049 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1214 2023-04-19 06:29:50.000000 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/PKG-INFO
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      257 2023-04-19 06:29:50.000000 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        1 2023-04-19 06:29:50.000000 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       36 2023-04-19 06:29:50.000000 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/entry_points.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       12 2023-04-19 06:29:50.000000 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/requires.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        4 2023-04-19 06:29:50.000000 cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/top_level.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       38 2023-04-19 06:29:50.901460 cli-aws-mfa-0.0.2/setup.cfg
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      950 2023-04-19 06:29:36.000000 cli-aws-mfa-0.0.2/setup.py
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 06:32:44.543070 cli-aws-mfa-0.0.3/
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 06:32:44.541780 cli-aws-mfa-0.0.3/MFA/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 05:43:29.000000 cli-aws-mfa-0.0.3/MFA/__init__.py
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     2649 2023-04-19 05:48:10.000000 cli-aws-mfa-0.0.3/MFA/mfa.py
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1214 2023-04-19 06:32:44.542881 cli-aws-mfa-0.0.3/PKG-INFO
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      992 2023-04-19 05:56:14.000000 cli-aws-mfa-0.0.3/README.md
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 06:32:44.542719 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1214 2023-04-19 06:32:44.000000 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      257 2023-04-19 06:32:44.000000 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        1 2023-04-19 06:32:44.000000 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       41 2023-04-19 06:32:44.000000 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       12 2023-04-19 06:32:44.000000 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/requires.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        4 2023-04-19 06:32:44.000000 cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/top_level.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       38 2023-04-19 06:32:44.543103 cli-aws-mfa-0.0.3/setup.cfg
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      955 2023-04-19 06:32:34.000000 cli-aws-mfa-0.0.3/setup.py
```

### Comparing `cli-aws-mfa-0.0.2/MFA/mfa.py` & `cli-aws-mfa-0.0.3/MFA/mfa.py`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.2/PKG-INFO` & `cli-aws-mfa-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI AWS MFA
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
```

### Comparing `cli-aws-mfa-0.0.2/README.md` & `cli-aws-mfa-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.2/cli_aws_mfa.egg-info/PKG-INFO` & `cli-aws-mfa-0.0.3/cli_aws_mfa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.2
+Version: 0.0.3
 Summary: CLI AWS MFA
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
```

### Comparing `cli-aws-mfa-0.0.2/setup.py` & `cli-aws-mfa-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "CLI AWS MFA"
 LONG_DESCRIPTION = "Use MFA to increase the security of your AWS environment. Signing in with MFA requires an authentication code from an MFA device. Each user can have a maximum of 8 MFA devices assigned"
 
 # Setting up
 setup(
     name="cli-aws-mfa",
     version=VERSION,
@@ -20,12 +20,12 @@
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=["MFA"],
     keywords=["aws", "mfa", "virtual"],
     entry_points={
         "console_scripts": [
-            "cli-aws-mfa = cli",
+            "cli-aws-mfa = main:cli",
         ]
     },
     install_requires=["click", "boto3"],
 )
```

