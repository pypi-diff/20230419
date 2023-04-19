# Comparing `tmp/piknik-0.3.0.tar.gz` & `tmp/piknik-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.0.tar", last modified: Tue Mar 21 20:54:01 2023, max compression
+gzip compressed data, was "piknik-0.3.1.tar", last modified: Wed Apr 19 08:30:04 2023, max compression
```

## Comparing `piknik-0.3.0.tar` & `piknik-0.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/
--rw-r--r--   0 lash      (1000) lash      (1000)      992 2023-03-21 20:53:45.000000 piknik-0.3.0/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-03-21 20:54:01.923312 piknik-0.3.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      538 2023-01-16 11:02:46.000000 piknik-0.3.0/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.0/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.0/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6025 2023-01-16 11:02:46.000000 piknik-0.3.0/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2731 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.0/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.0/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.0/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.0/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     4837 2022-12-05 09:13:24.000000 piknik-0.3.0/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5917 2023-01-16 11:02:46.000000 piknik-0.3.0/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.0/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     1727 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2175 2023-03-21 20:53:45.000000 piknik-0.3.0/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.0/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-03-21 20:54:01.000000 piknik-0.3.0/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-03-21 20:54:01.000000 piknik-0.3.0/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:54:01.000000 piknik-0.3.0/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-03-21 20:54:01.000000 piknik-0.3.0/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-03-21 20:54:01.000000 piknik-0.3.0/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-03-21 20:54:01.000000 piknik-0.3.0/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2022-11-18 08:08:40.000000 piknik-0.3.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-03-21 20:54:01.923312 piknik-0.3.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.0/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-21 20:54:01.923312 piknik-0.3.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.0/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.0/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.0/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.0/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.0/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.0/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.0/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.0/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.0/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.0/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1058 2023-04-19 08:29:17.000000 piknik-0.3.1/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.1/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 08:30:04.286626 piknik-0.3.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      538 2023-01-16 11:02:46.000000 piknik-0.3.1/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.1/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.1/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6025 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2727 2023-04-19 08:29:17.000000 piknik-0.3.1/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.1/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.1/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     4837 2022-12-05 09:13:24.000000 piknik-0.3.1/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5917 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.1/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1727 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2175 2023-03-21 20:53:45.000000 piknik-0.3.1/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.1/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-19 08:30:04.000000 piknik-0.3.1/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2022-11-18 08:08:40.000000 piknik-0.3.1/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-19 08:30:04.289959 piknik-0.3.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.1/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.1/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 08:30:04.286626 piknik-0.3.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.1/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.1/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.1/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.1/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.1/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.1/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.1/tests/test_tag.py
```

### Comparing `piknik-0.3.0/CHANGELOG` & `piknik-0.3.1/CHANGELOG`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+- 0.3.1
+	* Fix fail when generating html to outfile with show cli
 - 0.3.0
 	* Implement cli as subcommands
 - 0.2.3
 	* Add possibility to set dependencies between issues
 	* Set default data directory under working directory
 	* Add accept shortcut flag to piknik-mod
 - 0.2.2
```

### Comparing `piknik-0.3.0/LICENSE` & `piknik-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/PKG-INFO` & `piknik-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.0/ROADMAP` & `piknik-0.3.1/ROADMAP`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/basket.py` & `piknik-0.3.1/piknik/basket.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/cli/__init__.py` & `piknik-0.3.1/piknik/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/cli/comment.py` & `piknik-0.3.1/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/cli/mod.py` & `piknik-0.3.1/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/cli/show.py` & `piknik-0.3.1/piknik/cli/show.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,17 @@
 accumulator_f = None
 accumulator = None
 
 logg = logging.getLogger(__name__)
 
 
 
-def set_accumulator(ctx, issue_id=None):
+def set_accumulator(ctx, m, issue_id=None):
     global accumulator_f
     global accumulator
-    global m
     if ctx.files_dir != None:
         fb = None
         if issue_id == None:
             fb = 'index.html'
         else:
             fb = issue_id + '.html'
         fp = os.path.join(ctx.files_dir, fb)
@@ -77,21 +76,21 @@
     accumulator_f = None
 
     issues = []
     if ctx.issue_id:
         issues.append(ctx.issue_id)
 
     if ctx.issue_id == None:
-        accumulator = set_accumulator(ctx)
+        accumulator = set_accumulator(ctx, m)
         renderer = m.Renderer(ctx.basket, accumulator=accumulator)
         renderer.apply()
         issues = reset_accumulator()
 
     for issue_id in issues:
-        accumulator = set_accumulator(ctx, issue_id=issue_id)
+        accumulator = set_accumulator(ctx, m, issue_id=issue_id)
         issue = ctx.basket.get(issue_id)
         tags = ctx.basket.tags(issue_id)
         state = ctx.basket.get_state(issue_id)
         verifier = PGPSigner(home_dir=ctx.gpg_home, skip_verify=False)
         renderer = m.Renderer(ctx.basket, wrapper=verifier, accumulator=accumulator)
 
         renderer.apply_begin()
```

### Comparing `piknik-0.3.0/piknik/crypto.py` & `piknik-0.3.1/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/issue.py` & `piknik-0.3.1/piknik/issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/msg.py` & `piknik-0.3.1/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/render/base.py` & `piknik-0.3.1/piknik/render/base.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/render/html.py` & `piknik-0.3.1/piknik/render/html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/render/plain.py` & `piknik-0.3.1/piknik/render/plain.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/runnable/cmd.py` & `piknik-0.3.1/piknik/runnable/cmd.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/store/__init__.py` & `piknik-0.3.1/piknik/store/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik/wrap.py` & `piknik-0.3.1/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/piknik.egg-info/PKG-INFO` & `piknik-0.3.1/piknik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.0
+Version: 0.3.1
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.0/piknik.egg-info/SOURCES.txt` & `piknik-0.3.1/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/setup.cfg` & `piknik-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piknik
-version = 0.3.0
+version = 0.3.1
 description = CLI issue tracker
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-cache
 keywords = 
 	bugs
 	issues
```

### Comparing `piknik-0.3.0/setup.py` & `piknik-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_assign.py` & `piknik-0.3.1/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_basic.py` & `piknik-0.3.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_crypto.py` & `piknik-0.3.1/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_dep.py` & `piknik-0.3.1/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_html.py` & `piknik-0.3.1/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_issue.py` & `piknik-0.3.1/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_msg.py` & `piknik-0.3.1/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_render.py` & `piknik-0.3.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_store.py` & `piknik-0.3.1/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.0/tests/test_tag.py` & `piknik-0.3.1/tests/test_tag.py`

 * *Files identical despite different names*

