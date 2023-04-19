# Comparing `tmp/shell-themer-0.1.tar.gz` & `tmp/shell-themer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell-themer-0.1.tar", last modified: Sat Apr  1 17:57:31 2023, max compression
+gzip compressed data, was "shell-themer-0.2.0.tar", last modified: Wed Apr 19 17:49:48 2023, max compression
```

## Comparing `shell-themer-0.1.tar` & `shell-themer-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-01 17:57:31.437429 shell-themer-0.1/
--rw-r--r--   0 jared      (501) staff       (20)      430 2023-03-24 22:21:41.000000 shell-themer-0.1/.gitignore
--rw-r--r--   0 jared      (501) staff       (20)      328 2023-03-25 22:52:01.000000 shell-themer-0.1/CHANGELOG.md
--rw-r--r--   0 jared      (501) staff       (20)     1062 2023-03-05 21:05:40.000000 shell-themer-0.1/LICENSE
--rw-r--r--   0 jared      (501) staff       (20)     3594 2023-04-01 17:57:31.437281 shell-themer-0.1/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)     1352 2023-04-01 17:52:12.000000 shell-themer-0.1/README.md
--rw-r--r--   0 jared      (501) staff       (20)     1710 2023-03-30 04:56:55.000000 shell-themer-0.1/TODO.md
--rw-r--r--   0 jared      (501) staff       (20)     1770 2023-03-27 06:03:39.000000 shell-themer-0.1/pyproject.toml
--rw-r--r--   0 jared      (501) staff       (20)       38 2023-04-01 17:57:31.437464 shell-themer-0.1/setup.cfg
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-01 17:57:31.433051 shell-themer-0.1/src/
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-01 17:57:31.435173 shell-themer-0.1/src/shell_themer/
--rw-r--r--   0 jared      (501) staff       (20)     1614 2023-03-26 17:34:17.000000 shell-themer-0.1/src/shell_themer/__init__.py
--rw-r--r--   0 jared      (501) staff       (20)     3241 2023-03-30 04:14:52.000000 shell-themer-0.1/src/shell_themer/__main__.py
--rwxr-xr-x   0 jared      (501) staff       (20)    26354 2023-03-30 05:08:14.000000 shell-themer-0.1/src/shell_themer/themer.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-01 17:57:31.436183 shell-themer-0.1/src/shell_themer.egg-info/
--rw-r--r--   0 jared      (501) staff       (20)     3594 2023-04-01 17:57:31.000000 shell-themer-0.1/src/shell_themer.egg-info/PKG-INFO
--rw-r--r--   0 jared      (501) staff       (20)      484 2023-04-01 17:57:31.000000 shell-themer-0.1/src/shell_themer.egg-info/SOURCES.txt
--rw-r--r--   0 jared      (501) staff       (20)        1 2023-04-01 17:57:31.000000 shell-themer-0.1/src/shell_themer.egg-info/dependency_links.txt
--rw-r--r--   0 jared      (501) staff       (20)       60 2023-04-01 17:57:31.000000 shell-themer-0.1/src/shell_themer.egg-info/entry_points.txt
--rw-r--r--   0 jared      (501) staff       (20)      168 2023-04-01 17:57:31.000000 shell-themer-0.1/src/shell_themer.egg-info/requires.txt
--rw-r--r--   0 jared      (501) staff       (20)       13 2023-04-01 17:57:31.000000 shell-themer-0.1/src/shell_themer.egg-info/top_level.txt
--rw-r--r--   0 jared      (501) staff       (20)     4206 2023-03-25 13:43:01.000000 shell-themer-0.1/tasks.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-01 17:57:31.436730 shell-themer-0.1/tests/
--rw-r--r--   0 jared      (501) staff       (20)     1910 2023-03-30 04:16:52.000000 shell-themer-0.1/tests/conftest.py
--rw-r--r--   0 jared      (501) staff       (20)    12647 2023-03-30 04:23:43.000000 shell-themer-0.1/tests/test_processors.py
--rw-r--r--   0 jared      (501) staff       (20)     7191 2023-03-30 03:53:06.000000 shell-themer-0.1/tests/test_themer.py
-drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-01 17:57:31.436938 shell-themer-0.1/themes/
--rw-r--r--   0 jared      (501) staff       (20)     9218 2023-03-28 23:15:33.000000 shell-themer-0.1/themes/dracula.toml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.167468 shell-themer-0.2.0/
+-rw-r--r--   0 jared      (501) staff       (20)      430 2023-03-24 22:19:37.000000 shell-themer-0.2.0/.gitignore
+-rw-r--r--   0 jared      (501) staff       (20)      724 2023-04-19 17:43:58.000000 shell-themer-0.2.0/CHANGELOG.md
+-rw-r--r--   0 jared      (501) staff       (20)     5359 2023-04-19 17:43:58.000000 shell-themer-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 jared      (501) staff       (20)     1062 2023-03-15 00:19:15.000000 shell-themer-0.2.0/LICENSE
+-rw-r--r--   0 jared      (501) staff       (20)     3596 2023-04-19 17:49:48.167323 shell-themer-0.2.0/PKG-INFO
+-rw-r--r--   0 jared      (501) staff       (20)     1352 2023-04-07 23:49:41.000000 shell-themer-0.2.0/README.md
+-rw-r--r--   0 jared      (501) staff       (20)     2085 2023-04-15 04:34:30.000000 shell-themer-0.2.0/TODO.md
+-rw-r--r--   0 jared      (501) staff       (20)     2635 2023-04-15 03:22:17.000000 shell-themer-0.2.0/pyproject.toml
+-rw-r--r--   0 jared      (501) staff       (20)       38 2023-04-19 17:49:48.167505 shell-themer-0.2.0/setup.cfg
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.163814 shell-themer-0.2.0/src/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.165464 shell-themer-0.2.0/src/shell_themer/
+-rw-r--r--   0 jared      (501) staff       (20)     1228 2023-04-14 15:39:07.000000 shell-themer-0.2.0/src/shell_themer/__init__.py
+-rw-r--r--   0 jared      (501) staff       (20)     1350 2023-04-15 23:38:46.000000 shell-themer-0.2.0/src/shell_themer/__main__.py
+-rwxr-xr-x   0 jared      (501) staff       (20)    37599 2023-04-15 22:11:33.000000 shell-themer-0.2.0/src/shell_themer/themer.py
+-rw-r--r--   0 jared      (501) staff       (20)     1608 2023-04-15 03:09:24.000000 shell-themer-0.2.0/src/shell_themer/version.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.166157 shell-themer-0.2.0/src/shell_themer.egg-info/
+-rw-r--r--   0 jared      (501) staff       (20)     3596 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/PKG-INFO
+-rw-r--r--   0 jared      (501) staff       (20)      595 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/SOURCES.txt
+-rw-r--r--   0 jared      (501) staff       (20)        1 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/dependency_links.txt
+-rw-r--r--   0 jared      (501) staff       (20)       65 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/entry_points.txt
+-rw-r--r--   0 jared      (501) staff       (20)      168 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/requires.txt
+-rw-r--r--   0 jared      (501) staff       (20)       13 2023-04-19 17:49:48.000000 shell-themer-0.2.0/src/shell_themer.egg-info/top_level.txt
+-rw-r--r--   0 jared      (501) staff       (20)     4196 2023-04-19 17:49:33.000000 shell-themer-0.2.0/tasks.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.166991 shell-themer-0.2.0/tests/
+-rw-r--r--   0 jared      (501) staff       (20)     2512 2023-04-15 21:59:15.000000 shell-themer-0.2.0/tests/conftest.py
+-rw-r--r--   0 jared      (501) staff       (20)    19596 2023-04-13 23:30:40.000000 shell-themer-0.2.0/tests/test_generate.py
+-rw-r--r--   0 jared      (501) staff       (20)     2150 2023-04-11 14:03:52.000000 shell-themer-0.2.0/tests/test_list.py
+-rw-r--r--   0 jared      (501) staff       (20)     7093 2023-04-15 23:38:46.000000 shell-themer-0.2.0/tests/test_main_dispatch.py
+-rw-r--r--   0 jared      (501) staff       (20)     2318 2023-04-11 15:55:44.000000 shell-themer-0.2.0/tests/test_preview.py
+-rw-r--r--   0 jared      (501) staff       (20)    14331 2023-04-15 20:24:06.000000 shell-themer-0.2.0/tests/test_themer.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-19 17:49:48.167112 shell-themer-0.2.0/themes/
+-rw-r--r--   0 jared      (501) staff       (20)     9310 2023-04-13 23:29:31.000000 shell-themer-0.2.0/themes/dracula.toml
```

### Comparing `shell-themer-0.1/LICENSE` & `shell-themer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shell-themer-0.1/PKG-INFO` & `shell-themer-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-themer
-Version: 0.1
+Version: 0.2.0
 Summary: Use consistent color themes for a variety of command line tools.
 Author-email: Jared Crapo <jared@kotfu.net>
 License: MIT License
         
         Copyright (c) 2023 kotfu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `shell-themer-0.1/README.md` & `shell-themer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shell-themer-0.1/TODO.md` & `shell-themer-0.2.0/TODO.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,25 @@
   - show how to set BAT_THEME
 - document how to load a theme
     - eval $(shell-themer) is bad, try the code from `$ starship init bash` instead
 - document a "magic" styles named "background", "foreground", and "text"
   - these will be used by the preview command to show the style properly
   - text should be foreground on background
 - document environment interpolations
+- document variable interpolations
+- document enabled and enabled_if - enabled_if shell commands should not cause side effects because
+  they can get executed on a "dry run" of generation
+- document shell generator, including multiline commands and usage with enable_if
 
 ## shell-themer subcommands
 
 [x] themes = -f and -t are ignored, shows a list of all available themes from $THEME_DIR
 [x] preview = show the theme name, version, and file, and all active styles from the specified theme or from $THEME_DIR
 [x] {activate|process|render|brew|make|generate} = process the theme and spew out all the environment variables
   - don't like activate because it doesn't really activate the theme
   - don't like process because we use processors for something else
   - generate seems the best so far, then we have generator = "fzf"
 - init = generate the code for the theme-activate (using fzf if not specified), theme-reload
-- help = show help
+[x] honor NO_COLOR env variable
+[x] add --no-color option
+[x] add --colors= option
+[x] add SHELL_THEMER_COLORS env variable
```

### Comparing `shell-themer-0.1/src/shell_themer/__init__.py` & `shell-themer-0.2.0/src/shell_themer/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,29 +17,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
-"""
-ksc is a library and command line program for parsing and standardizing
-keyboard shortcuts
-"""
+"""retrive version information for this package"""
 
 try:
     # for python 3.8+
     import importlib.metadata as importlib_metadata
 except ImportError:  # pragma: nocover
     # for python < 3.8
     import importlib_metadata
 
-from .themer import (
-    Themer,
-)
 
-try:
-    __version__ = importlib_metadata.version(__name__)
-except importlib_metadata.PackageNotFoundError:  # pragma: nocover
-    __version__ = "unknown"
-
-VERSION_STRING = __version__
+def version_string():
+    """return a version string suitable for display to a user"""
+    try:
+        ver = importlib_metadata.version("shell_themer")
+    except importlib_metadata.PackageNotFoundError:  # pragma: nocover
+        ver = "unknown"
+    return ver
```

### Comparing `shell-themer-0.1/src/shell_themer.egg-info/PKG-INFO` & `shell-themer-0.2.0/src/shell_themer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-themer
-Version: 0.1
+Version: 0.2.0
 Summary: Use consistent color themes for a variety of command line tools.
 Author-email: Jared Crapo <jared@kotfu.net>
 License: MIT License
         
         Copyright (c) 2023 kotfu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `shell-themer-0.1/tasks.py` & `shell-themer-0.2.0/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 namespace_clean.add_task(pytest_clean, "pytest")
 
 
 @invoke.task
 def pylint(context):
     "Check code quality using pylint"
-    context.run("pylint src/ksc tests", echo=True)
+    context.run("pylint src tests", echo=True)
 
 
 namespace.add_task(pylint)
 namespace_check.add_task(pylint)
 
 
 @invoke.task
@@ -179,20 +179,20 @@
 
 namespace.add_task(build)
 
 
 @invoke.task(pre=[build])
 def pypi(context):
     "Build and upload a distribution to pypi"
-    context.run("twine upload dist/*")
+    context.run("twine upload --respository pypi dist/*")
 
 
 namespace.add_task(pypi)
 
 
 @invoke.task(pre=[build])
 def pypi_test(context):
     "Build and upload a distribution to https://test.pypi.org"
-    context.run("twine upload --repository-url https://test.pypi.org/legacy/ dist/*")
+    context.run("twine upload --repository testpypi dist/*")
 
 
 namespace.add_task(pypi_test)
```

### Comparing `shell-themer-0.1/tests/conftest.py` & `shell-themer-0.2.0/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,33 +23,49 @@
 #
 # pylint: disable=protected-access, missing-function-docstring, redefined-outer-name
 # pylint: disable=missing-module-docstring, unused-variable
 
 import pytest
 
 from shell_themer import Themer
-from shell_themer.__main__ import build_parser
-
-
-@pytest.fixture
-def parser():
-    return build_parser()
 
 
 @pytest.fixture
 def thm():
     thm = Themer(prog="shell-themer")
     return thm
 
 
 @pytest.fixture
-def thm_cmdline(thm, parser, mocker):
+def thm_cmdline(thm, mocker):
+    # defining a fixture that returns a function
+    # allows us to call the fixture and pass parameters to it
+    # ie:
+    #
+    # def test_generate_environment_unset_list(thm_cmdline, capsys):
+    #     tomlstr = """
+    #     [scope.ls]
+    #     # set some environment variables
+    #     environment.unset = ["SOMEVAR", "ANOTHERVAR"]
+    #     environment.export.LS_COLORS = "ace ventura"
+    #     """
+    #     exit_code = thm_cmdline("generate", tomlstr)
+    #     ...
+
     def _executor(cmdline, toml=None):
-        argv = cmdline.split(" ")
-        args = parser.parse_args(argv)
+        if isinstance(cmdline, str):
+            argv = cmdline.split(" ")
+        elif isinstance(cmdline, list):
+            argv = cmdline
+        else:
+            argv = []
+        try:
+            args = thm.argparser().parse_args(argv)
+        except SystemExit as err:
+            return err.code
         if toml:
             thm.loads(toml)
-        # now monkeypatch load_from_args() because that won't work
+        # monkeypatch load_from_args() because that won't work so well
         mocker.patch("shell_themer.Themer.load_from_args", autospec=True)
         return thm.dispatch(args)
 
     return _executor
```

### Comparing `shell-themer-0.1/tests/test_processors.py` & `shell-themer-0.2.0/tests/test_generate.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,167 +28,300 @@
 import rich.style
 import rich.errors
 
 from shell_themer import Themer
 
 
 #
+# test high level generation functions
+#
+def test_generate_single_scope(thm_cmdline, capsys):
+    tomlstr = """
+        [styles]
+        background =  "#282a36"
+        foreground =  "#f8f8f2"
+        current_line =  "#f8f8f2 on #44475a"
+        comment =  "#6272a4"
+        cyan =  "#8be9fd"
+        green =  "#50fa7b"
+        orange =  "#ffb86c"
+        pink =  "#ff79c6"
+        purple =  "#bd93f9"
+        red =  "#ff5555"
+        yellow =  "#f1fa8c"
+
+        [scope.iterm]
+        generator = "iterm"
+        style.foreground = "foreground"
+        style.background = "background"
+
+        [scope.fzf]
+        generator = "fzf"
+
+        # attributes specific to fzf
+        environment_variable = "FZF_DEFAULT_OPTS"
+
+        # command line options
+        opt.--prompt = ">"
+        opt.--border = "single"
+        opt.--pointer = "•"
+        opt.--info = "hidden"
+        opt.--no-sort = true
+        opt."+i" = true
+
+        # styles
+        style.text = "foreground"
+        style.label = "green"
+        style.border = "orange"
+        style.selected = "current_line"
+        style.prompt = "green"
+        style.indicator = "cyan"
+        style.match = "pink"
+        style.localstyle = "green on black"
+    """
+    exit_code = thm_cmdline("generate -s fzf", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert out
+    assert not err
+    assert out.count("\n") == 1
+
+
+def test_generate_unknown_scope(thm_cmdline, capsys):
+    tomlstr = """
+        [styles]
+        background =  "#282a36"
+        foreground =  "#f8f8f2"
+
+        [scope.iterm]
+        generator = "iterm"
+        style.foreground = "foreground"
+        style.background = "background"
+
+        [scope.ls]
+        # set some environment variables
+        environment.unset = ["SOMEVAR", "ANOTHERVAR"]
+        environment.export.LS_COLORS = "ace ventura"
+    """
+    exit_code = thm_cmdline("generate -s unknownscope", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert not out
+    assert err
+
+
+def test_generate_no_scopes(thm_cmdline, capsys):
+    tomlstr = """
+        [styles]
+        background =  "#282a36"
+        foreground =  "#f8f8f2"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not out
+    assert not err
+
+
+#
 # test rendering of elements common to all scopes
 #
-INTERPOLATIONS = [
-    ("{dark_orange}", "#ff6c1c"),
-    ("{dark_orange:hex}", "#ff6c1c"),
-    ("{dark_orange:hexnohash}", "ff6c1c"),
+ENV_INTERPOLATIONS = [
+    ("{style:dark_orange}", "#ff6c1c"),
+    ("{style:dark_orange:hex}", "#ff6c1c"),
+    ("{style:dark_orange:hexnohash}", "ff6c1c"),
     # for an unknown format or style, don't do any replacement
-    ("{current_line}", "{current_line}"),
-    ("{dark_orange:unknown}", "{dark_orange:unknown}"),
+    ("{style:current_line}", "{style:current_line}"),
+    ("{style:dark_orange:unknown}", "{style:dark_orange:unknown}"),
+    # we have to have the style keyword, or it all just gets passed through
+    ("{dark_orange}", "{dark_orange}"),
+    ("{variable:green}", "{variable:green}"),
     # escaped opening bracket, becasue this is toml, if you want a backslash
     # you have to you \\ because toml strings can contain escape sequences
-    (r"\\{bright_blue}", "{bright_blue}"),
-    (r"\\{ some other  things}", "{ some other  things}"),
-    # if you don't have matched brackets, don't expect the backslash
+    (r"\\{style:bright_blue}", "{style:bright_blue}"),
+    # if you don't have matched brackets, or are missing the
+    # literal 'style:' keyword, don't expect the backslash
     # to be removed. again here we have two backslashes in the first
     # argument so that it will survive toml string escaping
+    (r"\\{ some other  things}", r"\{ some other  things}"),
     (r"\\{escaped unmatched bracket", r"\{escaped unmatched bracket"),
+    # try a mixed variable and style interpolation
+    ("{style:dark_orange} {var:someopts}", "#ff6c1c --option=fred -v"),
 ]
 
 
-@pytest.mark.parametrize("phrase, interpolated", INTERPOLATIONS)
+@pytest.mark.parametrize("phrase, interpolated", ENV_INTERPOLATIONS)
 def test_generate_environment_interpolation(thm_cmdline, capsys, phrase, interpolated):
     tomlstr = f"""
-    [styles]
-    dark_orange = "#ff6c1c"
+        [variables]
+        someopts = "--option=fred -v"
+
+        [styles]
+        dark_orange = "#ff6c1c"
 
-    [scope.gum]
-    environment.export.GUM_OPTS = " --cursor-foreground={phrase}"
+        [scope.gum]
+        environment.export.GUM_OPTS = " --cursor-foreground={phrase}"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert out == f'export GUM_OPTS=" --cursor-foreground={interpolated}"\n'
 
 
 def test_generate_environment_unset_list(thm_cmdline, capsys):
     tomlstr = """
-    [scope.ls]
-    # set some environment variables
-    environment.unset = ["SOMEVAR", "ANOTHERVAR"]
-    environment.export.LS_COLORS = "ace ventura"
-"""
+        [scope.ls]
+        # set some environment variables
+        environment.unset = ["SOMEVAR", "ANOTHERVAR"]
+        environment.export.LS_COLORS = "ace ventura"
+    """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "unset SOMEVAR" in out
     assert "unset ANOTHERVAR" in out
     assert 'export LS_COLORS="ace ventura"' in out
 
 
 def test_generate_environment_unset_string(thm_cmdline, capsys):
     tomlstr = """
-    [scope.unset]
-    environment.unset = "NOLISTVAR"
+        [scope.unset]
+        environment.unset = "NOLISTVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "unset NOLISTVAR" in out
 
 
 def test_generate_enabled(thm_cmdline, capsys):
     tomlstr = """
-    [scope.nolistvar]
-    enabled = false
-    environment.unset = "NOLISTVAR"
-
-    [scope.somevar]
-    enabled = true
-    environment.unset = "SOMEVAR"
+        [scope.nolistvar]
+        enabled = false
+        environment.unset = "NOLISTVAR"
+
+        [scope.somevar]
+        enabled = true
+        environment.unset = "SOMEVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "unset SOMEVAR" in out
     assert not "unset NOLISTVAR" in out
 
 
 def test_generate_enabled_false_enabled_if_ignored(thm_cmdline, capsys):
     tomlstr = """
-    [scope.unset]
-    enabled = false
-    enabled_if = "[[ 1 == 1 ]]"
-    environment.unset = "NOLISTVAR"
+        [scope.unset]
+        enabled = false
+        enabled_if = "[[ 1 == 1 ]]"
+        environment.unset = "NOLISTVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert not out
 
 
 def test_generate_enabled_true_enabed_if_ignored(thm_cmdline, capsys):
     tomlstr = """
-    [scope.unset]
-    enabled = true
-    enabled_if = "[[ 0 == 1 ]]"
-    environment.unset = "NOLISTVAR"
+        [scope.unset]
+        enabled = true
+        enabled_if = "[[ 0 == 1 ]]"
+        environment.unset = "NOLISTVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "unset NOLISTVAR" in out
 
 
+def test_generate_enabled_invalid_value(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.unset]
+        enabled = "notaboolean"
+        environment.unset = "NOLISTVAR"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert not out
+    assert "to be true or false" in err
+
+
 ENABLED_IFS = [
     ("", True),
     ("echo", True),
     ("[[ 1 == 1 ]]", True),
     ("[[ 1 == 0 ]]", False),
+    ("{var:echocmd} hi", True),
+    ("{variable:falsetest}", False),
 ]
 
 
 @pytest.mark.parametrize("cmd, enabled", ENABLED_IFS)
 def test_generate_enabled_if(cmd, enabled, thm_cmdline, capsys):
     tomlstr = f"""
-    [scope.unset]
-    enabled_if = "{cmd}"
-    environment.unset = "ENVVAR"
+        [variables]
+        echocmd = "/bin/echo"
+        falsetest = "[[ 1 == 0]]"
+
+        [scope.unset]
+        enabled_if = "{cmd}"
+        environment.unset = "ENVVAR"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     if enabled:
         assert "unset ENVVAR" in out
     else:
         assert not out
 
 
 def test_generate_comments(thm_cmdline, capsys):
     tomlstr = """
-    [scope.nolistvar]
-    enabled = false
-    environment.unset = "NOLISTVAR"
-
-    [scope.somevar]
-    enabled = true
-    environment.unset = "SOMEVAR"
+        [scope.nolistvar]
+        enabled = false
+        environment.unset = "NOLISTVAR"
+
+        [scope.somevar]
+        enabled = true
+        environment.unset = "SOMEVAR"
     """
     exit_code = thm_cmdline("generate --comment", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert "# [scope.nolistvar]" in out
     assert "# [scope.somevar]" in out
     assert "unset SOMEVAR" in out
     assert not "unset NOLISTVAR" in out
 
+
+def test_unknown_generator(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.myprog]
+        generator = "mrfusion"
+        environment.unset = "SOMEVAR"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert "unknown generator" in err
+    assert "mrfusion" in err
+
+
 #
 # test the fzf generator
 #
 ATTRIBS_TO_FZF = [
     ("bold", "regular:bold"),
     ("underline", "regular:underline"),
     ("reverse", "regular:reverse"),
@@ -230,46 +363,51 @@
 def test_fzf_from_style(thm, name, styledef, fzf):
     style = rich.style.Style.parse(styledef)
     assert fzf == thm._fzf_from_style(name, style)
 
 
 def test_fzf_opts(thm_cmdline, capsys):
     tomlstr = """
-[scope.fzf]
-generator = "fzf"
-environment_variable = "QQQ"
-opt."+i" = true
-opt.--border = "rounded"
+        [variables]
+        bstyle = "rounded"
+
+        [scope.fzf]
+        generator = "fzf"
+        environment_variable = "QQQ"
+        opt."+i" = true
+        opt.--border = "{var:bstyle}"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert out == """export QQQ=" +i --border='rounded'"\n"""
 
 
 def test_fzf_no_opts(thm_cmdline, capsys):
     tomlstr = """
-[scope.fzf]
-generator = "fzf"
-environment_variable = "QQQ"
+        [variables]
+        varname = "ZZ"
+        [scope.fzf]
+        generator = "fzf"
+        environment_variable = "Q{var:varname}QQ"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
-    assert out == """export QQQ=""\n"""
+    assert out == """export QZZQQ=""\n"""
 
 
 def test_fzf_no_varname(thm_cmdline, capsys):
     tomlstr = """
-[scope.fzf]
-generator = "fzf"
-opt."+i" = true
-opt.--border = "rounded"
+        [scope.fzf]
+        generator = "fzf"
+        opt."+i" = true
+        opt.--border = "rounded"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_ERROR
     assert not out
     assert "fzf generator requires 'environment_variable'" in err
 
@@ -303,100 +441,199 @@
     ("file_with_capability", "red on black", "ca=31;40"),
 ]
 
 
 @pytest.mark.parametrize("name, styledef, lsc", STYLE_TO_LSCOLORS)
 def test_ls_colors_from_style(thm, name, styledef, lsc):
     style = rich.style.Style.parse(styledef)
-    assert lsc == thm._ls_colors_from_style(name, style)
+    assert lsc == thm._ls_colors_from_style("scope", name, style)
 
 
 def test_ls_colors_no_styles(thm_cmdline, capsys):
     tomlstr = """
-[scope.lsc]
-generator = "ls_colors"
+        [scope.lsc]
+        generator = "ls_colors"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert out == 'export LS_COLORS=""\n'
 
 
+def test_ls_colors_unknown_style(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.lsc]
+        generator = "ls_colors"
+        style.bundleid = "default"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_ERROR
+    assert "unknown style" in err
+    assert "lsc" in err
+
+
 def test_ls_colors_environment_variable(thm_cmdline, capsys):
     tomlstr = """
-[scope.lsc]
-generator = "ls_colors"
-environment_variable = "OTHER_LS_COLOR"
-style.file = "default"
+        [scope.lsc]
+        generator = "ls_colors"
+        environment_variable = "OTHER_LS_COLOR"
+        style.file = "default"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     assert out == 'export OTHER_LS_COLOR="fi=0"\n'
 
 
 def test_ls_colors_clear_builtin(thm_cmdline, capsys):
     tomlstr = """
-[scope.lsc]
-generator = "ls_colors"
-clear_builtin = true
-style.directory = "bright_blue"
+        [scope.lsc]
+        generator = "ls_colors"
+        clear_builtin = true
+        style.directory = "bright_blue"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
-    assert (
-        out
-        == 'export LS_COLORS="no=0:fi=0:di=94:ln=0:mh=0:pi=0:so=0:do=0:bd=0:cd=0:or=0:mi=0:su=0:sg=0:st=0:ow=0:tw=0:ex=0:ca=0"\n'
+    expected = (
+        'export LS_COLORS="no=0:fi=0:di=94:ln=0:'
+        "mh=0:pi=0:so=0:do=0:bd=0:cd=0:or=0:mi=0:"
+        'su=0:sg=0:st=0:ow=0:tw=0:ex=0:ca=0"\n'
     )
+    assert out == expected
 
 
 def test_ls_colors_clear_builtin_not_boolean(thm_cmdline, capsys):
     tomlstr = """
-[scope.lsc]
-generator = "ls_colors"
-clear_builtin = "error"
-style.directory = "bright_blue"
+        [scope.lsc]
+        generator = "ls_colors"
+        clear_builtin = "error"
+        style.directory = "bright_blue"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_ERROR
     assert not out
     assert "'clear_builtin' to be true or false" in err
 
 
 #
 # test the iterm generator
 #
 def test_iterm(thm_cmdline, capsys):
     tomlstr = """
-[scope.iterm]
-generator = "iterm"
-style.foreground = "#ffeebb"
-style.background = "#221122"
+        [scope.iterm]
+        generator = "iterm"
+        style.foreground = "#ffeebb"
+        style.background = "#221122"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     lines = out.splitlines()
     assert len(lines) == 2
     assert lines[0] == r'builtin echo -e "\e]1337;SetColors=fg=ffeebb\a"'
     assert lines[1] == r'builtin echo -e "\e]1337;SetColors=bg=221122\a"'
 
 
 def test_iterm_bgonly(thm_cmdline, capsys):
     tomlstr = """
-[scope.iterm]
-generator = "iterm"
-style.background = "#b2cacd"
+        [scope.iterm]
+        generator = "iterm"
+        style.background = "#b2cacd"
     """
     exit_code = thm_cmdline("generate", tomlstr)
     out, err = capsys.readouterr()
     assert exit_code == Themer.EXIT_SUCCESS
     assert not err
     lines = out.splitlines()
     assert len(lines) == 1
     assert lines[0] == r'builtin echo -e "\e]1337;SetColors=bg=b2cacd\a"'
+
+
+#
+# test the shellcommand generator
+#
+def test_shell(thm_cmdline, capsys):
+    tomlstr = """
+        [variables]
+        greeting = "hello there"
+
+        [styles]
+        purple = "#A020F0"
+
+        [scope.shortcut]
+        generator = "shell"
+        command.first = "echo {var:greeting}"
+        command.next = "echo general kenobi"
+        command.last = "echo {style:purple}"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert out == "echo hello there\necho general kenobi\necho #a020f0\n"
+
+
+def test_shell_enabled_if(thm_cmdline, capsys):
+    # we have separate tests for enabled_if, but since it's super useful with the
+    # shell generator, i'm including another test here
+    tomlstr = """
+        [scope.shortcut]
+        generator = "shell"
+        enabled_if = "[[ 1 == 0 ]]"
+        command.first = "shortcuts run 'My Shortcut Name'"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert not out
+
+
+def test_shell_multiline(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.multiline]
+        generator = "shell"
+        command.long = '''
+echo hello there
+echo general kenobi
+if [[ 1 == 1 ]]; then
+  echo "yes sir"
+fi
+'''
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    # yes we have two line breaks at the end of what we expect
+    # because there are single line commands, we have to output
+    # a newline after the command
+    # but on multiline commands that might give an extra newline
+    # at the end of the day, that makes zero difference in
+    # functionality, but it matters for testing, hence this note
+    expected = """echo hello there
+echo general kenobi
+if [[ 1 == 1 ]]; then
+  echo "yes sir"
+fi
+
+"""
+    assert out == expected
+
+
+def test_shell_no_commands(thm_cmdline, capsys):
+    tomlstr = """
+        [scope.shortcut]
+        generator = "shell"
+    """
+    exit_code = thm_cmdline("generate", tomlstr)
+    out, err = capsys.readouterr()
+    assert exit_code == Themer.EXIT_SUCCESS
+    assert not err
+    assert not out
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shell-themer-0.1/themes/dracula.toml` & `shell-themer-0.2.0/themes/dracula.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 #
 # definition of dracula theme
 
 version = "1.0.0"
 name = "dracula"
 
-# styles defined here use the syntax of the python rich library
+[variables]
+# any key here can be inserted anywhere
+# using the {var:variable_name} syntax
+
 
+# styles defined here use the syntax of the python rich library
 [styles]
 # These are from https://draculatheme.com/contribute
 # Even though we define the bacula background color here, we don't use
 # it, we just use the default terminal background color
 background =  "#282a36"
 foreground =  "#f8f8f2"
```

