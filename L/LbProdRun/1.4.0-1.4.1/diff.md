# Comparing `tmp/LbProdRun-1.4.0.tar.gz` & `tmp/LbProdRun-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbProdRun-1.4.0.tar", last modified: Mon Apr 17 15:58:42 2023, max compression
+gzip compressed data, was "LbProdRun-1.4.1.tar", last modified: Wed Apr 19 09:27:16 2023, max compression
```

## Comparing `LbProdRun-1.4.0.tar` & `LbProdRun-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     2055 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2482 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    16310 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      388 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2233 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1104 2023-04-17 15:58:42.928000 LbProdRun-1.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.920000 LbProdRun-1.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/src/LbProdRun/
--rw-r--r--   0 root         (0) root         (0)    12037 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/src/LbProdRun/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/src/LbProdRun/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/src/LbProdRun/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/src/LbProdRun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      155 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-17 15:58:42.000000 LbProdRun-1.4.0/src/LbProdRun.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:58:42.924000 LbProdRun-1.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4749 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-04-17 15:58:21.000000 LbProdRun-1.4.0/tests/test_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    16310 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      388 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-04-19 09:27:16.844000 LbProdRun-1.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.836000 LbProdRun-1.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/src/LbProdRun/
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/src/LbProdRun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/src/LbProdRun/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/src/LbProdRun/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/src/LbProdRun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      155 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-19 09:27:16.000000 LbProdRun-1.4.1/src/LbProdRun.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:27:16.840000 LbProdRun-1.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     4749 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-04-19 09:26:55.000000 LbProdRun-1.4.1/tests/test_options.py
```

### Comparing `LbProdRun-1.4.0/.gitignore` & `LbProdRun-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/.gitlab-ci.yml` & `LbProdRun-1.4.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/.pre-commit-config.yaml` & `LbProdRun-1.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/.pylintrc` & `LbProdRun-1.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/LICENSE` & `LbProdRun-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/PKG-INFO` & `LbProdRun-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.4.0/README.md` & `LbProdRun-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/setup.cfg` & `LbProdRun-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/src/LbProdRun/__init__.py` & `LbProdRun-1.4.1/src/LbProdRun/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,18 @@
     if not prmon:
         pass
     elif interactive:
         typer.secho("Not using prmon as this is an interactive run!", fg="yellow")
     elif shutil.which("prmon") is None:
         typer.secho("Not using prmon as it wasn't found on $PATH!", fg="yellow")
     else:
-        command += ["prmon", "--interval", "60"]
+        command += ["prmon"]
+        command += ["--interval", os.environ.get("LBPRODRUN_PRMON_INTERVAL", "60")]
         command += ["--filename", f"prmon_{job_spec.output.prefix}.txt"]
+        command += ["--json-summary", f"prmon_{job_spec.output.prefix}.json"]
         command += ["--"]
 
     if isinstance(job_spec.application, JobSpecV1.FullDevApplication):
         command += [str(job_spec.application.run_script.absolute())]
     else:
         command += ["lb-run"]
         command += ["--siteroot=/cvmfs/lhcb.cern.ch/lib/"]
@@ -152,15 +154,16 @@
     command = ["lbexec", job_spec.options.entrypoint, str(options_yaml_fn)]
     return command + job_spec.options.extra_args
 
 
 def _write_options_yaml(job_spec, path: Path, verbose=False):
     """Write an options file for lbexec"""
     options = job_spec.options.extra_options.copy()
-    options["write_decoding_keys_to_git"] = False
+    # FIXME: Can't actually use this option yet as it doesn't fail if the keys are missing
+    # options["write_decoding_keys_to_git"] = False
 
     if job_spec.input.files:
         options["input_files"] = job_spec.input.files
     if job_spec.db_tags.dddb_tag:
         options["dddb_tag"] = job_spec.db_tags.dddb_tag
     if job_spec.db_tags.conddb_tag:
         options["conddb_tag"] = job_spec.db_tags.conddb_tag
```

### Comparing `LbProdRun-1.4.0/src/LbProdRun/__main__.py` & `LbProdRun-1.4.1/src/LbProdRun/__main__.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/src/LbProdRun/models.py` & `LbProdRun-1.4.1/src/LbProdRun/models.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/src/LbProdRun.egg-info/PKG-INFO` & `LbProdRun-1.4.1/src/LbProdRun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.4.0/tests/test_cli.py` & `LbProdRun-1.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.4.0/tests/test_options.py` & `LbProdRun-1.4.1/tests/test_options.py`

 * *Files identical despite different names*

