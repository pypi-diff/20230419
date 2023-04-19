# Comparing `tmp/pineappl-0.6.0a5.tar.gz` & `tmp/pineappl-0.6.0a6.tar.gz`

## Comparing `pineappl-0.6.0a5.tar` & `pineappl-0.6.0a6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a5/local_dependencies/pineappl/Cargo.toml
--rw-r--r--   0     1001      123      594 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/README.md
--rw-r--r--   0     1001      123    30237 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/bin.rs
--rw-r--r--   0     1001      123      256 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/convert.rs
--rw-r--r--   0     1001      123     2962 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/empty_subgrid.rs
--rw-r--r--   0     1001      123    22471 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/evolution.rs
--rw-r--r--   0     1001      123    14977 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/fk_table.rs
--rw-r--r--   0     1001      123    96033 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/grid.rs
--rw-r--r--   0     1001      123    25456 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123    43946 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/lagrange_subgrid.rs
--rw-r--r--   0     1001      123      471 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/lib.rs
--rw-r--r--   0     1001      123    16120 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/lumi.rs
--rw-r--r--   0     1001      123     4860 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/ntuple_subgrid.rs
--rw-r--r--   0     1001      123     7912 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/pids.rs
--rw-r--r--   0     1001      123    36204 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/sparse_array3.rs
--rw-r--r--   0     1001      123    10342 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/src/subgrid.rs
--rw-r--r--   0     1001      123    14487 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/local_dependencies/pineappl/tests/drell_yan_lo.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a5/Cargo.toml
--rw-r--r--   0     1001      123      352 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/.gitignore
--rw-r--r--   0     1001      123      783 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/README.md
--rw-r--r--   0     1001      123      235 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/.gitignore
--rw-r--r--   0     1001      123      876 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/make.bat
--rw-r--r--   0     1001      123        0 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/_static/.gitkeep
--rw-r--r--   0     1001      123     6097 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/conf.py
--rw-r--r--   0     1001      123      886 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/implementation.rst
--rw-r--r--   0     1001      123     1295 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/index.rst
--rw-r--r--   0     1001      123       91 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/indices.rst
--rw-r--r--   0     1001      123     1148 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/installation.rst
--rw-r--r--   0     1001      123     2534 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/recipes.rst
--rw-r--r--   0     1001      123        0 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/refs.bib
--rw-r--r--   0     1001      123      951 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/docs/source/shared/roles.rst
--rw-r--r--   0     1001      123      893 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/package/Containerfile
--rw-r--r--   0     1001      123     3584 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/package/README.md
--rwxr-xr-x   0     1001      123      219 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/package/maturin
--rw-r--r--   0     1001      123      115 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/__init__.py
--rw-r--r--   0     1001      123      516 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/bin.py
--rw-r--r--   0     1001      123     1688 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/fk_table.py
--rw-r--r--   0     1001      123    12505 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/grid.py
--rw-r--r--   0     1001      123      762 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/import_only_subgrid.py
--rw-r--r--   0     1001      123      379 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/lumi.py
--rw-r--r--   0     1001      123      254 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/subgrid.py
--rw-r--r--   0     1001      123      430 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pineappl/utils.py
--rw-r--r--   0     1001      123     1141 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/pyproject.toml
--rw-r--r--   0     1001      123      674 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/bin.rs
--rw-r--r--   0     1001      123     1078 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/evolution.rs
--rw-r--r--   0     1001      123     6438 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/fk_table.rs
--rw-r--r--   0     1001      123    22300 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/grid.rs
--rw-r--r--   0     1001      123     1799 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/import_only_subgrid.rs
--rw-r--r--   0     1001      123      874 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/lib.rs
--rw-r--r--   0     1001      123     1109 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/lumi.rs
--rw-r--r--   0     1001      123     4261 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/src/subgrid.rs
--rw-r--r--   0     1001      123      324 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/tests/conftest.py
--rw-r--r--   0     1001      123      355 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/tests/test_bin.py
--rw-r--r--   0     1001      123     6124 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/tests/test_grid.py
--rw-r--r--   0     1001      123      237 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/tests/test_lumi.py
--rw-r--r--   0     1001      123      868 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/tests/test_sugrid.py
--rw-r--r--   0     1001      123    44390 2023-03-30 15:51:37.000000 pineappl-0.6.0a5/Cargo.lock
--rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a5/PKG-INFO
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 pineappl-0.6.0a6/local_dependencies/pineappl/Cargo.toml
+-rw-r--r--   0     1001      123      594 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/README.md
+-rw-r--r--   0     1001      123    37886 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/bin.rs
+-rw-r--r--   0     1001      123      256 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/convert.rs
+-rw-r--r--   0     1001      123     2962 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/empty_subgrid.rs
+-rw-r--r--   0     1001      123    22471 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/evolution.rs
+-rw-r--r--   0     1001      123    15042 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/fk_table.rs
+-rw-r--r--   0     1001      123    96582 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/grid.rs
+-rw-r--r--   0     1001      123    25442 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123    43946 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/lagrange_subgrid.rs
+-rw-r--r--   0     1001      123      471 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/lib.rs
+-rw-r--r--   0     1001      123    16120 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/lumi.rs
+-rw-r--r--   0     1001      123     4853 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/ntuple_subgrid.rs
+-rw-r--r--   0     1001      123     7912 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/pids.rs
+-rw-r--r--   0     1001      123    36204 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/sparse_array3.rs
+-rw-r--r--   0     1001      123    10342 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/src/subgrid.rs
+-rw-r--r--   0     1001      123    16425 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/local_dependencies/pineappl/tests/drell_yan_lo.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 pineappl-0.6.0a6/Cargo.toml
+-rw-r--r--   0     1001      123      352 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/.gitignore
+-rw-r--r--   0     1001      123      783 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/README.md
+-rw-r--r--   0     1001      123      235 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/.gitignore
+-rw-r--r--   0     1001      123      876 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/make.bat
+-rw-r--r--   0     1001      123        0 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/_static/.gitkeep
+-rw-r--r--   0     1001      123     6097 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/conf.py
+-rw-r--r--   0     1001      123      886 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/implementation.rst
+-rw-r--r--   0     1001      123     1295 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/index.rst
+-rw-r--r--   0     1001      123       91 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/indices.rst
+-rw-r--r--   0     1001      123     1148 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/installation.rst
+-rw-r--r--   0     1001      123     2534 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/recipes.rst
+-rw-r--r--   0     1001      123        0 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/refs.bib
+-rw-r--r--   0     1001      123      951 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/docs/source/shared/roles.rst
+-rw-r--r--   0     1001      123      893 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/package/Containerfile
+-rw-r--r--   0     1001      123     3584 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/package/README.md
+-rwxr-xr-x   0     1001      123      219 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/package/maturin
+-rw-r--r--   0     1001      123      115 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/__init__.py
+-rw-r--r--   0     1001      123      516 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/bin.py
+-rw-r--r--   0     1001      123     1688 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/fk_table.py
+-rw-r--r--   0     1001      123    12505 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/grid.py
+-rw-r--r--   0     1001      123      762 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/import_only_subgrid.py
+-rw-r--r--   0     1001      123      379 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/lumi.py
+-rw-r--r--   0     1001      123      254 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/subgrid.py
+-rw-r--r--   0     1001      123      430 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pineappl/utils.py
+-rw-r--r--   0     1001      123     1141 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/pyproject.toml
+-rw-r--r--   0     1001      123      674 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/bin.rs
+-rw-r--r--   0     1001      123     1078 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/evolution.rs
+-rw-r--r--   0     1001      123     6438 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/fk_table.rs
+-rw-r--r--   0     1001      123    22338 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/grid.rs
+-rw-r--r--   0     1001      123     1799 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/import_only_subgrid.rs
+-rw-r--r--   0     1001      123      874 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/lib.rs
+-rw-r--r--   0     1001      123     1109 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/lumi.rs
+-rw-r--r--   0     1001      123     4261 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/src/subgrid.rs
+-rw-r--r--   0     1001      123      324 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/tests/conftest.py
+-rw-r--r--   0     1001      123      355 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/tests/test_bin.py
+-rw-r--r--   0     1001      123     6124 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/tests/test_grid.py
+-rw-r--r--   0     1001      123      237 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/tests/test_lumi.py
+-rw-r--r--   0     1001      123      868 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/tests/test_sugrid.py
+-rw-r--r--   0     1001      123    44398 2023-04-19 08:55:49.000000 pineappl-0.6.0a6/Cargo.lock
+-rw-r--r--   0        0        0     2373 1970-01-01 00:00:00.000000 pineappl-0.6.0a6/PKG-INFO
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/Cargo.toml` & `pineappl-0.6.0a6/local_dependencies/pineappl/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.5"
+version= "0.6.0-alpha.6"
 
 [dependencies]
 arrayvec = "0.7.2"
 bincode = "1.3.3"
 enum_dispatch = "0.3.7"
 float-cmp = "0.9.0"
 git-version = "0.3.5"
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/README.md` & `pineappl-0.6.0a6/local_dependencies/pineappl/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/bin.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/bin.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 //! Module that contains helpers for binning observables
 
 use super::convert::{f64_from_usize, usize_from_f64};
 use float_cmp::approx_eq;
+use itertools::izip;
 use itertools::Itertools;
 use serde::{Deserialize, Serialize};
 use std::f64;
 use std::ops::Range;
+use std::str::FromStr;
 use thiserror::Error;
 
 #[derive(Clone, Debug, Deserialize, PartialEq, Serialize)]
 enum Limits {
     Equal { left: f64, right: f64, bins: usize },
     Unequal { limits: Vec<f64> },
 }
@@ -81,31 +83,207 @@
 /// Captures all information about the bins in a grid.
 #[derive(Debug)]
 pub struct BinInfo<'a> {
     limits: &'a BinLimits,
     remapper: Option<&'a BinRemapper>,
 }
 
+/// Error type returned by [`BinRemapper::from_str`]
+#[derive(Debug, Error)]
+#[error("{0}")]
+pub struct ParseBinRemapperError(String);
+
+impl FromStr for BinRemapper {
+    type Err = ParseBinRemapperError;
+
+    fn from_str(s: &str) -> Result<Self, Self::Err> {
+        let remaps: Result<Vec<Vec<Vec<_>>>, Self::Err> = s
+            .split(';')
+            .map(|string| {
+                string
+                    .split('|')
+                    .map(|string| {
+                        string
+                            .find(':')
+                            .map_or(string, |index| {
+                                let (lhs, rhs) = string.split_at(index);
+                                let rhs = &rhs[1..]; // remove ':' which is contained with `split_at`
+
+                                // extract the part that doesn't belong to the ':' specification
+                                match (lhs.trim().parse::<usize>(), rhs.trim().parse::<usize>()) {
+                                    (Err(_), Ok(_)) => lhs,
+                                    (Ok(_), Err(_)) => rhs,
+                                    _ => "",
+                                }
+                            })
+                            .split(',')
+                            .filter_map(|string| {
+                                let string = string.trim();
+                                if string.is_empty() {
+                                    None
+                                } else {
+                                    Some(string.parse::<f64>().map_err(|_| {
+                                        ParseBinRemapperError(format!(
+                                            "unable to parse limit '{string}'"
+                                        ))
+                                    }))
+                                }
+                            })
+                            .collect()
+                    })
+                    .collect()
+            })
+            .collect();
+        let mut remaps = remaps?;
+
+        if remaps[0].len() != 1 {
+            return Err(ParseBinRemapperError(
+                "'|' syntax not meaningful for first dimension".to_string(),
+            ));
+        }
+
+        // go over `remaps` again, and repeat previous entries as requested with the `|` syntax
+        for vec in &mut remaps {
+            for i in 1..vec.len() {
+                if vec[i].is_empty() {
+                    if vec[i - 1].is_empty() {
+                        return Err(ParseBinRemapperError(
+                            "empty repetition with '|'".to_string(),
+                        ));
+                    }
+
+                    vec[i] = vec[i - 1].clone();
+                }
+            }
+        }
+
+        // go over `remaps` again, this time remove bin as requested with the `:N` or `N:` syntax
+        for (vec, string) in remaps.iter_mut().zip(s.split(';')) {
+            for (vec, string) in vec.iter_mut().zip(string.split('|')) {
+                let (lhs, rhs) = {
+                    let split: Vec<_> = string.split(':').collect();
+
+                    if split.len() == 1 {
+                        // there's no colon
+                        continue;
+                    }
+
+                    if split.len() != 2 {
+                        return Err(ParseBinRemapperError(format!(
+                            "too many ':' found: '{}'",
+                            string
+                        )));
+                    }
+
+                    (split[0].parse::<usize>(), split[1].parse::<usize>())
+                };
+
+                if let Ok(num) = rhs {
+                    vec.truncate(vec.len() - num);
+                }
+
+                if let Ok(num) = lhs {
+                    vec.drain(0..num);
+                }
+
+                if lhs.is_err() && rhs.is_err() {
+                    return Err(ParseBinRemapperError(format!(
+                        "unable to parse ':' syntax from: '{}'",
+                        string
+                    )));
+                }
+
+                if vec.len() <= 1 {
+                    return Err(ParseBinRemapperError(
+                        "no limits due to ':' syntax".to_string(),
+                    ));
+                }
+            }
+        }
+
+        let dimensions = remaps.len();
+        let mut normalizations = Vec::new();
+        let mut limits = Vec::new();
+        let mut buffer = Vec::with_capacity(dimensions);
+        let mut pipe_indices = vec![0; dimensions];
+        let mut last_indices = vec![0; dimensions];
+
+        'looop: for indices in remaps
+            .iter()
+            .map(|vec| 0..vec.iter().map(|vec| vec.len() - 1).max().unwrap())
+            .multi_cartesian_product()
+        {
+            // calculate `pipe_indices`, which stores the indices for the second dimension of `remaps`
+            for d in 0..dimensions - 1 {
+                if indices[d] > last_indices[d] {
+                    for dp in d + 1..dimensions {
+                        if remaps[dp].len() != 1 {
+                            pipe_indices[dp] += 1;
+                        }
+                    }
+                }
+            }
+
+            last_indices = indices.clone();
+
+            let mut normalization = 1.0;
+
+            for (remap, &pipe_index, &i) in izip!(&remaps, &pipe_indices, &indices) {
+                if let Some(r) = remap.get(pipe_index) {
+                    if r.len() <= (i + 1) {
+                        buffer.clear();
+
+                        // this index doesn't exist
+                        continue 'looop;
+                    }
+
+                    let left = r[i];
+                    let right = r[i + 1];
+
+                    buffer.push((left, right));
+                    normalization *= right - left;
+                } else {
+                    return Err(ParseBinRemapperError(
+                        "missing '|' specification: number of variants too small".to_string(),
+                    ));
+                }
+            }
+
+            limits.append(&mut buffer);
+            normalizations.push(normalization);
+        }
+
+        Ok(Self {
+            normalizations,
+            limits,
+        })
+    }
+}
+
 impl<'a> BinInfo<'a> {
     /// Constructor.
     #[must_use]
     pub const fn new(limits: &'a BinLimits, remapper: Option<&'a BinRemapper>) -> Self {
         Self { limits, remapper }
     }
 
     /// Return the bin limits for the bin with index `bin`.
+    #[must_use]
     pub fn bin_limits(&self, bin: usize) -> Vec<(f64, f64)> {
         // TODO: make return type a Cow
-        if let Some(remapper) = self.remapper {
-            let dim = remapper.dimensions();
-            remapper.limits()[bin * dim..(bin + 1) * dim].to_vec()
-        } else {
-            let limits = &self.limits.limits()[bin..=bin + 1];
-            vec![(limits[0], limits[1])]
-        }
+        self.remapper.map_or_else(
+            || {
+                let limits = &self.limits.limits()[bin..=bin + 1];
+                vec![(limits[0], limits[1])]
+            },
+            |remapper| {
+                let dim = remapper.dimensions();
+                remapper.limits()[bin * dim..(bin + 1) * dim].to_vec()
+            },
+        )
     }
 
     /// Returns the number of bins.
     #[must_use]
     pub fn bins(&self) -> usize {
         self.limits.bins()
     }
@@ -114,14 +292,15 @@
     #[must_use]
     pub fn dimensions(&self) -> usize {
         self.remapper.map_or(1, BinRemapper::dimensions)
     }
 
     /// Return the index of the bin corresponding to `limits`. If no bin is found `None` is
     /// returned.
+    #[must_use]
     pub fn find_bin(&self, limits: &[(f64, f64)]) -> Option<usize> {
         (0..self.bins())
             .map(|bin| self.bin_limits(bin))
             .position(|lim| lim == limits)
     }
 
     /// Returns all left-limits for the specified dimension. If the dimension does not exist, an
@@ -928,8 +1107,50 @@
     //fn bin_remapper_merge_bins_panic() {
     //    let mut remapper =
     //        BinRemapper::new(vec![1.0; 3], vec![(0.0, 0.25), (0.5, 0.75), (0.75, 1.0)]).unwrap();
 
     //    //assert_eq!(remapper.slices(), [(0, 1), (1, 3)]);
     //    remapper.merge_bins(0..3).unwrap();
     //}
+
+    #[test]
+    #[should_panic(expected = "'|' syntax not meaningful for first dimension")]
+    fn pipe_syntax_first_dimension() {
+        BinRemapper::from_str("|0,1,2").unwrap();
+    }
+
+    #[test]
+    #[should_panic(expected = "empty repetition with '|'")]
+    fn pipe_syntax_first_empty() {
+        BinRemapper::from_str("0,1,2;0,2,4;||").unwrap();
+    }
+
+    #[test]
+    #[should_panic(expected = "too many ':' found: '::'")]
+    fn colon_syntax_too_many_colons() {
+        BinRemapper::from_str("0,1,2;0,2,4;1,2,3,4,5|::").unwrap();
+    }
+
+    #[test]
+    #[should_panic(expected = "unable to parse ':' syntax from: '2.5:'")]
+    fn colon_syntax_bad_lhs() {
+        BinRemapper::from_str("0,1,2;0,2,4;1,2,3,4,5|2.5:|:3|:3").unwrap();
+    }
+
+    #[test]
+    #[should_panic(expected = "unable to parse ':' syntax from: ':2.5'")]
+    fn colon_syntax_bad_rhs() {
+        BinRemapper::from_str("0,1,2;0,2,4;1,2,3,4,5|:2.5|:3|:3").unwrap();
+    }
+
+    #[test]
+    #[should_panic(expected = "no limits due to ':' syntax")]
+    fn colon_syntax_no_limits() {
+        BinRemapper::from_str("0,1,2;0,2,4;1,2,3,4,5|:4|:3|:3").unwrap();
+    }
+
+    #[test]
+    #[should_panic(expected = "missing '|' specification: number of variants too small")]
+    fn pipe_syntax_too_few_pipes() {
+        BinRemapper::from_str("0,1,2;0,2,4;1,2,3|4,5,6|7,8,9").unwrap();
+    }
 }
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/empty_subgrid.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/empty_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/evolution.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/fk_table.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/fk_table.rs`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,19 @@
 impl FkTable {
     /// Returns the [`Grid`] object for this `FkTable`.
     #[must_use]
     pub const fn grid(&self) -> &Grid {
         &self.grid
     }
 
+    /// Converts the `FkTable` back to a [`Grid`].
+    pub fn into_grid(self) -> Grid {
+        self.grid
+    }
+
     /// Returns the FK table represented as a four-dimensional array indexed by `bin`, `lumi`,
     /// `x1` and `x2`, in this order.
     #[must_use]
     pub fn table(&self) -> Array4<f64> {
         let has_pdf1 = self.grid.has_pdf1();
         let has_pdf2 = self.grid.has_pdf2();
         let x_grid = self.x_grid();
@@ -372,18 +377,16 @@
 
                 if mu2_grid.len() > 1 {
                     return Err(TryFromGridError::MultipleScales);
                 }
 
                 if muf2 < 0.0 {
                     muf2 = mu2_grid[0].fac;
-                } else {
-                    if muf2 != mu2_grid[0].fac {
-                        return Err(TryFromGridError::MultipleScales);
-                    }
+                } else if muf2 != mu2_grid[0].fac {
+                    return Err(TryFromGridError::MultipleScales);
                 }
             }
         }
 
         for lumi in grid.lumi() {
             let entry = lumi.entry();
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/grid.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/grid.rs`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 use std::cmp::Ordering;
 use std::collections::HashMap;
 use std::convert::{TryFrom, TryInto};
 use std::io::{self, BufRead, BufReader, BufWriter, Read, Write};
 use std::iter;
 use std::mem;
 use std::ops::Range;
+use std::slice;
 use thiserror::Error;
 
 // TODO: when possible change the types from `u32` to `u8` to change `try_into` to `into`
 
 /// Coupling powers for each grid.
 #[derive(Clone, Debug, Deserialize, Eq, Hash, PartialEq, Serialize)]
 pub struct Order {
@@ -73,19 +74,19 @@
             alphas,
             alpha,
             logxir,
             logxif,
         }
     }
 
-    /// Return a mask suitable to pass as the `order_mask` parameter of [`Grid::convolute`]. The
-    /// selection of `orders` is controlled using the `max_as` and `max_al` parameters, for
-    /// instance setting `max_as = 1` and `max_al = 0` selects the LO QCD only, `max_as = 2` and
-    /// `max_al = 0` the NLO QCD; setting `max_as = 3` and `max_al = 2` would select all NLOs, and
-    /// the NNLO QCD.
+    /// Return a mask suitable to pass as the `order_mask` parameter of [`Grid::convolute`],
+    /// [`Grid::evolve`] or [`Grid::evolve_info`]. The selection of `orders` is controlled using
+    /// the `max_as` and `max_al` parameters, for instance setting `max_as = 1` and `max_al = 0`
+    /// selects the LO QCD only, `max_as = 2` and `max_al = 0` the NLO QCD; setting `max_as = 3`
+    /// and `max_al = 2` would select all NLOs, and the NNLO QCD.
     ///
     /// # Example
     ///
     /// In the case of Drell—Yan, there are the following orders:
     ///
     /// - exactly one leading order (LO),
     /// - two next-to-leading orders (NLO), which are
@@ -105,44 +106,44 @@
     ///     Order::new(0, 3, 0, 0), //  NLO  EW    :          alpha^3
     ///     Order::new(2, 2, 0, 0), // NNLO QCD    : alphas^2 alpha^2
     ///     Order::new(1, 3, 0, 0), // NNLO QCD—EW : alphas   alpha^3
     ///     Order::new(0, 4, 0, 0), // NNLO EW     :          alpha^4
     /// ];
     ///
     /// // LO EW
-    /// assert_eq!(Order::create_mask(&orders, 0, 1), [true, false, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 0, 1, false), [true, false, false, false, false, false]);
     /// // LO QCD
-    /// assert_eq!(Order::create_mask(&orders, 1, 0), [true, false, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 1, 0, false), [true, false, false, false, false, false]);
     /// // LO
-    /// assert_eq!(Order::create_mask(&orders, 1, 1), [true, false, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 1, 1, false), [true, false, false, false, false, false]);
     /// // NLO QCD
-    /// assert_eq!(Order::create_mask(&orders, 2, 0), [true, true, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 2, 0, false), [true, true, false, false, false, false]);
     /// // NLO EW
-    /// assert_eq!(Order::create_mask(&orders, 0, 2), [true, false, true, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 0, 2, false), [true, false, true, false, false, false]);
     /// // NNLO QCD
-    /// assert_eq!(Order::create_mask(&orders, 3, 0), [true, true, false, true, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 3, 0, false), [true, true, false, true, false, false]);
     /// // NNLO EW
-    /// assert_eq!(Order::create_mask(&orders, 0, 3), [true, false, true, false, false, true]);
+    /// assert_eq!(Order::create_mask(&orders, 0, 3, false), [true, false, true, false, false, true]);
     /// ```
     ///
-    /// Although not shown in the example above, orders containing non-zero powers of logarithms
-    /// are selected as well:
+    /// Orders containing non-zero powers of logarithms can be selected as well if `logs` is set to
+    /// `true`:
     ///
     /// ```rust
     /// use pineappl::grid::Order;
     ///
     /// let orders = [
     ///     Order::new(0, 2, 0, 0), //  LO         :        alpha^2
     ///     Order::new(1, 2, 0, 0), //  NLO QCD    : alphas alpha^2
     ///     Order::new(1, 2, 1, 0), //  NLO QCD    : alphas alpha^2 logxif
     ///     Order::new(0, 3, 0, 0), //  NLO  EW    :        alpha^3
     ///     Order::new(0, 3, 1, 0), //  NLO  EW    :        alpha^3 logxif
     /// ];
     ///
-    /// assert_eq!(Order::create_mask(&orders, 0, 2), [true, false, false, true, true]);
+    /// assert_eq!(Order::create_mask(&orders, 0, 2, true), [true, false, false, true, true]);
     /// ```
     ///
     /// For the more complicated example of top-pair production one can see the difference between
     /// the selection for different LOs:
     ///
     /// ```rust
     /// use pineappl::grid::Order;
@@ -154,22 +155,22 @@
     ///     Order::new(3, 0, 0, 0), //  NLO QCD    : alphas^3
     ///     Order::new(2, 1, 0, 0), //  NLO QCD—EW : alphas^2 alpha
     ///     Order::new(1, 2, 0, 0), //  NLO QCD—EW : alphas   alpha^2
     ///     Order::new(0, 3, 0, 0), //  NLO EW     :          alpha^3
     /// ];
     ///
     /// // LO EW
-    /// assert_eq!(Order::create_mask(&orders, 0, 1), [false, false, true, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 0, 1, false), [false, false, true, false, false, false, false]);
     /// // LO QCD
-    /// assert_eq!(Order::create_mask(&orders, 1, 0), [true, false, false, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 1, 0, false), [true, false, false, false, false, false, false]);
     /// // LO
-    /// assert_eq!(Order::create_mask(&orders, 1, 1), [true, true, true, false, false, false, false]);
+    /// assert_eq!(Order::create_mask(&orders, 1, 1, false), [true, true, true, false, false, false, false]);
     /// ```
     #[must_use]
-    pub fn create_mask(orders: &[Self], max_as: u32, max_al: u32) -> Vec<bool> {
+    pub fn create_mask(orders: &[Self], max_as: u32, max_al: u32, logs: bool) -> Vec<bool> {
         // smallest sum of alphas and alpha
         let lo = orders
             .iter()
             .map(|Self { alphas, alpha, .. }| alphas + alpha)
             .min()
             .unwrap_or_default();
 
@@ -192,25 +193,36 @@
             .unwrap_or_default();
 
         let max = max_as.max(max_al);
         let min = max_as.min(max_al);
 
         orders
             .iter()
-            .map(|Self { alphas, alpha, .. }| {
-                let pto = alphas + alpha - lo;
+            .map(
+                |&Self {
+                     alphas,
+                     alpha,
+                     logxir,
+                     logxif,
+                 }| {
+                    if !logs && (logxir > 0 || logxif > 0) {
+                        return false;
+                    }
 
-                alphas + alpha < min + lo
-                    || (alphas + alpha < max + lo
-                        && match max_as.cmp(&max_al) {
-                            Ordering::Greater => lo_as + pto == *alphas,
-                            Ordering::Less => lo_al + pto == *alpha,
-                            Ordering::Equal => false,
-                        })
-            })
+                    let pto = alphas + alpha - lo;
+
+                    alphas + alpha < min + lo
+                        || (alphas + alpha < max + lo
+                            && match max_as.cmp(&max_al) {
+                                Ordering::Greater => lo_as + pto == alphas,
+                                Ordering::Less => lo_al + pto == alpha,
+                                Ordering::Equal => false,
+                            })
+                },
+            )
             .collect()
     }
 }
 
 /// This structure represents a position (`x1`, `x2`, `q2`) in a `Subgrid` together with a
 /// corresponding `weight`. The type `W` can either be a `f64` or `()`, which is used when multiple
 /// weights should be signaled.
@@ -906,15 +918,15 @@
         self.orders.append(&mut new_orders);
         self.lumi.append(&mut new_entries);
 
         let bin_indices: Vec<_> = (0..other.bin_info().bins())
             .map(|bin| {
                 self.bin_info()
                     .find_bin(&other.bin_info().bin_limits(bin))
-                    .expect(&format!("failed for {}", bin))
+                    .unwrap_or_else(|| panic!("failed for {bin}"))
             })
             .collect();
 
         for ((i, j, k), subgrid) in other
             .subgrids
             .indexed_iter_mut()
             .filter(|((_, _, _), subgrid)| !subgrid.is_empty())
@@ -1399,33 +1411,33 @@
         let initial_state_2 = self.initial_state_2();
 
         // are the initial states hadrons?
         let has_pdf1 = self.has_pdf1();
         let has_pdf2 = self.has_pdf2();
 
         let pids1 = if has_pdf1 {
-            eko_info.grid_axes.pids.clone()
+            &eko_info.grid_axes.pids
         } else {
-            vec![initial_state_1]
+            slice::from_ref(&initial_state_1)
         };
         let pids2 = if has_pdf2 {
-            eko_info.grid_axes.pids.clone()
+            &eko_info.grid_axes.pids
         } else {
-            vec![initial_state_2]
+            slice::from_ref(&initial_state_2)
         };
         // create target luminosities
         let tgt_pids1 = if has_pdf1 {
-            eko_info.target_pids.clone()
+            &eko_info.target_pids
         } else {
-            vec![initial_state_1]
+            slice::from_ref(&initial_state_1)
         };
         let tgt_pids2 = if has_pdf2 {
-            eko_info.target_pids.clone()
+            &eko_info.target_pids
         } else {
-            vec![initial_state_2]
+            slice::from_ref(&initial_state_2)
         };
         let lumi: Vec<_> = tgt_pids1
             .iter()
             .cartesian_product(tgt_pids2.iter())
             .map(|(a, b)| lumi_entry![*a, *b, 1.0])
             .collect();
 
@@ -2082,75 +2094,75 @@
             Order::new(0, 3, 0, 0), //  NLO  EW    :          alpha^3
             Order::new(2, 2, 0, 0), // NNLO QCD    : alphas^2 alpha^2
             Order::new(1, 3, 0, 0), // NNLO QCD—EW : alphas   alpha^3
             Order::new(0, 4, 0, 0), // NNLO EW     :          alpha^4
         ];
 
         assert_eq!(
-            Order::create_mask(&orders, 0, 0),
+            Order::create_mask(&orders, 0, 0, false),
             [false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 0, 1),
+            Order::create_mask(&orders, 0, 1, false),
             [true, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 0, 2),
+            Order::create_mask(&orders, 0, 2, false),
             [true, false, true, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 0, 3),
+            Order::create_mask(&orders, 0, 3, false),
             [true, false, true, false, false, true]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 0),
+            Order::create_mask(&orders, 1, 0, false),
             [true, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 1),
+            Order::create_mask(&orders, 1, 1, false),
             [true, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 2),
+            Order::create_mask(&orders, 1, 2, false),
             [true, false, true, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 3),
+            Order::create_mask(&orders, 1, 3, false),
             [true, false, true, false, false, true]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 0),
+            Order::create_mask(&orders, 2, 0, false),
             [true, true, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 1),
+            Order::create_mask(&orders, 2, 1, false),
             [true, true, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 2),
+            Order::create_mask(&orders, 2, 2, false),
             [true, true, true, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 3),
+            Order::create_mask(&orders, 2, 3, false),
             [true, true, true, false, false, true]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 0),
+            Order::create_mask(&orders, 3, 0, false),
             [true, true, false, true, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 1),
+            Order::create_mask(&orders, 3, 1, false),
             [true, true, false, true, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 2),
+            Order::create_mask(&orders, 3, 2, false),
             [true, true, true, true, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 3),
+            Order::create_mask(&orders, 3, 3, false),
             [true, true, true, true, true, true]
         );
 
         // Top-pair production orders
         let orders = [
             Order::new(2, 0, 0, 0), //   LO QCD    : alphas^2
             Order::new(1, 1, 0, 0), //   LO QCD—EW : alphas   alpha
@@ -2163,75 +2175,75 @@
             Order::new(3, 1, 0, 0), // NNLO QCD—EW : alphas^3 alpha
             Order::new(2, 2, 0, 0), // NNLO QCD—EW : alphas^2 alpha^2
             Order::new(1, 3, 0, 0), // NNLO QCD—EW : alphas   alpha^3
             Order::new(0, 4, 0, 0), // NNLO EW     :          alpha^4
         ];
 
         assert_eq!(
-            Order::create_mask(&orders, 0, 0),
+            Order::create_mask(&orders, 0, 0, false),
             [false, false, false, false, false, false, false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 0, 1),
+            Order::create_mask(&orders, 0, 1, false),
             [false, false, true, false, false, false, false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 0, 2),
+            Order::create_mask(&orders, 0, 2, false),
             [false, false, true, false, false, false, true, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 0, 3),
+            Order::create_mask(&orders, 0, 3, false),
             [false, false, true, false, false, false, true, false, false, false, false, true]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 0),
+            Order::create_mask(&orders, 1, 0, false),
             [true, false, false, false, false, false, false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 1),
+            Order::create_mask(&orders, 1, 1, false),
             [true, true, true, false, false, false, false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 2),
+            Order::create_mask(&orders, 1, 2, false),
             [true, true, true, false, false, false, true, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 1, 3),
+            Order::create_mask(&orders, 1, 3, false),
             [true, true, true, false, false, false, true, false, false, false, false, true]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 0),
+            Order::create_mask(&orders, 2, 0, false),
             [true, false, false, true, false, false, false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 1),
+            Order::create_mask(&orders, 2, 1, false),
             [true, true, true, true, false, false, false, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 2),
+            Order::create_mask(&orders, 2, 2, false),
             [true, true, true, true, true, true, true, false, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 2, 3),
+            Order::create_mask(&orders, 2, 3, false),
             [true, true, true, true, true, true, true, false, false, false, false, true]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 0),
+            Order::create_mask(&orders, 3, 0, false),
             [true, false, false, true, false, false, false, true, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 1),
+            Order::create_mask(&orders, 3, 1, false),
             [true, true, true, true, false, false, false, true, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 2),
+            Order::create_mask(&orders, 3, 2, false),
             [true, true, true, true, true, true, true, true, false, false, false, false]
         );
         assert_eq!(
-            Order::create_mask(&orders, 3, 3),
+            Order::create_mask(&orders, 3, 3, false),
             [true, true, true, true, true, true, true, true, true, true, true, true]
         );
     }
 
     #[test]
     fn grid_with_subgrid_type() {
         let subgrid_type = String::from("Idontexist");
@@ -2454,25 +2466,19 @@
         );
 
         grid.key_values_mut()
             .insert("initial_state_1".into(), "-2212".into());
         grid.set_key_value("initial_state_2", "-2212");
 
         assert_eq!(
-            grid.key_values()
-                .unwrap()
-                .get("initial_state_1".into())
-                .unwrap(),
+            grid.key_values().unwrap().get("initial_state_1").unwrap(),
             "-2212"
         );
         assert_eq!(
-            grid.key_values()
-                .unwrap()
-                .get("initial_state_2".into())
-                .unwrap(),
+            grid.key_values().unwrap().get("initial_state_2").unwrap(),
             "-2212"
         );
     }
 
     // TODO: properly test axes returned
 
     #[allow(deprecated)]
@@ -2549,18 +2555,18 @@
             muf2_0: 1.,
             alphas: vec![1.],
             xir: 1.,
             xif: 1.,
             target_x_grid: target_x_grid.clone(),
             target_pids: target_pids.clone(),
             grid_axes: GridAxes {
-                x_grid: axes.x_grid.clone(),
-                pids: axes.pids.clone(),
+                x_grid: axes.x_grid,
+                pids: axes.pids,
                 mur2_grid: axes.mur2_grid.clone(),
-                muf2_grid: axes.muf2_grid.clone(),
+                muf2_grid: axes.muf2_grid,
             },
             lumi_id_types,
         };
         let operator = ndarray::Array::from_shape_vec(
             (1, 3, 3, 3, 3),
             (0..4)
                 .map(|_| (0..3))
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/import_only_subgrid.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/import_only_subgrid.rs`

 * *Files 0% similar despite different names*

```diff
@@ -400,19 +400,18 @@
                     prev.0.start.min(imu2)..prev.0.end.max(imu2 + 1),
                     prev.1.start.min(ix1)..prev.1.end.max(ix1 + 1),
                     prev.2.start.min(ix2)..prev.2.end.max(ix2 + 1),
                 )
             },
         );
 
-        let (mu2_grid, static_scale) = if let Some(scale) = subgrid.static_scale() {
-            (vec![scale], true)
-        } else {
-            (subgrid.mu2_grid()[mu2_range.clone()].to_vec(), false)
-        };
+        let (mu2_grid, static_scale) = subgrid.static_scale().map_or_else(
+            || (subgrid.mu2_grid()[mu2_range.clone()].to_vec(), false),
+            |scale| (vec![scale], true),
+        );
         let x1_grid = subgrid.x1_grid()[x1_range.clone()].to_vec();
         let x2_grid = subgrid.x2_grid()[x2_range.clone()].to_vec();
 
         let mut array = SparseArray3::new(mu2_grid.len(), x1_grid.len(), x2_grid.len());
 
         for ((imu2, ix1, ix2), value) in subgrid.indexed_iter() {
             // if there's a static scale we want every value to be added to same grid point
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/lagrange_subgrid.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/lagrange_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/lumi.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/ntuple_subgrid.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/ntuple_subgrid.rs`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         assert_eq!(subgrid1.mu2_grid().as_ref(), []);
         assert_eq!(subgrid1.x1_grid().as_ref(), []);
         assert_eq!(subgrid1.x2_grid().as_ref(), []);
 
         subgrid1.symmetrize();
         subgrid1.scale(2.0);
 
-        let mut subgrid2: SubgridEnum = subgrid1.clone_empty().into();
+        let mut subgrid2: SubgridEnum = subgrid1.clone_empty();
 
         subgrid2.fill(&Ntuple {
             x1: 0.0,
             x2: 0.0,
             q2: 0.0,
             weight: 1.0,
         });
```

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/pids.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/pids.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/sparse_array3.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/sparse_array3.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/src/subgrid.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/src/subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/local_dependencies/pineappl/tests/drell_yan_lo.rs` & `pineappl-0.6.0a6/local_dependencies/pineappl/tests/drell_yan_lo.rs`

 * *Files 14% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 }
 
 fn fill_drell_yan_lo_grid(
     rng: &mut impl Rng,
     calls: usize,
     subgrid_type: &str,
     dynamic: bool,
+    reweight: bool,
 ) -> Result<Grid> {
     let lumi = vec![
         // photons
         lumi_entry![22, 22, 1.0],
     ];
 
     // only LO alpha^2
@@ -91,24 +92,24 @@
     let mut subgrid_params = SubgridParams::default();
     let mut extra = ExtraSubgridParams::default();
 
     subgrid_params.set_q2_bins(30);
     subgrid_params.set_q2_max(1e6);
     subgrid_params.set_q2_min(1e2);
     subgrid_params.set_q2_order(3);
-    subgrid_params.set_reweight(true);
+    subgrid_params.set_reweight(reweight);
     subgrid_params.set_x_bins(50);
     subgrid_params.set_x_max(1.0);
     subgrid_params.set_x_min(2e-7);
     subgrid_params.set_x_order(3);
     extra.set_x2_bins(50);
     extra.set_x2_max(1.0);
     extra.set_x2_min(2e-7);
     extra.set_x2_order(3);
-    extra.set_reweight2(true);
+    extra.set_reweight2(reweight);
 
     // create the PineAPPL grid
     let mut grid = Grid::with_subgrid_type(
         lumi,
         orders,
         bin_limits,
         subgrid_params,
@@ -139,16 +140,15 @@
         jacobian *= hbarc2 / (calls as f64);
 
         // cuts for LO for the invariant-mass slice containing the Z-peak from CMSDY2D11
         if (ptl < 14.0)
             || (yll.abs() > 2.4)
             || (ylp > 2.4)
             || (ylm > 2.4)
-            || (mll < 60.0)
-            || (mll > 120.0)
+            || !(60.0..=120.0).contains(&mll)
         {
             continue;
         }
 
         let weight = jacobian * int_photo(s, u, t);
         let q2 = if dynamic { mll * mll } else { 90.0 * 90.0 };
 
@@ -160,35 +160,37 @@
 
 fn perform_grid_tests(
     subgrid_type: &str,
     dynamic: bool,
     reference: &[f64],
     reference_after_ssd: &[f64],
     x_grid: &[f64],
+    reweight: bool,
 ) -> Result<()> {
     let mut rng = Pcg64::new(0xcafef00dd15ea5e5, 0xa02bdbf7bb3c0a7ac28fa16a64abf96);
-    let mut grid = fill_drell_yan_lo_grid(&mut rng, 500_000, subgrid_type, dynamic)?;
+    let mut grid = fill_drell_yan_lo_grid(&mut rng, 500_000, subgrid_type, dynamic, reweight)?;
 
     // TEST 1: `merge` and `scale`
     grid.merge(fill_drell_yan_lo_grid(
         &mut rng,
         500_000,
         subgrid_type,
         dynamic,
+        reweight,
     )?)?;
     grid.scale(0.5);
 
     // suppress LHAPDF banners
     lhapdf::set_verbosity(0);
 
     let pdf_set = "NNPDF31_nlo_as_0118_luxqed";
 
-    assert!(lhapdf::available_pdf_sets().iter().any(|x| x == &pdf_set));
+    assert!(lhapdf::available_pdf_sets().iter().any(|x| x == pdf_set));
 
-    let pdf = Pdf::with_setname_and_member(&pdf_set, 0)?;
+    let pdf = Pdf::with_setname_and_member(pdf_set, 0)?;
     let mut xfx = |id, x, q2| pdf.xfx_q2(id, x, q2);
     let mut alphas = |_| 0.0;
 
     // TEST 2: `read` and `write`
     let mut file = Cursor::new(Vec::new());
     grid.write(&mut file)?;
     file.set_position(0);
@@ -418,14 +420,41 @@
     6.385631160399488e-2,
     4.866968827833745e-2,
     3.379282482821324e-2,
     1.9494720220040448e-2,
     6.880478270711603e-3,
 ];
 
+const DYNAMIC_REFERENCE_NO_REWEIGHT: [f64; 24] = [
+    5.07858012983822e-1,
+    5.175284452774326e-1,
+    5.450720052517568e-1,
+    4.831265401289246e-1,
+    4.714770822390454e-1,
+    4.7332381643255367e-1,
+    4.6911980551007526e-1,
+    4.274224757508723e-1,
+    4.2874742764343926e-1,
+    3.898631579204727e-1,
+    3.419807843167341e-1,
+    3.112011822819245e-1,
+    2.6582805074531396e-1,
+    2.3669405399362703e-1,
+    1.999186753344747e-1,
+    1.6877228654478332e-1,
+    1.4593203448521183e-1,
+    1.1312893772255903e-1,
+    8.906983809157609e-2,
+    6.368194887638147e-2,
+    4.852988118458943e-2,
+    3.369252022300261e-2,
+    1.943724748356927e-2,
+    6.8603903480790075e-3,
+];
+
 #[test]
 fn dy_aa_lagrange_static() -> Result<()> {
     perform_grid_tests(
         "LagrangeSubgrid",
         false,
         &STATIC_REFERENCE,
         &STATIC_REFERENCE_AFTER_SSD,
@@ -433,28 +462,36 @@
             0.030521584007828916,
             0.02108918668378717,
             0.014375068581090129,
             0.009699159574043398,
             0.006496206194633799,
             0.004328500638820811,
         ],
+        true,
     )
 }
 
-// TODO: fix unexpected loss of precision after `optimize` in `dy_aa_lagrange_v1_static`
-
-//#[test]
-//fn dy_aa_lagrange_v1_static() -> Result<()> {
-//    perform_grid_tests(
-//        "LagrangeSubgridV1",
-//        false,
-//        &STATIC_REFERENCE,
-//        &STATIC_REFERENCE_AFTER_SSD,
-//    )
-//}
+#[test]
+fn dy_aa_lagrange_v1_static() -> Result<()> {
+    perform_grid_tests(
+        "LagrangeSubgridV1",
+        false,
+        &STATIC_REFERENCE,
+        &STATIC_REFERENCE, // LagrangeSubgridV1 doesn't have static-scale detection
+        &[
+            0.030521584007828916,
+            0.02108918668378717,
+            0.014375068581090129,
+            0.009699159574043398,
+            0.006496206194633799,
+            0.004328500638820811,
+        ],
+        true,
+    )
+}
 
 #[test]
 fn dy_aa_lagrange_v2_static() -> Result<()> {
     perform_grid_tests(
         "LagrangeSubgridV2",
         false,
         &STATIC_REFERENCE,
@@ -463,14 +500,15 @@
             0.030521584007828916,
             0.02108918668378717,
             0.014375068581090129,
             0.009699159574043398,
             0.006496206194633799,
             0.004328500638820811,
         ],
+        true,
     )
 }
 
 #[test]
 fn dy_aa_lagrange_dynamic() -> Result<()> {
     perform_grid_tests(
         "LagrangeSubgrid",
@@ -481,14 +519,15 @@
             0.030521584007828916,
             0.02108918668378717,
             0.014375068581090129,
             0.009699159574043398,
             0.006496206194633799,
             0.004328500638820811,
         ],
+        true,
     )
 }
 
 #[test]
 fn dy_aa_lagrange_v1_dynamic() -> Result<()> {
     perform_grid_tests(
         "LagrangeSubgridV1",
@@ -499,14 +538,34 @@
             0.030521584007828916,
             0.02108918668378717,
             0.014375068581090129,
             0.009699159574043398,
             0.006496206194633799,
             0.004328500638820811,
         ],
+        true,
+    )
+}
+
+#[test]
+fn dy_aa_lagrange_v1_dynamic_no_reweight() -> Result<()> {
+    perform_grid_tests(
+        "LagrangeSubgridV1",
+        true,
+        &DYNAMIC_REFERENCE_NO_REWEIGHT,
+        &DYNAMIC_REFERENCE_NO_REWEIGHT,
+        &[
+            0.030521584007828916,
+            0.02108918668378717,
+            0.014375068581090129,
+            0.009699159574043398,
+            0.006496206194633799,
+            0.004328500638820811,
+        ],
+        false,
     )
 }
 
 #[test]
 fn dy_aa_lagrange_v2_dynamic() -> Result<()> {
     perform_grid_tests(
         "LagrangeSubgridV2",
@@ -517,14 +576,34 @@
             0.030521584007828916,
             0.02108918668378717,
             0.014375068581090129,
             0.009699159574043398,
             0.006496206194633799,
             0.004328500638820811,
         ],
+        true,
+    )
+}
+
+#[test]
+fn dy_aa_lagrange_v2_dynamic_no_reweight() -> Result<()> {
+    perform_grid_tests(
+        "LagrangeSubgridV2",
+        true,
+        &DYNAMIC_REFERENCE_NO_REWEIGHT,
+        &DYNAMIC_REFERENCE_NO_REWEIGHT,
+        &[
+            0.030521584007828916,
+            0.02108918668378717,
+            0.014375068581090129,
+            0.009699159574043398,
+            0.006496206194633799,
+            0.004328500638820811,
+        ],
+        false,
     )
 }
 
 #[test]
 fn dy_aa_lagrange_sparse_dynamic() -> Result<()> {
     perform_grid_tests(
         "LagrangeSparseSubgrid",
@@ -535,9 +614,10 @@
             0.030521584007828916,
             0.02108918668378717,
             0.014375068581090129,
             0.009699159574043398,
             0.006496206194633799,
             0.004328500638820811,
         ],
+        true,
     )
 }
```

### Comparing `pineappl-0.6.0a5/Cargo.toml` & `pineappl-0.6.0a6/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 categories= ["science"]
 edition= "2021"
 keywords= ["high-energy-physics", "physics"]
 license= "GPL-3.0-or-later"
 repository= "https://github.com/NNPDF/pineappl"
 rust-version= "1.64.0"
-version= "0.6.0-alpha.5"
+version= "0.6.0-alpha.6"
 
 [package.metadata.maturin]
 name = "pineappl"
 
 [lib]
 name = "pineappl"
 crate-type = ["cdylib"]
 
 [dependencies]
 itertools = "0.10.1"
 ndarray = "0.15.4"
 numpy = "0.16.2"
-pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.5" }
+pineappl = { path = "local_dependencies/pineappl", version = "0.6.0-alpha.6" }
 pyo3 = { features = ["extension-module"], version = "0.16.4" }
```

### Comparing `pineappl-0.6.0a5/README.md` & `pineappl-0.6.0a6/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/Makefile` & `pineappl-0.6.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/make.bat` & `pineappl-0.6.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/source/conf.py` & `pineappl-0.6.0a6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/source/implementation.rst` & `pineappl-0.6.0a6/docs/source/implementation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/source/index.rst` & `pineappl-0.6.0a6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/source/installation.rst` & `pineappl-0.6.0a6/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/source/recipes.rst` & `pineappl-0.6.0a6/docs/source/recipes.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/docs/source/shared/roles.rst` & `pineappl-0.6.0a6/docs/source/shared/roles.rst`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/package/Containerfile` & `pineappl-0.6.0a6/package/Containerfile`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/package/README.md` & `pineappl-0.6.0a6/package/README.md`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/pineappl/bin.py` & `pineappl-0.6.0a6/pineappl/bin.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/pineappl/fk_table.py` & `pineappl-0.6.0a6/pineappl/fk_table.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/pineappl/grid.py` & `pineappl-0.6.0a6/pineappl/grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/pineappl/import_only_subgrid.py` & `pineappl-0.6.0a6/pineappl/import_only_subgrid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/pyproject.toml` & `pineappl-0.6.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/bin.rs` & `pineappl-0.6.0a6/src/bin.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/evolution.rs` & `pineappl-0.6.0a6/src/evolution.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/fk_table.rs` & `pineappl-0.6.0a6/src/fk_table.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/grid.rs` & `pineappl-0.6.0a6/src/grid.rs`

 * *Files 1% similar despite different names*

```diff
@@ -78,20 +78,22 @@
     /// numpy.ndarray(bool)
     ///     boolean array, to be used as orders' mask
     #[staticmethod]
     pub fn create_mask<'py>(
         orders: Vec<PyRef<Self>>,
         max_as: u32,
         max_al: u32,
+        logs: bool,
         py: Python<'py>,
     ) -> &'py PyArray1<bool> {
         Order::create_mask(
             &orders.iter().map(|o| o.order.clone()).collect::<Vec<_>>(),
             max_as,
             max_al,
+            logs,
         )
         .into_pyarray(py)
     }
 }
 
 /// PyO3 wrapper to :rustdoc:`pineappl::grid::Grid <grid/struct.Grid.html>`
 ///
```

### Comparing `pineappl-0.6.0a5/src/import_only_subgrid.rs` & `pineappl-0.6.0a6/src/import_only_subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/lib.rs` & `pineappl-0.6.0a6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/lumi.rs` & `pineappl-0.6.0a6/src/lumi.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/src/subgrid.rs` & `pineappl-0.6.0a6/src/subgrid.rs`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/tests/test_grid.py` & `pineappl-0.6.0a6/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/tests/test_sugrid.py` & `pineappl-0.6.0a6/tests/test_sugrid.py`

 * *Files identical despite different names*

### Comparing `pineappl-0.6.0a5/Cargo.lock` & `pineappl-0.6.0a6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
  "once_cell",
  "pest",
  "sha1",
 ]
 
 [[package]]
 name = "pineappl"
-version = "0.6.0-alpha.5"
+version = "0.6.0-alpha.6"
 dependencies = [
  "anyhow",
  "arrayvec",
  "bincode",
  "enum_dispatch",
  "float-cmp",
  "git-version",
@@ -995,38 +995,39 @@
  "serde",
  "serde_yaml",
  "thiserror",
 ]
 
 [[package]]
 name = "pineappl_applgrid"
-version = "0.6.0-alpha.5"
+version = "0.6.0-alpha.6"
 dependencies = [
  "cc",
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_capi"
-version = "0.6.0-alpha.5"
+version = "0.6.0-alpha.6"
 dependencies = [
  "itertools",
  "pineappl",
 ]
 
 [[package]]
 name = "pineappl_cli"
-version = "0.6.0-alpha.5"
+version = "0.6.0-alpha.6"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "assert_fs",
  "clap",
  "clap_mangen",
+ "cxx",
  "enum_dispatch",
  "flate2",
  "float-cmp",
  "git-version",
  "itertools",
  "lhapdf",
  "libc",
@@ -1042,23 +1043,23 @@
  "serde",
  "serde_yaml",
  "tar",
 ]
 
 [[package]]
 name = "pineappl_fastnlo"
-version = "0.6.0-alpha.5"
+version = "0.6.0-alpha.6"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "pineappl_py"
-version = "0.6.0-alpha.5"
+version = "0.6.0-alpha.6"
 dependencies = [
  "itertools",
  "ndarray",
  "numpy",
  "pineappl",
  "pyo3",
 ]
```

### Comparing `pineappl-0.6.0a5/PKG-INFO` & `pineappl-0.6.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pineappl
-Version: 0.6.0a5
+Version: 0.6.0a6
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: numpy>=1.16.0,<2.0.0
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx_rtd_theme; extra == 'docs'
 Requires-Dist: sphinxcontrib-bibtex; extra == 'docs'
 Requires-Dist: nbsphinx; extra == 'docs'
-Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-cov; extra == 'test'
-Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: docs
 Summary: Python bindings to PineAPPL
 Keywords: high-energy-physics,physics
 Author: Christopher Schwan <handgranaten-herbert@posteo.de>, Alessandro Candido <candido.ale@gmail.com>, Felix Hekhorn <felix.hekhorn@mi.infn.it>
 Author-email: Christopher Schwan <handgranaten-herbert@posteo.de>, Alessandro Candido <candido.ale@gmail.com>, Felix Hekhorn <felix.hekhorn@mi.infn.it>
 License: GPL-3.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://n3pdf.github.io/pineappl/
 Project-URL: documentation, https://pineappl.readthedocs.io/
 Project-URL: changelog, https://github.com/NNPDF/pineappl/blob/master/CHANGELOG.md
-Project-URL: homepage, https://n3pdf.github.io/pineappl/
 
 [![PyPI version](https://badge.fury.io/py/pineappl.svg)](https://badge.fury.io/py/pineappl)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pineappl/badges/installer/conda.svg)](https://anaconda.org/conda-forge/pineappl)
 [![AUR](https://img.shields.io/aur/version/pineappl)](https://aur.archlinux.org/packages/pineappl)
 [![Documentation Status](https://readthedocs.org/projects/pineappl/badge/?version=latest)](https://pineappl.readthedocs.io/en/latest/?badge=latest)
 
 # Python bindings for PineAPPL
```

