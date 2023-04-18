# Comparing `tmp/ape-cairo-0.6.0.tar.gz` & `tmp/ape-cairo-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-cairo-0.6.0.tar", last modified: Wed Feb  1 20:03:02 2023, max compression
+gzip compressed data, was "ape-cairo-0.6.1.tar", last modified: Tue Apr 18 22:32:33 2023, max compression
```

## Comparing `ape-cairo-0.6.0.tar` & `ape-cairo-0.6.1.tar`

### file list

```diff
@@ -1,64 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/ape_cairo/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/ape_cairo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/ape_cairo/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/ape_cairo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/ape_cairo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-01 20:03:02.000000 ape-cairo-0.6.0/ape_cairo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/Account.cairo
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/Storage.cairo
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/UseDependency.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/namespace0/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/namespace0/library.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/namespace1/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/namespace1/library.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/tests/contracts/openzeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/openzeppelin/account/
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/openzeppelin/account/library.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/tests/contracts/openzeppelin/introspection/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/openzeppelin/introspection/erc165/
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/openzeppelin/introspection/erc165/library.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/openzeppelin/upgrades/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/openzeppelin/upgrades/library.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/tests/contracts/openzeppelin/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/contracts/openzeppelin/utils/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/contracts/openzeppelin/utils/constants/library.cairo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/tests/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.912056 ape-cairo-0.6.0/tests/dependency/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 20:03:02.916056 ape-cairo-0.6.0/tests/dependency/src/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/dependency/src/dependency/Dependency.cairo
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-02-01 20:01:40.000000 ape-cairo-0.6.0/tests/test_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.653475 ape-cairo-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.649475 ape-cairo-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.649475 ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.649475 ape-cairo-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-18 22:32:33.653475 ape-cairo-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.649475 ape-cairo-0.6.1/ape_cairo/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/ape_cairo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/ape_cairo/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/ape_cairo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.649475 ape-cairo-0.6.1/ape_cairo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 22:32:33.000000 ape-cairo-0.6.1/ape_cairo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-18 22:32:33.653475 ape-cairo-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.649475 ape-cairo-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.653475 ape-cairo-0.6.1/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/contracts/account.cairo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.653475 ape-cairo-0.6.1/tests/contracts/namespace/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/contracts/namespace/storage.cairo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:32:33.653475 ape-cairo-0.6.1/tests/contracts/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/contracts/storage/importme.cairo
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/contracts/storage.cairo
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-18 22:31:40.000000 ape-cairo-0.6.1/tests/test_compile.py
```

### Comparing `ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-cairo-0.6.1/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/.github/release-drafter.yml` & `ape-cairo-0.6.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/.github/workflows/commitlint.yaml` & `ape-cairo-0.6.1/.github/workflows/commitlint.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -17,11 +17,11 @@
           uses: actions/setup-python@v4
           with:
               python-version: 3.9
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
-            pip install .[dev]
+            pip install commitizen
 
         - name: Check commit history
           run: cz check --rev-range $(git rev-list --all --reverse | head -1)..HEAD
```

### Comparing `ape-cairo-0.6.0/.github/workflows/prtitle.yaml` & `ape-cairo-0.6.1/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/.github/workflows/publish.yaml` & `ape-cairo-0.6.1/.github/workflows/publish.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
-        python-version: 3.8
+        python-version: 3.9
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
         
     - name: Build
```

### Comparing `ape-cairo-0.6.0/.github/workflows/test.yaml` & `ape-cairo-0.6.1/.github/workflows/test.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
-              python-version: 3.8
+              python-version: 3.9
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
 
         - name: Run Black
@@ -59,24 +59,43 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9]
+                python-version: [3.9, "3.10"]
+
+        env:
+          GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          CAIRO_VERSION: v1.0.0-alpha.6
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
               python-version: ${{ matrix.python-version }}
 
+        - name: Install Rust
+          uses: actions-rs/toolchain@v1
+          with:
+            toolchain: stable
+            default: true
+            override: true
+
+        - name: Clone Cairo
+          run: |
+            git clone https://github.com/starkware-libs/cairo.git tests/cairo
+            pushd tests/cairo
+            git fetch --tags
+            git checkout ${{ env.CAIRO_VERSION }}
+            popd
+
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
 
         - name: Run Tests
           run: pytest -m "not fuzzing" -n 0 -s --cov
```

### Comparing `ape-cairo-0.6.0/.gitignore` & `ape-cairo-0.6.1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -115,11 +115,12 @@
 dmypy.json
 
 # setuptools-scm
 version.py
 
 # Ape stuff
 .build/
+tests/cairo
 
 **/.DS_Store
 *.swp
 *.swo
```

### Comparing `ape-cairo-0.6.0/.pre-commit-config.yaml` & `ape-cairo-0.6.1/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
-        additional_dependencies: [types-setuptools, pydantic]
+        additional_dependencies: [types-setuptools, pydantic==1.10.4]
 
 -   repo: https://github.com/executablebooks/mdformat
-    rev: 0.7.14
+    rev: 0.7.16
     hooks:
     -   id: mdformat
         additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
 
 default_language_version:
     python: python3
```

### Comparing `ape-cairo-0.6.0/CONTRIBUTING.md` & `ape-cairo-0.6.1/CONTRIBUTING.md`

 * *Files 23% similar despite different names*

```diff
@@ -43,7 +43,12 @@
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
 Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+
+## Tests
+
+To run the tests, follow the README but use `tests/cairo` as your directory for cloning Cairo.
+This is so the `ape-config.yaml` can be easily used by both CI-CD and local environments.
```

### Comparing `ape-cairo-0.6.0/LICENSE` & `ape-cairo-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/PKG-INFO` & `ape-cairo-0.6.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,15 @@
 Metadata-Version: 2.1
 Name: ape-cairo
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-cairo: A compiler plugin for the cairo programming language
 Home-page: https://github.com/ApeWorX/ape-cairo
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape compiler plugin around [the Cairo language](https://github.com/starkware-libs/cairo-lang).
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-cairo
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-cairo.git
-        cd ape-cairo
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        In a project directory where there are `.cairo` files in your `contracts/` directory, run the `compile` command:
-        
-        ```bash
-        ape compile
-        ```
-        
-        ### Configure Dependencies
-        
-        You can configure dependencies, such as from `GitHub`, using your `ape-config.yaml` file.
-        
-        There are two things you need to add:
-        
-        1. Add your dependency to Ape's root `dependencies:` key to trigger downloading and compiling it.
-        2. Configure the `ape-cairo` plugin to load that dependency in your project.
-        
-        For more information on dependencies, [see this guide](https://docs.apeworx.io/ape/stable/userguides/config.html#dependencies).
-        
-        Your `ape-config.yaml` will look something like:
-        
-        ```yaml
-        dependencies:
-          - name: OpenZeppelinCairo
-            github: OpenZeppelin/cairo-contracts
-            version: 0.1.0
-            contracts_folder: src
-        
-        cairo:
-          dependencies:
-            - OpenZeppelinCairo@0.1.0
-        ```
-        
-        **NOTE**: We are changing the `contracts/` folder to be `src` for this dependency.
-        
-        Now, in my `contracts/` folder, I can import from `openzeppelin`:
-        
-        ```cairo
-        from openzeppelin.token.erc20.library import (
-            ERC20_name,
-            ERC20_symbol,
-            ERC20_totalSupply,
-            ERC20_decimals,
-            ERC20_balanceOf,
-            ERC20_allowance,
-            ERC20_mint,
-            ERC20_burn,
-            ERC20_initializer,
-            ERC20_approve,
-            ERC20_increaseAllowance,
-            ERC20_decreaseAllowance,
-            ERC20_transfer,
-            ERC20_transferFrom
-        )
-        ```
-        
-        ## Development
-        
-        This project is in development and should be considered a beta.
-        Things might not be in their final state and breaking changes may occur.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -109,7 +19,110 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ape compiler plugin around [the Cairo language](https://github.com/starkware-libs/cairo-lang).
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [Rust](https://www.rust-lang.org/)
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-cairo
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-cairo.git
+cd ape-cairo
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, you will need to tell `ape-cairo` how to use the Cairo compiler.
+There are two ways to do this:
+
+1. Configure your Cairo manifest path in your `ape-config.yaml`.
+2. Build or add Cairo compiler binaries to your $PATH.
+
+Both options require cloning the Cairo compiler source code:
+
+```sh
+git clone git@github.com:starkware-libs/cairo.git
+cd cairo
+git fetch --all
+git checkout <tag>  # e.g. v1.0.0-alpha.6
+```
+
+To do the first option, add the following to your `ape-config.yaml` file:
+
+```yaml
+cairo:
+  manifest: /Users/home/path/to/cairo/Cargo.toml
+```
+
+Now, when compiling, Ape will use the command `cargo run --bin <BIN> --manifest-path <CAIRO-MANIFEST>`.
+To do the second option instead, build the release binaries for your OS:
+
+```sh
+cargo build --release
+```
+
+**NOTE**: This requires being in the same directory as Cairo.
+
+After the build completes, add the target path to your global $PATH variable.
+(You may want to add this to your `.zshrc` / `.bashrc` file):
+
+```sh
+export PATH=$PATH:$HOME/path/to/cairo/target/release
+```
+
+Verify you have `sierra-compile` in your `$PATH` by doing:
+
+```bash
+which sierra-compile
+```
+
+**WARN**: Note that when using Cairo-lang the python package, it will add conflicting binaries with the same name.
+You will need to ensure you are using the correct binaries if you have `cairo-lang` the Python package installed.
+
+```shell
+which starknet-compile
+```
+
+Alternatively, the first approach avoids this problem.
+
+### Using the Compiler
+
+In a project directory where there are `.cairo` files in your `contracts/` directory, run the `compile` command:
+
+```bash
+ape compile
+```
+
+It should create `ContractType` objects in your `.build/` folder containing the necessary Sierra code for contract declaration.
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
+
+
```

### Comparing `ape-cairo-0.6.0/ape_cairo.egg-info/PKG-INFO` & `ape-cairo-0.6.1/ape_cairo.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,15 @@
 Metadata-Version: 2.1
 Name: ape-cairo
-Version: 0.6.0
+Version: 0.6.1
 Summary: ape-cairo: A compiler plugin for the cairo programming language
 Home-page: https://github.com/ApeWorX/ape-cairo
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
-Description: # Quick Start
-        
-        Ape compiler plugin around [the Cairo language](https://github.com/starkware-libs/cairo-lang).
-        
-        ## Dependencies
-        
-        - [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
-        
-        ## Installation
-        
-        ### via `pip`
-        
-        You can install the latest release via [`pip`](https://pypi.org/project/pip/):
-        
-        ```bash
-        pip install ape-cairo
-        ```
-        
-        ### via `setuptools`
-        
-        You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
-        
-        ```bash
-        git clone https://github.com/ApeWorX/ape-cairo.git
-        cd ape-cairo
-        python3 setup.py install
-        ```
-        
-        ## Quick Usage
-        
-        In a project directory where there are `.cairo` files in your `contracts/` directory, run the `compile` command:
-        
-        ```bash
-        ape compile
-        ```
-        
-        ### Configure Dependencies
-        
-        You can configure dependencies, such as from `GitHub`, using your `ape-config.yaml` file.
-        
-        There are two things you need to add:
-        
-        1. Add your dependency to Ape's root `dependencies:` key to trigger downloading and compiling it.
-        2. Configure the `ape-cairo` plugin to load that dependency in your project.
-        
-        For more information on dependencies, [see this guide](https://docs.apeworx.io/ape/stable/userguides/config.html#dependencies).
-        
-        Your `ape-config.yaml` will look something like:
-        
-        ```yaml
-        dependencies:
-          - name: OpenZeppelinCairo
-            github: OpenZeppelin/cairo-contracts
-            version: 0.1.0
-            contracts_folder: src
-        
-        cairo:
-          dependencies:
-            - OpenZeppelinCairo@0.1.0
-        ```
-        
-        **NOTE**: We are changing the `contracts/` folder to be `src` for this dependency.
-        
-        Now, in my `contracts/` folder, I can import from `openzeppelin`:
-        
-        ```cairo
-        from openzeppelin.token.erc20.library import (
-            ERC20_name,
-            ERC20_symbol,
-            ERC20_totalSupply,
-            ERC20_decimals,
-            ERC20_balanceOf,
-            ERC20_allowance,
-            ERC20_mint,
-            ERC20_burn,
-            ERC20_initializer,
-            ERC20_approve,
-            ERC20_increaseAllowance,
-            ERC20_decreaseAllowance,
-            ERC20_transfer,
-            ERC20_transferFrom
-        )
-        ```
-        
-        ## Development
-        
-        This project is in development and should be considered a beta.
-        Things might not be in their final state and breaking changes may occur.
-        Comments, questions, criticisms and pull requests are welcomed.
-        
 Keywords: ethereum
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
@@ -109,7 +19,110 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
+License-File: LICENSE
+
+# Quick Start
+
+Ape compiler plugin around [the Cairo language](https://github.com/starkware-libs/cairo-lang).
+
+## Dependencies
+
+- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [Rust](https://www.rust-lang.org/)
+
+## Installation
+
+### via `pip`
+
+You can install the latest release via [`pip`](https://pypi.org/project/pip/):
+
+```bash
+pip install ape-cairo
+```
+
+### via `setuptools`
+
+You can clone the repository and use [`setuptools`](https://github.com/pypa/setuptools) for the most up-to-date version:
+
+```bash
+git clone https://github.com/ApeWorX/ape-cairo.git
+cd ape-cairo
+python3 setup.py install
+```
+
+## Quick Usage
+
+First, you will need to tell `ape-cairo` how to use the Cairo compiler.
+There are two ways to do this:
+
+1. Configure your Cairo manifest path in your `ape-config.yaml`.
+2. Build or add Cairo compiler binaries to your $PATH.
+
+Both options require cloning the Cairo compiler source code:
+
+```sh
+git clone git@github.com:starkware-libs/cairo.git
+cd cairo
+git fetch --all
+git checkout <tag>  # e.g. v1.0.0-alpha.6
+```
+
+To do the first option, add the following to your `ape-config.yaml` file:
+
+```yaml
+cairo:
+  manifest: /Users/home/path/to/cairo/Cargo.toml
+```
+
+Now, when compiling, Ape will use the command `cargo run --bin <BIN> --manifest-path <CAIRO-MANIFEST>`.
+To do the second option instead, build the release binaries for your OS:
+
+```sh
+cargo build --release
+```
+
+**NOTE**: This requires being in the same directory as Cairo.
+
+After the build completes, add the target path to your global $PATH variable.
+(You may want to add this to your `.zshrc` / `.bashrc` file):
+
+```sh
+export PATH=$PATH:$HOME/path/to/cairo/target/release
+```
+
+Verify you have `sierra-compile` in your `$PATH` by doing:
+
+```bash
+which sierra-compile
+```
+
+**WARN**: Note that when using Cairo-lang the python package, it will add conflicting binaries with the same name.
+You will need to ensure you are using the correct binaries if you have `cairo-lang` the Python package installed.
+
+```shell
+which starknet-compile
+```
+
+Alternatively, the first approach avoids this problem.
+
+### Using the Compiler
+
+In a project directory where there are `.cairo` files in your `contracts/` directory, run the `compile` command:
+
+```bash
+ape compile
+```
+
+It should create `ContractType` objects in your `.build/` folder containing the necessary Sierra code for contract declaration.
+
+## Development
+
+This project is in development and should be considered a beta.
+Things might not be in their final state and breaking changes may occur.
+Comments, questions, criticisms and pull requests are welcomed.
+
+
```

### Comparing `ape-cairo-0.6.0/pyproject.toml` & `ape-cairo-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-cairo-0.6.0/setup.py` & `ape-cairo-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
-        "pytest>=6.0",  # Core testing package
+        "pytest>=6.0,<8",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
-        "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
+        "hypothesis>=6.70,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0",  # auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
-        "mdformat>=0.7.16",  # Auto-formatter for markdown
-        "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
-        "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
+        "flake8>=6.0.0,<7",  # Style linter
+        "isort>=5.10.1,<6",  # Import sorting linter
+        "mdformat>=0.7.16,<0.8",  # Auto-formatter for markdown
+        "mdformat-gfm>=0.3.5,<0.4",  # Needed for formatting GitHub-flavored markdown
+        "mdformat-frontmatter>=0.4.1,<0.5",  # Needed for headers in GH issue templates
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "wheel",  # Packaging tool
         "twine",  # Package upload tool
     ],
     "dev": [
-        "commitizen>=2.19,<2.20",  # Manage commits and publishing releases
+        "commitizen>=2.42,<3",  # Manage commits and publishing releases
         "pre-commit",  # Ensure that linters are run prior to committing
         "pytest-watch",  # `ptw` test watcher/runner
         "IPython",  # Console for interacting
         "ipdb",  # Debugger (Must use `export PYTHONBREAKPOINT=ipdb.set_trace`)
     ],
 }
 
@@ -53,17 +53,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-cairo",
     include_package_data=True,
     install_requires=[
-        "cairo-lang>=0.10.3,<0.11",
-        "starknet_py>=0.14.0a0,<0.15",
-        "eth-ape>=0.6.1,<0.7",
+        "eth-ape>=0.6.8,<0.7",
         "ethpm-types",  # Use same version as eth-ape
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_cairo"],
     license="Apache-2.0",
     zip_safe=False,
```

### Comparing `ape-cairo-0.6.0/tests/conftest.py` & `ape-cairo-0.6.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 ape.config.PROJECT_FOLDER = Path(mkdtemp()).resolve()
 
 
 PROJECT_DIRECTORY = Path(__file__).parent
 SOURCE_CODE_DIRECTORY = PROJECT_DIRECTORY / "contracts"
 DEPENDENCY_DIRECTORY = PROJECT_DIRECTORY / "dependency"
 DEPENDENCY_SOURCE_CODE_DIRECTORY = DEPENDENCY_DIRECTORY / "src"
+NON_SOURCE_FILES = ("importme",)
 SOURCE_FILES = [
     p
     for p in [
         Path(str(p).replace(str(SOURCE_CODE_DIRECTORY), "").strip("/"))
         for p in get_all_files_in_directory(SOURCE_CODE_DIRECTORY)
     ]
-    if not str(p).startswith(".cache")
+    if not str(p).startswith(".cache") and p.stem not in NON_SOURCE_FILES
 ]
 
 
 @pytest.fixture
 def config():
     return ape.config
```

