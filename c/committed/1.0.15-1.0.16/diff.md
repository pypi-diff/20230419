# Comparing `tmp/committed-1.0.15.tar.gz` & `tmp/committed-1.0.16.tar.gz`

## Comparing `committed-1.0.15.tar` & `committed-1.0.16.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.15/pyproject.toml
--rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 committed-1.0.15/rust_src/committed/Cargo.toml
--rw-r--r--   0     1001      123     9680 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/checks.rs
--rw-r--r--   0     1001      123     1414 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/color.rs
--rw-r--r--   0     1001      123     4614 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/config.rs
--rw-r--r--   0     1001      123      461 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/conventional.rs
--rw-r--r--   0     1001      123     1914 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/git.rs
--rw-r--r--   0     1001      123      109 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/lib.rs
--rw-r--r--   0     1001      123    13085 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/main.rs
--rw-r--r--   0     1001      123     1764 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/no_style.rs
--rw-r--r--   0     1001      123     5273 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/report.rs
--rw-r--r--   0     1001      123      198 2023-04-13 16:04:16.000000 committed-1.0.15/rust_src/committed/src/style.rs
--rw-r--r--   0     1001      123    30418 2023-04-13 16:04:16.000000 committed-1.0.15/Cargo.lock
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.15/PKG-INFO
+-rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 committed-1.0.16/pyproject.toml
+-rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 committed-1.0.16/rust_src/committed/Cargo.toml
+-rw-r--r--   0     1001      123     9680 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/checks.rs
+-rw-r--r--   0     1001      123     1414 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/color.rs
+-rw-r--r--   0     1001      123     4614 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/config.rs
+-rw-r--r--   0     1001      123      461 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/conventional.rs
+-rw-r--r--   0     1001      123     1914 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/git.rs
+-rw-r--r--   0     1001      123      109 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/lib.rs
+-rw-r--r--   0     1001      123    13075 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/main.rs
+-rw-r--r--   0     1001      123     1764 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/no_style.rs
+-rw-r--r--   0     1001      123     5273 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/report.rs
+-rw-r--r--   0     1001      123      198 2023-04-19 13:42:26.000000 committed-1.0.16/rust_src/committed/src/style.rs
+-rw-r--r--   0     1001      123    29692 2023-04-19 13:42:26.000000 committed-1.0.16/Cargo.lock
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 committed-1.0.16/PKG-INFO
```

### Comparing `committed-1.0.15/rust_src/committed/Cargo.toml` & `committed-1.0.16/rust_src/committed/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "committed"
-version = "1.0.15"
+version = "1.0.16"
 description = "Nitpicking commit history since beabf39"
 documentation = "https://docs.rs/committed"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/committed"
@@ -45,16 +45,15 @@
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 toml = "0.7"
 unicode-segmentation = "1.10.1"
 log = "0.4"
 env_logger = "0.10"
 clap-verbosity-flag = "2.0"
-concolor = { version = "0.1.1" }
-concolor-clap = { version = "0.1.0", features = ["api"] }
+colorchoice-clap = "1.0.0"
 grep-cli = "0.1"
 imperative = "1.0.4"
 derive_more = "0.99.17"
 itertools = "0.10.5"
 proc-exit = "2.0"
 human-panic = "1.1.3"
 anstream = "0.3.0"
```

### Comparing `committed-1.0.15/rust_src/committed/src/checks.rs` & `committed-1.0.16/rust_src/committed/src/checks.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.15/rust_src/committed/src/color.rs` & `committed-1.0.16/rust_src/committed/src/color.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.15/rust_src/committed/src/config.rs` & `committed-1.0.16/rust_src/committed/src/config.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.15/rust_src/committed/src/git.rs` & `committed-1.0.16/rust_src/committed/src/git.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.15/rust_src/committed/src/main.rs` & `committed-1.0.16/rust_src/committed/src/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,15 @@
 mod config;
 mod git;
 mod report;
 
 const UNKNOWN_ERR: proc_exit::Code = proc_exit::Code::new(2);
 
 #[derive(Debug, Parser)]
-#[command(
-    about,
-    version,
-    color = concolor_clap::color_choice(),
-)]
+#[command(about, version)]
 #[command(group = clap::ArgGroup::new("mode").multiple(false))]
 struct Options {
     #[arg(group = "mode")]
     commits: Option<String>,
 
     #[arg(long, group = "mode")]
     /// Check a message in a file with `-` for stdin
@@ -60,15 +56,15 @@
         value_enum,
         ignore_case(true),
         default_value = "brief"
     )]
     format: Format,
 
     #[command(flatten)]
-    color: concolor_clap::Color,
+    color: colorchoice_clap::Color,
 
     #[command(flatten)]
     verbose: clap_verbosity_flag::Verbosity,
 }
 
 impl Options {
     fn to_config(&self) -> config::Config {
@@ -132,19 +128,19 @@
     toml::from_str(&text).map_err(|e| e.into())
 }
 
 fn init_logging(level: Option<log::Level>) {
     if let Some(level) = level {
         let mut builder = env_logger::Builder::new();
 
-        let colored = concolor::get(concolor::Stream::Stderr).ansi_color();
-        builder.write_style(if colored {
-            env_logger::WriteStyle::Always
-        } else {
+        let choice = anstream::AutoStream::choice(&std::io::stderr());
+        builder.write_style(if matches!(choice, anstream::ColorChoice::Never) {
             env_logger::WriteStyle::Never
+        } else {
+            env_logger::WriteStyle::Always
         });
 
         builder.filter(None, level.to_level_filter());
 
         if level == log::LevelFilter::Trace {
             builder.format_timestamp_secs();
         } else {
@@ -161,15 +157,15 @@
         builder.init();
     }
 }
 
 fn run() -> proc_exit::ExitResult {
     let options = Options::parse();
 
-    options.color.apply();
+    options.color.write_global();
 
     init_logging(options.verbose.log_level());
 
     let repo = options
         .work_tree
         .canonicalize()
         .with_code(proc_exit::sysexits::USAGE_ERR)?;
```

### Comparing `committed-1.0.15/rust_src/committed/src/no_style.rs` & `committed-1.0.16/rust_src/committed/src/no_style.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.15/rust_src/committed/src/report.rs` & `committed-1.0.16/rust_src/committed/src/report.rs`

 * *Files identical despite different names*

### Comparing `committed-1.0.15/Cargo.lock` & `committed-1.0.16/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -201,24 +201,33 @@
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
+name = "colorchoice-clap"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "412e88a3a3a3f52e436909b49beb467a05649e8b0dda0e6202bd05c1b63dbc49"
+dependencies = [
+ "clap",
+ "colorchoice",
+]
+
+[[package]]
 name = "committed"
-version = "1.0.15"
+version = "1.0.16"
 dependencies = [
  "anstream",
  "anstyle",
  "anyhow",
  "clap",
  "clap-verbosity-flag",
- "concolor",
- "concolor-clap",
+ "colorchoice-clap",
  "derive_more",
  "env_logger",
  "git-conventional",
  "git2",
  "grep-cli",
  "human-panic",
  "imperative",
@@ -231,51 +240,14 @@
  "serde_json",
  "toml",
  "unicase",
  "unicode-segmentation",
 ]
 
 [[package]]
-name = "concolor"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b946244a988c390a94667ae0e3958411fa40cc46ea496a929b263d883f5f9c3"
-dependencies = [
- "bitflags",
- "concolor-override",
- "concolor-query",
- "is-terminal",
-]
-
-[[package]]
-name = "concolor-clap"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435ff0007a3bb04099fe1beedc6b76e7dd5340c90b168008ac0d7e87441de1bf"
-dependencies = [
- "clap",
- "concolor",
-]
-
-[[package]]
-name = "concolor-override"
-version = "1.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a855d4a1978dc52fb0536a04d384c2c0c1aa273597f08b77c8c4d3b2eec6037f"
-
-[[package]]
-name = "concolor-query"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b20c6ac2524cb0ddc8ceac2368f2208399dad8fa31175f14b08ae28b9d07766"
-dependencies = [
- "windows-sys 0.45.0",
-]
-
-[[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
 name = "derive_more"
```

### Comparing `committed-1.0.15/PKG-INFO` & `committed-1.0.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: committed
-Version: 1.0.15
+Version: 1.0.16
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
-    rev: v1.0.15
+    rev: v1.0.16
     hooks:
       - id: committed
 ```
 
 The `committed` id installs a prebuilt executable from GitHub releases. If
 one does not exist for the target platform, or if one built from
 sources is preferred, use `committed-src` as the hook id instead.
```

