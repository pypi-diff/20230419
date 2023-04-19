# Comparing `tmp/piknik-0.3.2.tar.gz` & `tmp/piknik-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.2.tar", last modified: Wed Apr 19 10:46:50 2023, max compression
+gzip compressed data, was "piknik-0.3.3.tar", last modified: Wed Apr 19 19:07:27 2023, max compression
```

## Comparing `piknik-0.3.2.tar` & `piknik-0.3.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/
--rw-r--r--   0 lash      (1000) lash      (1000)     1208 2023-04-19 10:45:31.000000 piknik-0.3.2/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.2/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.2/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:46:50.373290 piknik-0.3.2/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-19 09:43:40.000000 piknik-0.3.2/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.2/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.2/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-19 09:43:40.000000 piknik-0.3.2/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      750 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2727 2023-04-19 08:29:17.000000 piknik-0.3.2/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.2/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.2/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.2/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     4837 2022-12-05 09:13:24.000000 piknik-0.3.2/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5917 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.2/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     1842 2023-04-19 09:43:40.000000 piknik-0.3.2/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-19 10:45:31.000000 piknik-0.3.2/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.2/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-19 10:46:50.000000 piknik-0.3.2/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-19 10:45:31.000000 piknik-0.3.2/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-19 10:46:50.373290 piknik-0.3.2/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.2/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.2/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:46:50.373290 piknik-0.3.2/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.2/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.2/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.2/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.2/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.2/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.2/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.2/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1361 2023-04-19 18:54:19.000000 piknik-0.3.3/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.3/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.3/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 19:07:27.616628 piknik-0.3.3/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-19 09:43:40.000000 piknik-0.3.3/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.3/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.613295 piknik-0.3.3/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.3/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-19 09:43:40.000000 piknik-0.3.3/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      834 2023-04-19 18:03:40.000000 piknik-0.3.3/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-19 18:03:31.000000 piknik-0.3.3/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.3/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.3/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.3/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.3/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.3/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-19 18:47:55.000000 piknik-0.3.3/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6203 2023-04-19 18:51:30.000000 piknik-0.3.3/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.3/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1842 2023-04-19 17:48:28.000000 piknik-0.3.3/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-19 10:45:31.000000 piknik-0.3.3/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.3/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.613295 piknik-0.3.3/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-19 19:07:27.000000 piknik-0.3.3/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-19 10:45:31.000000 piknik-0.3.3/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      829 2023-04-19 19:07:27.616628 piknik-0.3.3/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.3/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.3/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 19:07:27.616628 piknik-0.3.3/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.3/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.3/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.3/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.3/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.3/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.3/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.3/tests/test_tag.py
```

### Comparing `piknik-0.3.2/CHANGELOG` & `piknik-0.3.3/CHANGELOG`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+- 0.3.3
+	* Enable state filtering controls from cli
+	* Make finished issues not visible by default
+	* Fix last state category truncate in html rendering
 - 0.3.2
 	* Add handler for setting pending state
 	* Upgrade shep to handle empty tag directories when transferring (empty) state directories over git
 - 0.3.1
 	* Fix fail when generating html to outfile with show cli
 - 0.3.0
 	* Implement cli as subcommands
```

### Comparing `piknik-0.3.2/LICENSE` & `piknik-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/PKG-INFO` & `piknik-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.2
+Version: 0.3.3
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.2/ROADMAP` & `piknik-0.3.3/ROADMAP`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/basket.py` & `piknik-0.3.3/piknik/basket.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/cli/__init__.py` & `piknik-0.3.3/piknik/cli/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from piknik.crypto import PGPSigner
 
 class Context:
 
     def __init__(self, arg, assembler, mode=0, gpg_home=os.environ.get('GPGHOME')):
         self.issue_id = arg.issue_id
         self.files_dir = arg.files_dir
+        self.show_finished = arg.show_finished
+        self.show_states = arg.state
         #self.store_factory = FileStoreFactory(arg.d)
         store_factory = FileStoreFactory(arg.d)
         self.signer = None
         sign_fn = None
         if hasattr(arg, 's'):
             self.signer = PGPSigner(default_key=arg.s, use_agent=True)
             sign_fn = self.signer.sign
```

### Comparing `piknik-0.3.2/piknik/cli/comment.py` & `piknik-0.3.3/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/cli/mod.py` & `piknik-0.3.3/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/cli/show.py` & `piknik-0.3.3/piknik/cli/show.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,26 +75,30 @@
     accumulator = None
     accumulator_f = None
 
     issues = []
     if ctx.issue_id:
         issues.append(ctx.issue_id)
 
+    states_skip = []
+    if not ctx.show_finished:
+        states_skip.append('FINISHED')
+
     if ctx.issue_id == None:
         accumulator = set_accumulator(ctx, m)
-        renderer = m.Renderer(ctx.basket, accumulator=accumulator)
+        renderer = m.Renderer(ctx.basket, accumulator=accumulator, states_include=ctx.show_states, states_skip=states_skip)
         renderer.apply()
         issues = reset_accumulator()
 
     for issue_id in issues:
         accumulator = set_accumulator(ctx, m, issue_id=issue_id)
         issue = ctx.basket.get(issue_id)
         tags = ctx.basket.tags(issue_id)
         state = ctx.basket.get_state(issue_id)
         verifier = PGPSigner(home_dir=ctx.gpg_home, skip_verify=False)
-        renderer = m.Renderer(ctx.basket, wrapper=verifier, accumulator=accumulator)
+        renderer = m.Renderer(ctx.basket, wrapper=verifier, accumulator=accumulator, states_include=ctx.show_states, states_skip=states_skip)
 
         renderer.apply_begin()
         renderer.apply_issue(state, issue, tags)
         renderer.apply_end()
         
         reset_accumulator()
```

### Comparing `piknik-0.3.2/piknik/crypto.py` & `piknik-0.3.3/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/issue.py` & `piknik-0.3.3/piknik/issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/msg.py` & `piknik-0.3.3/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/render/base.py` & `piknik-0.3.3/piknik/render/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,29 +10,47 @@
 
 def stream_accumulator(v, w=sys.stdout):
     w.write(v)
 
 
 class Renderer:
 
-    def __init__(self, basket, accumulator=None, wrapper=None):
+    def __init__(self, basket, accumulator=None, wrapper=None, states_include=[], states_skip=[]):
         self.b = basket
         self.a = accumulator
         self.w = wrapper
         if self.w == None:
             logg.info('no wrapper defined. no message parts will be output')
         self.render_mode = 0
+        self.states = []
+        self.__make_state_filter(states_include, states_skip)
+       
+
+    def __make_state_filter(self, include, skip):
+        have_include = False
+        for i in range(len(include)):
+            include[i] = include[i].upper()
+            have_include = True
+        for i in range(len(skip)):
+            skip[i] = skip[i].upper()
+        for state in self.b.states():
+            if have_include:
+                if state not in include:
+                    continue
+            elif state in skip:
+                continue
+            self.states.append(state)
 
 
     def add(self, v, accumulator=None):
         if accumulator == None:
             accumulator = self.a
         if accumulator != None:
             if v != None:
-                accumulator(v)
+                r = accumulator(v)
 
 
     def apply_envelope_pre(self, state, issue, tags, envelope, accumulator=None):
         pass
 
 
     def apply_envelope_post(self, state, issue, tags, envelope, accumulator=None):
@@ -143,15 +161,16 @@
         pass
 
 
     def apply(self, accumulator=None):
         r = self.apply_begin()
         self.add(r)
 
-        for state in self.b.states():
+        #for state in self.b.states():
+        for state in self.states:
             r = self.apply_state_pre(state)
             self.add(r)
             r = self.apply_state(state)
             self.add(r)
             r = self.apply_state_post(state)
             self.add(r)
```

### Comparing `piknik-0.3.2/piknik/render/html.py` & `piknik-0.3.3/piknik/render/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,32 @@
         self.category = ul(_id='state_list')
         self.category_content = None
         self.issue = None
         self.msg = None
         #self.envelope_content = None
         self.envelope = None
         self.w = w
+        self.last_v = None
         self.issues = []
 
 
     def add(self, v, w=None):
         if w == None:
             w = self.w
         if len(v) == 0:
             if self.envelope != None:
                 self.msg.add(self.envelope)
             if self.msg != None:
                 self.category.add(self.msg)
                 #self.doc.add(self.msg)
             self.doc.add(self.category)
+            if self.last_v != None:
+                self.category.add(li(self.last_v))
             w.write(self.doc.render())
-            return
+            return False
 
         v_id = getattr(v, 'id', '')
         logg.debug('add id {}'.format(v_id))
         if len(v_id) > 1:
             if v_id[:2] == 's_':
                 if self.issue != None:
                     self.category_content.add(self.issue)
@@ -64,22 +67,25 @@
                     self.msg.add(self.envelope)
                 #self.envelope_content = v
                 self.envelope = li()
             elif v_id[:4] == 'd_m_':
                 self.envelope.add(v)
         else:
             self.doc = v
+            self.last_v = None
+        self.last_v = v
+        return True
 
 
 class Renderer(BaseRenderer):
 
-    def __init__(self, basket, accumulator=None, wrapper=None, outdir=None):
+    def __init__(self, basket, accumulator=None, wrapper=None, outdir=None, states_include=[], states_skip=[]):
         if accumulator == None:
             accumulator = Accumulator().add
-        super(Renderer, self).__init__(basket, accumulator=accumulator, wrapper=wrapper)
+        super(Renderer, self).__init__(basket, accumulator=accumulator, wrapper=wrapper, states_include=states_include, states_skip=states_skip)
         self.outdir = outdir
 
 
     def apply_state(self, state, accumulator=None):
         self.render_mode = 1
         v = div(_id='s_' + state.lower())
         v.add(h2(state))
```

### Comparing `piknik-0.3.2/piknik/render/plain.py` & `piknik-0.3.3/piknik/render/plain.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/runnable/cmd.py` & `piknik-0.3.3/piknik/runnable/cmd.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/store/__init__.py` & `piknik-0.3.3/piknik/store/__init__.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik/wrap.py` & `piknik-0.3.3/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/piknik.egg-info/PKG-INFO` & `piknik-0.3.3/piknik.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.2
+Version: 0.3.3
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/eth-cache
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.2/piknik.egg-info/SOURCES.txt` & `piknik-0.3.3/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/setup.cfg` & `piknik-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piknik
-version = 0.3.2
+version = 0.3.3
 description = CLI issue tracker
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-cache
 keywords = 
 	bugs
 	issues
```

### Comparing `piknik-0.3.2/setup.py` & `piknik-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_assign.py` & `piknik-0.3.3/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_basic.py` & `piknik-0.3.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_crypto.py` & `piknik-0.3.3/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_dep.py` & `piknik-0.3.3/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_html.py` & `piknik-0.3.3/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_issue.py` & `piknik-0.3.3/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_msg.py` & `piknik-0.3.3/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_render.py` & `piknik-0.3.3/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_store.py` & `piknik-0.3.3/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.2/tests/test_tag.py` & `piknik-0.3.3/tests/test_tag.py`

 * *Files identical despite different names*

