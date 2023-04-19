# Comparing `tmp/sirqle-0.1.3.tar.gz` & `tmp/sirqle-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirqle-0.1.3.tar", last modified: Fri Apr 14 11:36:59 2023, max compression
+gzip compressed data, was "sirqle-0.1.4.tar", last modified: Wed Apr 19 10:46:39 2023, max compression
```

## Comparing `sirqle-0.1.3.tar` & `sirqle-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.1.3/.github/workflows/bump.yml
--rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.1.3/.gitignore
--rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    18092 2022-11-07 10:38:03.624761 sirqle-0.1.3/LICENSE
--rw-r--r--   0        0        0     1001 2023-04-14 11:36:55.995009 sirqle-0.1.3/Makefile
--rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.1.3/README.md
--rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.1.3/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.1.3/docs/index.md
--rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.1.3/docs/reference.md
--rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.1.3/mkdocs.yml
--rw-r--r--   0        0        0     1337 2023-04-14 11:36:34.655036 sirqle-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.1.3/requirements.txt
--rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.1.3/requirements_dev.txt
--rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.1.3/setup.py
--rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.1.3/src/sirqle/__init__.py
--rw-r--r--   0        0        0     9639 2023-04-14 11:36:06.627074 sirqle-0.1.3/src/sirqle/query.py
--rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.1.3/tests/test_create.py
--rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.1.3/tests/test_insert.py
--rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.1.4/.github/workflows/bump.yml
+-rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    18092 2022-11-07 10:38:03.624761 sirqle-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1001 2023-04-14 11:36:55.995009 sirqle-0.1.4/Makefile
+-rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.1.4/README.md
+-rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.1.4/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.1.4/docs/index.md
+-rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.1.4/docs/reference.md
+-rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.1.4/mkdocs.yml
+-rw-r--r--   0        0        0     1337 2023-04-19 10:46:31.734917 sirqle-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.1.4/requirements_dev.txt
+-rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.1.4/setup.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.1.4/src/sirqle/__init__.py
+-rw-r--r--   0        0        0     9652 2023-04-19 10:46:01.722884 sirqle-0.1.4/src/sirqle/query.py
+-rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.1.4/tests/test_create.py
+-rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.1.4/tests/test_insert.py
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.1.4/PKG-INFO
```

### Comparing `sirqle-0.1.3/.github/workflows/bump.yml` & `sirqle-0.1.4/.github/workflows/bump.yml`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/.gitignore` & `sirqle-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/.pre-commit-config.yaml` & `sirqle-0.1.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/LICENSE` & `sirqle-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/Makefile` & `sirqle-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/README.md` & `sirqle-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/docs/gen_ref_pages.py` & `sirqle-0.1.4/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/docs/index.md` & `sirqle-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/pyproject.toml` & `sirqle-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sirqle"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Pythia Dev Team", email = "dev@pythia.social" }]
 description = "SurrealDB Query interface"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = ["python-dotenv", "surrealdb==0.3.0"]
 license = { file = "LICENSE" }
 [project.urls]
@@ -49,15 +49,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.3"
+version = "0.1.4"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 bump_message = "bump: $current_version → $new_version [skip ci]"
 
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
```

### Comparing `sirqle-0.1.3/requirements_dev.txt` & `sirqle-0.1.4/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/src/sirqle/query.py` & `sirqle-0.1.4/src/sirqle/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
         if args:
             self.query += " RETURN "
-            self.query += self._parse_args(args)
+            self.query += self._parse_args(args, quote=False)
         else:
             warn(
                 "No arguments for RETURN statement. RETURN statement not \
                 added to the query."
             )
         return self
```

### Comparing `sirqle-0.1.3/tests/test_create.py` & `sirqle-0.1.4/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/tests/test_insert.py` & `sirqle-0.1.4/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.3/PKG-INFO` & `sirqle-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirqle
-Version: 0.1.3
+Version: 0.1.4
 Summary: SurrealDB Query interface
 Author-email: Pythia Dev Team <dev@pythia.social>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: surrealdb==0.3.0
 Requires-Dist: pre-commit ; extra == "dev"
```

