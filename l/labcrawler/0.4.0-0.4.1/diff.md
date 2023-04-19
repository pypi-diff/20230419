# Comparing `tmp/labcrawler-0.4.0.tar.gz` & `tmp/labcrawler-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labcrawler-0.4.0.tar", last modified: Wed Apr 19 18:08:51 2023, max compression
+gzip compressed data, was "labcrawler-0.4.1.tar", last modified: Wed Apr 19 19:05:43 2023, max compression
```

## Comparing `labcrawler-0.4.0.tar` & `labcrawler-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 18:08:51.027929 labcrawler-0.4.0/
--rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-0.4.0/LICENSE
--rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-19 18:08:27.000000 labcrawler-0.4.0/MANIFEST.in
--rw-r--r--   0 francispotter   (501) staff       (20)     9034 2023-04-19 18:08:51.027523 labcrawler-0.4.0/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)     8752 2023-04-19 18:08:27.000000 labcrawler-0.4.0/README.md
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 18:08:51.022677 labcrawler-0.4.0/labcrawler/
--rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-0.4.0/labcrawler/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/__main__.py
--rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/_legacy.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3311 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/analysis.py
--rw-r--r--   0 francispotter   (501) staff       (20)     5354 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/cli.py
--rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-0.4.0/labcrawler/gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)     3040 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/gitlab_ci_data_loader.py
--rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-0.4.0/labcrawler/gitlab_repository_files_extractor.py
--rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/project_data_file.py
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 18:08:51.026319 labcrawler-0.4.0/labcrawler/templates/
--rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/templates/__init__.py
--rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/templates/labcrawler.json.template
--rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-19 18:08:27.000000 labcrawler-0.4.0/labcrawler/templates/meltano.yml
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 18:08:51.025033 labcrawler-0.4.0/labcrawler.egg-info/
--rw-r--r--   0 francispotter   (501) staff       (20)     9034 2023-04-19 18:08:51.000000 labcrawler-0.4.0/labcrawler.egg-info/PKG-INFO
--rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-19 18:08:51.000000 labcrawler-0.4.0/labcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-19 18:08:51.000000 labcrawler-0.4.0/labcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-19 18:08:51.000000 labcrawler-0.4.0/labcrawler.egg-info/entry_points.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-19 18:08:51.000000 labcrawler-0.4.0/labcrawler.egg-info/requires.txt
--rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-19 18:08:51.000000 labcrawler-0.4.0/labcrawler.egg-info/top_level.txt
--rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-19 18:08:27.000000 labcrawler-0.4.0/pyproject.toml
--rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-19 18:08:51.028032 labcrawler-0.4.0/setup.cfg
-drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 18:08:51.026785 labcrawler-0.4.0/test/
--rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-0.4.0/test/test_gitlab_ci_config.py
--rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-19 18:08:36.000000 labcrawler-0.4.0/version
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:05:43.197943 labcrawler-0.4.1/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1071 2023-03-20 17:28:47.000000 labcrawler-0.4.1/LICENSE
+-rw-r--r--   0 francispotter   (501) staff       (20)       30 2023-04-19 19:01:23.000000 labcrawler-0.4.1/MANIFEST.in
+-rw-r--r--   0 francispotter   (501) staff       (20)     9034 2023-04-19 19:05:43.197001 labcrawler-0.4.1/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)     8752 2023-04-19 19:01:23.000000 labcrawler-0.4.1/README.md
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:05:43.188360 labcrawler-0.4.1/labcrawler/
+-rw-r--r--   0 francispotter   (501) staff       (20)        0 2023-04-05 15:51:26.000000 labcrawler-0.4.1/labcrawler/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)       90 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/__main__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     4267 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/_legacy.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3474 2023-04-19 19:02:51.000000 labcrawler-0.4.1/labcrawler/analysis.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     5354 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/cli.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     1101 2023-04-05 15:42:21.000000 labcrawler-0.4.1/labcrawler/gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     3040 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/gitlab_ci_data_loader.py
+-rw-r--r--   0 francispotter   (501) staff       (20)     2388 2023-04-05 15:46:57.000000 labcrawler-0.4.1/labcrawler/gitlab_repository_files_extractor.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      451 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/project_data_file.py
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:05:43.193745 labcrawler-0.4.1/labcrawler/templates/
+-rw-r--r--   0 francispotter   (501) staff       (20)       51 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/templates/__init__.py
+-rw-r--r--   0 francispotter   (501) staff       (20)      264 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/templates/labcrawler.json.template
+-rw-r--r--   0 francispotter   (501) staff       (20)     1003 2023-04-19 19:01:23.000000 labcrawler-0.4.1/labcrawler/templates/meltano.yml
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:05:43.191873 labcrawler-0.4.1/labcrawler.egg-info/
+-rw-r--r--   0 francispotter   (501) staff       (20)     9034 2023-04-19 19:05:43.000000 labcrawler-0.4.1/labcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 francispotter   (501) staff       (20)      656 2023-04-19 19:05:43.000000 labcrawler-0.4.1/labcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)        1 2023-04-19 19:05:43.000000 labcrawler-0.4.1/labcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       87 2023-04-19 19:05:43.000000 labcrawler-0.4.1/labcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       64 2023-04-19 19:05:43.000000 labcrawler-0.4.1/labcrawler.egg-info/requires.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)       11 2023-04-19 19:05:43.000000 labcrawler-0.4.1/labcrawler.egg-info/top_level.txt
+-rw-r--r--   0 francispotter   (501) staff       (20)      689 2023-04-19 19:01:23.000000 labcrawler-0.4.1/pyproject.toml
+-rw-r--r--   0 francispotter   (501) staff       (20)       38 2023-04-19 19:05:43.198071 labcrawler-0.4.1/setup.cfg
+drwxr-xr-x   0 francispotter   (501) staff       (20)        0 2023-04-19 19:05:43.194403 labcrawler-0.4.1/test/
+-rw-r--r--   0 francispotter   (501) staff       (20)     1721 2023-04-05 15:42:37.000000 labcrawler-0.4.1/test/test_gitlab_ci_config.py
+-rw-r--r--   0 francispotter   (501) staff       (20)        5 2023-04-19 19:05:32.000000 labcrawler-0.4.1/version
```

### Comparing `labcrawler-0.4.0/LICENSE` & `labcrawler-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/PKG-INFO` & `labcrawler-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 0.4.0
+Version: 0.4.1
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labcrawler-0.4.0/README.md` & `labcrawler-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler/_legacy.py` & `labcrawler-0.4.1/labcrawler/_legacy.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler/analysis.py` & `labcrawler-0.4.1/labcrawler/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,17 +39,20 @@
 class AssembledDataSet(DataSet):
 
     def __init__(self, raw:RawDataSet):
         self.access_levels = \
                 DataFrame(data = [[0,'No access'], [5,'Minimal access'],
                 [10, 'Guest'], [20, 'Reporter'], [30, 'Developer'], [40, 'Maintainer'],
                 [50, 'Owner']], columns = ['id', 'name']).set_index('id')
-        self.groups = raw.groups.set_index('id')
-        self.projects = raw.projects.set_index('id')
-        self.users = raw.users.set_index('id')
+        if isinstance(raw.groups, DataFrame):
+                self.groups = raw.groups.set_index('id')
+        if isinstance(raw.projects, DataFrame):
+                self.projects = raw.projects.set_index('id')
+        if isinstance(raw.users, DataFrame):
+                self.users = raw.users.set_index('id')
         self.branches = raw.branches.set_index('project_id').\
                 join(self.projects[['path_with_namespace']].add_prefix('project_'))
         if isinstance(raw.merge_requests, DataFrame):
                 self.merge_requests = raw.merge_requests.set_index('project_id').\
                         join(self.projects[['path_with_namespace']].add_prefix('project_'))
         if isinstance(raw.project_members, DataFrame):
                 self.project_members = raw.project_members.\
```

### Comparing `labcrawler-0.4.0/labcrawler/cli.py` & `labcrawler-0.4.1/labcrawler/cli.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler/gitlab_ci_config.py` & `labcrawler-0.4.1/labcrawler/gitlab_ci_config.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler/gitlab_ci_data_loader.py` & `labcrawler-0.4.1/labcrawler/gitlab_ci_data_loader.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler/gitlab_repository_files_extractor.py` & `labcrawler-0.4.1/labcrawler/gitlab_repository_files_extractor.py`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler/templates/meltano.yml` & `labcrawler-0.4.1/labcrawler/templates/meltano.yml`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/labcrawler.egg-info/PKG-INFO` & `labcrawler-0.4.1/labcrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labcrawler
-Version: 0.4.0
+Version: 0.4.1
 Summary: Analysis tool for GitLab project and CI configurations
 Author-email: Steampunk Wizard <labcrawler@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.6.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `labcrawler-0.4.0/labcrawler.egg-info/SOURCES.txt` & `labcrawler-0.4.1/labcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/pyproject.toml` & `labcrawler-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `labcrawler-0.4.0/test/test_gitlab_ci_config.py` & `labcrawler-0.4.1/test/test_gitlab_ci_config.py`

 * *Files identical despite different names*

