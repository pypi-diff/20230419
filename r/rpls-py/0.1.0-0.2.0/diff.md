# Comparing `tmp/rpls_py-0.1.0.tar.gz` & `tmp/rpls_py-0.2.0.tar.gz`

## Comparing `rpls_py-0.1.0.tar` & `rpls_py-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 rpls_py-0.1.0/Cargo.toml
--rw-rw-r--   0     1000     1000     2905 2023-04-17 22:53:47.000000 rpls_py-0.1.0/.github/workflows/CI.yml
--rw-rw-r--   0     1000     1000      327 2023-04-17 19:52:01.000000 rpls_py-0.1.0/.gitignore
--rw-rw-r--   0     1000     1000        9 2023-04-17 18:22:01.000000 rpls_py-0.1.0/README.md
--rw-rw-r--   0     1000     1000      369 2023-04-17 18:23:20.000000 rpls_py-0.1.0/pyproject.toml
--rw-rw-r--   0     1000     1000      125 2023-04-17 19:51:20.000000 rpls_py-0.1.0/requirements.txt
--rw-rw-r--   0     1000     1000     1347 2023-04-17 22:53:25.000000 rpls_py-0.1.0/src/lib.rs
--rw-rw-r--   0     1000     1000    40625 2023-04-17 22:52:37.000000 rpls_py-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 rpls_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      294 1970-01-01 00:00:00.000000 rpls_py-0.2.0/Cargo.toml
+-rw-rw-r--   0     1000     1000     2905 2023-04-17 22:53:47.000000 rpls_py-0.2.0/.github/workflows/CI.yml
+-rw-rw-r--   0     1000     1000      327 2023-04-17 19:52:01.000000 rpls_py-0.2.0/.gitignore
+-rw-rw-r--   0     1000     1000        9 2023-04-17 18:22:01.000000 rpls_py-0.2.0/README.md
+-rw-rw-r--   0     1000     1000      369 2023-04-17 18:23:20.000000 rpls_py-0.2.0/pyproject.toml
+-rw-rw-r--   0     1000     1000      125 2023-04-17 19:51:20.000000 rpls_py-0.2.0/requirements.txt
+-rw-rw-r--   0     1000     1000     1453 2023-04-19 19:55:06.000000 rpls_py-0.2.0/src/lib.rs
+-rw-rw-r--   0     1000     1000    40625 2023-04-19 19:56:37.000000 rpls_py-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      335 1970-01-01 00:00:00.000000 rpls_py-0.2.0/PKG-INFO
```

### Comparing `rpls_py-0.1.0/.github/workflows/CI.yml` & `rpls_py-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rpls_py-0.1.0/src/lib.rs` & `rpls_py-0.2.0/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#![warn(
+     clippy::all,
+     clippy::pedantic,
+     clippy::nursery,
+     clippy::cargo,
+ )]
+
 use pyo3::prelude::*;
 use rpls;
 
 fn convert_bd_pairs(bd_pairs: Vec<(f32, f32)>) -> Vec<rpls::birthdeath::BirthDeath>{
     bd_pairs.into_iter().map(|pair| rpls::birthdeath::BirthDeath{birth: pair.0, death: pair.1}).collect()
 }
 
@@ -25,15 +32,15 @@
     Ok(convert_landscape(landscapes))
 
 }
 
 #[pyfunction]
 fn pairs_to_l2_norm(bd_pairs: Vec<(f32, f32)>, k: usize, debug: bool) -> PyResult<f32> {
     let bd_pairs = convert_bd_pairs(bd_pairs);
-    Ok(rpls::rpls::pairs_to_l2_norm(bd_pairs, k, debug))
+    Ok(rpls::rpls::pairs_to_l2_norm(bd_pairs, k, debug).unwrap())
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn rpls_py(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(pairs_to_landscape, m)?)?;
     m.add_function(wrap_pyfunction!(pairs_to_l2_norm, m)?)?;
```

### Comparing `rpls_py-0.1.0/Cargo.lock` & `rpls_py-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1020,27 +1020,27 @@
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5864e7ef1a6b7bcf1d6ca3f655e65e724ed3b52546a0d0a663c991522f552ea"
 
 [[package]]
 name = "rpls"
 version = "0.2.0"
-source = "git+https://github.com/tph5595/rpls.git#2fd282363a64d27202a74e4d762a991780efb990"
+source = "git+https://github.com/tph5595/rpls.git#98b683a3f8a733c44e9b28e7cd68f3a4f9c8b6c2"
 dependencies = [
  "clap",
  "csv",
  "float-ord 0.3.2",
  "geo",
  "geo-types",
  "plotters",
 ]
 
 [[package]]
 name = "rpls-py"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "rpls",
 ]
 
 [[package]]
 name = "rstar"
```

