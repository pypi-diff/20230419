# Comparing `tmp/pineappl-0.6.0a7.tar.gz` & `tmp/pineappl-0.6.0a8.tar.gz`

## Comparing `pineappl-0.6.0a7.tar` & `pineappl-0.6.0a8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a7/local_dependencies/pineappl/Cargo.toml
--rw-r--r--   0     1001      123      594 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/README.md
--rw-r--r--   0     1001      123    37886 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/bin.rs
--rw-r--r--   0     1001      123      256 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/convert.rs
--rw-r--r--   0     1001      123     2962 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/empty_subgrid.rs
--rw-r--r--   0     1001      123    22471 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/evolution.rs
--rw-r--r--   0     1001      123    15042 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/fk_table.rs
--rw-r--r--   0     1001      123    96582 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/grid.rs
--rw-r--r--   0     1001      123    25442 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123    43946 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/lagrange_subgrid.rs
--rw-r--r--   0     1001      123      471 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/lib.rs
--rw-r--r--   0     1001      123    16120 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/lumi.rs
--rw-r--r--   0     1001      123     4853 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/ntuple_subgrid.rs
--rw-r--r--   0     1001      123     7912 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/pids.rs
--rw-r--r--   0     1001      123    36204 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/sparse_array3.rs
--rw-r--r--   0     1001      123    10342 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/src/subgrid.rs
--rw-r--r--   0     1001      123    16425 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/local_dependencies/pineappl/tests/drell_yan_lo.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a7/Cargo.toml
--rw-r--r--   0     1001      123      352 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/.gitignore
--rw-r--r--   0     1001      123      783 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/README.md
--rw-r--r--   0     1001      123      235 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/.gitignore
--rw-r--r--   0     1001      123      876 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/make.bat
--rw-r--r--   0     1001      123        0 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/_static/.gitkeep
--rw-r--r--   0     1001      123     6097 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/conf.py
--rw-r--r--   0     1001      123      886 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/implementation.rst
--rw-r--r--   0     1001      123     1295 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/index.rst
--rw-r--r--   0     1001      123       91 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/indices.rst
--rw-r--r--   0     1001      123     1148 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/installation.rst
--rw-r--r--   0     1001      123     2534 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/recipes.rst
--rw-r--r--   0     1001      123        0 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/refs.bib
--rw-r--r--   0     1001      123      951 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/docs/source/shared/roles.rst
--rw-r--r--   0     1001      123      893 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/package/Containerfile
--rw-r--r--   0     1001      123     3584 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/package/README.md
--rwxr-xr-x   0     1001      123      219 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/package/maturin
--rw-r--r--   0     1001      123      115 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/__init__.py
--rw-r--r--   0     1001      123      516 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/bin.py
--rw-r--r--   0     1001      123     1688 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/fk_table.py
--rw-r--r--   0     1001      123    12505 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/grid.py
--rw-r--r--   0     1001      123      762 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/import_only_subgrid.py
--rw-r--r--   0     1001      123      379 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/lumi.py
--rw-r--r--   0     1001      123      254 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/subgrid.py
--rw-r--r--   0     1001      123      430 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pineappl/utils.py
--rw-r--r--   0     1001      123     1141 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/pyproject.toml
--rw-r--r--   0     1001      123      674 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/bin.rs
--rw-r--r--   0     1001      123     1078 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/evolution.rs
--rw-r--r--   0     1001      123     6438 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/fk_table.rs
--rw-r--r--   0     1001      123    22338 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/grid.rs
--rw-r--r--   0     1001      123     1799 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123      874 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/lib.rs
--rw-r--r--   0     1001      123     1109 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/lumi.rs
--rw-r--r--   0     1001      123     4261 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/src/subgrid.rs
--rw-r--r--   0     1001      123      324 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/tests/conftest.py
--rw-r--r--   0     1001      123      355 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/tests/test_bin.py
--rw-r--r--   0     1001      123     6124 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/tests/test_grid.py
--rw-r--r--   0     1001      123      237 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/tests/test_lumi.py
--rw-r--r--   0     1001      123      868 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/tests/test_sugrid.py
--rw-r--r--   0     1001      123    44398 2023-04-19 09:52:11.000000 pineappl-0.6.0a7/Cargo.lock
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a7/PKG-INFO
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a8/local_dependencies/pineappl/Cargo.toml
+-rw-r--r--   0     1001      123      594 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/README.md
+-rw-r--r--   0     1001      123    37886 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/bin.rs
+-rw-r--r--   0     1001      123      256 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/convert.rs
+-rw-r--r--   0     1001      123     2962 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/empty_subgrid.rs
+-rw-r--r--   0     1001      123    22471 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/evolution.rs
+-rw-r--r--   0     1001      123    15042 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/fk_table.rs
+-rw-r--r--   0     1001      123    96582 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/grid.rs
+-rw-r--r--   0     1001      123    25442 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123    43946 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/lagrange_subgrid.rs
+-rw-r--r--   0     1001      123      471 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/lib.rs
+-rw-r--r--   0     1001      123    16120 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/lumi.rs
+-rw-r--r--   0     1001      123     4853 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/ntuple_subgrid.rs
+-rw-r--r--   0     1001      123     7912 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/pids.rs
+-rw-r--r--   0     1001      123    36204 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/sparse_array3.rs
+-rw-r--r--   0     1001      123    10342 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/src/subgrid.rs
+-rw-r--r--   0     1001      123    16425 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/local_dependencies/pineappl/tests/drell_yan_lo.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a8/Cargo.toml
+-rw-r--r--   0     1001      123      352 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/.gitignore
+-rw-r--r--   0     1001      123      783 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/README.md
+-rw-r--r--   0     1001      123      235 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/.gitignore
+-rw-r--r--   0     1001      123      876 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/make.bat
+-rw-r--r--   0     1001      123        0 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/_static/.gitkeep
+-rw-r--r--   0     1001      123     6097 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/conf.py
+-rw-r--r--   0     1001      123      886 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/implementation.rst
+-rw-r--r--   0     1001      123     1295 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/index.rst
+-rw-r--r--   0     1001      123       91 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/indices.rst
+-rw-r--r--   0     1001      123     1148 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/installation.rst
+-rw-r--r--   0     1001      123     2534 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/recipes.rst
+-rw-r--r--   0     1001      123        0 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/refs.bib
+-rw-r--r--   0     1001      123      951 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/docs/source/shared/roles.rst
+-rw-r--r--   0     1001      123      893 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/package/Containerfile
+-rw-r--r--   0     1001      123     3584 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/package/README.md
+-rwxr-xr-x   0     1001      123      219 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/package/maturin
+-rw-r--r--   0     1001      123      115 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/__init__.py
+-rw-r--r--   0     1001      123      516 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/bin.py
+-rw-r--r--   0     1001      123     1688 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/fk_table.py
+-rw-r--r--   0     1001      123    12505 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/grid.py
+-rw-r--r--   0     1001      123      762 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/import_only_subgrid.py
+-rw-r--r--   0     1001      123      379 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/lumi.py
+-rw-r--r--   0     1001      123      254 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/subgrid.py
+-rw-r--r--   0     1001      123      430 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pineappl/utils.py
+-rw-r--r--   0     1001      123     1141 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/pyproject.toml
+-rw-r--r--   0     1001      123      674 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/bin.rs
+-rw-r--r--   0     1001      123     1078 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/evolution.rs
+-rw-r--r--   0     1001      123     6438 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/fk_table.rs
+-rw-r--r--   0     1001      123    22338 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/grid.rs
+-rw-r--r--   0     1001      123     1799 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123      874 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/lib.rs
+-rw-r--r--   0     1001      123     1109 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/lumi.rs
+-rw-r--r--   0     1001      123     4261 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/src/subgrid.rs
+-rw-r--r--   0     1001      123      324 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/conftest.py
+-rw-r--r--   0     1001      123      355 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_bin.py
+-rw-r--r--   0     1001      123     6124 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_grid.py
+-rw-r--r--   0     1001      123      237 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_lumi.py
+-rw-r--r--   0     1001      123      868 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/tests/test_sugrid.py
+-rw-r--r--   0     1001      123    44398 2023-04-19 11:31:59.000000 pineappl-0.6.0a8/Cargo.lock
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a8/PKG-INFO
```

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/Cargo.toml` & `pineappl-0.6.0a8/local_dependencies/pineappl/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.7"
+version= "0.6.0-alpha.8"
 
 [dependencies]
 arrayvec = "0.7.2"
 bincode = "1.3.3"
 enum_dispatch = "0.3.7"
 float-cmp = "0.9.0"
 git-version = "0.3.5"
```

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/README.md` & `pineappl-0.6.0a8/local_dependencies/pineappl/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/bin.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/bin.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/empty_subgrid.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/empty_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/evolution.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/fk_table.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/fk_table.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/grid.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/grid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/import_only_subgrid.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/import_only_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/lagrange_subgrid.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/lagrange_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/lumi.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/ntuple_subgrid.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/ntuple_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/pids.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/pids.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/sparse_array3.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/sparse_array3.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/src/subgrid.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/src/subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/local_dependencies/pineappl/tests/drell_yan_lo.rs` & `pineappl-0.6.0a8/local_dependencies/pineappl/tests/drell_yan_lo.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/Cargo.toml` & `pineappl-0.6.0a8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.7"
+version= "0.6.0-alpha.8"
 
 [package.metadata.maturin]
 name = "pineappl"
 
 [lib]
 name = "pineappl"
 crate-type = ["cdylib"]
 
 [dependencies]
 itertools = "0.10.1"
 ndarray = "0.15.4"
 numpy = "0.16.2"
-pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.7" }
+pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.8" }
 pyo3 = { features = ["extension-module"], version = "0.16.4" }
```

### Comparing `pineappl-0.6.0a7/README.md` & `pineappl-0.6.0a8/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/Makefile` & `pineappl-0.6.0a8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/make.bat` & `pineappl-0.6.0a8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/source/conf.py` & `pineappl-0.6.0a8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/source/implementation.rst` & `pineappl-0.6.0a8/docs/source/implementation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/source/index.rst` & `pineappl-0.6.0a8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/source/installation.rst` & `pineappl-0.6.0a8/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/source/recipes.rst` & `pineappl-0.6.0a8/docs/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/docs/source/shared/roles.rst` & `pineappl-0.6.0a8/docs/source/shared/roles.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/package/Containerfile` & `pineappl-0.6.0a8/package/Containerfile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/package/README.md` & `pineappl-0.6.0a8/package/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/pineappl/bin.py` & `pineappl-0.6.0a8/pineappl/bin.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/pineappl/fk_table.py` & `pineappl-0.6.0a8/pineappl/fk_table.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/pineappl/grid.py` & `pineappl-0.6.0a8/pineappl/grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/pineappl/import_only_subgrid.py` & `pineappl-0.6.0a8/pineappl/import_only_subgrid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/pyproject.toml` & `pineappl-0.6.0a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/bin.rs` & `pineappl-0.6.0a8/src/bin.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/evolution.rs` & `pineappl-0.6.0a8/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/fk_table.rs` & `pineappl-0.6.0a8/src/fk_table.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/grid.rs` & `pineappl-0.6.0a8/src/grid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/import_only_subgrid.rs` & `pineappl-0.6.0a8/src/import_only_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/lib.rs` & `pineappl-0.6.0a8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/lumi.rs` & `pineappl-0.6.0a8/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/src/subgrid.rs` & `pineappl-0.6.0a8/src/subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/tests/test_grid.py` & `pineappl-0.6.0a8/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/tests/test_sugrid.py` & `pineappl-0.6.0a8/tests/test_sugrid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a7/Cargo.lock` & `pineappl-0.6.0a8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
  "once_cell",
  "pest",
  "sha1",
 ]
 
 [[package]]
 name = "pineappl"
-version = "0.6.0-alpha.7"
+version = "0.6.0-alpha.8"
 dependencies = [
  "anyhow",
  "arrayvec",
  "bincode",
  "enum_dispatch",
  "float-cmp",
  "git-version",
@@ -995,32 +995,32 @@
  "serde",
  "serde_yaml",
  "thiserror",
 ]
 
 [[package]]
 name = "pineappl_applgrid"
-version = "0.6.0-alpha.7"
+version = "0.6.0-alpha.8"
 dependencies = [
  "cc",
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_capi"
-version = "0.6.0-alpha.7"
+version = "0.6.0-alpha.8"
 dependencies = [
  "itertools",
  "pineappl",
 ]
 
 [[package]]
 name = "pineappl_cli"
-version = "0.6.0-alpha.7"
+version = "0.6.0-alpha.8"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "clap",
  "clap_mangen",
  "cxx",
@@ -1043,23 +1043,23 @@
  "serde",
  "serde_yaml",
  "tar",
 ]
 
 [[package]]
 name = "pineappl_fastnlo"
-version = "0.6.0-alpha.7"
+version = "0.6.0-alpha.8"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_py"
-version = "0.6.0-alpha.7"
+version = "0.6.0-alpha.8"
 dependencies = [
  "itertools",
  "ndarray",
  "numpy",
  "pineappl",
  "pyo3",
 ]
```

### Comparing `pineappl-0.6.0a7/PKG-INFO` & `pineappl-0.6.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pineappl
-Version: 0.6.0a7
+Version: 0.6.0a8
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

