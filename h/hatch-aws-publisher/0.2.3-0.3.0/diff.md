# Comparing `tmp/hatch_aws_publisher-0.2.3.tar.gz` & `tmp/hatch_aws_publisher-0.3.0.tar.gz`

## Comparing `hatch_aws_publisher-0.2.3.tar` & `hatch_aws_publisher-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/hatch_aws_publisher/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/hatch_aws_publisher/hooks.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/hatch_aws_publisher/publisher.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/README.md
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/hatch_aws_publisher/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/hatch_aws_publisher/hooks.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/hatch_aws_publisher/publisher.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/README.md
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 hatch_aws_publisher-0.3.0/PKG-INFO
```

### Comparing `hatch_aws_publisher-0.2.3/LICENSE.txt` & `hatch_aws_publisher-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_aws_publisher-0.2.3/README.md` & `hatch_aws_publisher-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hatch_aws_publisher-0.2.3/pyproject.toml` & `hatch_aws_publisher-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-aws-publisher"
-version = "0.2.3"
+version = "0.3.0"
 description = 'Hatch plugin for deploying to AWS with SAM'
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 keywords = ["hatch", "aws", "plugin", "sam", "lambda"]
 authors = [{ name = "aka-raccoon", email = "aka-raccoon@pm.me" }]
 classifiers = [
@@ -104,15 +104,15 @@
   "slow: marks tests as slow (deselect with '-m \"not slow\"')",
   "serial",
 ]
 filterwarnings = ["ignore:.*are deprecated.*:Warning"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.3"
+version = "0.3.0"
 version_files = ["pyproject.toml:^version"]
 tag_format = "$version"
 bump_message = "bump: $current_version → $new_version"
 
 [tool.hatch.build]
 exclude = [".github", "tests", ".editorconfig"]
 sources = ["src"]
```

### Comparing `hatch_aws_publisher-0.2.3/PKG-INFO` & `hatch_aws_publisher-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-aws-publisher
-Version: 0.2.3
+Version: 0.3.0
 Summary: Hatch plugin for deploying to AWS with SAM
 Project-URL: Documentation, https://github.com/aka-raccoon/hatch-aws-publishery#readme
 Project-URL: Issues, https://github.com/aka-raccoon/hatch-aws-publisher/issues
 Project-URL: Source, https://github.com/aka-raccoon/hatch-aws-publisher
 Author-email: aka-raccoon <aka-raccoon@pm.me>
 License: MIT License
```

