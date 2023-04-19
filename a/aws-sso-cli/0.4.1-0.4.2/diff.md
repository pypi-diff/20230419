# Comparing `tmp/aws-sso-cli-0.4.1.tar.gz` & `tmp/aws-sso-cli-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-sso-cli-0.4.1.tar", last modified: Mon Apr 17 14:40:40 2023, max compression
+gzip compressed data, was "aws-sso-cli-0.4.2.tar", last modified: Wed Apr 19 19:03:46 2023, max compression
```

## Comparing `aws-sso-cli-0.4.1.tar` & `aws-sso-cli-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-17 14:40:40.360392 aws-sso-cli-0.4.1/
--rw-r--r--   0 pdebelak   (501) staff       (20)     1070 2023-03-10 20:54:39.000000 aws-sso-cli-0.4.1/LICENSE
--rw-r--r--   0 pdebelak   (501) staff       (20)     1350 2023-04-17 14:40:40.360459 aws-sso-cli-0.4.1/PKG-INFO
--rw-r--r--   0 pdebelak   (501) staff       (20)     1076 2023-04-17 14:15:35.000000 aws-sso-cli-0.4.1/README.md
-drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-17 14:40:40.359039 aws-sso-cli-0.4.1/aws_sso_cli/
--rw-r--r--   0 pdebelak   (501) staff       (20)     6378 2023-04-17 14:37:36.000000 aws-sso-cli-0.4.1/aws_sso_cli/__init__.py
-drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-17 14:40:40.360050 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/
--rw-r--r--   0 pdebelak   (501) staff       (20)     1350 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/PKG-INFO
--rw-r--r--   0 pdebelak   (501) staff       (20)      295 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pdebelak   (501) staff       (20)        1 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pdebelak   (501) staff       (20)       49 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/entry_points.txt
--rw-r--r--   0 pdebelak   (501) staff       (20)       36 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/requires.txt
--rw-r--r--   0 pdebelak   (501) staff       (20)       12 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/aws_sso_cli.egg-info/top_level.txt
-drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-17 14:40:40.358249 aws-sso-cli-0.4.1/docs/
-drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-17 14:40:40.360232 aws-sso-cli-0.4.1/docs/man/
--rw-r--r--   0 pdebelak   (501) staff       (20)      893 2023-04-17 14:40:40.000000 aws-sso-cli-0.4.1/docs/man/aws-sso-cli.1
--rw-r--r--   0 pdebelak   (501) staff       (20)      591 2023-04-17 14:40:40.360765 aws-sso-cli-0.4.1/setup.cfg
--rw-r--r--   0 pdebelak   (501) staff       (20)       97 2023-04-17 14:12:51.000000 aws-sso-cli-0.4.1/setup.py
+drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-19 19:03:46.255552 aws-sso-cli-0.4.2/
+-rw-r--r--   0 pdebelak   (501) staff       (20)     1070 2023-03-10 20:54:39.000000 aws-sso-cli-0.4.2/LICENSE
+-rw-r--r--   0 pdebelak   (501) staff       (20)     1548 2023-04-19 19:03:46.255608 aws-sso-cli-0.4.2/PKG-INFO
+-rw-r--r--   0 pdebelak   (501) staff       (20)     1274 2023-04-19 18:38:03.000000 aws-sso-cli-0.4.2/README.md
+drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-19 19:03:46.254460 aws-sso-cli-0.4.2/aws_sso_cli/
+-rw-r--r--   0 pdebelak   (501) staff       (20)     6547 2023-04-19 18:59:07.000000 aws-sso-cli-0.4.2/aws_sso_cli/__init__.py
+drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-19 19:03:46.255287 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/
+-rw-r--r--   0 pdebelak   (501) staff       (20)     1548 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pdebelak   (501) staff       (20)      295 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pdebelak   (501) staff       (20)        1 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pdebelak   (501) staff       (20)       49 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pdebelak   (501) staff       (20)       36 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/requires.txt
+-rw-r--r--   0 pdebelak   (501) staff       (20)       12 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/aws_sso_cli.egg-info/top_level.txt
+drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-19 19:03:46.253628 aws-sso-cli-0.4.2/docs/
+drwxr-xr-x   0 pdebelak   (501) staff       (20)        0 2023-04-19 19:03:46.255431 aws-sso-cli-0.4.2/docs/man/
+-rw-r--r--   0 pdebelak   (501) staff       (20)      893 2023-04-19 19:03:46.000000 aws-sso-cli-0.4.2/docs/man/aws-sso-cli.1
+-rw-r--r--   0 pdebelak   (501) staff       (20)      591 2023-04-19 19:03:46.255872 aws-sso-cli-0.4.2/setup.cfg
+-rw-r--r--   0 pdebelak   (501) staff       (20)       97 2023-04-17 14:12:51.000000 aws-sso-cli-0.4.2/setup.py
```

### Comparing `aws-sso-cli-0.4.1/LICENSE` & `aws-sso-cli-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-sso-cli-0.4.1/PKG-INFO` & `aws-sso-cli-0.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1
-Name: aws-sso-cli
-Version: 0.4.1
-Summary: A program to simplify logging in and setting credentials using AWS SSO.
-Author: Peter Debelak
-Author-email: pdebelak@gmail.com
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # aws-sso-cli
 
 A program to simplify logging in and setting credentials using AWS
 SSO.
 
+## Installation
+
+This can be installed via `pip`:
+
+```
+pip install aws-sso-cli
+```
+
+You can also find wheels from the [releases page on
+gitlab](https://gitlab.com/pdebelak/aws-sso-cli/-/releases).
+
 ## Usage
 
 Running `aws-sso-cli` with no arguments will check if you are logged
 in, and log in with `aws sso login` if you are not. It will
 additionally create or update your credentials file (in either
 `$AWS_SHARED_CREDENTIALS_FILE` if defined or defaulting to
 `$HOME/.aws/credentials`) after logging in and will attempt to log you
```

### Comparing `aws-sso-cli-0.4.1/aws_sso_cli/__init__.py` & `aws-sso-cli-0.4.2/aws_sso_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Dict, Optional
 
 import boto3
 import botocore.exceptions
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 def main(cli_args=None):
     parser = build_parser()
     arguments = parser.parse_args(cli_args)
     session = boto3.Session(profile_name=arguments.profile)
     sso = AwsSsoLogin(arguments.profile, session)
@@ -121,24 +121,29 @@
     def update_section(self, section: str, values: Dict[str, str]):
         if self._config.has_section(section):
             new_values = self._config[section]
         else:
             self._config.add_section(section)
             new_values = {}
         for key, value in values.items():
-            new_values[key] = value
+            if value is None:
+                if key in new_values:
+                    del new_values[key]
+            else:
+                new_values[key] = value
         self._config[section] = new_values
         with self._credentials_file.open("w") as f:
             self._config.write(f)
 
     def set_from(self, session: boto3.Session):
         credentials = session.get_credentials()
         profile_config = {
             "aws_access_key_id": credentials.access_key,
             "aws_secret_access_key": credentials.secret_key,
+            "aws_session_token": None,
         }
         if credentials.token:
             profile_config["aws_session_token"] = credentials.token
         self.update_section(session.profile_name, profile_config)
 
 
 class AwsDocker:
```

### Comparing `aws-sso-cli-0.4.1/aws_sso_cli.egg-info/PKG-INFO` & `aws-sso-cli-0.4.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 Metadata-Version: 2.1
 Name: aws-sso-cli
-Version: 0.4.1
+Version: 0.4.2
 Summary: A program to simplify logging in and setting credentials using AWS SSO.
 Author: Peter Debelak
 Author-email: pdebelak@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # aws-sso-cli
 
 A program to simplify logging in and setting credentials using AWS
 SSO.
 
+## Installation
+
+This can be installed via `pip`:
+
+```
+pip install aws-sso-cli
+```
+
+You can also find wheels from the [releases page on
+gitlab](https://gitlab.com/pdebelak/aws-sso-cli/-/releases).
+
 ## Usage
 
 Running `aws-sso-cli` with no arguments will check if you are logged
 in, and log in with `aws sso login` if you are not. It will
 additionally create or update your credentials file (in either
 `$AWS_SHARED_CREDENTIALS_FILE` if defined or defaulting to
 `$HOME/.aws/credentials`) after logging in and will attempt to log you
```

### Comparing `aws-sso-cli-0.4.1/docs/man/aws-sso-cli.1` & `aws-sso-cli-0.4.2/docs/man/aws-sso-cli.1`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.TH AWS\-SSO\-CLI "1" "2023\-04\-17" "aws\-sso\-cli" "Generated Python Manual"
+.TH AWS\-SSO\-CLI "1" "2023\-04\-19" "aws\-sso\-cli" "Generated Python Manual"
 .SH NAME
 aws\-sso\-cli
 .SH SYNOPSIS
 .B aws\-sso\-cli
 [-h] [-p PROFILE] [-v] [-f] [--docker-force]
 .SH DESCRIPTION
 A program to log into AWS SSO if not already logged in.
```

### Comparing `aws-sso-cli-0.4.1/setup.cfg` & `aws-sso-cli-0.4.2/setup.cfg`

 * *Files identical despite different names*

