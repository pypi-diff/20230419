# Comparing `tmp/piknik-0.3.1.tar.gz` & `tmp/piknik-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.1.tar", last modified: Wed Apr 19 08:30:04 2023, max compression
+gzip compressed data, was "piknik-0.3.2.tar", last modified: Wed Apr 19 10:46:50 2023, max compression
```

## Comparing `piknik-0.3.1.tar` & `piknik-0.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/
--rw-r--r--   0 lash      (1000) lash      (1000)     1058 2023-04-19 08:29:17.000000 piknik-0.3.1/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.1/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 08:30:04.286626 piknik-0.3.1/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      538 2023-01-16 11:02:46.000000 piknik-0.3.1/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.1/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.1/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6025 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2727 2023-04-19 08:29:17.000000 piknik-0.3.1/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.1/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.1/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     4837 2022-12-05 09:13:24.000000 piknik-0.3.1/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5917 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     1727 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2175 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.1/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2022-11-18 08:08:40.000000 piknik-0.3.1/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-19 08:30:04.289959 piknik-0.3.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.1/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.1/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.1/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.1/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.1/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.1/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.1/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.1/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1208 2023-04-19 10:45:31.000000 piknik-0.3.2/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:46:50.373290 piknik-0.3.2/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-19 09:43:40.000000 piknik-0.3.2/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.2/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.2/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-19 09:43:40.000000 piknik-0.3.2/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2727 2023-04-19 08:29:17.000000 piknik-0.3.2/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.2/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.2/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4837 2022-12-05 09:13:24.000000 piknik-0.3.2/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5917 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1842 2023-04-19 09:43:40.000000 piknik-0.3.2/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-19 10:45:31.000000 piknik-0.3.2/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.2/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-19 10:45:31.000000 piknik-0.3.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-19 10:46:50.373290 piknik-0.3.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.2/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.2/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.2/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.2/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.2/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.2/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.2/tests/test_tag.py
```

### Comparing `piknik-0.3.1/CHANGELOG` & `piknik-0.3.2/CHANGELOG`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+- 0.3.2
+	* Add handler for setting pending state
+	* Upgrade shep to handle empty tag directories when transferring (empty) state directories over git
 - 0.3.1
 	* Fix fail when generating html to outfile with show cli
 - 0.3.0
 	* Implement cli as subcommands
 - 0.2.3
 	* Add possibility to set dependencies between issues
 	* Set default data directory under working directory
```

### Comparing `piknik-0.3.1/LICENSE` & `piknik-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/PKG-INFO` & `piknik-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.1/ROADMAP` & `piknik-0.3.2/ROADMAP`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-- 0.5.0
+- 0.6
 	* Verify and enforce cryptographic key of identity for assignments
-- 0.4.0
+- 0.5
+	* HTTP server for making state edits for issues locally (e.g. drag).
+- 0.4
 	* HTTP server for making state edits for issues locally (e.g. drag).
-- 0.3.0
 	* Automatially embed VCS target and source hash to issue and issue messages.
 		- target: current hash target to merge into (var)
 		- source: current hash source to merge (var)
 	* Target alias for issue, e.g. version, revision, may be:
 		- inherit from other issue
 		- target hash above
 		- git tag
```

### Comparing `piknik-0.3.1/piknik/basket.py` & `piknik-0.3.2/piknik/basket.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,18 @@
         if category == None:
             category = self.state.BACKLOG
         else:
             category = self.state.from_name(category)
         return self.state.list(category)
 
 
+    def state_pending(self, issue_id):
+        self.state.move(issue_id, self.state.PENDING)
+
+
     def state_doing(self, issue_id):
         self.state.move(issue_id, self.state.DOING)
 
 
     def state_review(self, issue_id):
         self.state.move(issue_id, self.state.REVIEW)
```

### Comparing `piknik-0.3.1/piknik/cli/__init__.py` & `piknik-0.3.2/piknik/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/cli/comment.py` & `piknik-0.3.2/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/cli/mod.py` & `piknik-0.3.2/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/cli/show.py` & `piknik-0.3.2/piknik/cli/show.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/crypto.py` & `piknik-0.3.2/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/issue.py` & `piknik-0.3.2/piknik/issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/msg.py` & `piknik-0.3.2/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/render/base.py` & `piknik-0.3.2/piknik/render/base.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/render/html.py` & `piknik-0.3.2/piknik/render/html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/render/plain.py` & `piknik-0.3.2/piknik/render/plain.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik/runnable/cmd.py` & `piknik-0.3.2/piknik/runnable/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 logging.basicConfig(level=logging.WARNING)
 logg = logging.getLogger()
 
 argp = argparse.ArgumentParser()
 argp.add_argument('-d', type=str, help='Data directory')
 argp.add_argument('-f', '--files', dest='f', action='store_true', help='Save attachments to filesystem')
 argp.add_argument('-o', '--files-dir', dest='files_dir', type=str, help='Directory to output saved files to')
+argp.add_argument('-v', action='store_true', help='Turn on debug logs')
 argp.add_argument('-i','--issue-id',  type=str, help='Issue id to show')
 argp.add_argument('cmd', type=str, help='subcommand to execute')
 strargs = copy.copy(sys.argv[1:])
 try:
     strargs.remove('-h')
 except ValueError:
     pass
@@ -48,14 +49,16 @@
     m = importlib.import_module('piknik.cli.comment')
 else:
     raise ValueError('unknown subcommand')
 
 
 argp = m.subparser(argp)
 arg = argp.parse_args(sys.argv[1:])
+if arg.v:
+    logg.setLevel(logging.DEBUG)
 
 m.ctx = Context(arg, m.assembler)
 
 
 def main():
     global m
     m.main()
```

### Comparing `piknik-0.3.1/piknik/store/__init__.py` & `piknik-0.3.2/piknik/store/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 continue
             elif k[0] == '_':
                 aliases.append(k)
                 continue
             state.add(k)
 
         for v in aliases:
-            s = state.from_elements(v)
+            s = state.from_elements(v, create_missing=True)
             state.alias(v, s)
                 
         return state
 
 
     def create_messages(self):
         d = os.path.join(self.directory, '.msg')
```

### Comparing `piknik-0.3.1/piknik/wrap.py` & `piknik-0.3.2/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/piknik.egg-info/PKG-INFO` & `piknik-0.3.2/piknik.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.1
+Version: 0.3.2
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.1/piknik.egg-info/SOURCES.txt` & `piknik-0.3.2/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/setup.cfg` & `piknik-0.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piknik
-version = 0.3.1
+version = 0.3.2
 description = CLI issue tracker
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-cache
 keywords = 
 	bugs
 	issues
```

### Comparing `piknik-0.3.1/setup.py` & `piknik-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_assign.py` & `piknik-0.3.2/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_basic.py` & `piknik-0.3.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_crypto.py` & `piknik-0.3.2/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_dep.py` & `piknik-0.3.2/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_html.py` & `piknik-0.3.2/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_issue.py` & `piknik-0.3.2/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_msg.py` & `piknik-0.3.2/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_render.py` & `piknik-0.3.2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_store.py` & `piknik-0.3.2/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.1/tests/test_tag.py` & `piknik-0.3.2/tests/test_tag.py`

 * *Files identical despite different names*

