# Comparing `tmp/cli-aws-mfa-0.0.5.tar.gz` & `tmp/cli-aws-mfa-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-aws-mfa-0.0.5.tar", last modified: Wed Apr 19 11:29:03 2023, max compression
+gzip compressed data, was "cli-aws-mfa-0.0.6.tar", last modified: Wed Apr 19 11:34:14 2023, max compression
```

## Comparing `cli-aws-mfa-0.0.5.tar` & `cli-aws-mfa-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:29:03.765271 cli-aws-mfa-0.0.5/
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:29:03.764071 cli-aws-mfa-0.0.5/MFA/
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 05:43:29.000000 cli-aws-mfa-0.0.5/MFA/__init__.py
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     4341 2023-04-19 11:26:05.000000 cli-aws-mfa-0.0.5/MFA/mfa.py
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1214 2023-04-19 11:29:03.765046 cli-aws-mfa-0.0.5/PKG-INFO
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      992 2023-04-19 05:56:14.000000 cli-aws-mfa-0.0.5/README.md
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1658 2023-04-19 11:27:22.000000 cli-aws-mfa-0.0.5/cli.py
-drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:29:03.764866 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/
--rw-r--r--   0 imajeetyadav   (501) staff       (20)     1214 2023-04-19 11:29:03.000000 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/PKG-INFO
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      264 2023-04-19 11:29:03.000000 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        1 2023-04-19 11:29:03.000000 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       40 2023-04-19 11:29:03.000000 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/entry_points.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       12 2023-04-19 11:29:03.000000 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/requires.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)        8 2023-04-19 11:29:03.000000 cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/top_level.txt
--rw-r--r--   0 imajeetyadav   (501) staff       (20)       38 2023-04-19 11:29:03.765309 cli-aws-mfa-0.0.5/setup.cfg
--rw-r--r--   0 imajeetyadav   (501) staff       (20)      978 2023-04-19 11:28:27.000000 cli-aws-mfa-0.0.5/setup.py
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:34:14.155319 cli-aws-mfa-0.0.6/
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:34:14.153961 cli-aws-mfa-0.0.6/MFA/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 05:43:29.000000 cli-aws-mfa-0.0.6/MFA/__init__.py
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     4341 2023-04-19 11:26:05.000000 cli-aws-mfa-0.0.6/MFA/mfa.py
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1370 2023-04-19 11:34:14.155115 cli-aws-mfa-0.0.6/PKG-INFO
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1122 2023-04-19 11:32:09.000000 cli-aws-mfa-0.0.6/README.md
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1658 2023-04-19 11:27:22.000000 cli-aws-mfa-0.0.6/cli.py
+drwxr-xr-x   0 imajeetyadav   (501) staff       (20)        0 2023-04-19 11:34:14.154932 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)     1370 2023-04-19 11:34:14.000000 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      264 2023-04-19 11:34:14.000000 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        1 2023-04-19 11:34:14.000000 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       40 2023-04-19 11:34:14.000000 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       12 2023-04-19 11:34:14.000000 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/requires.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)        8 2023-04-19 11:34:14.000000 cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/top_level.txt
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)       38 2023-04-19 11:34:14.155356 cli-aws-mfa-0.0.6/setup.cfg
+-rw-r--r--   0 imajeetyadav   (501) staff       (20)      949 2023-04-19 11:33:47.000000 cli-aws-mfa-0.0.6/setup.py
```

### Comparing `cli-aws-mfa-0.0.5/MFA/mfa.py` & `cli-aws-mfa-0.0.6/MFA/mfa.py`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.5/PKG-INFO` & `cli-aws-mfa-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.5
-Summary: CLI AWS MFA
+Version: 0.0.6
+Summary: AWS MFA - Manage Session Token easily
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
 
 
 # AWS CLI MFA
 
 Developed by Ajeet Yadav
 
 ## Example of How To Use
 
+```
+# Setup ARN and profile name
+cli-aws-mfa init
+
+# Refresh Session Token
+cli-aws-mfa refresh 
+
+```
+
+## Policy Used for CLI MFA
+
 ```json
 {
     "Version": "2012-10-17",
     "Statement": [
         {
             "Sid": "MustBeSignedInWithMFA",
             "Effect": "Deny",
```

### Comparing `cli-aws-mfa-0.0.5/cli.py` & `cli-aws-mfa-0.0.6/cli.py`

 * *Files identical despite different names*

### Comparing `cli-aws-mfa-0.0.5/cli_aws_mfa.egg-info/PKG-INFO` & `cli-aws-mfa-0.0.6/cli_aws_mfa.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 Metadata-Version: 2.1
 Name: cli-aws-mfa
-Version: 0.0.5
-Summary: CLI AWS MFA
+Version: 0.0.6
+Summary: AWS MFA - Manage Session Token easily
 Author: imajeetyadav (Ajeet Yadav)
 Author-email: <hello@codingprotocols.com>
 Keywords: aws,mfa,virtual
 Description-Content-Type: text/markdown
 
 
 # AWS CLI MFA
 
 Developed by Ajeet Yadav
 
 ## Example of How To Use
 
+```
+# Setup ARN and profile name
+cli-aws-mfa init
+
+# Refresh Session Token
+cli-aws-mfa refresh 
+
+```
+
+## Policy Used for CLI MFA
+
 ```json
 {
     "Version": "2012-10-17",
     "Statement": [
         {
             "Sid": "MustBeSignedInWithMFA",
             "Effect": "Deny",
```

### Comparing `cli-aws-mfa-0.0.5/setup.py` & `cli-aws-mfa-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.5"
-DESCRIPTION = "CLI AWS MFA"
-LONG_DESCRIPTION = "Use MFA to increase the security of your AWS environment. Signing in with MFA requires an authentication code from an MFA device. Each user can have a maximum of 8 MFA devices assigned"
+VERSION = "0.0.6"
+DESCRIPTION = "AWS MFA - Manage Session Token easily"
+LONG_DESCRIPTION = "Use MFA to increase the security of your AWS environment. Signing in with MFA requires an authentication code from an MFA device."
 
 # Setting up
 setup(
     name="cli-aws-mfa",
     version=VERSION,
     author="imajeetyadav (Ajeet Yadav)",
     author_email="<hello@codingprotocols.com>",
```

