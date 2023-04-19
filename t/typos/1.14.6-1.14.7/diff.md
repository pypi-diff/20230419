# Comparing `tmp/typos-1.14.6.tar.gz` & `tmp/typos-1.14.7.tar.gz`

## Comparing `typos-1.14.6.tar` & `typos-1.14.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44797 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  5965618 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.14.6/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-04-13 16:36:45.000000 typos-1.14.6/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.14.6/pyproject.toml
--rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 typos-1.14.6/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12565 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21534 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32485 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5359 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-04-13 16:36:45.000000 typos-1.14.6/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123    51732 2023-04-13 16:36:44.000000 typos-1.14.6/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.14.6/PKG-INFO
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.14.7/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  5965618 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 typos-1.14.7/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.14.7/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.14.7/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.14.7/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44797 2023-04-19 13:37:00.000000 typos-1.14.7/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.14.7/pyproject.toml
+-rw-r--r--   0        0        0     3028 1970-01-01 00:00:00.000000 typos-1.14.7/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12565 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21534 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32485 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     5359 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-04-19 13:37:00.000000 typos-1.14.7/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123    51732 2023-04-19 13:37:00.000000 typos-1.14.7/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.14.7/PKG-INFO
```

### Comparing `typos-1.14.6/local_dependencies/typos/Cargo.toml` & `typos-1.14.7/local_dependencies/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos/src/check.rs` & `typos-1.14.7/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos/src/dict.rs` & `typos-1.14.7/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos/src/tokens.rs` & `typos-1.14.7/local_dependencies/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/dictgen/Cargo.toml` & `typos-1.14.7/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/dictgen/src/map.rs` & `typos-1.14.7/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/dictgen/src/table.rs` & `typos-1.14.7/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/dictgen/src/trie.rs` & `typos-1.14.7/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos-dict/Cargo.toml` & `typos-1.14.7/local_dependencies/typos-dict/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.14.7/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos-vars/Cargo.toml` & `typos-1.14.7/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.14.7/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/varcon-core/Cargo.toml` & `typos-1.14.7/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.14.7/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/varcon-core/src/lib.rs` & `typos-1.14.7/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/local_dependencies/varcon-core/src/parser.rs` & `typos-1.14.7/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/Cargo.toml` & `typos-1.14.7/rust_src/typos-cli/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.14.6"
+version = "1.14.7"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.14.6/rust_src/typos-cli/benches/checks.rs` & `typos-1.14.7/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/benches/corrections.rs` & `typos-1.14.7/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/benches/data.rs` & `typos-1.14.7/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.14.7/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.14.7/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.14.7/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.14.7/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/config.rs` & `typos-1.14.7/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/default_types.rs` & `typos-1.14.7/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/dict.rs` & `typos-1.14.7/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/file.rs` & `typos-1.14.7/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/file_type.rs` & `typos-1.14.7/rust_src/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/policy.rs` & `typos-1.14.7/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/rust_src/typos-cli/src/report.rs` & `typos-1.14.7/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.14.6/Cargo.lock` & `typos-1.14.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1586,15 +1586,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.14.6"
+version = "1.14.7"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
```

### Comparing `typos-1.14.6/PKG-INFO` & `typos-1.14.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.14.6
+Version: 1.14.7
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

