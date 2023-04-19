# Comparing `tmp/gardener-cicd-cli-1.2033.0.tar.gz` & `tmp/gardener-cicd-cli-1.2034.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-cli-1.2033.0.tar", last modified: Fri Apr 14 08:39:49 2023, max compression
+gzip compressed data, was "gardener-cicd-cli-1.2034.0.tar", last modified: Wed Apr 19 05:08:17 2023, max compression
```

## Comparing `gardener-cicd-cli-1.2033.0.tar` & `gardener-cicd-cli-1.2034.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:49.521397 gardener-cicd-cli-1.2033.0/
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-14 08:39:49.521397 gardener-cicd-cli-1.2033.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:49.517397 gardener-cicd-cli-1.2033.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3554 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/bin/component-cli
--rwxr-xr-x   0 root         (0) root         (0)      369 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/bin/helm
--rwxr-xr-x   0 root         (0) root         (0)     5611 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/bin/launch-dockerd.sh
--rwxr-xr-x   0 root         (0) root         (0)     3301 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/bin/purge_history
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/bin/yaml2json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:49.517397 gardener-cicd-cli-1.2033.0/gardener_ci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/_cfg_mgmt.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/_clamav.py
--rw-r--r--   0 root         (0) root         (0)     6463 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/_concourse.py
--rw-r--r--   0 root         (0) root         (0)     7657 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/_oci.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/_osinfo.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/_slack.py
--rw-r--r--   0 root         (0) root         (0)    11365 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/bdba.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/cd.py
--rw-r--r--   0 root         (0) root         (0)     1899 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/checkmarx_cli.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/cli_gen.py
--rw-r--r--   0 root         (0) root         (0)     7669 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/compliance.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/config.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/containerutil.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/docker.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/elastic.py
--rw-r--r--   0 root         (0) root         (0)     3512 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/gh.py
--rw-r--r--   0 root         (0) root         (0)     4935 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/githubutil.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/ocm.py
--rw-r--r--   0 root         (0) root         (0)    12255 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/productutil_v2.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/whdutil.py
--rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/gardener_ci/yaml2json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:49.521397 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-14 08:39:49.000000 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-14 08:39:49.000000 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:39:49.000000 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-04-14 08:39:49.000000 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-14 08:39:49.000000 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-14 08:39:49.000000 gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 08:39:49.521397 gardener-cicd-cli-1.2033.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1514 2023-04-14 08:09:43.000000 gardener-cicd-cli-1.2033.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:08:17.669009 gardener-cicd-cli-1.2034.0/
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-19 05:08:17.669009 gardener-cicd-cli-1.2034.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:08:17.665009 gardener-cicd-cli-1.2034.0/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10484 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/bin/component-cli
+-rwxr-xr-x   0 root         (0) root         (0)      369 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/bin/helm
+-rwxr-xr-x   0 root         (0) root         (0)     5611 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/bin/launch-dockerd.sh
+-rwxr-xr-x   0 root         (0) root         (0)     3301 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/bin/purge_history
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/bin/yaml2json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:08:17.669009 gardener-cicd-cli-1.2034.0/gardener_ci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/_cfg_mgmt.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/_clamav.py
+-rw-r--r--   0 root         (0) root         (0)     6463 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/_concourse.py
+-rw-r--r--   0 root         (0) root         (0)     7657 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/_oci.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/_osinfo.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/_slack.py
+-rw-r--r--   0 root         (0) root         (0)    11365 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/bdba.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/cd.py
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/checkmarx_cli.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/cli_gen.py
+-rw-r--r--   0 root         (0) root         (0)     7669 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/compliance.py
+-rw-r--r--   0 root         (0) root         (0)     3188 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/config.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/containerutil.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/elastic.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/gh.py
+-rw-r--r--   0 root         (0) root         (0)     4935 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/githubutil.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/ocm.py
+-rw-r--r--   0 root         (0) root         (0)    12274 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/productutil_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/whdutil.py
+-rwxr-xr-x   0 root         (0) root         (0)      265 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/gardener_ci/yaml2json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:08:17.669009 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-19 05:08:17.000000 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-19 05:08:17.000000 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 05:08:17.000000 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-04-19 05:08:17.000000 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-19 05:08:17.000000 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-19 05:08:17.000000 gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 05:08:17.669009 gardener-cicd-cli-1.2034.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1514 2023-04-19 05:07:28.000000 gardener-cicd-cli-1.2034.0/setup.py
```

### Comparing `gardener-cicd-cli-1.2033.0/bin/launch-dockerd.sh` & `gardener-cicd-cli-1.2034.0/bin/launch-dockerd.sh`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/bin/purge_history` & `gardener-cicd-cli-1.2034.0/bin/purge_history`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/_cfg_mgmt.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/_cfg_mgmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/_clamav.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/_clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/_concourse.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/_concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/_oci.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/_oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/_osinfo.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/_osinfo.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/bdba.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/bdba.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/cd.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/cd.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/checkmarx_cli.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/checkmarx_cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/cli_gen.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/cli_gen.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/compliance.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/compliance.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/config.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/config.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/containerutil.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/containerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/docker.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/docker.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/elastic.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/elastic.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/gh.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/gh.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/githubutil.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/githubutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/ocm.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/ocm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/pipeline.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         raw = yaml.safe_load(f)
 
     if not branch_cfg:
         return raw
 
     cfg_entry = branch_cfg.cfg_entry_for_branch(branch=branch_name)
 
+    if not cfg_entry:
+        return raw
+
     return ci.util.merge_dicts(
         raw,
         cfg_entry.override_definitions(),
     )
 
 
 def _component_name(
@@ -391,15 +394,14 @@
         )
         logger.info(f'copied to {outfile=}')
         exit(0)
 
     cli = os.path.join(own_dir, 'cli_gen.py')
     dependencies_cmd = ' '.join((
         cli,
-        'gardener-ci',
         'productutil_v2',
         'add_dependencies',
         '--descriptor-src-file', base_component_descriptor_file.name,
         '--descriptor-out-file', base_component_descriptor_file.name,
         '--component-version', base_component.version,
         '--component-name', base_component.name,
     ))
```

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/productutil_v2.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/productutil_v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_ci/whdutil.py` & `gardener-cicd-cli-1.2034.0/gardener_ci/whdutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/gardener_cicd_cli.egg-info/SOURCES.txt` & `gardener-cicd-cli-1.2034.0/gardener_cicd_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-cli-1.2033.0/setup.py` & `gardener-cicd-cli-1.2034.0/setup.py`

 * *Files identical despite different names*

