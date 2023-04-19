# Comparing `tmp/gpush-2.1.1.tar.gz` & `tmp/gpush-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpush-2.1.1.tar", last modified: Wed Apr 12 19:34:49 2023, max compression
+gzip compressed data, was "gpush-3.0.0.tar", last modified: Wed Apr 19 07:06:47 2023, max compression
```

## Comparing `gpush-2.1.1.tar` & `gpush-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:34:49.469299 gpush-2.1.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-12 19:34:46.000000 gpush-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-12 19:34:49.469299 gpush-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1188 2023-04-12 19:34:46.000000 gpush-2.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 19:34:47.000000 gpush-2.1.1/_version.py
--rwxr-xr-x   0 root         (0) root         (0)     3234 2023-04-12 19:34:46.000000 gpush-2.1.1/gpush
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 19:34:49.469299 gpush-2.1.1/gpush.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1300 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 19:34:49.000000 gpush-2.1.1/gpush.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      227 2023-04-12 19:34:46.000000 gpush-2.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 19:34:49.469299 gpush-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-12 19:34:46.000000 gpush-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:06:47.782716 gpush-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 07:06:45.000000 gpush-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-19 07:06:47.782716 gpush-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-04-19 07:06:45.000000 gpush-3.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-19 07:06:45.000000 gpush-3.0.0/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-04-19 07:06:47.000000 gpush-3.0.0/gpush
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 07:06:47.782716 gpush-3.0.0/gpush.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-19 07:06:47.000000 gpush-3.0.0/gpush.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-19 07:06:47.000000 gpush-3.0.0/gpush.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 07:06:47.000000 gpush-3.0.0/gpush.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-19 07:06:47.000000 gpush-3.0.0/gpush.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-19 07:06:47.000000 gpush-3.0.0/gpush.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)     3949 2023-04-19 07:06:45.000000 gpush-3.0.0/gpush.py
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-19 07:06:45.000000 gpush-3.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 07:06:47.782716 gpush-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      774 2023-04-19 07:06:45.000000 gpush-3.0.0/setup.py
```

### Comparing `gpush-2.1.1/LICENSE` & `gpush-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpush-2.1.1/PKG-INFO` & `gpush-3.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: gpush
-Version: 2.1.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gpush
 
 `gpush` is a command line utility for standardising commit messages using [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
 
 # Installation
 
 This package is available for installation via pypi
@@ -33,10 +27,22 @@
 Alternatively, create an alias in your zshrc file (Use appropriate profile file if you do not use zsh)
 
 echo "alias gpush=\"python3 /path/to/git/gpush/gpush\"" >> ~/.zshrc
 To start using straight away, source your file
 
 source ~/.zshrc
 
+# Unit tests
+
+To run unit tests, execute the following command, you will need to have pytest installed and set environment
+variable `GITHUB_TOKEN` to a valid GitHub token that has permissions to create/delete and push to a repository
+within your account.
+
+```
+make test
+```
+
+The unit tests will create a test repository within your account for each unit test before testing functionality and deleting the repository.
+
 # python-semantic-release
 
 `gpush` generates commit messages that are compliant with [python-semantic-release](https://python-semantic-release.readthedocs.io/en/latest/). See example in the [GitHub Repository](https://github.com/tjtharrison/gpush/blob/main/.github/workflows/semver.yaml)
```

### Comparing `gpush-2.1.1/gpush` & `gpush-3.0.0/gpush`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 
 """
 Python script to handle git commit and push to standardise commit messages using conventional commit
 messages.
 
-Usage: gpush
+Usage: gpush.py
 """
 
+import argparse
+import sys
+
 import inquirer
 from git import Repo
-import argparse
+
 from _version import __version__
 
 version = __version__
 
 parser = argparse.ArgumentParser(
     prog="gpush " + version,
     description="Git commit helper for conventional commit messages",
@@ -27,18 +30,32 @@
     help="[Default: False] Option to enable git commit",
 )
 parser.add_argument(
     "--no-push",
     action="store_false",
     help="[Default: False] Option to enable git push",
 )
+parser.add_argument(
+    "--message",
+    action="store",
+    help="[Default: None] Override message prompt and use the provided message",
+)
 
 args = parser.parse_args()
 
 
+def get_version():
+    """
+    Function to return the current version of gpush.py
+
+    :return: String containing the current version of gpush.py
+    """
+    return version
+
+
 def git_commit(commit_message):
     """
     Function to commit changes to Git on the current branch for the repository
     :param commit_message: String containing the conventional commit message formatted commit
     message
     :return: True/False
     """
@@ -103,20 +120,37 @@
 
     commit_message_final = (
         answers["type"] + is_breaking_change + ": " + answers["commit_message"]
     )
     return commit_message_final
 
 
-if __name__ == "__main__":
+def main():
+    """
+    Main function to execute the script
+    :return:
+    """
     if args.version:
-        print(version)
+        print(get_version())
     else:
         try:
             if args.no_commit:
-                commit_message = collect_details()
+                print(args.message)
+                if str(args.message) != "None":
+                    commit_message = args.message
+                else:
+                    print("Got here")
+                    commit_message = collect_details()
                 git_commit(commit_message)
             if args.no_push:
                 git_push()
         except Exception as error_message:
             print("Some error occurred while pushing the code:")
             print(str(error_message))
+            raise
+    return True
+
+
+if __name__ == "__main__":
+    """
+    Main function to execute the script"""
+    main()
```

