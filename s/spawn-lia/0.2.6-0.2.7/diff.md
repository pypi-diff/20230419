# Comparing `tmp/spawn-lia-0.2.6.tar.gz` & `tmp/spawn-lia-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spawn-lia-0.2.6.tar", last modified: Sat Apr 15 20:40:27 2023, max compression
+gzip compressed data, was "spawn-lia-0.2.7.tar", last modified: Wed Apr 19 19:31:04 2023, max compression
```

## Comparing `spawn-lia-0.2.6.tar` & `spawn-lia-0.2.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.645855 spawn-lia-0.2.6/
--rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/LICENSE.txt
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)     3835 2023-04-07 19:35:39.000000 spawn-lia-0.2.6/README.md
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/bounty/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/bounty/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     4814 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/bounty/heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      554 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/bounty/testing.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/conversation/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1028 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/conversation/ask_to_proceed.py
--rw-r--r--   0 developer  (1001) developer  (1001)      103 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/decision.py
--rw-r--r--   0 developer  (1001) developer  (1001)      960 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/conversation/emojis.py
--rw-r--r--   0 developer  (1001) developer  (1001)      395 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/end_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)      506 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/conversation/get_input.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1015 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/start_message.py
--rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/conversation/virtualenv.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/git_operations/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/git_operations/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)      974 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/git_operations/push.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/git_operations/verify_branch.py
--rw-r--r--   0 developer  (1001) developer  (1001)      608 2023-04-15 20:40:15.000000 spawn-lia-0.2.6/lia/main.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/simplify/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/simplify/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1768 2023-04-15 20:40:16.000000 spawn-lia-0.2.6/lia/simplify/create_venv.py
--rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/simplify/verify_package.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/lia/support/
--rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.6/lia/support/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1260 2023-04-15 19:23:40.000000 spawn-lia-0.2.6/lia/support/deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-15 20:40:27.645855 spawn-lia-0.2.6/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-15 20:40:08.000000 spawn-lia-0.2.6/setup.py
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/spawn_lia.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1001)     4301 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1001)      894 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/entry_points.txt
--rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/requires.txt
--rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-15 20:40:27.000000 spawn-lia-0.2.6/spawn_lia.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-15 20:40:27.642521 spawn-lia-0.2.6/tests/
--rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.6/tests/test_deploy.py
--rw-r--r--   0 developer  (1001) developer  (1001)     5008 2023-04-15 20:39:34.000000 spawn-lia-0.2.6/tests/test_git_operations.py
--rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.6/tests/test_heal.py
--rw-r--r--   0 developer  (1001) developer  (1001)      885 2023-04-15 20:39:34.000000 spawn-lia-0.2.6/tests/test_venv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/
+-rw-r--r--   0 developer  (1001) developer  (1001)    34693 2023-04-19 19:30:54.000000 spawn-lia-0.2.7/LICENSE.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)     4659 2023-04-19 19:30:12.000000 spawn-lia-0.2.7/README.md
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.156620 spawn-lia-0.2.7/lia/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/bounty/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/bounty/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     4814 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/bounty/heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      554 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/bounty/testing.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/conversation/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1028 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/conversation/ask_to_proceed.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      103 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/decision.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      960 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/conversation/emojis.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      395 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/end_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      506 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/conversation/get_input.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1015 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/start_message.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     2218 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/conversation/virtualenv.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/git_operations/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/git_operations/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1546 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/git_operations/push.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1486 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/git_operations/verify_branch.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      608 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/lia/main.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/simplify/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/simplify/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1768 2023-04-19 19:30:55.000000 spawn-lia-0.2.7/lia/simplify/create_venv.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      246 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/simplify/verify_package.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/lia/support/
+-rw-r--r--   0 developer  (1001) developer  (1001)        0 2023-04-14 19:08:10.000000 spawn-lia-0.2.7/lia/support/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1260 2023-04-15 19:23:40.000000 spawn-lia-0.2.7/lia/support/deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)       38 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/setup.cfg
+-rw-r--r--   0 developer  (1001) developer  (1001)     1156 2023-04-19 19:30:21.000000 spawn-lia-0.2.7/setup.py
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/spawn_lia.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1001)     5125 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1001)      894 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        1 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       40 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)       96 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1001)        4 2023-04-19 19:31:04.000000 spawn-lia-0.2.7/spawn_lia.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (1001) developer  (1001)        0 2023-04-19 19:31:04.159954 spawn-lia-0.2.7/tests/
+-rw-r--r--   0 developer  (1001) developer  (1001)      626 2023-04-07 19:00:56.000000 spawn-lia-0.2.7/tests/test_deploy.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     5018 2023-04-19 19:25:28.000000 spawn-lia-0.2.7/tests/test_git_operations.py
+-rw-r--r--   0 developer  (1001) developer  (1001)     1140 2023-04-12 17:06:07.000000 spawn-lia-0.2.7/tests/test_heal.py
+-rw-r--r--   0 developer  (1001) developer  (1001)      885 2023-04-15 20:42:23.000000 spawn-lia-0.2.7/tests/test_venv.py
```

### Comparing `spawn-lia-0.2.6/LICENSE.txt` & `spawn-lia-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/PKG-INFO` & `spawn-lia-0.2.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: spawn-lia
-Version: 0.2.6
-Summary: The most wanted support
-Home-page: https://codeberg.org/cap_jmk/lia
-Author: Julian M. Kleber
-Author-email: julian.kleber@sail.black
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # lia
 
 [![Downloads](https://static.pepy.tech/personalized-badge/spawn-lia?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/spawn-lia)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20-blue)
 ![Style Black](https://warehouse-camo.ingress.cmh1.psfhosted.org/fbfdc7754183ecf079bc71ddeabaf88f6cbc5c00/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d626c61636b2d3030303030302e737667)
 [![PyPI - Version](https://img.shields.io/pypi/v/spawn-lia.svg)](https://pypi.org/project/spawn-lia)
@@ -28,14 +14,16 @@
 
 <!-- TOC -->
 - [1. Why?](#1-why)
 - [2. What?](#2-what)
 - [3. Lia](#3-lia)
 - [4. Installation](#4-installation)
 - [5. Usage](#5-usage)
+- [6. # Deployments](#6--deployments)
+    - [6.1. Git operations](#61-git-operations)
 <!-- /TOC -->
 
 ## 1. Why?
 
 Remember code is poetry. And we write our own story. And for this, we need a support.
 
 Without a support, all your efforts will fail. A support takes care we do all the necessary things we would not find time during battles. We need a support. So we asked `lia` to join us.
@@ -56,15 +44,19 @@
 
 In fact, the name is so similar to `lua` a common language for creating cyber weapons that altering the name into something more beautiful pays attention to the fact that `lia` is doing more or less the exact opposite of `lua`.
 
 Also check the movie [Warcraft](https://www.imdb.com/title/tt0803096/) for background information about the story. It is going on for some time now. But we decided to not just sit still since the world became full of war recently. Thats why we will grow into our predestined roles. Its destiny.
 
 You can't avoid destiny. It is even waste of time trying to. Surrendering is a proven method for manifestation. You probably know that anyways.
 
-We are excited what the future has prepared for us. ⛵
+If you read through books about Agile Development, Refactoring and Clean Coding you maybe realize that security, value generation, and awesome products do have a lot to do with these books. `Thus, true developers have one common enemy: The Fel.` 
+
+We hope the tool brings you joy in winning your daily battles against the Fel. 
+
+We built for a better future. And we are excited what the future has prepared for us. ⛵
 
 ## 4. Installation
 
 ```bash
 pip install spawn-lia
 ```
 
@@ -90,30 +82,56 @@
 
 ```bash
 cast spawn-lia
 ```
 
 ## 5. Usage
 
+To get general information about the spells `lia` has to offer run the plain command
+
+```bash
+lia
+```
+
+### CI 
+
 To improve the quality of your package and doing local CI do:
 
 ```bash
 lia heal package
 ```
 
 Do not be afraid you will probably see many errors. This behavior is intended and shall raise your attention to all sorts of errors, bugs, technical debt and antipatterns in your code.
 
 Getting rid of everything may be tedious but it is doable. We are going through the same process. It improved everything for us.
 
 If you need more information about typing, then the `mypy` [documentation](https://mypy.readthedocs.io/en/stable/getting_started.html) is a great place to start.
 
+### CI in container
+
+For all remote CI systems like Drone CI, Woodpecker, Actions, etc. 
+
+```bash
+lia heal package
+```
+
+### 5.1. Deployments
+
 To deploy you package do
 
+
 ```bash
 lia deploy package 
 ```
 
+### 5.2. Git operations 
+
+```bash
+lia push origin_name
+```
+where origin name is the name of your remote, e.g. `origin`
+
 # Support the Development
 
 To support the development you can
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

### Comparing `spawn-lia-0.2.6/README.md` & `spawn-lia-0.2.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,240 +1,321 @@
-00000000: 2320 6c69 610a 0a5b 215b 446f 776e 6c6f  # lia..[![Downlo
-00000010: 6164 735d 2868 7474 7073 3a2f 2f73 7461  ads](https://sta
-00000020: 7469 632e 7065 7079 2e74 6563 682f 7065  tic.pepy.tech/pe
-00000030: 7273 6f6e 616c 697a 6564 2d62 6164 6765  rsonalized-badge
-00000040: 2f73 7061 776e 2d6c 6961 3f70 6572 696f  /spawn-lia?perio
-00000050: 643d 746f 7461 6c26 756e 6974 733d 696e  d=total&units=in
-00000060: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
-00000070: 656d 266c 6566 745f 636f 6c6f 723d 626c  em&left_color=bl
-00000080: 6163 6b26 7269 6768 745f 636f 6c6f 723d  ack&right_color=
-00000090: 6f72 616e 6765 266c 6566 745f 7465 7874  orange&left_text
-000000a0: 3d44 6f77 6e6c 6f61 6473 295d 2868 7474  =Downloads)](htt
-000000b0: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
-000000c0: 726f 6a65 6374 2f73 7061 776e 2d6c 6961  roject/spawn-lia
-000000d0: 290a 5b21 5b4c 6963 656e 7365 3a20 4750  ).[![License: GP
-000000e0: 4c20 7633 5d28 6874 7470 733a 2f2f 696d  L v3](https://im
-000000f0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000100: 6765 2f4c 6963 656e 7365 2d47 504c 5f76  ge/License-GPL_v
-00000110: 332d 626c 7565 2e73 7667 295d 2868 7474  3-blue.svg)](htt
-00000120: 7073 3a2f 2f77 7777 2e67 6e75 2e6f 7267  ps://www.gnu.org
-00000130: 2f6c 6963 656e 7365 732f 6770 6c2d 332e  /licenses/gpl-3.
-00000140: 3029 0a21 5b50 7974 686f 6e20 5665 7273  0).![Python Vers
-00000150: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
-00000160: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000170: 6765 2f70 7974 686f 6e2d 332e 3825 3230  ge/python-3.8%20
-00000180: 2537 4325 3230 332e 3925 3230 2537 4325  %7C%203.9%20%7C%
-00000190: 3230 332e 3130 2532 3025 3743 2532 3033  203.10%20%7C%203
-000001a0: 2e31 3125 3230 2537 4325 3230 2d62 6c75  .11%20%7C%20-blu
-000001b0: 6529 0a21 5b53 7479 6c65 2042 6c61 636b  e).![Style Black
-000001c0: 5d28 6874 7470 733a 2f2f 7761 7265 686f  ](https://wareho
-000001d0: 7573 652d 6361 6d6f 2e69 6e67 7265 7373  use-camo.ingress
-000001e0: 2e63 6d68 312e 7073 6668 6f73 7465 642e  .cmh1.psfhosted.
-000001f0: 6f72 672f 6662 6664 6337 3735 3431 3833  org/fbfdc7754183
-00000200: 6563 6630 3739 6263 3731 6464 6561 6261  ecf079bc71ddeaba
-00000210: 6638 3866 3663 6263 3563 3030 2f36 3837  f88f6cbc5c00/687
-00000220: 3437 3437 3037 3333 6132 6632 6636 3936  47470733a2f2f696
-00000230: 6436 3732 6537 3336 3836 3936 3536 6336  d672e736869656c6
-00000240: 3437 3332 6536 3936 6632 6636 3236 3136  4732e696f2f62616
-00000250: 3436 3736 3532 6636 3336 6636 3436 3532  467652f636f64652
-00000260: 3533 3233 3037 3337 3437 3936 6336 3532  532307374796c652
-00000270: 6436 3236 6336 3136 3336 6232 6433 3033  d626c61636b2d303
-00000280: 3033 3033 3033 3033 3032 6537 3337 3636  0303030302e73766
-00000290: 3729 0a5b 215b 5079 5049 202d 2056 6572  7).[![PyPI - Ver
-000002a0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-000002b0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000002c0: 692f 762f 7370 6177 6e2d 6c69 612e 7376  i/v/spawn-lia.sv
-000002d0: 6729 5d28 6874 7470 733a 2f2f 7079 7069  g)](https://pypi
-000002e0: 2e6f 7267 2f70 726f 6a65 6374 2f73 7061  .org/project/spa
-000002f0: 776e 2d6c 6961 290a 0a21 5b4c 6961 5d28  wn-lia)..![Lia](
-00000300: 6c69 612e 6a70 6729 0a0a 2d2d 2d2d 2d0a  lia.jpg)..-----.
-00000310: 0a2a 2a54 6162 6c65 206f 6620 436f 6e74  .**Table of Cont
-00000320: 656e 7473 2a2a 0a0a 3c21 2d2d 2054 4f43  ents**..<!-- TOC
-00000330: 202d 2d3e 0a2d 205b 312e 2057 6879 3f5d   -->.- [1. Why?]
-00000340: 2823 312d 7768 7929 0a2d 205b 322e 2057  (#1-why).- [2. W
-00000350: 6861 743f 5d28 2332 2d77 6861 7429 0a2d  hat?](#2-what).-
-00000360: 205b 332e 204c 6961 5d28 2333 2d6c 6961   [3. Lia](#3-lia
-00000370: 290a 2d20 5b34 2e20 496e 7374 616c 6c61  ).- [4. Installa
-00000380: 7469 6f6e 5d28 2334 2d69 6e73 7461 6c6c  tion](#4-install
-00000390: 6174 696f 6e29 0a2d 205b 352e 2055 7361  ation).- [5. Usa
-000003a0: 6765 5d28 2335 2d75 7361 6765 290a 3c21  ge](#5-usage).<!
-000003b0: 2d2d 202f 544f 4320 2d2d 3e0a 0a23 2320  -- /TOC -->..## 
-000003c0: 312e 2057 6879 3f0a 0a52 656d 656d 6265  1. Why?..Remembe
-000003d0: 7220 636f 6465 2069 7320 706f 6574 7279  r code is poetry
-000003e0: 2e20 416e 6420 7765 2077 7269 7465 206f  . And we write o
-000003f0: 7572 206f 776e 2073 746f 7279 2e20 416e  ur own story. An
-00000400: 6420 666f 7220 7468 6973 2c20 7765 206e  d for this, we n
-00000410: 6565 6420 6120 7375 7070 6f72 742e 0a0a  eed a support...
-00000420: 5769 7468 6f75 7420 6120 7375 7070 6f72  Without a suppor
-00000430: 742c 2061 6c6c 2079 6f75 7220 6566 666f  t, all your effo
-00000440: 7274 7320 7769 6c6c 2066 6169 6c2e 2041  rts will fail. A
-00000450: 2073 7570 706f 7274 2074 616b 6573 2063   support takes c
-00000460: 6172 6520 7765 2064 6f20 616c 6c20 7468  are we do all th
-00000470: 6520 6e65 6365 7373 6172 7920 7468 696e  e necessary thin
-00000480: 6773 2077 6520 776f 756c 6420 6e6f 7420  gs we would not 
-00000490: 6669 6e64 2074 696d 6520 6475 7269 6e67  find time during
-000004a0: 2062 6174 746c 6573 2e20 5765 206e 6565   battles. We nee
-000004b0: 6420 6120 7375 7070 6f72 742e 2053 6f20  d a support. So 
-000004c0: 7765 2061 736b 6564 2060 6c69 6160 2074  we asked `lia` t
-000004d0: 6f20 6a6f 696e 2075 732e 0a0a 5368 6520  o join us...She 
-000004e0: 7072 6f74 6563 7473 2075 7320 6672 6f6d  protects us from
-000004f0: 206d 616c 6963 696f 7573 2061 6476 6572   malicious adver
-00000500: 7361 7269 6573 2c20 616e 6420 6865 616c  saries, and heal
-00000510: 7320 6f75 7220 6f72 6761 6e69 7a61 7469  s our organizati
-00000520: 6f6e 2062 7920 6d61 6b69 6e67 206f 7572  on by making our
-00000530: 2070 6f65 7472 7920 6265 7474 6572 2061   poetry better a
-00000540: 6e64 2074 6865 7265 6279 206f 7572 2073  nd thereby our s
-00000550: 746f 7279 2e0a 0a23 2320 322e 2057 6861  tory...## 2. Wha
-00000560: 743f 0a0a 606c 6961 6020 6973 2074 6865  t?..`lia` is the
-00000570: 2062 6573 7420 7375 7070 6f72 7420 796f   best support yo
-00000580: 7520 6361 6e20 686f 7065 2066 6f72 2e20  u can hope for. 
-00000590: 5368 6520 6865 6c70 7320 7573 2074 6f20  She helps us to 
-000005a0: 6d61 696e 7461 696e 206f 7572 2073 6869  maintain our shi
-000005b0: 702c 2066 6967 6874 2065 6e65 6d69 6573  p, fight enemies
-000005c0: 2c20 616e 6420 7769 6e20 6375 7374 6f6d  , and win custom
-000005d0: 6572 732e 0a0a 2323 2033 2e20 4c69 610a  ers...## 3. Lia.
-000005e0: 0a57 6879 2064 6964 2077 6520 6e61 6d65  .Why did we name
-000005f0: 2074 6865 2070 6163 6b61 6765 2060 6c69   the package `li
-00000600: 6160 3f0a 0a41 7320 6120 7368 6f72 7420  a`?..As a short 
-00000610: 666f 726d 206f 6620 456c 6973 6162 6574  form of Elisabet
-00000620: 682c 204c 6961 206d 6561 6e73 2022 476f  h, Lia means "Go
-00000630: 6420 6973 2066 756c 6c6e 6573 7322 2c20  d is fullness", 
-00000640: 2247 6f64 2069 7320 6d79 206f 6174 6822  "God is my oath"
-00000650: 206f 7220 2247 6f64 2073 7765 6172 7322   or "God swears"
-00000660: 2e20 4672 6f6d 2041 6d69 6c69 6120 4c69  . From Amilia Li
-00000670: 6120 6765 7473 2074 6865 206d 6561 6e69  a gets the meani
-00000680: 6e67 7320 2274 6865 207a 6561 6c6f 7573  ngs "the zealous
-00000690: 222c 2022 7468 6520 696d 6974 6174 6f72  ", "the imitator
-000006a0: 2220 6f72 2022 7468 6520 636f 6d70 6574  " or "the compet
-000006b0: 6974 6f72 2220 616e 6420 6672 6f6d 204a  itor" and from J
-000006c0: 756c 6961 2022 6672 6f6d 2074 6865 2066  ulia "from the f
-000006d0: 616d 696c 7920 6f66 2074 6865 204a 756c  amily of the Jul
-000006e0: 6969 2220 6f72 2022 636f 6e73 6563 7261  ii" or "consecra
-000006f0: 7465 6420 746f 204a 7570 6974 6572 222e  ted to Jupiter".
-00000700: 204c 6961 2069 7320 616c 736f 2074 6865   Lia is also the
-00000710: 2049 7269 7368 2077 6f72 6420 666f 7220   Irish word for 
-00000720: 2268 6561 6c65 7222 2e0a 0a41 6c6c 206f  "healer"...All o
-00000730: 7468 6572 206d 6561 6e69 6e67 7320 646f  ther meanings do
-00000740: 206e 6f74 206d 6174 7465 7220 696e 2074   not matter in t
-00000750: 6869 7320 636f 6e74 6578 7420 7768 6174  his context what
-00000760: 736f 6576 6572 2e0a 0a49 6e20 6661 6374  soever...In fact
-00000770: 2c20 7468 6520 6e61 6d65 2069 7320 736f  , the name is so
-00000780: 2073 696d 696c 6172 2074 6f20 606c 7561   similar to `lua
-00000790: 6020 6120 636f 6d6d 6f6e 206c 616e 6775  ` a common langu
-000007a0: 6167 6520 666f 7220 6372 6561 7469 6e67  age for creating
-000007b0: 2063 7962 6572 2077 6561 706f 6e73 2074   cyber weapons t
-000007c0: 6861 7420 616c 7465 7269 6e67 2074 6865  hat altering the
-000007d0: 206e 616d 6520 696e 746f 2073 6f6d 6574   name into somet
-000007e0: 6869 6e67 206d 6f72 6520 6265 6175 7469  hing more beauti
-000007f0: 6675 6c20 7061 7973 2061 7474 656e 7469  ful pays attenti
-00000800: 6f6e 2074 6f20 7468 6520 6661 6374 2074  on to the fact t
-00000810: 6861 7420 606c 6961 6020 6973 2064 6f69  hat `lia` is doi
-00000820: 6e67 206d 6f72 6520 6f72 206c 6573 7320  ng more or less 
-00000830: 7468 6520 6578 6163 7420 6f70 706f 7369  the exact opposi
-00000840: 7465 206f 6620 606c 7561 602e 0a0a 416c  te of `lua`...Al
-00000850: 736f 2063 6865 636b 2074 6865 206d 6f76  so check the mov
-00000860: 6965 205b 5761 7263 7261 6674 5d28 6874  ie [Warcraft](ht
-00000870: 7470 733a 2f2f 7777 772e 696d 6462 2e63  tps://www.imdb.c
-00000880: 6f6d 2f74 6974 6c65 2f74 7430 3830 3330  om/title/tt08030
-00000890: 3936 2f29 2066 6f72 2062 6163 6b67 726f  96/) for backgro
-000008a0: 756e 6420 696e 666f 726d 6174 696f 6e20  und information 
-000008b0: 6162 6f75 7420 7468 6520 7374 6f72 792e  about the story.
-000008c0: 2049 7420 6973 2067 6f69 6e67 206f 6e20   It is going on 
-000008d0: 666f 7220 736f 6d65 2074 696d 6520 6e6f  for some time no
-000008e0: 772e 2042 7574 2077 6520 6465 6369 6465  w. But we decide
-000008f0: 6420 746f 206e 6f74 206a 7573 7420 7369  d to not just si
-00000900: 7420 7374 696c 6c20 7369 6e63 6520 7468  t still since th
-00000910: 6520 776f 726c 6420 6265 6361 6d65 2066  e world became f
-00000920: 756c 6c20 6f66 2077 6172 2072 6563 656e  ull of war recen
-00000930: 746c 792e 2054 6861 7473 2077 6879 2077  tly. Thats why w
-00000940: 6520 7769 6c6c 2067 726f 7720 696e 746f  e will grow into
-00000950: 206f 7572 2070 7265 6465 7374 696e 6564   our predestined
-00000960: 2072 6f6c 6573 2e20 4974 7320 6465 7374   roles. Its dest
-00000970: 696e 792e 0a0a 596f 7520 6361 6e27 7420  iny...You can't 
-00000980: 6176 6f69 6420 6465 7374 696e 792e 2049  avoid destiny. I
-00000990: 7420 6973 2065 7665 6e20 7761 7374 6520  t is even waste 
-000009a0: 6f66 2074 696d 6520 7472 7969 6e67 2074  of time trying t
-000009b0: 6f2e 2053 7572 7265 6e64 6572 696e 6720  o. Surrendering 
-000009c0: 6973 2061 2070 726f 7665 6e20 6d65 7468  is a proven meth
-000009d0: 6f64 2066 6f72 206d 616e 6966 6573 7461  od for manifesta
-000009e0: 7469 6f6e 2e20 596f 7520 7072 6f62 6162  tion. You probab
-000009f0: 6c79 206b 6e6f 7720 7468 6174 2061 6e79  ly know that any
-00000a00: 7761 7973 2e0a 0a57 6520 6172 6520 6578  ways...We are ex
-00000a10: 6369 7465 6420 7768 6174 2074 6865 2066  cited what the f
-00000a20: 7574 7572 6520 6861 7320 7072 6570 6172  uture has prepar
-00000a30: 6564 2066 6f72 2075 732e 20e2 9bb5 0a0a  ed for us. .....
-00000a40: 2323 2034 2e20 496e 7374 616c 6c61 7469  ## 4. Installati
-00000a50: 6f6e 0a0a 6060 6062 6173 680a 7069 7020  on..```bash.pip 
-00000a60: 696e 7374 616c 6c20 7370 6177 6e2d 6c69  install spawn-li
-00000a70: 610a 6060 600a 0a49 6620 796f 7520 7761  a.```..If you wa
-00000a80: 6e74 2074 6f20 6765 7420 7265 616c 6c79  nt to get really
-00000a90: 2066 616e 6379 2028 6974 2072 6561 6c6c   fancy (it reall
-00000aa0: 7920 6d61 6b65 7320 6120 6c6f 7420 6d6f  y makes a lot mo
-00000ab0: 7265 2066 756e 2920 6372 6561 7465 2061  re fun) create a
-00000ac0: 6e20 616c 6961 7320 666f 7220 6070 6970  n alias for `pip
-00000ad0: 2069 6e73 7461 6c6c 600a 0a60 6060 6261   install`..```ba
-00000ae0: 7368 0a6e 616e 6f20 7e2f 2e62 6173 6872  sh.nano ~/.bashr
-00000af0: 630a 6060 600a 0a41 6e64 2061 7070 656e  c.```..And appen
-00000b00: 640a 0a60 6060 6261 7368 0a61 6c69 6173  d..```bash.alias
-00000b10: 2063 6173 743d 2770 6970 2069 6e73 7461   cast='pip insta
-00000b20: 6c6c 270a 6060 600a 0a41 6674 6572 2073  ll'.```..After s
-00000b30: 6176 696e 6720 7275 6e0a 0a60 6060 6261  aving run..```ba
-00000b40: 7368 0a73 6f75 7263 6520 7e2f 2e62 6173  sh.source ~/.bas
-00000b50: 6872 630a 6060 600a 0a54 6865 6e20 6669  hrc.```..Then fi
-00000b60: 6e61 6c6c 792c 0a0a 6060 6062 6173 680a  nally,..```bash.
-00000b70: 6361 7374 2073 7061 776e 2d6c 6961 0a60  cast spawn-lia.`
-00000b80: 6060 0a0a 2323 2035 2e20 5573 6167 650a  ``..## 5. Usage.
-00000b90: 0a54 6f20 696d 7072 6f76 6520 7468 6520  .To improve the 
-00000ba0: 7175 616c 6974 7920 6f66 2079 6f75 7220  quality of your 
-00000bb0: 7061 636b 6167 6520 616e 6420 646f 696e  package and doin
-00000bc0: 6720 6c6f 6361 6c20 4349 2064 6f3a 0a0a  g local CI do:..
-00000bd0: 6060 6062 6173 680a 6c69 6120 6865 616c  ```bash.lia heal
-00000be0: 2070 6163 6b61 6765 0a60 6060 0a0a 446f   package.```..Do
-00000bf0: 206e 6f74 2062 6520 6166 7261 6964 2079   not be afraid y
-00000c00: 6f75 2077 696c 6c20 7072 6f62 6162 6c79  ou will probably
-00000c10: 2073 6565 206d 616e 7920 6572 726f 7273   see many errors
-00000c20: 2e20 5468 6973 2062 6568 6176 696f 7220  . This behavior 
-00000c30: 6973 2069 6e74 656e 6465 6420 616e 6420  is intended and 
-00000c40: 7368 616c 6c20 7261 6973 6520 796f 7572  shall raise your
-00000c50: 2061 7474 656e 7469 6f6e 2074 6f20 616c   attention to al
-00000c60: 6c20 736f 7274 7320 6f66 2065 7272 6f72  l sorts of error
-00000c70: 732c 2062 7567 732c 2074 6563 686e 6963  s, bugs, technic
-00000c80: 616c 2064 6562 7420 616e 6420 616e 7469  al debt and anti
-00000c90: 7061 7474 6572 6e73 2069 6e20 796f 7572  patterns in your
-00000ca0: 2063 6f64 652e 0a0a 4765 7474 696e 6720   code...Getting 
-00000cb0: 7269 6420 6f66 2065 7665 7279 7468 696e  rid of everythin
-00000cc0: 6720 6d61 7920 6265 2074 6564 696f 7573  g may be tedious
-00000cd0: 2062 7574 2069 7420 6973 2064 6f61 626c   but it is doabl
-00000ce0: 652e 2057 6520 6172 6520 676f 696e 6720  e. We are going 
-00000cf0: 7468 726f 7567 6820 7468 6520 7361 6d65  through the same
-00000d00: 2070 726f 6365 7373 2e20 4974 2069 6d70   process. It imp
-00000d10: 726f 7665 6420 6576 6572 7974 6869 6e67  roved everything
-00000d20: 2066 6f72 2075 732e 0a0a 4966 2079 6f75   for us...If you
-00000d30: 206e 6565 6420 6d6f 7265 2069 6e66 6f72   need more infor
-00000d40: 6d61 7469 6f6e 2061 626f 7574 2074 7970  mation about typ
-00000d50: 696e 672c 2074 6865 6e20 7468 6520 606d  ing, then the `m
-00000d60: 7970 7960 205b 646f 6375 6d65 6e74 6174  ypy` [documentat
-00000d70: 696f 6e5d 2868 7474 7073 3a2f 2f6d 7970  ion](https://myp
-00000d80: 792e 7265 6164 7468 6564 6f63 732e 696f  y.readthedocs.io
-00000d90: 2f65 6e2f 7374 6162 6c65 2f67 6574 7469  /en/stable/getti
-00000da0: 6e67 5f73 7461 7274 6564 2e68 746d 6c29  ng_started.html)
-00000db0: 2069 7320 6120 6772 6561 7420 706c 6163   is a great plac
-00000dc0: 6520 746f 2073 7461 7274 2e0a 0a54 6f20  e to start...To 
-00000dd0: 6465 706c 6f79 2079 6f75 2070 6163 6b61  deploy you packa
-00000de0: 6765 2064 6f0a 0a60 6060 6261 7368 0a6c  ge do..```bash.l
-00000df0: 6961 2064 6570 6c6f 7920 7061 636b 6167  ia deploy packag
-00000e00: 6520 0a60 6060 0a0a 2320 5375 7070 6f72  e .```..# Suppor
-00000e10: 7420 7468 6520 4465 7665 6c6f 706d 656e  t the Developmen
-00000e20: 740a 0a54 6f20 7375 7070 6f72 7420 7468  t..To support th
-00000e30: 6520 6465 7665 6c6f 706d 656e 7420 796f  e development yo
-00000e40: 7520 6361 6e0a 0a3c 6120 6872 6566 3d22  u can..<a href="
-00000e50: 6874 7470 733a 2f2f 7777 772e 6275 796d  https://www.buym
-00000e60: 6561 636f 6666 6565 2e63 6f6d 2f63 6170  eacoffee.com/cap
-00000e70: 6a6d 6b22 2074 6172 6765 743d 225f 626c  jmk" target="_bl
-00000e80: 616e 6b22 3e3c 696d 6720 7372 633d 2268  ank"><img src="h
-00000e90: 7474 7073 3a2f 2f63 646e 2e62 7579 6d65  ttps://cdn.buyme
-00000ea0: 6163 6f66 6665 652e 636f 6d2f 6275 7474  acoffee.com/butt
-00000eb0: 6f6e 732f 6465 6661 756c 742d 6f72 616e  ons/default-oran
-00000ec0: 6765 2e70 6e67 2220 616c 743d 2242 7579  ge.png" alt="Buy
-00000ed0: 204d 6520 4120 436f 6666 6565 2220 6865   Me A Coffee" he
-00000ee0: 6967 6874 3d22 3431 2220 7769 6474 683d  ight="41" width=
-00000ef0: 2231 3734 223e 3c2f 613e 0a              "174"></a>.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 7370 6177  : 2.1.Name: spaw
+00000020: 6e2d 6c69 610a 5665 7273 696f 6e3a 2030  n-lia.Version: 0
+00000030: 2e32 2e37 0a53 756d 6d61 7279 3a20 5468  .2.7.Summary: Th
+00000040: 6520 6d6f 7374 2077 616e 7465 6420 7375  e most wanted su
+00000050: 7070 6f72 740a 486f 6d65 2d70 6167 653a  pport.Home-page:
+00000060: 2068 7474 7073 3a2f 2f63 6f64 6562 6572   https://codeber
+00000070: 672e 6f72 672f 6361 705f 6a6d 6b2f 6c69  g.org/cap_jmk/li
+00000080: 610a 4175 7468 6f72 3a20 4a75 6c69 616e  a.Author: Julian
+00000090: 204d 2e20 4b6c 6562 6572 0a41 7574 686f   M. Kleber.Autho
+000000a0: 722d 656d 6169 6c3a 206a 756c 6961 6e2e  r-email: julian.
+000000b0: 6b6c 6562 6572 4073 6169 6c2e 626c 6163  kleber@sail.blac
+000000c0: 6b0a 436c 6173 7369 6669 6572 3a20 5072  k.Classifier: Pr
+000000d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000000e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000000f0: 330a 436c 6173 7369 6669 6572 3a20 4c69  3.Classifier: Li
+00000100: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+00000110: 726f 7665 6420 3a3a 2047 4e55 2047 656e  roved :: GNU Gen
+00000120: 6572 616c 2050 7562 6c69 6320 4c69 6365  eral Public Lice
+00000130: 6e73 6520 7633 206f 7220 6c61 7465 7220  nse v3 or later 
+00000140: 2847 504c 7633 2b29 0a43 6c61 7373 6966  (GPLv3+).Classif
+00000150: 6965 723a 204f 7065 7261 7469 6e67 2053  ier: Operating S
+00000160: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000170: 7065 6e64 656e 740a 5265 7175 6972 6573  pendent.Requires
+00000180: 2d50 7974 686f 6e3a 203e 3d33 2e38 0a44  -Python: >=3.8.D
+00000190: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000001a0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000001b0: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+000001c0: 696c 653a 204c 4943 454e 5345 2e74 7874  ile: LICENSE.txt
+000001d0: 0a0a 2320 6c69 610a 0a5b 215b 446f 776e  ..# lia..[![Down
+000001e0: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
+000001f0: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
+00000200: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
+00000210: 6765 2f73 7061 776e 2d6c 6961 3f70 6572  ge/spawn-lia?per
+00000220: 696f 643d 746f 7461 6c26 756e 6974 733d  iod=total&units=
+00000230: 696e 7465 726e 6174 696f 6e61 6c5f 7379  international_sy
+00000240: 7374 656d 266c 6566 745f 636f 6c6f 723d  stem&left_color=
+00000250: 626c 6163 6b26 7269 6768 745f 636f 6c6f  black&right_colo
+00000260: 723d 6f72 616e 6765 266c 6566 745f 7465  r=orange&left_te
+00000270: 7874 3d44 6f77 6e6c 6f61 6473 295d 2868  xt=Downloads)](h
+00000280: 7474 7073 3a2f 2f70 6570 792e 7465 6368  ttps://pepy.tech
+00000290: 2f70 726f 6a65 6374 2f73 7061 776e 2d6c  /project/spawn-l
+000002a0: 6961 290a 5b21 5b4c 6963 656e 7365 3a20  ia).[![License: 
+000002b0: 4750 4c20 7633 5d28 6874 7470 733a 2f2f  GPL v3](https://
+000002c0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000002d0: 6164 6765 2f4c 6963 656e 7365 2d47 504c  adge/License-GPL
+000002e0: 5f76 332d 626c 7565 2e73 7667 295d 2868  _v3-blue.svg)](h
+000002f0: 7474 7073 3a2f 2f77 7777 2e67 6e75 2e6f  ttps://www.gnu.o
+00000300: 7267 2f6c 6963 656e 7365 732f 6770 6c2d  rg/licenses/gpl-
+00000310: 332e 3029 0a21 5b50 7974 686f 6e20 5665  3.0).![Python Ve
+00000320: 7273 696f 6e73 5d28 6874 7470 733a 2f2f  rsions](https://
+00000330: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000340: 6164 6765 2f70 7974 686f 6e2d 332e 3825  adge/python-3.8%
+00000350: 3230 2537 4325 3230 332e 3925 3230 2537  20%7C%203.9%20%7
+00000360: 4325 3230 332e 3130 2532 3025 3743 2532  C%203.10%20%7C%2
+00000370: 3033 2e31 3125 3230 2537 4325 3230 2d62  03.11%20%7C%20-b
+00000380: 6c75 6529 0a21 5b53 7479 6c65 2042 6c61  lue).![Style Bla
+00000390: 636b 5d28 6874 7470 733a 2f2f 7761 7265  ck](https://ware
+000003a0: 686f 7573 652d 6361 6d6f 2e69 6e67 7265  house-camo.ingre
+000003b0: 7373 2e63 6d68 312e 7073 6668 6f73 7465  ss.cmh1.psfhoste
+000003c0: 642e 6f72 672f 6662 6664 6337 3735 3431  d.org/fbfdc77541
+000003d0: 3833 6563 6630 3739 6263 3731 6464 6561  83ecf079bc71ddea
+000003e0: 6261 6638 3866 3663 6263 3563 3030 2f36  baf88f6cbc5c00/6
+000003f0: 3837 3437 3437 3037 3333 6132 6632 6636  8747470733a2f2f6
+00000400: 3936 6436 3732 6537 3336 3836 3936 3536  96d672e736869656
+00000410: 6336 3437 3332 6536 3936 6632 6636 3236  c64732e696f2f626
+00000420: 3136 3436 3736 3532 6636 3336 6636 3436  16467652f636f646
+00000430: 3532 3533 3233 3037 3337 3437 3936 6336  52532307374796c6
+00000440: 3532 6436 3236 6336 3136 3336 6232 6433  52d626c61636b2d3
+00000450: 3033 3033 3033 3033 3033 3032 6537 3337  030303030302e737
+00000460: 3636 3729 0a5b 215b 5079 5049 202d 2056  667).[![PyPI - V
+00000470: 6572 7369 6f6e 5d28 6874 7470 733a 2f2f  ersion](https://
+00000480: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000490: 7970 692f 762f 7370 6177 6e2d 6c69 612e  ypi/v/spawn-lia.
+000004a0: 7376 6729 5d28 6874 7470 733a 2f2f 7079  svg)](https://py
+000004b0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f73  pi.org/project/s
+000004c0: 7061 776e 2d6c 6961 290a 0a21 5b4c 6961  pawn-lia)..![Lia
+000004d0: 5d28 6c69 612e 6a70 6729 0a0a 2d2d 2d2d  ](lia.jpg)..----
+000004e0: 2d0a 0a2a 2a54 6162 6c65 206f 6620 436f  -..**Table of Co
+000004f0: 6e74 656e 7473 2a2a 0a0a 3c21 2d2d 2054  ntents**..<!-- T
+00000500: 4f43 202d 2d3e 0a2d 205b 312e 2057 6879  OC -->.- [1. Why
+00000510: 3f5d 2823 312d 7768 7929 0a2d 205b 322e  ?](#1-why).- [2.
+00000520: 2057 6861 743f 5d28 2332 2d77 6861 7429   What?](#2-what)
+00000530: 0a2d 205b 332e 204c 6961 5d28 2333 2d6c  .- [3. Lia](#3-l
+00000540: 6961 290a 2d20 5b34 2e20 496e 7374 616c  ia).- [4. Instal
+00000550: 6c61 7469 6f6e 5d28 2334 2d69 6e73 7461  lation](#4-insta
+00000560: 6c6c 6174 696f 6e29 0a2d 205b 352e 2055  llation).- [5. U
+00000570: 7361 6765 5d28 2335 2d75 7361 6765 290a  sage](#5-usage).
+00000580: 2d20 5b36 2e20 2320 4465 706c 6f79 6d65  - [6. # Deployme
+00000590: 6e74 735d 2823 362d 2d64 6570 6c6f 796d  nts](#6--deploym
+000005a0: 656e 7473 290a 2020 2020 2d20 5b36 2e31  ents).    - [6.1
+000005b0: 2e20 4769 7420 6f70 6572 6174 696f 6e73  . Git operations
+000005c0: 5d28 2336 312d 6769 742d 6f70 6572 6174  ](#61-git-operat
+000005d0: 696f 6e73 290a 3c21 2d2d 202f 544f 4320  ions).<!-- /TOC 
+000005e0: 2d2d 3e0a 0a23 2320 312e 2057 6879 3f0a  -->..## 1. Why?.
+000005f0: 0a52 656d 656d 6265 7220 636f 6465 2069  .Remember code i
+00000600: 7320 706f 6574 7279 2e20 416e 6420 7765  s poetry. And we
+00000610: 2077 7269 7465 206f 7572 206f 776e 2073   write our own s
+00000620: 746f 7279 2e20 416e 6420 666f 7220 7468  tory. And for th
+00000630: 6973 2c20 7765 206e 6565 6420 6120 7375  is, we need a su
+00000640: 7070 6f72 742e 0a0a 5769 7468 6f75 7420  pport...Without 
+00000650: 6120 7375 7070 6f72 742c 2061 6c6c 2079  a support, all y
+00000660: 6f75 7220 6566 666f 7274 7320 7769 6c6c  our efforts will
+00000670: 2066 6169 6c2e 2041 2073 7570 706f 7274   fail. A support
+00000680: 2074 616b 6573 2063 6172 6520 7765 2064   takes care we d
+00000690: 6f20 616c 6c20 7468 6520 6e65 6365 7373  o all the necess
+000006a0: 6172 7920 7468 696e 6773 2077 6520 776f  ary things we wo
+000006b0: 756c 6420 6e6f 7420 6669 6e64 2074 696d  uld not find tim
+000006c0: 6520 6475 7269 6e67 2062 6174 746c 6573  e during battles
+000006d0: 2e20 5765 206e 6565 6420 6120 7375 7070  . We need a supp
+000006e0: 6f72 742e 2053 6f20 7765 2061 736b 6564  ort. So we asked
+000006f0: 2060 6c69 6160 2074 6f20 6a6f 696e 2075   `lia` to join u
+00000700: 732e 0a0a 5368 6520 7072 6f74 6563 7473  s...She protects
+00000710: 2075 7320 6672 6f6d 206d 616c 6963 696f   us from malicio
+00000720: 7573 2061 6476 6572 7361 7269 6573 2c20  us adversaries, 
+00000730: 616e 6420 6865 616c 7320 6f75 7220 6f72  and heals our or
+00000740: 6761 6e69 7a61 7469 6f6e 2062 7920 6d61  ganization by ma
+00000750: 6b69 6e67 206f 7572 2070 6f65 7472 7920  king our poetry 
+00000760: 6265 7474 6572 2061 6e64 2074 6865 7265  better and there
+00000770: 6279 206f 7572 2073 746f 7279 2e0a 0a23  by our story...#
+00000780: 2320 322e 2057 6861 743f 0a0a 606c 6961  # 2. What?..`lia
+00000790: 6020 6973 2074 6865 2062 6573 7420 7375  ` is the best su
+000007a0: 7070 6f72 7420 796f 7520 6361 6e20 686f  pport you can ho
+000007b0: 7065 2066 6f72 2e20 5368 6520 6865 6c70  pe for. She help
+000007c0: 7320 7573 2074 6f20 6d61 696e 7461 696e  s us to maintain
+000007d0: 206f 7572 2073 6869 702c 2066 6967 6874   our ship, fight
+000007e0: 2065 6e65 6d69 6573 2c20 616e 6420 7769   enemies, and wi
+000007f0: 6e20 6375 7374 6f6d 6572 732e 0a0a 2323  n customers...##
+00000800: 2033 2e20 4c69 610a 0a57 6879 2064 6964   3. Lia..Why did
+00000810: 2077 6520 6e61 6d65 2074 6865 2070 6163   we name the pac
+00000820: 6b61 6765 2060 6c69 6160 3f0a 0a41 7320  kage `lia`?..As 
+00000830: 6120 7368 6f72 7420 666f 726d 206f 6620  a short form of 
+00000840: 456c 6973 6162 6574 682c 204c 6961 206d  Elisabeth, Lia m
+00000850: 6561 6e73 2022 476f 6420 6973 2066 756c  eans "God is ful
+00000860: 6c6e 6573 7322 2c20 2247 6f64 2069 7320  lness", "God is 
+00000870: 6d79 206f 6174 6822 206f 7220 2247 6f64  my oath" or "God
+00000880: 2073 7765 6172 7322 2e20 4672 6f6d 2041   swears". From A
+00000890: 6d69 6c69 6120 4c69 6120 6765 7473 2074  milia Lia gets t
+000008a0: 6865 206d 6561 6e69 6e67 7320 2274 6865  he meanings "the
+000008b0: 207a 6561 6c6f 7573 222c 2022 7468 6520   zealous", "the 
+000008c0: 696d 6974 6174 6f72 2220 6f72 2022 7468  imitator" or "th
+000008d0: 6520 636f 6d70 6574 6974 6f72 2220 616e  e competitor" an
+000008e0: 6420 6672 6f6d 204a 756c 6961 2022 6672  d from Julia "fr
+000008f0: 6f6d 2074 6865 2066 616d 696c 7920 6f66  om the family of
+00000900: 2074 6865 204a 756c 6969 2220 6f72 2022   the Julii" or "
+00000910: 636f 6e73 6563 7261 7465 6420 746f 204a  consecrated to J
+00000920: 7570 6974 6572 222e 204c 6961 2069 7320  upiter". Lia is 
+00000930: 616c 736f 2074 6865 2049 7269 7368 2077  also the Irish w
+00000940: 6f72 6420 666f 7220 2268 6561 6c65 7222  ord for "healer"
+00000950: 2e0a 0a41 6c6c 206f 7468 6572 206d 6561  ...All other mea
+00000960: 6e69 6e67 7320 646f 206e 6f74 206d 6174  nings do not mat
+00000970: 7465 7220 696e 2074 6869 7320 636f 6e74  ter in this cont
+00000980: 6578 7420 7768 6174 736f 6576 6572 2e0a  ext whatsoever..
+00000990: 0a49 6e20 6661 6374 2c20 7468 6520 6e61  .In fact, the na
+000009a0: 6d65 2069 7320 736f 2073 696d 696c 6172  me is so similar
+000009b0: 2074 6f20 606c 7561 6020 6120 636f 6d6d   to `lua` a comm
+000009c0: 6f6e 206c 616e 6775 6167 6520 666f 7220  on language for 
+000009d0: 6372 6561 7469 6e67 2063 7962 6572 2077  creating cyber w
+000009e0: 6561 706f 6e73 2074 6861 7420 616c 7465  eapons that alte
+000009f0: 7269 6e67 2074 6865 206e 616d 6520 696e  ring the name in
+00000a00: 746f 2073 6f6d 6574 6869 6e67 206d 6f72  to something mor
+00000a10: 6520 6265 6175 7469 6675 6c20 7061 7973  e beautiful pays
+00000a20: 2061 7474 656e 7469 6f6e 2074 6f20 7468   attention to th
+00000a30: 6520 6661 6374 2074 6861 7420 606c 6961  e fact that `lia
+00000a40: 6020 6973 2064 6f69 6e67 206d 6f72 6520  ` is doing more 
+00000a50: 6f72 206c 6573 7320 7468 6520 6578 6163  or less the exac
+00000a60: 7420 6f70 706f 7369 7465 206f 6620 606c  t opposite of `l
+00000a70: 7561 602e 0a0a 416c 736f 2063 6865 636b  ua`...Also check
+00000a80: 2074 6865 206d 6f76 6965 205b 5761 7263   the movie [Warc
+00000a90: 7261 6674 5d28 6874 7470 733a 2f2f 7777  raft](https://ww
+00000aa0: 772e 696d 6462 2e63 6f6d 2f74 6974 6c65  w.imdb.com/title
+00000ab0: 2f74 7430 3830 3330 3936 2f29 2066 6f72  /tt0803096/) for
+00000ac0: 2062 6163 6b67 726f 756e 6420 696e 666f   background info
+00000ad0: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
+00000ae0: 6520 7374 6f72 792e 2049 7420 6973 2067  e story. It is g
+00000af0: 6f69 6e67 206f 6e20 666f 7220 736f 6d65  oing on for some
+00000b00: 2074 696d 6520 6e6f 772e 2042 7574 2077   time now. But w
+00000b10: 6520 6465 6369 6465 6420 746f 206e 6f74  e decided to not
+00000b20: 206a 7573 7420 7369 7420 7374 696c 6c20   just sit still 
+00000b30: 7369 6e63 6520 7468 6520 776f 726c 6420  since the world 
+00000b40: 6265 6361 6d65 2066 756c 6c20 6f66 2077  became full of w
+00000b50: 6172 2072 6563 656e 746c 792e 2054 6861  ar recently. Tha
+00000b60: 7473 2077 6879 2077 6520 7769 6c6c 2067  ts why we will g
+00000b70: 726f 7720 696e 746f 206f 7572 2070 7265  row into our pre
+00000b80: 6465 7374 696e 6564 2072 6f6c 6573 2e20  destined roles. 
+00000b90: 4974 7320 6465 7374 696e 792e 0a0a 596f  Its destiny...Yo
+00000ba0: 7520 6361 6e27 7420 6176 6f69 6420 6465  u can't avoid de
+00000bb0: 7374 696e 792e 2049 7420 6973 2065 7665  stiny. It is eve
+00000bc0: 6e20 7761 7374 6520 6f66 2074 696d 6520  n waste of time 
+00000bd0: 7472 7969 6e67 2074 6f2e 2053 7572 7265  trying to. Surre
+00000be0: 6e64 6572 696e 6720 6973 2061 2070 726f  ndering is a pro
+00000bf0: 7665 6e20 6d65 7468 6f64 2066 6f72 206d  ven method for m
+00000c00: 616e 6966 6573 7461 7469 6f6e 2e20 596f  anifestation. Yo
+00000c10: 7520 7072 6f62 6162 6c79 206b 6e6f 7720  u probably know 
+00000c20: 7468 6174 2061 6e79 7761 7973 2e0a 0a49  that anyways...I
+00000c30: 6620 796f 7520 7265 6164 2074 6872 6f75  f you read throu
+00000c40: 6768 2062 6f6f 6b73 2061 626f 7574 2041  gh books about A
+00000c50: 6769 6c65 2044 6576 656c 6f70 6d65 6e74  gile Development
+00000c60: 2c20 5265 6661 6374 6f72 696e 6720 616e  , Refactoring an
+00000c70: 6420 436c 6561 6e20 436f 6469 6e67 2079  d Clean Coding y
+00000c80: 6f75 206d 6179 6265 2072 6561 6c69 7a65  ou maybe realize
+00000c90: 2074 6861 7420 7365 6375 7269 7479 2c20   that security, 
+00000ca0: 7661 6c75 6520 6765 6e65 7261 7469 6f6e  value generation
+00000cb0: 2c20 616e 6420 6177 6573 6f6d 6520 7072  , and awesome pr
+00000cc0: 6f64 7563 7473 2064 6f20 6861 7665 2061  oducts do have a
+00000cd0: 206c 6f74 2074 6f20 646f 2077 6974 6820   lot to do with 
+00000ce0: 7468 6573 6520 626f 6f6b 732e 2060 5468  these books. `Th
+00000cf0: 7573 2c20 7472 7565 2064 6576 656c 6f70  us, true develop
+00000d00: 6572 7320 6861 7665 206f 6e65 2063 6f6d  ers have one com
+00000d10: 6d6f 6e20 656e 656d 793a 2054 6865 2046  mon enemy: The F
+00000d20: 656c 2e60 200a 0a57 6520 686f 7065 2074  el.` ..We hope t
+00000d30: 6865 2074 6f6f 6c20 6272 696e 6773 2079  he tool brings y
+00000d40: 6f75 206a 6f79 2069 6e20 7769 6e6e 696e  ou joy in winnin
+00000d50: 6720 796f 7572 2064 6169 6c79 2062 6174  g your daily bat
+00000d60: 746c 6573 2061 6761 696e 7374 2074 6865  tles against the
+00000d70: 2046 656c 2e20 0a0a 5765 2062 7569 6c74   Fel. ..We built
+00000d80: 2066 6f72 2061 2062 6574 7465 7220 6675   for a better fu
+00000d90: 7475 7265 2e20 416e 6420 7765 2061 7265  ture. And we are
+00000da0: 2065 7863 6974 6564 2077 6861 7420 7468   excited what th
+00000db0: 6520 6675 7475 7265 2068 6173 2070 7265  e future has pre
+00000dc0: 7061 7265 6420 666f 7220 7573 2e20 e29b  pared for us. ..
+00000dd0: b50a 0a23 2320 342e 2049 6e73 7461 6c6c  ...## 4. Install
+00000de0: 6174 696f 6e0a 0a60 6060 6261 7368 0a70  ation..```bash.p
+00000df0: 6970 2069 6e73 7461 6c6c 2073 7061 776e  ip install spawn
+00000e00: 2d6c 6961 0a60 6060 0a0a 4966 2079 6f75  -lia.```..If you
+00000e10: 2077 616e 7420 746f 2067 6574 2072 6561   want to get rea
+00000e20: 6c6c 7920 6661 6e63 7920 2869 7420 7265  lly fancy (it re
+00000e30: 616c 6c79 206d 616b 6573 2061 206c 6f74  ally makes a lot
+00000e40: 206d 6f72 6520 6675 6e29 2063 7265 6174   more fun) creat
+00000e50: 6520 616e 2061 6c69 6173 2066 6f72 2060  e an alias for `
+00000e60: 7069 7020 696e 7374 616c 6c60 0a0a 6060  pip install`..``
+00000e70: 6062 6173 680a 6e61 6e6f 207e 2f2e 6261  `bash.nano ~/.ba
+00000e80: 7368 7263 0a60 6060 0a0a 416e 6420 6170  shrc.```..And ap
+00000e90: 7065 6e64 0a0a 6060 6062 6173 680a 616c  pend..```bash.al
+00000ea0: 6961 7320 6361 7374 3d27 7069 7020 696e  ias cast='pip in
+00000eb0: 7374 616c 6c27 0a60 6060 0a0a 4166 7465  stall'.```..Afte
+00000ec0: 7220 7361 7669 6e67 2072 756e 0a0a 6060  r saving run..``
+00000ed0: 6062 6173 680a 736f 7572 6365 207e 2f2e  `bash.source ~/.
+00000ee0: 6261 7368 7263 0a60 6060 0a0a 5468 656e  bashrc.```..Then
+00000ef0: 2066 696e 616c 6c79 2c0a 0a60 6060 6261   finally,..```ba
+00000f00: 7368 0a63 6173 7420 7370 6177 6e2d 6c69  sh.cast spawn-li
+00000f10: 610a 6060 600a 0a23 2320 352e 2055 7361  a.```..## 5. Usa
+00000f20: 6765 0a0a 546f 2067 6574 2067 656e 6572  ge..To get gener
+00000f30: 616c 2069 6e66 6f72 6d61 7469 6f6e 2061  al information a
+00000f40: 626f 7574 2074 6865 2073 7065 6c6c 7320  bout the spells 
+00000f50: 606c 6961 6020 6861 7320 746f 206f 6666  `lia` has to off
+00000f60: 6572 2072 756e 2074 6865 2070 6c61 696e  er run the plain
+00000f70: 2063 6f6d 6d61 6e64 0a0a 6060 6062 6173   command..```bas
+00000f80: 680a 6c69 610a 6060 600a 0a23 2323 2043  h.lia.```..### C
+00000f90: 4920 0a0a 546f 2069 6d70 726f 7665 2074  I ..To improve t
+00000fa0: 6865 2071 7561 6c69 7479 206f 6620 796f  he quality of yo
+00000fb0: 7572 2070 6163 6b61 6765 2061 6e64 2064  ur package and d
+00000fc0: 6f69 6e67 206c 6f63 616c 2043 4920 646f  oing local CI do
+00000fd0: 3a0a 0a60 6060 6261 7368 0a6c 6961 2068  :..```bash.lia h
+00000fe0: 6561 6c20 7061 636b 6167 650a 6060 600a  eal package.```.
+00000ff0: 0a44 6f20 6e6f 7420 6265 2061 6672 6169  .Do not be afrai
+00001000: 6420 796f 7520 7769 6c6c 2070 726f 6261  d you will proba
+00001010: 626c 7920 7365 6520 6d61 6e79 2065 7272  bly see many err
+00001020: 6f72 732e 2054 6869 7320 6265 6861 7669  ors. This behavi
+00001030: 6f72 2069 7320 696e 7465 6e64 6564 2061  or is intended a
+00001040: 6e64 2073 6861 6c6c 2072 6169 7365 2079  nd shall raise y
+00001050: 6f75 7220 6174 7465 6e74 696f 6e20 746f  our attention to
+00001060: 2061 6c6c 2073 6f72 7473 206f 6620 6572   all sorts of er
+00001070: 726f 7273 2c20 6275 6773 2c20 7465 6368  rors, bugs, tech
+00001080: 6e69 6361 6c20 6465 6274 2061 6e64 2061  nical debt and a
+00001090: 6e74 6970 6174 7465 726e 7320 696e 2079  ntipatterns in y
+000010a0: 6f75 7220 636f 6465 2e0a 0a47 6574 7469  our code...Getti
+000010b0: 6e67 2072 6964 206f 6620 6576 6572 7974  ng rid of everyt
+000010c0: 6869 6e67 206d 6179 2062 6520 7465 6469  hing may be tedi
+000010d0: 6f75 7320 6275 7420 6974 2069 7320 646f  ous but it is do
+000010e0: 6162 6c65 2e20 5765 2061 7265 2067 6f69  able. We are goi
+000010f0: 6e67 2074 6872 6f75 6768 2074 6865 2073  ng through the s
+00001100: 616d 6520 7072 6f63 6573 732e 2049 7420  ame process. It 
+00001110: 696d 7072 6f76 6564 2065 7665 7279 7468  improved everyth
+00001120: 696e 6720 666f 7220 7573 2e0a 0a49 6620  ing for us...If 
+00001130: 796f 7520 6e65 6564 206d 6f72 6520 696e  you need more in
+00001140: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+00001150: 7479 7069 6e67 2c20 7468 656e 2074 6865  typing, then the
+00001160: 2060 6d79 7079 6020 5b64 6f63 756d 656e   `mypy` [documen
+00001170: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00001180: 6d79 7079 2e72 6561 6474 6865 646f 6373  mypy.readthedocs
+00001190: 2e69 6f2f 656e 2f73 7461 626c 652f 6765  .io/en/stable/ge
+000011a0: 7474 696e 675f 7374 6172 7465 642e 6874  tting_started.ht
+000011b0: 6d6c 2920 6973 2061 2067 7265 6174 2070  ml) is a great p
+000011c0: 6c61 6365 2074 6f20 7374 6172 742e 0a0a  lace to start...
+000011d0: 2323 2320 4349 2069 6e20 636f 6e74 6169  ### CI in contai
+000011e0: 6e65 720a 0a46 6f72 2061 6c6c 2072 656d  ner..For all rem
+000011f0: 6f74 6520 4349 2073 7973 7465 6d73 206c  ote CI systems l
+00001200: 696b 6520 4472 6f6e 6520 4349 2c20 576f  ike Drone CI, Wo
+00001210: 6f64 7065 636b 6572 2c20 4163 7469 6f6e  odpecker, Action
+00001220: 732c 2065 7463 2e20 0a0a 6060 6062 6173  s, etc. ..```bas
+00001230: 680a 6c69 6120 6865 616c 2070 6163 6b61  h.lia heal packa
+00001240: 6765 0a60 6060 0a0a 2323 2320 352e 312e  ge.```..### 5.1.
+00001250: 2044 6570 6c6f 796d 656e 7473 0a0a 546f   Deployments..To
+00001260: 2064 6570 6c6f 7920 796f 7520 7061 636b   deploy you pack
+00001270: 6167 6520 646f 0a0a 0a60 6060 6261 7368  age do...```bash
+00001280: 0a6c 6961 2064 6570 6c6f 7920 7061 636b  .lia deploy pack
+00001290: 6167 6520 0a60 6060 0a0a 2323 2320 352e  age .```..### 5.
+000012a0: 322e 2047 6974 206f 7065 7261 7469 6f6e  2. Git operation
+000012b0: 7320 0a0a 6060 6062 6173 680a 6c69 6120  s ..```bash.lia 
+000012c0: 7075 7368 206f 7269 6769 6e5f 6e61 6d65  push origin_name
+000012d0: 0a60 6060 0a77 6865 7265 206f 7269 6769  .```.where origi
+000012e0: 6e20 6e61 6d65 2069 7320 7468 6520 6e61  n name is the na
+000012f0: 6d65 206f 6620 796f 7572 2072 656d 6f74  me of your remot
+00001300: 652c 2065 2e67 2e20 606f 7269 6769 6e60  e, e.g. `origin`
+00001310: 0a0a 2320 5375 7070 6f72 7420 7468 6520  ..# Support the 
+00001320: 4465 7665 6c6f 706d 656e 740a 0a54 6f20  Development..To 
+00001330: 7375 7070 6f72 7420 7468 6520 6465 7665  support the deve
+00001340: 6c6f 706d 656e 7420 796f 7520 6361 6e0a  lopment you can.
+00001350: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00001360: 2f2f 7777 772e 6275 796d 6561 636f 6666  //www.buymeacoff
+00001370: 6565 2e63 6f6d 2f63 6170 6a6d 6b22 2074  ee.com/capjmk" t
+00001380: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00001390: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+000013a0: 2f63 646e 2e62 7579 6d65 6163 6f66 6665  /cdn.buymeacoffe
+000013b0: 652e 636f 6d2f 6275 7474 6f6e 732f 6465  e.com/buttons/de
+000013c0: 6661 756c 742d 6f72 616e 6765 2e70 6e67  fault-orange.png
+000013d0: 2220 616c 743d 2242 7579 204d 6520 4120  " alt="Buy Me A 
+000013e0: 436f 6666 6565 2220 6865 6967 6874 3d22  Coffee" height="
+000013f0: 3431 2220 7769 6474 683d 2231 3734 223e  41" width="174">
+00001400: 3c2f 613e 0a                             </a>.
```

### Comparing `spawn-lia-0.2.6/lia/bounty/heal.py` & `spawn-lia-0.2.7/lia/bounty/heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/bounty/testing.py` & `spawn-lia-0.2.7/lia/bounty/testing.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/conversation/ask_to_proceed.py` & `spawn-lia-0.2.7/lia/conversation/ask_to_proceed.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/conversation/emojis.py` & `spawn-lia-0.2.7/lia/conversation/emojis.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/conversation/start_message.py` & `spawn-lia-0.2.7/lia/conversation/start_message.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/conversation/virtualenv.py` & `spawn-lia-0.2.7/lia/conversation/virtualenv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/git_operations/push.py` & `spawn-lia-0.2.7/lia/git_operations/push.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,41 @@
     :param remote:str: Used to specify the remote repository we want to push to.
     :return: None.
 
     :doc-author: Julian M. Kleber
     """
 
     subprocess.run(["git add ."], check=True, shell=True)
+    subprocess.run([f"git push {remote}"], check=True, shell=True)
+
+
+def do_commit() -> None:
+    """
+    The do_commit function is used to commit the changes made in the current working directory.
+    The function takes no arguments and returns None.
+
+    :return: None.
+
+    :doc-author: Julian M. Kleber
+    """
+
+    commit_message = get_commit_message()
+
+    subprocess.run(
+        [f'git commit -m{"commit_message"}'], check=True, shell=True)
+
+
+def get_commit_message() -> str:
+    """
+    The get_commit_message function prompts the user for a commit message and returns it as a
+    string.
+
+    :return: The commit message.
+
+    :doc-author: Julian M. Kleber
+    """
 
     input_prompt = (
-        f"Let's document in the commit message what we have done {face_with_hearts}"
+        f"Let's document in the commit message what we have done {face_with_hearts}: "
     )
     commit_message = get_input(input_prompt)
-
-    subprocess.run([f'git commit -m{"input_prompt"}'], check=True, shell=True)
-    subprocess.run([f"git push {remote}"], check=True, shell=True)
+    return commit_message.decode("utf-8")
```

### Comparing `spawn-lia-0.2.6/lia/git_operations/verify_branch.py` & `spawn-lia-0.2.7/lia/git_operations/verify_branch.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/main.py` & `spawn-lia-0.2.7/lia/main.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/simplify/create_venv.py` & `spawn-lia-0.2.7/lia/simplify/create_venv.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/lia/support/deploy.py` & `spawn-lia-0.2.7/lia/support/deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/setup.py` & `spawn-lia-0.2.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="spawn-lia",
-    version="0.2.6",
+    version="0.2.7",
     packages=find_packages(include=["lia*"]),
     include_package_data=True,
     install_requires=[
         "Click",
         "black",
         "autopep8",
         "mypy",
```

### Comparing `spawn-lia-0.2.6/spawn_lia.egg-info/PKG-INFO` & `spawn-lia-0.2.7/spawn_lia.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spawn-lia
-Version: 0.2.6
+Version: 0.2.7
 Summary: The most wanted support
 Home-page: https://codeberg.org/cap_jmk/lia
 Author: Julian M. Kleber
 Author-email: julian.kleber@sail.black
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,16 @@
 
 <!-- TOC -->
 - [1. Why?](#1-why)
 - [2. What?](#2-what)
 - [3. Lia](#3-lia)
 - [4. Installation](#4-installation)
 - [5. Usage](#5-usage)
+- [6. # Deployments](#6--deployments)
+    - [6.1. Git operations](#61-git-operations)
 <!-- /TOC -->
 
 ## 1. Why?
 
 Remember code is poetry. And we write our own story. And for this, we need a support.
 
 Without a support, all your efforts will fail. A support takes care we do all the necessary things we would not find time during battles. We need a support. So we asked `lia` to join us.
@@ -56,15 +58,19 @@
 
 In fact, the name is so similar to `lua` a common language for creating cyber weapons that altering the name into something more beautiful pays attention to the fact that `lia` is doing more or less the exact opposite of `lua`.
 
 Also check the movie [Warcraft](https://www.imdb.com/title/tt0803096/) for background information about the story. It is going on for some time now. But we decided to not just sit still since the world became full of war recently. Thats why we will grow into our predestined roles. Its destiny.
 
 You can't avoid destiny. It is even waste of time trying to. Surrendering is a proven method for manifestation. You probably know that anyways.
 
-We are excited what the future has prepared for us. ⛵
+If you read through books about Agile Development, Refactoring and Clean Coding you maybe realize that security, value generation, and awesome products do have a lot to do with these books. `Thus, true developers have one common enemy: The Fel.` 
+
+We hope the tool brings you joy in winning your daily battles against the Fel. 
+
+We built for a better future. And we are excited what the future has prepared for us. ⛵
 
 ## 4. Installation
 
 ```bash
 pip install spawn-lia
 ```
 
@@ -90,30 +96,56 @@
 
 ```bash
 cast spawn-lia
 ```
 
 ## 5. Usage
 
+To get general information about the spells `lia` has to offer run the plain command
+
+```bash
+lia
+```
+
+### CI 
+
 To improve the quality of your package and doing local CI do:
 
 ```bash
 lia heal package
 ```
 
 Do not be afraid you will probably see many errors. This behavior is intended and shall raise your attention to all sorts of errors, bugs, technical debt and antipatterns in your code.
 
 Getting rid of everything may be tedious but it is doable. We are going through the same process. It improved everything for us.
 
 If you need more information about typing, then the `mypy` [documentation](https://mypy.readthedocs.io/en/stable/getting_started.html) is a great place to start.
 
+### CI in container
+
+For all remote CI systems like Drone CI, Woodpecker, Actions, etc. 
+
+```bash
+lia heal package
+```
+
+### 5.1. Deployments
+
 To deploy you package do
 
+
 ```bash
 lia deploy package 
 ```
 
+### 5.2. Git operations 
+
+```bash
+lia push origin_name
+```
+where origin name is the name of your remote, e.g. `origin`
+
 # Support the Development
 
 To support the development you can
 
 <a href="https://www.buymeacoffee.com/capjmk" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>
```

### Comparing `spawn-lia-0.2.6/spawn_lia.egg-info/SOURCES.txt` & `spawn-lia-0.2.7/spawn_lia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/tests/test_deploy.py` & `spawn-lia-0.2.7/tests/test_deploy.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/tests/test_git_operations.py` & `spawn-lia-0.2.7/tests/test_git_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         ["lia", "push"], stdin=PIPE, stdout=PIPE
     )
 
     out.stdin.write(b"push done by test\n")
     outputlog, errorlog = out.communicate()
 
     out.stdin.close()
-    assert 1 == 2, outputlog +" - " + errorlog
+    assert 1 == 2, str(outputlog) +" - " + str(errorlog)
     subprocess.run["git checkout dev"]
     out = subprocess.Popen(
         ["python", "./lia/git_operations/verify_branch.py"], stdin=PIPE, stdout=PIPE
     )
     
     outputlog, errorlog = out.communicate()
     out.stdin.close()
```

### Comparing `spawn-lia-0.2.6/tests/test_heal.py` & `spawn-lia-0.2.7/tests/test_heal.py`

 * *Files identical despite different names*

### Comparing `spawn-lia-0.2.6/tests/test_venv.py` & `spawn-lia-0.2.7/tests/test_venv.py`

 * *Files identical despite different names*

