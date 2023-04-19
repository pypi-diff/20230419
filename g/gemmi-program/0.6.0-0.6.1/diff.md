# Comparing `tmp/gemmi-program-0.6.0.tar.gz` & `tmp/gemmi-program-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmi-program-0.6.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "gemmi-program-0.6.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `gemmi-program-0.6.0.tar` & `gemmi-program-0.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1073 2022-11-09 12:37:21.000000 gemmi-program-0.6.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       15 2022-11-09 12:37:21.000000 gemmi-program-0.6.0/.gitignore
--rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 gemmi-program-0.6.0/CMakeLists.txt
--rw-r--r--   0        0        0      689 2022-11-09 12:37:21.000000 gemmi-program-0.6.0/README.md
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 gemmi-program-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1239 2022-11-09 12:37:21.000000 gemmi-program-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       15 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/.gitignore
+-rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/CMakeLists.txt
+-rw-r--r--   0        0        0      689 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/README.md
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1239 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/PKG-INFO
```

### Comparing `gemmi-program-0.6.0/.github/workflows/wheels.yml` & `gemmi-program-0.6.1/.github/workflows/wheels.yml`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,21 @@
       matrix:
         include:
           - os: ubuntu-22.04
             arch: "x86_64"
           - os: windows-2019
             arch: "AMD64"
           - os: macos-11
-            arch: "universal2"
+            arch: "x86_64 arm64"
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.12.0
+      uses: pypa/cibuildwheel@v2.12.2
       env:
         CIBW_BUILD: ${{ github.event.inputs.cibw_build }}
         CIBW_SKIP: ${{ github.event.inputs.cibw_skip }}
         CIBW_ARCHS: "${{ matrix.arch }}"
         # increase pip debugging output
         CIBW_BUILD_VERBOSITY: 1
```

### Comparing `gemmi-program-0.6.0/CMakeLists.txt` & `gemmi-program-0.6.1/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # and use this options when building:
 set(GEMMI_VERSION_INFO "from wheel")
 
 include(FetchContent)
 FetchContent_Declare(
   gemmi
   GIT_REPOSITORY https://github.com/project-gemmi/gemmi.git
-  GIT_TAG        73968c589112fbc769bb6716a298972b8ad2c3d7 # v0.6.0
+  GIT_TAG        7639b1f421207db15d76d1d5f7a813990a634633 # v0.6.1
 )
 
 # We don't want to install all gemmi files.
 # https://stackoverflow.com/questions/65527126/disable-install-for-fetchcontent
 FetchContent_GetProperties(gemmi)
 if (NOT gemmi_POPULATED)
   FetchContent_Populate(gemmi)
```

### Comparing `gemmi-program-0.6.0/README.md` & `gemmi-program-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `gemmi-program-0.6.0/pyproject.toml` & `gemmi-program-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["scikit-build-core>=0.2.1"]
+requires = ["scikit-build-core==0.2.1"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "gemmi-program"
-version = "0.6.0"
+version = "0.6.1"
 requires-python = ">=3.8"
 description="gemmi (program executable only)"
 readme = "README.md"
 authors = [{name="Marcin Wojdyr", email="wojdyr@gmail.com"}]
 urls.repository = "https://github.com/project-gemmi/gemmi_program_wheel"
 license = {text = "MPL-2.0"}  # or, at your option, LGPL-3.0
 classifiers = [
```

### Comparing `gemmi-program-0.6.0/PKG-INFO` & `gemmi-program-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemmi-program
-Version: 0.6.0
+Version: 0.6.1
 Summary: gemmi (program executable only)
 Author-Email: Marcin Wojdyr <wojdyr@gmail.com>
 License: MPL-2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

