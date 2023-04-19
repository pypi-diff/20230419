# Comparing `tmp/sovrin-1.2.0.dev1681906498.tar.gz` & `tmp/sovrin-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sovrin-1.2.0.dev1681906498.tar", last modified: Wed Apr 19 12:15:12 2023, max compression
+gzip compressed data, was "sovrin-1.2.0rc1.tar", last modified: Tue Jan 24 22:49:44 2023, max compression
```

## Comparing `sovrin-1.2.0.dev1681906498.tar` & `sovrin-1.2.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:15:12.657276 sovrin-1.2.0.dev1681906498/
--rw-r--r--   0 runner    (1001) docker     (122)    10763 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-04-19 12:15:12.657276 sovrin-1.2.0.dev1681906498/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 12:15:12.657276 sovrin-1.2.0.dev1681906498/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1296 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:15:12.657276 sovrin-1.2.0.dev1681906498/sovrin/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/__metadata__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2527 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_builder_genesis
--rw-r--r--   0 runner    (1001) docker     (122)     3637 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_live_genesis
--rw-r--r--   0 runner    (1001) docker     (122)     4819 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_local_genesis
--rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_sandbox_genesis
--rw-r--r--   0 runner    (1001) docker     (122)       98 2023-04-19 12:15:12.000000 sovrin-1.2.0.dev1681906498/sovrin/metadata.json
--rw-r--r--   0 runner    (1001) docker     (122)    75203 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_builder_genesis
--rw-r--r--   0 runner    (1001) docker     (122)    70777 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_live_genesis
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_local_genesis
--rw-r--r--   0 runner    (1001) docker     (122)   122850 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_sandbox_genesis
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-04-19 12:15:10.000000 sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_training_genesis
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 12:15:12.657276 sovrin-1.2.0.dev1681906498/sovrin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-04-19 12:15:12.000000 sovrin-1.2.0.dev1681906498/sovrin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-19 12:15:12.000000 sovrin-1.2.0.dev1681906498/sovrin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 12:15:12.000000 sovrin-1.2.0.dev1681906498/sovrin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-19 12:15:12.000000 sovrin-1.2.0.dev1681906498/sovrin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-19 12:15:12.000000 sovrin-1.2.0.dev1681906498/sovrin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 22:49:44.543370 sovrin-1.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (122)    10763 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-01-24 22:49:44.543370 sovrin-1.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5707 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-24 22:49:44.543370 sovrin-1.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1266 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 22:49:44.543370 sovrin-1.2.0rc1/sovrin/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/__metadata__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2527 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/domain_transactions_builder_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)     3637 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/domain_transactions_live_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)     4819 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/domain_transactions_local_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)     3353 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/domain_transactions_sandbox_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (122)    75203 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/pool_transactions_builder_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)    70777 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/pool_transactions_live_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/pool_transactions_local_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)   122850 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/pool_transactions_sandbox_genesis
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-01-24 22:49:42.000000 sovrin-1.2.0rc1/sovrin/pool_transactions_training_genesis
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-24 22:49:44.543370 sovrin-1.2.0rc1/sovrin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-01-24 22:49:44.000000 sovrin-1.2.0rc1/sovrin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-01-24 22:49:44.000000 sovrin-1.2.0rc1/sovrin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-24 22:49:44.000000 sovrin-1.2.0rc1/sovrin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-01-24 22:49:44.000000 sovrin-1.2.0rc1/sovrin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-24 22:49:44.000000 sovrin-1.2.0rc1/sovrin.egg-info/top_level.txt
```

### Comparing `sovrin-1.2.0.dev1681906498/LICENSE` & `sovrin-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/README.md` & `sovrin-1.2.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 If you want to contribute to Sovrin, it's likely that you'll want to do so via [indy-node](https://github.com/hyperledger/indy-node). You can view additional bugs, stories, and backlog for Indy in [Hyperledger's Jira](https://jira.hyperledger.org/projects/INDY). Use project name `INDY` (or `IS` for the Indy SDK).
 
 ## Connecting to an Existing Network
 
 In order to connect to an existing network your agent needs to utilize the appropriate `pool_transactions_genesis` file.  These files define the information required to connect to the foundational nodes for the given network.
 
 - [MainNet](https://raw.githubusercontent.com/sovrin-foundation/sovrin/stable/sovrin/pool_transactions_live_genesis)
-- [TestNet](https://raw.githubusercontent.com/sovrin-foundation/sovrin/stable/sovrin/pool_transactions_sandbox_genesis)
+- [StagingNet](https://raw.githubusercontent.com/sovrin-foundation/sovrin/stable/sovrin/pool_transactions_sandbox_genesis)
 - [BuilderNet](https://raw.githubusercontent.com/sovrin-foundation/sovrin/stable/sovrin/pool_transactions_builder_genesis)
 
 ## How to Add Documentation
 For new features and pull requests, maintainers should make sure that the **contributor has added an explanation for their changes in the docs folder before merging the PR.**
   
 Contributors should write an addition to a current file or add a new file to the docs/source/ folder that explains what their feature is and how it works. If needed, they may also add a link to more technical README's located nearer to the code.
```

### Comparing `sovrin-1.2.0.dev1681906498/setup.py` & `sovrin-1.2.0rc1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,9 +34,9 @@
     keywords='Sovrin Genesis Transactions',
     packages=find_packages(exclude=['docs', 'docs*']),
     package_data={
         '': ['*.txt', '*.md', '*.rst', '*.json', '*.conf', '*.html',
              '*.css', '*.ico', '*.png', 'LICENSE', 'LEGAL', '*.indy']},
     include_package_data=True,
 
-    install_requires=['indy-node==1.13.2.dev1678195950', 'sovtoken==1.1.0.dev1678291666', 'sovtokenfees==1.1.0.dev1678291666'],
+    install_requires=['indy-node==1.13.2.rc5', 'sovtoken==1.1.0.rc0', 'sovtokenfees==1.1.0.rc0'],
 )
```

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/__metadata__.py` & `sovrin-1.2.0rc1/sovrin/__metadata__.py`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_builder_genesis` & `sovrin-1.2.0rc1/sovrin/domain_transactions_builder_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_live_genesis` & `sovrin-1.2.0rc1/sovrin/domain_transactions_live_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_local_genesis` & `sovrin-1.2.0rc1/sovrin/domain_transactions_local_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/domain_transactions_sandbox_genesis` & `sovrin-1.2.0rc1/sovrin/domain_transactions_sandbox_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_builder_genesis` & `sovrin-1.2.0rc1/sovrin/pool_transactions_builder_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_live_genesis` & `sovrin-1.2.0rc1/sovrin/pool_transactions_live_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_local_genesis` & `sovrin-1.2.0rc1/sovrin/pool_transactions_local_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_sandbox_genesis` & `sovrin-1.2.0rc1/sovrin/pool_transactions_sandbox_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin/pool_transactions_training_genesis` & `sovrin-1.2.0rc1/sovrin/pool_transactions_training_genesis`

 * *Files identical despite different names*

### Comparing `sovrin-1.2.0.dev1681906498/sovrin.egg-info/SOURCES.txt` & `sovrin-1.2.0rc1/sovrin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

