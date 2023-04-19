# Comparing `tmp/committed-1.0.16.tar.gz` & `tmp/committed-1.0.17.tar.gz`

## Comparing `committed-1.0.16.tar` & `committed-1.0.17.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.16/pyproject.toml
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 committed-1.0.16/rust_src/committed/Cargo.toml
--rw-r--r--   0     1001      123     9680 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/checks.rs
--rw-r--r--   0     1001      123     1414 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/color.rs
--rw-r--r--   0     1001      123     4614 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/config.rs
--rw-r--r--   0     1001      123      461 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/conventional.rs
--rw-r--r--   0     1001      123     1914 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/git.rs
--rw-r--r--   0     1001      123      109 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/lib.rs
--rw-r--r--   0     1001      123    13075 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/main.rs
--rw-r--r--   0     1001      123     1764 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/no_style.rs
--rw-r--r--   0     1001      123     5273 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/report.rs
--rw-r--r--   0     1001      123      198 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/style.rs
--rw-r--r--   0     1001      123    29692 2023-04-19 13:42:26.000000 committed-1.0.16/Cargo.lock
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.16/PKG-INFO
+-rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.17/pyproject.toml
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 committed-1.0.17/rust_src/committed/Cargo.toml
+-rw-r--r--   0     1001      123     9680 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/checks.rs
+-rw-r--r--   0     1001      123     1414 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/color.rs
+-rw-r--r--   0     1001      123     4614 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/config.rs
+-rw-r--r--   0     1001      123      461 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/conventional.rs
+-rw-r--r--   0     1001      123     1914 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/git.rs
+-rw-r--r--   0     1001      123      109 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/lib.rs
+-rw-r--r--   0     1001      123    13075 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/main.rs
+-rw-r--r--   0     1001      123     1764 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/no_style.rs
+-rw-r--r--   0     1001      123     5273 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/report.rs
+-rw-r--r--   0     1001      123      198 2023-04-19 14:46:47.000000 committed-1.0.17/rust_src/committed/src/style.rs
+-rw-r--r--   0     1001      123    29692 2023-04-19 14:46:47.000000 committed-1.0.17/Cargo.lock
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.17/PKG-INFO
```

### Comparing `committed-1.0.16/rust_src/committed/Cargo.toml` & `committed-1.0.17/rust_src/committed/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "committed"
-version = "1.0.16"
+version = "1.0.17"
 description = "Nitpicking commit history since beabf39"
 documentation = "https://docs.rs/committed"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/committed"
```

### Comparing `committed-1.0.16/rust_src/committed/src/checks.rs` & `committed-1.0.17/rust_src/committed/src/checks.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/rust_src/committed/src/color.rs` & `committed-1.0.17/rust_src/committed/src/color.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/rust_src/committed/src/config.rs` & `committed-1.0.17/rust_src/committed/src/config.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/rust_src/committed/src/git.rs` & `committed-1.0.17/rust_src/committed/src/git.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/rust_src/committed/src/main.rs` & `committed-1.0.17/rust_src/committed/src/main.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/rust_src/committed/src/no_style.rs` & `committed-1.0.17/rust_src/committed/src/no_style.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/rust_src/committed/src/report.rs` & `committed-1.0.17/rust_src/committed/src/report.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.16/Cargo.lock` & `committed-1.0.17/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 dependencies = [
  "clap",
  "colorchoice",
 ]
 
 [[package]]
 name = "committed"
-version = "1.0.16"
+version = "1.0.17"
 dependencies = [
  "anstream",
  "anstyle",
  "anyhow",
  "clap",
  "clap-verbosity-flag",
  "colorchoice-clap",
```

### Comparing `committed-1.0.16/PKG-INFO` & `committed-1.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: committed
-Version: 1.0.16
+Version: 1.0.17
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Nitpicking commit history since beabf39
 Keywords: development
@@ -41,15 +41,15 @@
 
 To use `committed` with [`pre-commit`](https://pre-commit.com), point its
 config at this repository:
 
 ```yaml
 repos:
   - repo: https://github.com/crate-ci/committed
-    rev: v1.0.16
+    rev: v1.0.17
     hooks:
       - id: committed
 ```
 
 The `committed` id installs a prebuilt executable from GitHub releases. If
 one does not exist for the target platform, or if one built from
 sources is preferred, use `committed-src` as the hook id instead.
```

