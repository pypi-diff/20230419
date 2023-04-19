# Comparing `tmp/lezargus-0.0.1.dev0.tar.gz` & `tmp/lezargus-0.0.1.dev1.tar.gz`

## Comparing `lezargus-0.0.1.dev0.tar` & `lezargus-0.0.1.dev1.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/SECURITY.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/workspace.code-workspace
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/src/lezargus/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/src/lezargus/__version__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/tests/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/LICENSE.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/README.md
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/SECURITY.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/workspace.code-workspace
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/make.bat
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/source/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/docs/source/index.rst
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/src/lezargus/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/src/lezargus/__version__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/tests/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/tests/test_global.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/LICENSE.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/README.md
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 lezargus-0.0.1.dev1/PKG-INFO
```

### Comparing `lezargus-0.0.1.dev0/SECURITY.md` & `lezargus-0.0.1.dev1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev0/.gitignore` & `lezargus-0.0.1.dev1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -64,16 +64,14 @@
 # Flask stuff:
 instance/
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
-# Sphinx documentation
-docs/_build/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
@@ -121,9 +119,12 @@
 /site
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
+# ruff
+.ruff_cache/
+
 # Pyre type checker
 .pyre/
```

### Comparing `lezargus-0.0.1.dev0/LICENSE.txt` & `lezargus-0.0.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lezargus-0.0.1.dev0/pyproject.toml` & `lezargus-0.0.1.dev1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "Lezargus"
+name = "lezargus"
 dynamic = ["version"]
 description = "The accompanying data software package to the IRTF SPECTRE Spectrograph."
 readme = "README.md"
 requires-python = ">=3.11"
 license = "MIT"
 keywords = []
 authors = [
@@ -28,121 +28,100 @@
 Source = "https://github.com/psmd-iberutaru/Lezargus/Lezargus"
 
 [tool.hatch.version]
 path = "src/lezargus/__version__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
+  "lezargus",
   "coverage[toml]>=6.5",
-  "pytest",
+  "pytest>=7.3.0",
+  "black>=23.1.0",
+  "mypy>=1.0.0",
+  "pylint>=2.17.0",
+  "ruff>=0.0.261"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
-test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
+typing = "mypy --install-types --non-interactive {args:src/lezargus tests}"
+format = [
+  "black {args:.}",
+]
+cover = [
+  "coverage run -m pytest {args:tests}",
   "- coverage combine",
   "coverage report",
 ]
-cov = [
-  "test-cov",
-  "cov-report",
-]
-
-[[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
-
-[tool.hatch.envs.lint]
-detached = true
-dependencies = [
-  "black>=23.1.0",
-  "mypy>=1.0.0",
-  "ruff>=0.0.243",
-]
-[tool.hatch.envs.lint.scripts]
-typing = "mypy --install-types --non-interactive {args:src/lezargus tests}"
-style = [
-  "ruff {args:.}",
-  "black --check --diff {args:.}",
+lint = [
+  "ruff {args:src}",
+  "pylint {args:src}",
 ]
-fmt = [
-  "black {args:.}",
-  "ruff --fix {args:.}",
-  "style",
+lintfix = [
+  "ruff {args:src} --fix"
 ]
-all = [
-  "style",
+auxiliary = [
   "typing",
+  "lint",
+  "lintfix",
+  "test",
+  "cover",
+  "format",
 ]
 
+
+[[tool.hatch.envs.all.matrix]]
+python = ["3.11"]
+
 [tool.black]
-target-version = ["py37"]
-line-length = 120
-skip-string-normalization = true
+target-version = ["py311"]
+line-length = 80
 
 [tool.ruff]
-target-version = "py37"
-line-length = 120
+target-version = "py311"
+line-length = 80
 select = [
-  "A",
-  "ARG",
-  "B",
-  "C",
-  "DTZ",
-  "E",
-  "EM",
-  "F",
-  "FBT",
-  "I",
-  "ICN",
-  "ISC",
-  "N",
-  "PLC",
-  "PLE",
-  "PLR",
-  "PLW",
-  "Q",
-  "RUF",
-  "S",
-  "T",
-  "TID",
-  "UP",
-  "W",
-  "YTT",
+  "ALL",
 ]
 ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
-  # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+  # Incompatabilies; these are objectively wrong.
+  "D203", "D213"
 ]
 unfixable = [
-  # Don't touch unused imports
-  "F401",
 ]
 
 [tool.ruff.isort]
-known-first-party = ["lezargus"]
+known-third-party = ["lezargus"]
+force-single-line = true
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
+[tool.pylint]
+disable = [
+  "R0903", # (too-few-public-methods)
+  "R0913", # (too-many-arguments)
+  "W0105", # (pointless-string-statement)
+]
+
 [tool.coverage.run]
 source_pkgs = ["lezargus", "tests"]
 branch = true
 parallel = true
 omit = [
-  "src/lezargus/__about__.py",
+  "src/lezargus/__version__.py",
 ]
 
 [tool.coverage.paths]
 lezargus = ["src/lezargus", "*/lezargus/src/lezargus"]
 tests = ["tests", "*/lezargus/tests"]
 
 [tool.coverage.report]
```

### Comparing `lezargus-0.0.1.dev0/PKG-INFO` & `lezargus-0.0.1.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Lezargus
-Version: 0.0.1.dev0
+Name: lezargus
+Version: 0.0.1.dev1
 Summary: The accompanying data software package to the IRTF SPECTRE Spectrograph.
 Project-URL: Documentation, https://github.com/psmd-iberutaru/Lezargus/Lezargus#readme
 Project-URL: Issues, https://github.com/psmd-iberutaru/Lezargus/Lezargus/issues
 Project-URL: Source, https://github.com/psmd-iberutaru/Lezargus/Lezargus
 Author-email: Sparrow <psmd.iberutaru@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

