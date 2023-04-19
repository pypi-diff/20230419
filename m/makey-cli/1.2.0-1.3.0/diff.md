# Comparing `tmp/makey-cli-1.2.0.tar.gz` & `tmp/makey-cli-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makey-cli-1.2.0.tar", last modified: Tue May  3 20:21:00 2022, max compression
+gzip compressed data, was "makey-cli-1.3.0.tar", last modified: Wed Apr 19 21:19:36 2023, max compression
```

## Comparing `makey-cli-1.2.0.tar` & `makey-cli-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-03 20:21:00.765100 makey-cli-1.2.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2022-05-03 20:20:18.000000 makey-cli-1.2.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2022-05-03 20:21:00.765100 makey-cli-1.2.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2022-05-03 20:20:18.000000 makey-cli-1.2.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-03 20:21:00.765100 makey-cli-1.2.0/makey/
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2022-05-03 20:20:18.000000 makey-cli-1.2.0/makey/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1332 2022-05-03 20:20:18.000000 makey-cli-1.2.0/makey/makey.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-03 20:21:00.765100 makey-cli-1.2.0/makey_cli.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2067 2022-05-03 20:21:00.000000 makey-cli-1.2.0/makey_cli.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      297 2022-05-03 20:21:00.000000 makey-cli-1.2.0/makey_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-05-03 20:21:00.000000 makey-cli-1.2.0/makey_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       42 2022-05-03 20:21:00.000000 makey-cli-1.2.0/makey_cli.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2022-05-03 20:21:00.000000 makey-cli-1.2.0/makey_cli.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2022-05-03 20:21:00.000000 makey-cli-1.2.0/makey_cli.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-05-03 20:21:00.765100 makey-cli-1.2.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1359 2022-05-03 20:20:18.000000 makey-cli-1.2.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-05-03 20:21:00.765100 makey-cli-1.2.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-05-03 20:20:18.000000 makey-cli-1.2.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1774 2022-05-03 20:20:18.000000 makey-cli-1.2.0/tests/test_makey.py
+-rw-r--r--   0        0        0       66 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.flake8
+-rw-r--r--   0        0        0     1193 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1090 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1303 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      338 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.gitignore
+-rw-r--r--   0        0        0      211 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     1408 2023-04-19 21:19:27.002957 makey-cli-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1071 2023-04-19 21:19:27.002957 makey-cli-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1764 2023-04-19 21:19:27.002957 makey-cli-1.3.0/README.md
+-rw-r--r--   0        0        0      249 2023-04-19 21:19:27.002957 makey-cli-1.3.0/codecov.yml
+-rw-r--r--   0        0        0        0 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/.nojekyll
+-rw-r--r--   0        0        0      121 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_404.md
+-rw-r--r--   0        0        0      363 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_coverpage.md
+-rw-r--r--   0        0        0     1068 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_homepage.md
+-rw-r--r--   0        0        0      265 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/_sidebar.md
+-rw-r--r--   0        0        0     1682 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/changelog.md
+-rw-r--r--   0        0        0     1830 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/index.html
+-rw-r--r--   0        0        0     1117 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/install.md
+-rw-r--r--   0        0        0      309 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/issues.md
+-rw-r--r--   0        0        0      402 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/styles.css
+-rw-r--r--   0        0        0     1082 2023-04-19 21:19:27.002957 makey-cli-1.3.0/docs/usage.md
+-rw-r--r--   0        0        0      907 2023-04-19 21:19:27.002957 makey-cli-1.3.0/justfile
+-rw-r--r--   0        0        0     1040 2023-04-19 21:19:27.002957 makey-cli-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-04-19 21:19:27.006957 makey-cli-1.3.0/src/makey/__init__.py
+-rw-r--r--   0        0        0     1364 2023-04-19 21:19:27.006957 makey-cli-1.3.0/src/makey/makey.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:19:27.006957 makey-cli-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1744 2023-04-19 21:19:27.006957 makey-cli-1.3.0/tests/test_makey.py
+-rw-r--r--   0        0        0     2737 1970-01-01 00:00:00.000000 makey-cli-1.3.0/PKG-INFO
```

### Comparing `makey-cli-1.2.0/LICENSE` & `makey-cli-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makey-cli-1.2.0/PKG-INFO` & `makey-cli-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 Metadata-Version: 2.1
 Name: makey-cli
-Version: 1.2.0
-Summary: CLI passkey maker.
-Home-page: https://boldandbrad.github.io/makey-cli/
-Author: Bradley Wojcik
-Author-email: bradleycwojcik@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/boldandbrad/makey-cli/
-Project-URL: Bug Tracker, https://github.com/boldandbrad/makey-cli/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
+Version: 1.3.0
+Summary: A simple and lightweight tool for making secure passkeys in your terminal.
+Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: click>=8
+Requires-Dist: pyperclip>=1.8
+Requires-Dist: black ; extra == "dev"
+Requires-Dist: flake8 ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: isort ; extra == "dev"
+Requires-Dist: pre-commit ; extra == "dev"
+Requires-Dist: homebrew-pypi-poet ; extra == "dev"
+Requires-Dist: pytest >=6 ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test"
+Requires-Dist: pytest-mock ; extra == "test"
+Project-URL: Home, https://boldandbrad.github.io/makey-cli
+Project-URL: Issues, https://github.com/boldandbrad/makey-cli/issues
+Project-URL: Source, https://github.com/boldandbrad/makey-cli
 Provides-Extra: dev
-License-File: LICENSE
+Provides-Extra: test
 
 # makey-cli
 
-[![Build Status](https://api.travis-ci.com/boldandbrad/makey-cli.svg?branch=main)](https://travis-ci.com/github/boldandbrad/makey-cli)
+[![build status](https://img.shields.io/github/actions/workflow/status/boldandbrad/makey-cli/python-test.yml?branch=main&logo=github)](https://github.com/boldandbrad/makey-cli/actions/workflows/python-test.yml?query=branch%3Amain)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![codecov](https://codecov.io/gh/boldandbrad/makey-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/makey-cli)
-[![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmakey-cli%2F)](https://boldandbrad.github.io/makey-cli/)
-[![PyPI](https://img.shields.io/pypi/v/makey-cli)](https://pypi.org/project/makey-cli/)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/makey-cli)
+[![docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmakey-cli%2F)](https://boldandbrad.github.io/makey-cli/)
+[![pypi](https://img.shields.io/pypi/v/makey-cli)](https://pypi.org/project/makey-cli/)
+[![downloads](https://img.shields.io/pypi/dm/makey-cli)](https://pypistats.org/packages/makey-cli)
 
 > CLI passkey maker.
 
 A simple and lightweight tool for making secure passkeys in your terminal.
 
 **makey-cli** does not store information, produce logs, or make network
 connections. It even avoids printing passkeys in plain-text on screen by
@@ -64,8 +72,7 @@
 > For more usage details, read the **makey-cli** [usage guide](https://boldandbrad.github.io/makey-cli/#/usage).
 
 ## License
 
 Copyright (c) 2021 Bradley Wojcik. Released under the MIT License. See
 [LICENSE](LICENSE) for details.
 
-
```

### Comparing `makey-cli-1.2.0/makey/makey.py` & `makey-cli-1.3.0/src/makey/makey.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import click
-import pyperclip
-
 import string
 from secrets import choice
 
+import click
+import pyperclip
+
 ALWAYS_EXCLUDE = "\"'"
+DEFAULT_LENGTH = 16
 
 
 @click.command(help="CLI passkey maker.")
 @click.option(
     "-e",
     "--exclude",
     default="",
     is_flag=False,
     help="Characters to exclude.",
 )
 @click.option(
     "-l",
     "--length",
-    default=16,
+    default=DEFAULT_LENGTH,
     is_flag=False,
     help="Desired passkey length (default 16).",
 )
 @click.option(
     "-s",
     "--show",
     default=False,
```

### Comparing `makey-cli-1.2.0/makey_cli.egg-info/PKG-INFO` & `makey-cli-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,15 @@
-Metadata-Version: 2.1
-Name: makey-cli
-Version: 1.2.0
-Summary: CLI passkey maker.
-Home-page: https://boldandbrad.github.io/makey-cli/
-Author: Bradley Wojcik
-Author-email: bradleycwojcik@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/boldandbrad/makey-cli/
-Project-URL: Bug Tracker, https://github.com/boldandbrad/makey-cli/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # makey-cli
 
-[![Build Status](https://api.travis-ci.com/boldandbrad/makey-cli.svg?branch=main)](https://travis-ci.com/github/boldandbrad/makey-cli)
+[![build status](https://img.shields.io/github/actions/workflow/status/boldandbrad/makey-cli/python-test.yml?branch=main&logo=github)](https://github.com/boldandbrad/makey-cli/actions/workflows/python-test.yml?query=branch%3Amain)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![codecov](https://codecov.io/gh/boldandbrad/makey-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/makey-cli)
-[![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmakey-cli%2F)](https://boldandbrad.github.io/makey-cli/)
-[![PyPI](https://img.shields.io/pypi/v/makey-cli)](https://pypi.org/project/makey-cli/)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/makey-cli)
+[![docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmakey-cli%2F)](https://boldandbrad.github.io/makey-cli/)
+[![pypi](https://img.shields.io/pypi/v/makey-cli)](https://pypi.org/project/makey-cli/)
+[![downloads](https://img.shields.io/pypi/dm/makey-cli)](https://pypistats.org/packages/makey-cli)
 
 > CLI passkey maker.
 
 A simple and lightweight tool for making secure passkeys in your terminal.
 
 **makey-cli** does not store information, produce logs, or make network
 connections. It even avoids printing passkeys in plain-text on screen by
@@ -63,9 +46,7 @@
 
 > For more usage details, read the **makey-cli** [usage guide](https://boldandbrad.github.io/makey-cli/#/usage).
 
 ## License
 
 Copyright (c) 2021 Bradley Wojcik. Released under the MIT License. See
 [LICENSE](LICENSE) for details.
-
-
```

### Comparing `makey-cli-1.2.0/tests/test_makey.py` & `makey-cli-1.3.0/tests/test_makey.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,73 @@
-import os
-
-from click.testing import CliRunner
 import pyperclip
+from click.testing import CliRunner
 
-from makey.makey import cli
-
+from makey.makey import DEFAULT_LENGTH, cli
 
-DEFAULT_LENGTH = 16
 COPIED_STDOUT = "\tNew passkey copied to clipboard!\n"
 
 
-def test_makey():
-    if "TRAVIS" not in os.environ:
-        runner = CliRunner()
-        result = runner.invoke(cli, [])
-        assert result.exit_code == 0
+def test_makey(mocker):
+    mocker.patch("pyperclip.copy")
+
+    runner = CliRunner()
+    result = runner.invoke(cli, [])
+
+    assert result.exit_code == 0
+    pyperclip.copy.assert_called_once()
+    assert result.stdout == COPIED_STDOUT
+
+
+def test_makey_default_length(mocker):
+    mocker.patch("pyperclip.copy")
 
-        passkey = pyperclip.paste()
+    runner = CliRunner()
+    result = runner.invoke(cli, ["--show"])
 
-        assert result.stdout == COPIED_STDOUT
-        assert len(passkey) == DEFAULT_LENGTH
-        assert '"' not in passkey
-        assert "'" not in passkey
+    assert result.exit_code == 0
+    pyperclip.copy.assert_called_once()
 
+    passkey = result.stdout.rstrip()
 
-def test_makey_with_exclude():
-    if "TRAVIS" not in os.environ:
-        runner = CliRunner()
-        result = runner.invoke(cli, ["-e", "&"])
-        assert result.exit_code == 0
+    assert len(passkey) == DEFAULT_LENGTH
+    assert "'" not in passkey
+    assert '"' not in passkey
 
-        passkey = pyperclip.paste()
 
-        assert result.stdout == COPIED_STDOUT
-        assert len(passkey) == DEFAULT_LENGTH
-        assert "&" not in passkey
+def test_makey_exclude(mocker):
+    mocker.patch("pyperclip.copy")
 
+    runner = CliRunner()
+    result = runner.invoke(cli, ["-s", "-e", "&"])
 
-def test_makey_with_length():
-    if "TRAVIS" not in os.environ:
-        runner = CliRunner()
-        result = runner.invoke(cli, ["-l", "20"])
-        assert result.exit_code == 0
+    assert result.exit_code == 0
+    pyperclip.copy.assert_called_once()
 
-        passkey = pyperclip.paste()
+    passkey = result.stdout.rstrip()
 
-        assert result.stdout == COPIED_STDOUT
-        assert len(passkey) == 20
+    assert len(passkey) == DEFAULT_LENGTH
+    assert "'" not in passkey
+    assert '"' not in passkey
+    assert "&" not in passkey
 
 
-def test_makey_with_show():
-    if "TRAVIS" not in os.environ:
-        runner = CliRunner()
-        result = runner.invoke(cli, ["-s"])
-        assert result.exit_code == 0
+def test_makey_length(mocker):
+    mocker.patch("pyperclip.copy")
+
+    runner = CliRunner()
+    result = runner.invoke(cli, ["--show", "-l", 20])
+
+    assert result.exit_code == 0
+    pyperclip.copy.assert_called_once()
 
-        passkey = pyperclip.paste()
-        printedkey = result.stdout.replace("\n", "")
+    passkey = result.stdout.rstrip()
 
-        assert len(passkey) == DEFAULT_LENGTH
-        assert passkey == printedkey
+    assert len(passkey) == 20
+    assert "'" not in passkey
+    assert '"' not in passkey
 
 
 def test_version():
     runner = CliRunner()
     result = runner.invoke(cli, ["--version"])
     assert result.exit_code == 0
```

