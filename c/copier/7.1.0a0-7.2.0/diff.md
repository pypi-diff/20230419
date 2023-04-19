# Comparing `tmp/copier-7.1.0a0.tar.gz` & `tmp/copier-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copier-7.1.0a0.tar", max compression
+gzip compressed data, was "copier-7.2.0.tar", max compression
```

## Comparing `copier-7.1.0a0.tar` & `copier-7.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1076 2022-12-29 11:22:56.467372 copier-7.1.0a0/LICENSE
--rw-r--r--   0        0        0     5675 2022-12-29 11:22:56.467372 copier-7.1.0a0/README.md
--rw-r--r--   0        0        0      265 2022-12-29 11:23:14.811279 copier-7.1.0a0/copier/__init__.py
--rw-r--r--   0        0        0       81 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/__main__.py
--rw-r--r--   0        0        0    11237 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/cli.py
--rw-r--r--   0        0        0     3302 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/errors.py
--rw-r--r--   0        0        0    35683 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/main.py
--rw-r--r--   0        0        0     2477 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/subproject.py
--rw-r--r--   0        0        0    16175 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/template.py
--rw-r--r--   0        0        0     5483 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/tools.py
--rw-r--r--   0        0        0     1868 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/types.py
--rw-r--r--   0        0        0    15445 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/user_data.py
--rw-r--r--   0        0        0     5577 2022-12-29 11:22:56.467372 copier-7.1.0a0/copier/vcs.py
--rw-r--r--   0        0        0     3460 2022-12-29 11:23:14.807279 copier-7.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     7084 1970-01-01 00:00:00.000000 copier-7.1.0a0/setup.py
--rw-r--r--   0        0        0     7466 1970-01-01 00:00:00.000000 copier-7.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-19 17:40:07.270090 copier-7.2.0/LICENSE
+-rw-r--r--   0        0        0     6143 2023-04-19 17:40:07.270090 copier-7.2.0/README.md
+-rw-r--r--   0        0        0      263 2023-04-19 17:40:24.306022 copier-7.2.0/copier/__init__.py
+-rw-r--r--   0        0        0      198 2023-04-19 17:40:07.270090 copier-7.2.0/copier/__main__.py
+-rw-r--r--   0        0        0    11559 2023-04-19 17:40:07.270090 copier-7.2.0/copier/cli.py
+-rw-r--r--   0        0        0     3413 2023-04-19 17:40:07.270090 copier-7.2.0/copier/errors.py
+-rw-r--r--   0        0        0    36644 2023-04-19 17:40:07.270090 copier-7.2.0/copier/main.py
+-rw-r--r--   0        0        0     2476 2023-04-19 17:40:07.270090 copier-7.2.0/copier/subproject.py
+-rw-r--r--   0        0        0    16594 2023-04-19 17:40:07.270090 copier-7.2.0/copier/template.py
+-rw-r--r--   0        0        0     6234 2023-04-19 17:40:07.270090 copier-7.2.0/copier/tools.py
+-rw-r--r--   0        0        0     2243 2023-04-19 17:40:07.270090 copier-7.2.0/copier/types.py
+-rw-r--r--   0        0        0    15733 2023-04-19 17:40:07.274091 copier-7.2.0/copier/user_data.py
+-rw-r--r--   0        0        0     6730 2023-04-19 17:40:07.274091 copier-7.2.0/copier/vcs.py
+-rw-r--r--   0        0        0     3459 2023-04-19 17:40:24.306022 copier-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7983 1970-01-01 00:00:00.000000 copier-7.2.0/PKG-INFO
```

### Comparing `copier-7.1.0a0/LICENSE` & `copier-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `copier-7.1.0a0/README.md` & `copier-7.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,27 @@
 
 ## Installation
 
 1. Install Python 3.7 or newer (3.8 or newer if you're on Windows).
 1. Install Git 2.27 or newer.
 1. To use as a CLI app: `pipx install copier`
 1. To use as a library: `pip install copier` or `conda install -c conda-forge copier`
+1. To use with 100% reproducibility: `nix profile install github:copier-org/copier`
 
 ## Quick start
 
 To create a template:
 
 ```shell
-📁 my_copier_template ------------------------ # your template project
-├── 📄 copier.yml ---------------------------- # your template configuration
-├── 📁 .git ---------------------------------- # your template is a Git repository
-├── 📁 {{project_name}} ---------------------- # a folder with a templated name
-│   └── 📄 {{module_name}}.py.jinja ---------- # a file with a templated name
-└── 📄 {{_copier_conf.answers_file}}.jinja --- # answers are recorded here
+📁 my_copier_template                        # your template project
+├── 📄 copier.yml                            # your template configuration
+├── 📁 .git/                                 # your template is a Git repository
+├── 📁 {{project_name}}                      # a folder with a templated name
+│   └── 📄 {{module_name}}.py.jinja          # a file with a templated name
+└── 📄 {{_copier_conf.answers_file}}.jinja   # answers are recorded here
 ```
 
 ```yaml title="copier.yml"
 # questions
 project_name:
     type: str
     help: What is your project name?
@@ -134,12 +135,20 @@
 
 Special thanks go to [jpsca](https://github.com/jpsca) for originally creating `Copier`.
 This project would not be a thing without him.
 
 Many thanks to [pykong](https://github.com/pykong) who took over maintainership on the
 project, promoted it, and laid out the bases of what the project is today.
 
-Big thanks also go to [Yajo](https://github.com/Yajo) for his relentless zest for
+Big thanks also go to [yajo](https://github.com/yajo) for his relentless zest for
 improving `Copier` even further.
 
 Thanks a lot, [pawamoy](https://github.com/pawamoy) for polishing very important rough
 edges and improving the documentation and UX a lot.
+
+Also special thanks to [sisp](https://github.com/sisp) for being very helpful in
+polishing documentation, fixing bugs, helping the community and cleaning up the
+codebase.
+
+And thanks to all financial supporters and folks that give us a shiny star! ⭐
+
+[![Star History Chart](https://api.star-history.com/svg?repos=copier-org/copier&type=Date)](https://star-history.com/#copier-org/copier&Date)
```

### Comparing `copier-7.1.0a0/copier/cli.py` & `copier-7.2.0/copier/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 """
 Command line entrypoint. This module declares the Copier CLI applications.
 
 Basically, there are 3 different commands you can run:
 
 -   [`copier`][copier.cli.CopierApp], the main app, which is a shortcut for the
     `copy` and `update` subapps.
@@ -47,21 +46,19 @@
 import sys
 from functools import wraps
 from io import StringIO
 from pathlib import Path
 from textwrap import dedent
 from unittest.mock import patch
 
-import yaml
 from plumbum import cli, colors
 
-from copier.tools import copier_version
-
 from .errors import UserMessageError
 from .main import Worker
+from .tools import copier_version
 from .types import AnyByStrDict, OptStr, StrSeq
 
 
 def handle_exceptions(method):
     """Handle keyboard interruption while running a method."""
 
     @wraps(method)
@@ -126,23 +123,14 @@
         ["-a", "--answers-file"],
         default=None,
         help=(
             "Update using this path (relative to `destination_path`) "
             "to find the answers file"
         ),
     )
-    conflict: cli.SwitchAttr = cli.SwitchAttr(
-        ["-o", "--conflict"],
-        cli.Set("rej", "inline"),
-        default="rej",
-        help=(
-            "Behavior on conflict: rej=Create .rej file, inline=inline conflict "
-            "markers"
-        ),
-    )
     exclude: cli.SwitchAttr = cli.SwitchAttr(
         ["-x", "--exclude"],
         str,
         list=True,
         help=(
             "A name or shell-style pattern matching files or folders "
             "that must not be copied"
@@ -197,15 +185,14 @@
 
         Arguments:
             values: The list of values to apply.
                 Each value in the list is of the following form: `NAME=VALUE`.
         """
         for arg in values:
             key, value = arg.split("=", 1)
-            value = yaml.safe_load(value)
             self.data[key] = value
 
     def _worker(self, src_path: OptStr = None, dst_path: str = ".", **kwargs) -> Worker:
         """
         Run Copier's internal API using CLI switches.
 
         Arguments:
@@ -217,19 +204,19 @@
             data=self.data,
             dst_path=Path(dst_path),
             answers_file=self.answers_file,
             exclude=self.exclude,
             defaults=self.force or self.defaults,
             overwrite=self.force or self.overwrite,
             pretend=self.pretend,
+            skip_if_exists=self.skip,
             quiet=self.quiet,
             src_path=src_path,
             vcs_ref=self.vcs_ref,
             use_prereleases=self.prereleases,
-            conflict=self.conflict,
             **kwargs,
         )
 
     @handle_exceptions
     def main(self, *args: str) -> int:
         """Copier CLI app shortcuts.
 
@@ -311,14 +298,17 @@
 
 @CopierApp.subcommand("update")
 class CopierUpdateSubApp(cli.Application):
     """The `copier update` subcommand.
 
     Use this subcommand to update an existing subproject from a template
     that supports updates.
+
+    Attributes:
+        conflict: Set [conflict][] option.
     """
 
     DESCRIPTION = "Update a copy from its original template"
     DESCRIPTION_MORE = dedent(
         """\
         The copy must have a valid answers file which contains info
         from the last Copier execution, including the source template
@@ -327,35 +317,53 @@
         If that file contains also `_commit` and `destination_path` is a git
         repository, this command will do its best to respect the diff that you have
         generated since the last `copier` execution. To avoid that, use `copier copy`
         instead.
         """
     )
 
+    conflict: cli.SwitchAttr = cli.SwitchAttr(
+        ["-o", "--conflict"],
+        cli.Set("rej", "inline"),
+        default="rej",
+        help=(
+            "Behavior on conflict: rej=Create .rej file, inline=inline conflict "
+            "markers (inline is still experimental)"
+        ),
+    )
+    context_lines: cli.SwitchAttr = cli.SwitchAttr(
+        ["-c", "--context-lines"],
+        int,
+        default=1,
+        help=(
+            "Lines of context to use for detecting conflicts. Increase for "
+            "accuracy, decrease for resilience."
+        ),
+    )
+
     @handle_exceptions
     def main(self, destination_path: cli.ExistingDirectory = ".") -> int:
         """Call [run_update][copier.main.Worker.run_update].
 
         Parameters:
             destination_path:
                 Only the destination path is needed to update, because the
                 `src_path` comes from [the answers file][the-copier-answersyml-file].
 
                 The subproject must exist. If not specified, the currently
                 working directory is used.
         """
         self.parent._worker(
             dst_path=destination_path,
+            conflict=self.conflict,
+            context_lines=self.context_lines,
         ).run_update()
         return 0
 
 
 # Add --help-all results to docs
 if __doc__:
     help_io = StringIO()
     with patch("sys.stdout", help_io):
         CopierApp.run(["copier", "--help-all"], exit=False)
     help_io.seek(0)
     __doc__ += f"\n\nCLI help generated from `copier --help-all`:\n\n```\n{help_io.read()}\n```"
-
-if __name__ == "__main__":
-    CopierApp.run()
```

### Comparing `copier-7.1.0a0/copier/errors.py` & `copier-7.2.0/copier/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,7 +109,11 @@
 
 class OldTemplateWarning(UserWarning, CopierWarning):
     """Template was designed for an older Copier version."""
 
 
 class DirtyLocalWarning(UserWarning, CopierWarning):
     """Changes and untracked files present in template."""
+
+
+class ShallowCloneWarning(UserWarning, CopierWarning):
+    """The template repository is a shallow clone."""
```

### Comparing `copier-7.1.0a0/copier/main.py` & `copier-7.2.0/copier/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """Main functions and classes, used to generate or update projects."""
 
-import contextlib
 import os
 import platform
 import subprocess
 import sys
 from contextlib import suppress
 from dataclasses import asdict, field, replace
 from filecmp import dircmp
 from functools import partial
 from itertools import chain
 from pathlib import Path
-from shutil import copyfile, rmtree
-from typing import Callable, Iterable, List, Mapping, Optional, Sequence, Set
+from shutil import rmtree
+from typing import Callable, Iterable, Mapping, Optional, Sequence, Union
 from unicodedata import normalize
 
 from jinja2.loaders import FileSystemLoader
 from jinja2.sandbox import SandboxedEnvironment
 from pathspec import PathSpec
 from plumbum import ProcessExecutionError, colors
 from plumbum.cli.terminal import ask
 from plumbum.cmd import git
 from plumbum.machines import local
-from pydantic import ConfigDict, Extra
+from pydantic import ConfigDict, Extra, PositiveInt
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 from questionary import unsafe_prompt
 
 from .errors import CopierAnswersInterrupt, ExtensionNotFoundError, UserMessageError
 from .subproject import Subproject
 from .template import Task, Template
-from .tools import Style, TemporaryDirectory, printf
+from .tools import Style, TemporaryDirectory, printf, readlink
 from .types import (
+    MISSING,
     AnyByStrDict,
     JSONSerializable,
+    Literal,
     OptStr,
     RelativePath,
     StrOrPath,
     StrSeq,
 )
 from .user_data import DEFAULT_DATA, AnswersMap, Question
 
@@ -75,15 +76,17 @@
     -   [run_copy][copier.main.Worker.run_copy] to copy a subproject.
     -   [run_update][copier.main.Worker.run_update] to update a subproject.
     -   [run_auto][copier.main.Worker.run_auto] to let it choose whether you
         want to copy or update the subproject.
 
     Example:
         ```python
-        with Worker(src_path="https://github.com/copier-org/autopretty.git", "output") as worker:
+        with Worker(
+            src_path="https://github.com/copier-org/autopretty.git", "output"
+        ) as worker:
             worker.run_copy()
         ```
 
     Attributes:
         src_path:
             String that can be resolved to a template path, be it local or remote.
 
@@ -150,14 +153,23 @@
         quiet:
             When `True`, disable all output.
 
             See [quiet][].
 
         conflict:
             One of "rej" (default), "inline" (still experimental).
+
+        context_lines:
+            Lines of context to consider when solving conflicts in updates.
+
+            With more lines, context resolution is more accurate, but it will
+            also produce more conflicts if your subproject has evolved.
+
+            With less lines, context resolution is less accurate, but it will
+            respect better the evolution of your subproject.
     """
 
     src_path: Optional[str] = None
     dst_path: Path = field(default=Path("."))
     answers_file: Optional[RelativePath] = None
     vcs_ref: OptStr = None
     data: AnyByStrDict = field(default_factory=dict)
@@ -167,19 +179,22 @@
     cleanup_on_error: bool = True
     defaults: bool = False
     user_defaults: AnyByStrDict = field(default_factory=dict)
     overwrite: bool = False
     pretend: bool = False
     quiet: bool = False
     conflict: str = "rej"
+    context_lines: PositiveInt = 1
 
     def __enter__(self):
+        """Allow using worker as a context manager."""
         return self
 
     def __exit__(self, type, value, traceback):
+        """Clean up garbage files after worker usage ends."""
         if value is not None:
             # exception was raised from code inside context manager:
             # try to clean up, ignoring any exception, then re-raise
             with suppress(Exception):
                 self._cleanup()
             raise value
         # otherwise clean up and let any exception bubble up
@@ -225,27 +240,30 @@
                 use_shell = False
             if not self.quiet:
                 print(
                     colors.info
                     | f" > Running task {i + 1} of {len(tasks)}: {task_cmd}",
                     file=sys.stderr,
                 )
+            if self.pretend:
+                continue
             with local.cwd(self.subproject.local_abspath), local.env(**task.extra_env):
                 subprocess.run(task_cmd, shell=use_shell, check=True, env=local.env)
 
     def _render_context(self) -> Mapping:
         """Produce render context for Jinja."""
         # Backwards compatibility
         # FIXME Remove it?
         conf = asdict(self)
         conf.update(
             {
                 "answers_file": self.answers_relpath,
                 "src_path": self.template.local_abspath,
                 "vcs_ref_hash": self.template.commit_hash,
+                "sep": os.sep,
             }
         )
 
         return dict(
             DEFAULT_DATA,
             **self.answers.combined,
             _copier_answers=self._answers_to_remember(),
@@ -294,134 +312,136 @@
             return True
         return bool(ask(f" Overwrite {dst_relpath}?", default=True))
 
     def _render_allowed(
         self,
         dst_relpath: Path,
         is_dir: bool = False,
-        expected_contents: bytes = b"",
-        expected_permissions=None,
+        is_symlink: bool = False,
+        expected_contents: Union[bytes, Path] = b"",
     ) -> bool:
         """Determine if a file or directory can be rendered.
 
         Args:
-
             dst_relpath:
                 Relative path to destination.
             is_dir:
                 Indicate if the path must be treated as a directory or not.
+            is_symlink:
+                Indicate if the path must be treated as a symlink or not.
             expected_contents:
                 Used to compare existing file contents with them. Allows to know if
                 rendering is needed.
         """
         assert not dst_relpath.is_absolute()
         assert not expected_contents or not is_dir, "Dirs cannot have expected content"
         dst_abspath = Path(self.subproject.local_abspath, dst_relpath)
         if dst_relpath != Path(".") and self.match_exclude(dst_relpath):
             return False
         try:
-            previous_content = dst_abspath.read_bytes()
+            previous_content: Union[bytes, Path]
+            if is_symlink:
+                previous_content = readlink(dst_abspath)
+            else:
+                previous_content = dst_abspath.read_bytes()
         except FileNotFoundError:
             printf(
                 "create",
                 dst_relpath,
                 style=Style.OK,
                 quiet=self.quiet,
                 file_=sys.stderr,
             )
             return True
-        except (IsADirectoryError, PermissionError) as error:
+        except PermissionError as error:
             # HACK https://bugs.python.org/issue43095
-            if isinstance(error, PermissionError) and not (
-                error.errno == 13 and platform.system() == "Windows"
-            ):
+            if not (error.errno == 13 and platform.system() == "Windows"):
                 raise
-            if is_dir:
-                printf(
-                    "identical",
-                    dst_relpath,
-                    style=Style.IGNORE,
-                    quiet=self.quiet,
-                    file_=sys.stderr,
-                )
-                return True
-            return self._solve_render_conflict(dst_relpath)
-        else:
-            if previous_content == expected_contents:
-                printf(
-                    "identical",
-                    dst_relpath,
-                    style=Style.IGNORE,
-                    quiet=self.quiet,
-                    file_=sys.stderr,
-                )
-                return True
-            return self._solve_render_conflict(dst_relpath)
+        except IsADirectoryError:
+            assert is_dir
+        if is_dir or previous_content == expected_contents:
+            printf(
+                "identical",
+                dst_relpath,
+                style=Style.IGNORE,
+                quiet=self.quiet,
+                file_=sys.stderr,
+            )
+            return True
+        return self._solve_render_conflict(dst_relpath)
 
     @cached_property
     def answers(self) -> AnswersMap:
         """Container of all answers to the questionary.
 
         It asks the user the 1st time it is called, if running interactively.
         """
         result = AnswersMap(
             default=self.template.default_answers,
             user_defaults=self.user_defaults,
             init=self.data,
             last=self.subproject.last_answers,
             metadata=self.template.metadata,
         )
-        questions: List[Question] = []
+
         for var_name, details in self.template.questions_data.items():
+            question = Question(
+                answers=result,
+                jinja_env=self.jinja_env,
+                var_name=var_name,
+                **details,
+            )
             if var_name in result.init:
-                # Do not ask again
+                # Try to parse the answer value.
+                answer = question.parse_answer(result.init[var_name])
+                # Try to validate the answer value if the question has a
+                # validator.
+                question.validate_answer(answer)
+                # At this point, the answer value is valid. Do not ask the
+                # question again, but set answer as the user's answer instead.
+                result.user[var_name] = answer
                 continue
-            questions.append(
-                Question(
-                    answers=result,
-                    ask_user=not self.defaults,
-                    jinja_env=self.jinja_env,
-                    var_name=var_name,
-                    **details,
-                )
-            )
-        for question in questions:
+
             # Display TUI and ask user interactively only without --defaults
             try:
-                new_answer = (
-                    question.get_default()
-                    if self.defaults
-                    else unsafe_prompt(
+                if self.defaults:
+                    new_answer = question.get_default()
+                    if new_answer is MISSING:
+                        raise ValueError(f'Question "{var_name}" is required')
+                else:
+                    new_answer = unsafe_prompt(
                         [question.get_questionary_structure()], answers=result.combined
                     )[question.var_name]
-                )
             except KeyboardInterrupt as err:
                 raise CopierAnswersInterrupt(result, question, self.template) from err
             previous_answer = result.combined.get(question.var_name)
             # If question was skipped and it's the 1st
             # run, you could be getting a raw templated value
             default_answer = result.default.get(question.var_name)
             if new_answer == default_answer:
                 new_answer = question.render_value(default_answer)
                 new_answer = question.filter_answer(new_answer)
             if new_answer != previous_answer:
                 result.user[question.var_name] = new_answer
+
         return result
 
     @cached_property
     def answers_relpath(self) -> Path:
         """Obtain the proper relative path for the answers file.
 
         It comes from:
 
         1. User choice.
         2. Template default.
         3. Copier default.
         """
-        return self.answers_file or self.template.answers_relpath
+        path = self.answers_file or self.template.answers_relpath
+        template = self.jinja_env.from_string(str(path))
+        return Path(template.render(**self.answers.combined))
 
     @cached_property
     def all_exclusions(self) -> StrSeq:
         """Combine default, template and user-chosen exclusions."""
         return self.template.exclude + tuple(self.exclude)
 
     @cached_property
@@ -450,14 +470,28 @@
                 "Make sure to install these extensions alongside Copier itself.\n"
                 "See the docs at https://copier.readthedocs.io/en/latest/configuring/#jinja_extensions"
             )
         # patch the `to_json` filter to support Pydantic dataclasses
         env.filters["to_json"] = partial(
             env.filters["to_json"], default=pydantic_encoder
         )
+
+        # Add a global function to join filesystem paths.
+        separators = {
+            "posix": "/",
+            "windows": "\\",
+            "native": os.path.sep,
+        }
+
+        def _pathjoin(
+            *path: str, mode: Literal["posix", "windows", "native"] = "posix"
+        ) -> str:
+            return separators[mode].join(path)
+
+        env.globals["pathjoin"] = _pathjoin
         return env
 
     @cached_property
     def match_exclude(self) -> Callable[[Path], bool]:
         """Get a callable to match paths against all exclusions."""
         return self._path_matcher(self.all_exclusions)
 
@@ -471,15 +505,14 @@
             )
         )
 
     def _render_file(self, src_abspath: Path) -> None:
         """Render one file.
 
         Args:
-
             src_abspath:
                 The absolute path to the file that will be rendered.
         """
         # TODO Get from main.render_file()
         assert src_abspath.is_absolute()
         src_relpath = src_abspath.relative_to(self.template.local_abspath).as_posix()
         src_renderpath = src_abspath.relative_to(self.template_copy_root)
@@ -496,26 +529,60 @@
                 # suffix is empty, fallback to copy
                 new_content = src_abspath.read_bytes()
             else:
                 new_content = tpl.render(**self._render_context()).encode()
         else:
             new_content = src_abspath.read_bytes()
         dst_abspath = Path(self.subproject.local_abspath, dst_relpath)
-        if dst_abspath.is_dir():
-            return
         src_mode = src_abspath.stat().st_mode
+        if not self._render_allowed(dst_relpath, expected_contents=new_content):
+            return
+        if not self.pretend:
+            dst_abspath.parent.mkdir(parents=True, exist_ok=True)
+            dst_abspath.write_bytes(new_content)
+            dst_abspath.chmod(src_mode)
+
+    def _render_symlink(self, src_abspath: Path) -> None:
+        """Render one symlink.
+
+        Args:
+            src_abspath:
+                Symlink to be rendered. It must be an absolute path within
+                the template.
+        """
+        assert src_abspath.is_absolute()
+        src_relpath = src_abspath.relative_to(self.template_copy_root)
+        dst_relpath = self._render_path(src_relpath)
+        if dst_relpath is None:
+            return
+        dst_abspath = Path(self.subproject.local_abspath, dst_relpath)
+
+        src_target = readlink(src_abspath)
+        if src_abspath.name.endswith(self.template.templates_suffix):
+            dst_target = Path(self._render_string(str(src_target)))
+        else:
+            dst_target = src_target
+
         if not self._render_allowed(
             dst_relpath,
-            expected_contents=new_content,
-            expected_permissions=src_mode,
+            expected_contents=dst_target,
+            is_symlink=True,
         ):
             return
+
         if not self.pretend:
-            dst_abspath.write_bytes(new_content)
-            dst_abspath.chmod(src_mode)
+            # symlink_to doesn't overwrite existing files, so delete it first
+            if dst_abspath.is_symlink() or dst_abspath.exists():
+                dst_abspath.unlink()
+            dst_abspath.symlink_to(dst_target)
+            if sys.platform == "darwin":
+                # Only macOS supports permissions on symlinks.
+                # Other platforms just copy the permission of the target
+                src_mode = src_abspath.lstat().st_mode
+                dst_abspath.lchmod(src_mode)
 
     def _render_folder(self, src_abspath: Path) -> None:
         """Recursively render a folder.
 
         Args:
             src_path:
                 Folder to be rendered. It must be an absolute path within
@@ -530,14 +597,16 @@
             return
         dst_abspath = Path(self.subproject.local_abspath, dst_relpath)
         if not self.pretend:
             dst_abspath.mkdir(parents=True, exist_ok=True)
         for file in src_abspath.iterdir():
             if file.is_dir():
                 self._render_folder(file)
+            elif file.is_symlink() and self.template.preserve_symlinks:
+                self._render_symlink(file)
             else:
                 self._render_file(file)
 
     def _render_path(self, relpath: Path) -> Optional[Path]:
         """Render one relative path.
 
         Args:
@@ -547,28 +616,27 @@
         is_template = relpath.name.endswith(self.template.templates_suffix)
         templated_sibling = (
             self.template.local_abspath / f"{relpath}{self.template.templates_suffix}"
         )
         # With an empty suffix, the templated sibling always exists.
         if templated_sibling.exists() and self.template.templates_suffix:
             return None
+        if self.template.templates_suffix and is_template:
+            relpath = relpath.with_suffix("")
         rendered_parts = []
         for part in relpath.parts:
             # Skip folder if any part is rendered as an empty string
             part = self._render_string(part)
             if not part:
                 return None
+            # {{ _copier_conf.answers_file }} becomes the full path; in that case,
+            # restore part to be just the end leaf
+            if str(self.answers_relpath) == part:
+                part = Path(part).name
             rendered_parts.append(part)
-        with suppress(IndexError):
-            # With an empty suffix, the next instruction
-            # would erroneously empty the last rendered part
-            if is_template and self.template.templates_suffix:
-                rendered_parts[-1] = rendered_parts[-1][
-                    : -len(self.template.templates_suffix)
-                ]
         result = Path(*rendered_parts)
         if not is_template:
             templated_sibling = (
                 self.template.local_abspath
                 / f"{result}{self.template.templates_suffix}"
             )
             if templated_sibling.exists():
@@ -696,190 +764,138 @@
             # TODO Unify printing tools
             print(
                 f"Updating to template version {self.template.version}", file=sys.stderr
             )
         self._apply_update()
 
     def _apply_update(self):
-        if self.conflict == "inline":
-            # New implementation.
-            self._apply_update_inline_conflict_markers()
-            return
+        subproject_top = Path(
+            git(
+                "-C",
+                self.subproject.local_abspath,
+                "rev-parse",
+                "--show-toplevel",
+            ).strip()
+        )
+        subproject_subdir = self.subproject.local_abspath.relative_to(subproject_top)
 
-        # Old implementation.
-        # Copy old template into a temporary destination
         with TemporaryDirectory(
-            prefix=f"{__name__}.update_diff."
-        ) as old_copy, TemporaryDirectory(
-            prefix=f"{__name__}.recopy_diff."
-        ) as new_copy:
-            old_worker = self._make_old_worker(old_copy)
-            old_worker.run_copy()
-            recopy_worker = replace(
+            prefix=f"{__name__}.old_copy."
+        ) as old_copy, TemporaryDirectory(prefix=f"{__name__}.new_copy.") as new_copy:
+            # Copy old template into a temporary destination
+            old_worker = replace(
                 self,
-                dst_path=new_copy,
+                dst_path=old_copy / subproject_subdir,
                 data=self.subproject.last_answers,
                 defaults=True,
                 quiet=True,
                 src_path=self.subproject.template.url,
+                vcs_ref=self.subproject.template.commit,
             )
-            recopy_worker.run_copy()
-            compared = dircmp(old_copy, new_copy)
+            old_worker.run_copy()
             # Extract diff between temporary destination and real destination
             with local.cwd(old_copy):
-                subproject_top = git(
-                    "-C",
-                    self.subproject.local_abspath.absolute(),
-                    "rev-parse",
-                    "--show-toplevel",
-                ).strip()
                 self._git_initialize_repo()
-                git("remote", "add", "real_dst", "file://" + subproject_top)
+                git("remote", "add", "real_dst", "file://" + str(subproject_top))
                 git("fetch", "--depth=1", "real_dst", "HEAD")
-                diff_cmd = git["diff-tree", "--unified=1", "HEAD...FETCH_HEAD"]
+                diff_cmd = git[
+                    "diff-tree", f"--unified={self.context_lines}", "HEAD...FETCH_HEAD"
+                ]
                 try:
                     diff = diff_cmd("--inter-hunk-context=-1")
                 except ProcessExecutionError:
                     print(
                         colors.warn
                         | "Make sure Git >= 2.24 is installed to improve updates.",
                         file=sys.stderr,
                     )
                     diff = diff_cmd("--inter-hunk-context=0")
             # Run pre-migration tasks
             self._execute_tasks(
                 self.template.migration_tasks("before", self.subproject.template)
             )
-            self._uncached_copy()
+            # Clear last answers cache to load possible answers migration
+            with suppress(AttributeError):
+                del self.answers
+            with suppress(AttributeError):
+                del self.subproject.last_answers
+            # Do a normal update in final destination
+            self.run_copy()
+            # Render with the same answers in an empty dir to avoid pollution
+            new_worker = replace(
+                self,
+                dst_path=new_copy / subproject_subdir,
+                data=self.answers.combined,
+                defaults=True,
+                quiet=True,
+                src_path=self.subproject.template.url,
+            )
+            new_worker.run_copy()
+            compared = dircmp(old_copy, new_copy)
             # Try to apply cached diff into final destination
-            with local.cwd(self.subproject.local_abspath):
+            with local.cwd(subproject_top):
                 apply_cmd = git["apply", "--reject", "--exclude", self.answers_relpath]
                 for skip_pattern in chain(
                     self.skip_if_exists, self.template.skip_if_exists
                 ):
                     apply_cmd = apply_cmd["--exclude", skip_pattern]
                 (apply_cmd << diff)(retcode=None)
-
+                # TODO Test more, remove from experimental, make default
+                if self.conflict == "inline":
+                    status = git("status", "--porcelain").strip().splitlines()
+                    for line in status:
+                        # Find merge rejections
+                        if not (line.startswith("?? ") and line.endswith(".rej")):
+                            continue
+                        # FIXME Test with a file named '`â ñ"', see it fail, fix it
+                        fname = line[3:-4]
+                        # Undo possible non-rejected chunks
+                        git("checkout", "--", fname)
+                        # 3-way-merge the file directly
+                        git(
+                            "merge-file",
+                            "-L",
+                            "before updating",
+                            "-L",
+                            "last update",
+                            "-L",
+                            "after updating",
+                            fname,
+                            Path(old_copy) / fname,
+                            Path(new_copy) / fname,
+                            retcode=None,
+                        )
+                        # Remove rejection witness
+                        Path(f"{fname}.rej").unlink()
             # Trigger recursive removal of deleted files in last template version
-            _remove_old_files(self.subproject.local_abspath, compared)
-
-        # Run post-migration tasks
-        self._execute_tasks(
-            self.template.migration_tasks("after", self.subproject.template)
-        )
-
-    def _apply_update_inline_conflict_markers(self):
-        """Implements the apply_update() method using inline conflict markers."""
-        # Copy old template into a temporary destination
-        with TemporaryDirectory(
-            prefix=f"{__name__}.update_diff.reference."
-        ) as reference_dst_temp, TemporaryDirectory(
-            prefix=f"{__name__}.update_diff.original."
-        ) as old_copy, TemporaryDirectory(
-            prefix=f"{__name__}.update_diff.merge."
-        ) as merge_dst_temp:
-            # Copy reference to be used as base by merge-file
-            copytree(self.dst_path, reference_dst_temp, dirs_exist_ok=True)
-
-            # Compute modification from the original template to be used as other by merge-file
-            assert self.subproject
-            assert self.subproject.template
-            old_worker = self._make_old_worker(old_copy)
-            old_worker.run_copy()
-            with local.cwd(old_copy):
-                self._git_initialize_repo()
-
-            # Run pre-migration tasks
-            self._execute_tasks(
-                self.template.migration_tasks("before", self.subproject.template)
-            )
-            self._uncached_copy()
-
-            # Extract the list of files to merge
-            participating_files: Set[Path] = set()
-            for src_dir in (old_copy, reference_dst_temp):
-                for root, dirs, files in os.walk(src_dir, topdown=True):
-                    if root == src_dir and ".git" in dirs:
-                        dirs.remove(".git")
-                    root = Path(root).relative_to(src_dir)
-                    participating_files.update(Path(root, f) for f in files)
-
-            # Merging files
-            for basename in sorted(participating_files):
-                subfile_names = []
-                for subfile_kind, src_dir in [
-                    ("modified", reference_dst_temp),
-                    ("old upstream", old_copy),
-                    ("new upstream", self.dst_path),
-                ]:
-                    path = Path(src_dir, basename)
-                    if path.is_file():
-                        copyfile(path, Path(merge_dst_temp, subfile_kind))
-                    else:
-                        subfile_kind = os.devnull
-                    subfile_names.append(subfile_kind)
-
-                with local.cwd(merge_dst_temp):
-                    # https://git-scm.com/docs/git-merge-file
-                    output = git("merge-file", "-p", *subfile_names, retcode=None)
-
-                dest_path = Path(self.dst_path, basename)
-                # Remove the file if it was already removed in the project
-                if not output and "modified" not in subfile_names:
-                    with contextlib.suppress(FileNotFoundError):
-                        dest_path.unlink()
-                else:
-                    dest_path.parent.mkdir(parents=True, exist_ok=True)
-                    dest_path.write_text(output)
+            _remove_old_files(subproject_top, compared)
 
         # Run post-migration tasks
         self._execute_tasks(
             self.template.migration_tasks("after", self.subproject.template)
         )
 
-    def _uncached_copy(self):
-        """Copy template to destination without using answer cache."""
-        # Clear last answers cache to load possible answers migration
-        with suppress(AttributeError):
-            del self.answers
-        with suppress(AttributeError):
-            del self.subproject.last_answers
-        # Do a normal update in final destination
-        self.run_copy()
-
-    def _make_old_worker(self, old_copy):
-        """Create a worker to copy the old template into a temporary destination."""
-        old_worker = replace(
-            self,
-            dst_path=old_copy,
-            data=self.subproject.last_answers,
-            defaults=True,
-            quiet=True,
-            src_path=self.subproject.template.url,
-            vcs_ref=self.subproject.template.commit,
-        )
-        return old_worker
-
     def _git_initialize_repo(self):
         """Initialize a git repository in the current directory."""
         git("init", retcode=None)
         git("add", ".")
         git("config", "user.name", "Copier")
         git("config", "user.email", "copier@copier")
         # 1st commit could fail if any pre-commit hook reformats code
+        # 2nd commit uses --no-verify to disable pre-commit-like checks
         git("commit", "--allow-empty", "-am", "dumb commit 1", retcode=None)
-        git("commit", "--allow-empty", "-am", "dumb commit 2")
+        git("commit", "--allow-empty", "-am", "dumb commit 2", "--no-verify")
         git("config", "--unset", "user.name")
         git("config", "--unset", "user.email")
 
 
 def run_copy(
     src_path: str,
     dst_path: StrOrPath = ".",
-    data: AnyByStrDict = None,
+    data: Optional[AnyByStrDict] = None,
     **kwargs,
 ) -> Worker:
     """Copy a template to a destination, from zero.
 
     This is a shortcut for [run_copy][copier.main.Worker.run_copy].
 
     See [Worker][copier.main.Worker] fields to understand this function's args.
@@ -889,15 +905,15 @@
     with Worker(src_path=src_path, dst_path=Path(dst_path), **kwargs) as worker:
         worker.run_copy()
     return worker
 
 
 def run_update(
     dst_path: StrOrPath = ".",
-    data: AnyByStrDict = None,
+    data: Optional[AnyByStrDict] = None,
     **kwargs,
 ) -> Worker:
     """Update a subproject, from its template.
 
     This is a shortcut for [run_update][copier.main.Worker.run_update].
 
     See [Worker][copier.main.Worker] fields to understand this function's args.
@@ -908,15 +924,15 @@
         worker.run_update()
     return worker
 
 
 def run_auto(
     src_path: OptStr = None,
     dst_path: StrOrPath = ".",
-    data: AnyByStrDict = None,
+    data: Optional[AnyByStrDict] = None,
     **kwargs,
 ) -> Worker:
     """Generate or update a subproject.
 
     This is a shortcut for [run_auto][copier.main.Worker.run_auto].
 
     See [Worker][copier.main.Worker] fields to understand this function's args.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `copier-7.1.0a0/copier/subproject.py` & `copier-7.2.0/copier/subproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,26 +35,26 @@
             Relative path to [the answers file][the-copier-answersyml-file].
     """
 
     local_abspath: AbsolutePath
     answers_relpath: Path = Path(".copier-answers.yml")
 
     def is_dirty(self) -> bool:
-        """Indicates if the local template root is dirty.
+        """Indicate if the local template root is dirty.
 
         Only applicable for VCS-tracked templates.
         """
         if self.vcs == "git":
             with local.cwd(self.local_abspath):
                 return bool(git("status", "--porcelain").strip())
         return False
 
     @property
     def _raw_answers(self) -> AnyByStrDict:
-        """The last answers, loaded raw as yaml."""
+        """Get last answers, loaded raw as yaml."""
         try:
             return yaml.safe_load(
                 (self.local_abspath / self.answers_relpath).read_text()
             )
         except OSError:
             return {}
```

### Comparing `copier-7.1.0a0/copier/template.py` & `copier-7.2.0/copier/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,38 +84,44 @@
     Params:
         conf_path: The path to the `copier.yml` file.
         quiet: Used to configure the exception.
 
     Raises:
         InvalidConfigFileError: When the file is formatted badly.
     """
+
+    class _Loader(yaml.FullLoader):
+        """Intermediate class to avoid monkey-patching main loader."""
+
     YamlIncludeConstructor.add_to_loader_class(
-        loader_class=yaml.FullLoader, base_dir=conf_path.parent
+        loader_class=_Loader, base_dir=conf_path.parent
     )
 
-    try:
-        with open(conf_path) as f:
-            flattened_result = lflatten(yaml.load_all(f, Loader=yaml.FullLoader))
-            merged_options = defaultdict(list)
-            for option in (
-                "_exclude",
-                "_jinja_extensions",
-                "_secret_questions",
-                "_skip_if_exists",
-            ):
-                for result in flattened_result:
-                    try:
-                        values = result[option]
-                    except KeyError:
-                        pass
-                    else:
-                        merged_options[option].extend(values)
-            return dict(ChainMap(dict(merged_options), *reversed(flattened_result)))
-    except yaml.parser.ParserError as e:
-        raise InvalidConfigFileError(conf_path, quiet) from e
+    with open(conf_path) as f:
+        try:
+            flattened_result = lflatten(yaml.load_all(f, Loader=_Loader))
+        except yaml.parser.ParserError as e:
+            raise InvalidConfigFileError(conf_path, quiet) from e
+
+    merged_options = defaultdict(list)
+    for option in (
+        "_exclude",
+        "_jinja_extensions",
+        "_secret_questions",
+        "_skip_if_exists",
+    ):
+        for result in flattened_result:
+            try:
+                values = result[option]
+            except KeyError:
+                pass
+            else:
+                merged_options[option].extend(values)
+
+    return dict(ChainMap(dict(merged_options), *reversed(flattened_result)))
 
 
 def verify_copier_version(version_str: str) -> None:
     """Raise an error if the current Copier version is less than the given version.
 
     Args:
         version_str:
@@ -296,15 +302,20 @@
 
     @cached_property
     def exclude(self) -> Tuple[str, ...]:
         """Get exclusions specified in the template, or default ones.
 
         See [exclude][].
         """
-        return tuple(self.config_data.get("exclude", DEFAULT_EXCLUDE))
+        return tuple(
+            self.config_data.get(
+                "exclude",
+                DEFAULT_EXCLUDE if Path(self.subdirectory) == Path(".") else [],
+            )
+        )
 
     @cached_property
     def jinja_extensions(self) -> Tuple[str, ...]:
         """Get Jinja2 extensions specified in the template, or `()`.
 
         See [jinja_extensions][].
         """
@@ -356,15 +367,15 @@
                 }
                 for cmd in migration.get(stage, []):
                     result.append(Task(cmd=cmd, extra_env=extra_env))
         return result
 
     @cached_property
     def min_copier_version(self) -> Optional[Version]:
-        """Gets minimal copier version for the template and validates it.
+        """Get minimal copier version for the template and validates it.
 
         See [min_copier_version][].
         """
         try:
             return Version(self.config_data["min_copier_version"])
         except KeyError:
             return None
@@ -432,28 +443,38 @@
         """
         result = self.config_data.get("templates_suffix")
         if result is None:
             return DEFAULT_TEMPLATES_SUFFIX
         return result
 
     @cached_property
+    def preserve_symlinks(self) -> bool:
+        """Know if Copier should preserve symlinks when rendering the template.
+
+        See [preserve_symlinks][].
+        """
+        return bool(self.config_data.get("preserve_symlinks", False))
+
+    @cached_property
     def local_abspath(self) -> Path:
         """Get the absolute path to the template on disk.
 
         This may clone it if `url` points to a VCS-tracked template.
         Dirty changes for local VCS-tracked templates will be copied.
         """
         result = Path(self.url)
         if self.vcs == "git":
             result = Path(clone(self.url_expanded, self.ref))
             if self.ref is None:
                 checkout_latest_tag(result, self.use_prereleases)
         if not result.is_dir():
             raise ValueError("Local template must be a directory.")
-        return result.absolute()
+        with suppress(OSError):
+            result = result.resolve()
+        return result
 
     @cached_property
     def url_expanded(self) -> str:
         """Get usable URL.
 
         `url` can be specified in shortcut
         format, which wouldn't be understood by the underlying VCS system. This
```

### Comparing `copier-7.1.0a0/copier/tools.py` & `copier-7.2.0/copier/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 
 import colorama
 from packaging.version import Version
 from pydantic import StrictBool
 
 from .types import IntSeq
 
-try:
-    from importlib.metadata import version
-except ImportError:
-    # Python < 3.8
+# TODO Remove condition when dropping python 3.8 support
+if sys.version_info < (3, 8):
     from importlib_metadata import version
+else:
+    from importlib.metadata import version
 
 colorama.init()
 
 
 class Style:
+    """Common color styles."""
+
     OK: IntSeq = [colorama.Fore.GREEN, colorama.Style.BRIGHT]
     WARNING: IntSeq = [colorama.Fore.YELLOW, colorama.Style.BRIGHT]
     IGNORE: IntSeq = [colorama.Fore.CYAN]
     DANGER: IntSeq = [colorama.Fore.RED, colorama.Style.BRIGHT]
     RESET: IntSeq = [colorama.Fore.RESET, colorama.Style.RESET_ALL]
 
 
@@ -59,14 +61,15 @@
     action: str,
     msg: Any = "",
     style: Optional[IntSeq] = None,
     indent: int = 10,
     quiet: Union[bool, StrictBool] = False,
     file_: TextIO = sys.stdout,
 ) -> Optional[str]:
+    """Print string with common format."""
     if quiet:
         return None  # HACK: Satisfy MyPy
     _msg = str(msg)
     action = action.rjust(indent, " ")
     if not style:
         return action + _msg
 
@@ -74,14 +77,15 @@
     print(*out, sep="", file=file_)
     return None  # HACK: Satisfy MyPy
 
 
 def printf_exception(
     e: Exception, action: str, msg: str = "", indent: int = 0, quiet: bool = False
 ) -> None:
+    """Print exception with common format."""
     if not quiet:
         print("", file=sys.stderr)
         printf(action, msg=msg, style=Style.DANGER, indent=indent, file_=sys.stderr)
         print(HLINE, file=sys.stderr)
         print(e, file=sys.stderr)
         print(HLINE, file=sys.stderr)
 
@@ -110,14 +114,15 @@
         elif lower in {"n", "no", "f", "false", "off", "~", "null", "none"}:
             return False
     # Assume nothing
     return bool(value)
 
 
 def copy_file(src_path: Path, dst_path: Path, follow_symlinks: bool = True) -> None:
+    """Copy one file to another place."""
     shutil.copy2(src_path, dst_path, follow_symlinks=follow_symlinks)
 
 
 def force_str_end(original_str: str, end: str = "\n") -> str:
     """Make sure a `original_str` ends with `end`.
 
     Params:
@@ -162,13 +167,28 @@
 
     @classmethod
     def _cleanup(cls, name, warn_message):
         cls._robust_cleanup(name)
         warnings.warn(warn_message, ResourceWarning)
 
     def cleanup(self):
+        """Remove directory safely."""
         if self._finalizer.detach():
             self._robust_cleanup(self.name)
 
     @staticmethod
     def _robust_cleanup(name):
         shutil.rmtree(name, ignore_errors=False, onerror=handle_remove_readonly)
+
+
+def readlink(link: Path) -> Path:
+    """A custom version of os.readlink/pathlib.Path.readlink.
+
+    pathlib.Path.readlink is what we ideally would want to use, but it is only available on python>=3.9.
+    os.readlink doesn't support Path and bytes on Windows for python<3.8
+    """
+    if sys.version_info >= (3, 9):
+        return link.readlink()
+    elif sys.version_info >= (3, 8) or os.name != "nt":
+        return Path(os.readlink(link))
+    else:
+        return Path(os.readlink(str(link)))
```

### Comparing `copier-7.1.0a0/copier/types.py` & `copier-7.2.0/copier/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 """Complex types, annotations, validators."""
 
 import sys
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Sequence, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Mapping,
+    NewType,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
 
 from pydantic.validators import path_validator
 
 # HACK https://github.com/python/mypy/issues/8520#issuecomment-772081075
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
@@ -33,47 +43,57 @@
 OptStr = Optional[str]
 
 # miscellaneous
 T = TypeVar("T")
 JSONSerializable = (dict, list, str, int, float, bool, type(None))
 VCSTypes = Literal["git"]
 Env = Mapping[str, str]
+MissingType = NewType("MissingType", object)
+MISSING = MissingType(object())
 
 
 class AllowArbitraryTypes:
+    """Allow any type for this class."""
+
     arbitrary_types_allowed = True
 
 
 # Validators
 def path_is_absolute(value: Path) -> Path:
+    """Require absolute paths in an argument."""
     if not value.is_absolute():
         from .errors import PathNotAbsoluteError
 
         raise PathNotAbsoluteError(path=value)
     return value
 
 
 def path_is_relative(value: Path) -> Path:
+    """Require relative paths in an argument."""
     if value.is_absolute():
         from .errors import PathNotRelativeError
 
         raise PathNotRelativeError(path=value)
     return value
 
 
 # Validated types
 if TYPE_CHECKING:
     AbsolutePath = Path
     RelativePath = Path
 else:
 
     class AbsolutePath(Path):
+        """Require absolute paths in an argument."""
+
         @classmethod
         def __get_validators__(cls) -> "CallableGenerator":
             yield path_validator
             yield path_is_absolute
 
     class RelativePath(Path):
+        """Require relative paths in an argument."""
+
         @classmethod
         def __get_validators__(cls) -> "CallableGenerator":
             yield path_validator
             yield path_is_relative
```

### Comparing `copier-7.1.0a0/copier/user_data.py` & `copier-7.2.0/copier/user_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from hashlib import sha512
 from os import urandom
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
-    ChainMap as t_ChainMap,
     Dict,
     Mapping,
     Optional,
     Sequence,
     Union,
 )
 
@@ -28,15 +27,23 @@
 from pydantic import validator as pydantic_validator
 from pydantic.dataclasses import dataclass
 from pygments.lexers.data import JsonLexer, YamlLexer
 from questionary.prompts.common import Choice
 
 from .errors import InvalidTypeError, UserMessageError
 from .tools import cast_str_to_bool, force_str_end
-from .types import AllowArbitraryTypes, AnyByStrDict, OptStr, OptStrOrPath, StrOrPath
+from .types import (
+    MISSING,
+    AllowArbitraryTypes,
+    AnyByStrDict,
+    MissingType,
+    OptStr,
+    OptStrOrPath,
+    StrOrPath,
+)
 
 # HACK https://github.com/python/mypy/issues/8520#issuecomment-772081075
 if sys.version_info >= (3, 8):
     from functools import cached_property
 else:
     from backports.cached_property import cached_property
 
@@ -117,28 +124,29 @@
     init: AnyByStrDict = field(default_factory=dict)
     metadata: AnyByStrDict = field(default_factory=dict)
     last: AnyByStrDict = field(default_factory=dict)
     user_defaults: AnyByStrDict = field(default_factory=dict)
     default: AnyByStrDict = field(default_factory=dict)
 
     @cached_property
-    def combined(self) -> t_ChainMap[str, Any]:
+    def combined(self) -> Mapping[str, Any]:
         """Answers combined from different sources, sorted by priority."""
         return ChainMap(
             self.local,
             self.user,
             self.init,
             self.metadata,
             self.last,
             self.user_defaults,
             self.default,
             DEFAULT_DATA,
         )
 
     def old_commit(self) -> OptStr:
+        """Commit when the project was updated from this template the last time."""
         return self.last.get("_commit")
 
 
 @dataclass(config=AllowArbitraryTypes)
 class Question:
     """One question asked to the user.
 
@@ -191,17 +199,16 @@
             boolean values.
     """
 
     var_name: str
     answers: AnswersMap
     jinja_env: SandboxedEnvironment
     choices: Union[Dict[Any, Any], Sequence[Any]] = field(default_factory=list)
-    default: Any = None
+    default: Any = MISSING
     help: str = ""
-    ask_user: bool = False
     multiline: Union[str, bool] = False
     placeholder: str = ""
     secret: bool = False
     type: str = ""
     validator: str = ""
     when: Union[str, bool] = True
 
@@ -226,28 +233,32 @@
         except KeyError:
             try:
                 result = self.answers.last[self.var_name]
             except KeyError:
                 try:
                     result = self.answers.user_defaults[self.var_name]
                 except KeyError:
+                    if self.default is MISSING:
+                        return MISSING
                     result = self.render_value(self.default)
         result = cast_answer_type(result, cast_fn)
         return result
 
-    def get_default_rendered(self) -> Union[bool, str, Choice, None]:
+    def get_default_rendered(self) -> Union[bool, str, Choice, None, MissingType]:
         """Get default answer rendered for the questionary lib.
 
         The questionary lib expects some specific data types, and returns
         it when the user answers. Sometimes you need to compare the response
         to the rendered one, or viceversa.
 
         This helper allows such usages.
         """
         default = self.get_default()
+        if default is MISSING:
+            return MISSING
         # If there are choices, return the one that matches the expressed default
         if self.choices:
             for choice in self._formatted_choices:
                 if choice.value == default:
                     return choice
             return None
         # Yes/No questions expect and return bools
@@ -285,16 +296,14 @@
             # The value can be templated
             value = self.render_value(value)
             result.append(Choice(name, value))
         return result
 
     def filter_answer(self, answer) -> Any:
         """Cast the answer to the desired type."""
-        if answer == self.get_default_rendered():
-            return self.get_default()
         return cast_answer_type(answer, self.get_cast_fn())
 
     def get_message(self) -> str:
         """Get the message that will be printed to the user."""
         if self.help:
             rendered_help = self.render_value(self.help)
             if rendered_help:
@@ -310,26 +319,31 @@
         """Render and obtain the placeholder."""
         return self.render_value(self.placeholder)
 
     def get_questionary_structure(self) -> AnyByStrDict:
         """Get the question in a format that the questionary lib understands."""
         lexer = None
         result: AnyByStrDict = {
-            "default": self.get_default_rendered(),
             "filter": self.filter_answer,
             "message": self.get_message(),
             "mouse_support": True,
             "name": self.var_name,
             "qmark": "🕵️" if self.secret else "🎤",
             "when": self.get_when,
         }
+        default = self.get_default_rendered()
+        if default is not MISSING:
+            result["default"] = default
         questionary_type = "input"
         type_name = self.get_type_name()
         if type_name == "bool":
             questionary_type = "confirm"
+            # For backwards compatibility
+            if default is MISSING:
+                result["default"] = False
         if self.choices:
             questionary_type = "select"
             result["choices"] = self._formatted_choices
         if questionary_type == "input":
             if self.secret:
                 questionary_type = "password"
             elif type_name == "yaml":
@@ -355,47 +369,34 @@
 
     def get_type_name(self) -> str:
         """Render the type name and return it."""
         return self.render_value(self.type)
 
     def get_multiline(self) -> bool:
         """Get the value for multiline."""
-        multiline = self.render_value(self.multiline)
-        multiline = cast_answer_type(multiline, cast_str_to_bool)
-        return bool(multiline)
+        return cast_str_to_bool(self.render_value(self.multiline))
 
     def validate_answer(self, answer) -> bool:
         """Validate user answer."""
-        cast_fn = self.get_cast_fn()
         try:
-            ans = cast_fn(answer)
+            ans = self.parse_answer(answer)
         except Exception:
             return False
 
         try:
             err_msg = self.render_value(self.validator, {self.var_name: ans}).strip()
         except Exception as error:
             raise ValidationError(message=str(error)) from error
         if err_msg:
             raise ValidationError(message=err_msg)
         return True
 
     def get_when(self, answers) -> bool:
         """Get skip condition for question."""
-        if (
-            # Skip on --defaults
-            not self.ask_user
-            # Skip on --data=this_question=some_answer
-            or self.var_name in self.answers.init
-        ):
-            return False
-        when = self.when
-        when = self.render_value(when)
-        when = cast_answer_type(when, cast_str_to_bool)
-        return bool(when)
+        return cast_str_to_bool(self.render_value(self.when))
 
     def render_value(
         self, value: Any, extra_answers: Optional[AnyByStrDict] = None
     ) -> str:
         """Render a single templated value using Jinja.
 
         If the value cannot be used as a template, it will be returned as is.
@@ -408,14 +409,26 @@
             # value was not a string
             return value
         try:
             return template.render({**self.answers.combined, **(extra_answers or {})})
         except UndefinedError as error:
             raise UserMessageError(str(error)) from error
 
+    def parse_answer(self, answer: Any) -> Any:
+        """Parse the answer according to the question's type."""
+        cast_fn = self.get_cast_fn()
+        ans = cast_answer_type(answer, cast_fn)
+        choice_values = [
+            cast_answer_type(choice.value, cast_fn)
+            for choice in self._formatted_choices
+        ]
+        if choice_values and ans not in choice_values:
+            raise ValueError("Invalid choice")
+        return ans
+
 
 def parse_yaml_string(string: str) -> Any:
     """Parse a YAML string and raise a ValueError if parsing failed.
 
     This method is needed because :meth:`prompt` requires a ``ValueError``
     to repeat failed questions.
     """
@@ -435,17 +448,14 @@
             return yaml.safe_load(fd)
     except FileNotFoundError:
         return {}
 
 
 def cast_answer_type(answer: Any, type_fn: Callable) -> Any:
     """Cast answer to expected type."""
-    # Skip casting None into "None"
-    if type_fn is str and answer is None:
-        return answer
     try:
         return type_fn(answer)
     except (TypeError, AttributeError):
         # JSON or YAML failed because it wasn't a string; no need to convert
         return answer
```

### Comparing `copier-7.1.0a0/copier/vcs.py` & `copier-7.2.0/copier/vcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import sys
 from contextlib import suppress
 from pathlib import Path
 from tempfile import mkdtemp
 from warnings import warn
 
 from packaging import version
-from packaging.version import Version
+from packaging.version import InvalidVersion, Version
 from plumbum import TF, ProcessExecutionError, colors, local
 from plumbum.cmd import git
 
-from .errors import DirtyLocalWarning
+from .errors import DirtyLocalWarning, ShallowCloneWarning
 from .tools import TemporaryDirectory
 from .types import OptBool, OptStr, StrOrPath
 
 GIT_PREFIX = ("git@", "git://", "git+", "https://github.com/", "https://gitlab.com/")
 GIT_POSTFIX = ".git"
 GIT_VERSION = Version(re.findall(r"\d+\.\d+\.\d+", git("version"))[0])
 REPLACEMENTS = (
@@ -41,26 +41,34 @@
     try:
         git("-C", path, "rev-parse", "--show-toplevel")
         return True
     except (OSError, ProcessExecutionError):
         return False
 
 
+def is_git_shallow_repo(path: StrOrPath) -> bool:
+    """Indicate if a given path is a git shallow repo directory."""
+    try:
+        return git("-C", path, "rev-parse", "--is-shallow-repository").strip() == "true"
+    except (OSError, ProcessExecutionError):
+        return False
+
+
 def is_git_bundle(path: Path) -> bool:
     """Indicate if a path is a valid git bundle."""
     with suppress(OSError):
         path = path.resolve()
     with TemporaryDirectory(prefix=f"{__name__}.is_git_bundle.") as dirname:
         with local.cwd(dirname):
             git("init")
             return bool(git["bundle", "verify", path] & TF)
 
 
 def get_repo(url: str) -> OptStr:
-    """Transforms `url` into a git-parseable origin URL.
+    """Transform `url` into a git-parseable origin URL.
 
     Args:
         url:
             Valid examples:
 
             - gh:copier-org/copier
             - gl:copier-org/copier
@@ -97,15 +105,15 @@
     Parameters:
         local_repo:
             A git repository in the local filesystem.
         use_prereleases:
             If `False`, skip prerelease git tags.
     """
     with local.cwd(local_repo):
-        all_tags = git("tag").split()
+        all_tags = filter(valid_version, git("tag").split())
         if not use_prereleases:
             all_tags = filter(
                 lambda tag: not version.parse(tag).is_prerelease, all_tags
             )
         sorted_tags = sorted(all_tags, key=version.parse, reverse=True)
         try:
             latest_tag = str(sorted_tags[0])
@@ -129,23 +137,34 @@
     Args:
         url:
             Git-parseable URL of the repo. As returned by
             [get_repo][copier.vcs.get_repo].
         ref:
             Reference to checkout. For Git repos, defaults to `HEAD`.
     """
-
     location = mkdtemp(prefix=f"{__name__}.clone.")
     _clone = git["clone", "--no-checkout", url, location]
     # Faster clones if possible
     if GIT_VERSION >= Version("2.27"):
-        _clone = _clone["--filter=blob:none"]
+        url_match = re.match("(file://)?(.*)", url)
+        if url_match is not None:
+            file_url = url_match.groups()[-1]
+        else:
+            file_url = url
+        if is_git_shallow_repo(file_url):
+            warn(
+                f"The repository '{url}' is a shallow clone, this might lead to unexpected "
+                "failure or unusually high resource consumption.",
+                ShallowCloneWarning,
+            )
+        else:
+            _clone = _clone["--filter=blob:none"]
     _clone()
-
-    if not ref and os.path.exists(url) and Path(url).is_dir():
+    # Include dirty changes if checking out a local HEAD
+    if ref in {None, "HEAD"} and os.path.exists(url) and Path(url).is_dir():
         is_dirty = False
         with local.cwd(url):
             is_dirty = bool(git("status", "--porcelain").strip())
         if is_dirty:
             url_abspath = Path(url).absolute()
             with local.cwd(location):
                 git("--git-dir=.git", f"--work-tree={url_abspath}", "add", "-A")
@@ -159,11 +178,23 @@
                 )
                 warn(
                     "Dirty template changes included automatically.",
                     DirtyLocalWarning,
                 )
 
     with local.cwd(location):
-        git("checkout", ref or "HEAD")
+        git("checkout", "-f", ref or "HEAD")
         git("submodule", "update", "--checkout", "--init", "--recursive", "--force")
 
     return location
+
+
+def valid_version(version_: str) -> bool:
+    """Tell if a string is a valid [PEP 440][] version specifier.
+
+    [PEP 440]: https://peps.python.org/pep-0440/
+    """
+    try:
+        version.parse(version_)
+    except InvalidVersion:
+        return False
+    return True
```

### Comparing `copier-7.1.0a0/pyproject.toml` & `copier-7.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 [tool.poetry]
 name = "copier"
 # This version is a placeholder autoupdated by poetry-dynamic-versioning
-version = "7.1.0a0"
+version = "7.2.0"
 description = "A library for rendering project templates."
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 authors = ["Ben Felder <ben@felder.io>"]
 homepage = "https://github.com/copier-org/copier"
 repository = "https://github.com/copier-org/copier"
 readme = "README.md"
 
 [tool.poetry.scripts]
-copier = "copier.cli:CopierApp.run"
+copier = "copier.__main__:copier_app_run"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/copier-org/copier/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0" # HACK https://github.com/PyCQA/isort/issues/1945
 "backports.cached-property" = { version = ">=1.0.0", python = "<3.8" }
 colorama = ">=0.4.3"
 dunamai = ">=1.7.0"
 funcy = ">=1.17"
-importlib-metadata = { version = ">=3.4,<5.0", python = "<3.8" }
+importlib-metadata = { version = ">=3.4,<7.0", python = "<3.8" }
 jinja2 = ">=3.1.1"
 jinja2-ansible-filters = ">=1.3.1"
-packaging = ">=21.0" # packaging is needed when installing from PyPI
+packaging = ">=23.0"
 pathspec = ">=0.9.0"
 plumbum = ">=1.6.9"
 pydantic = ">=1.10.2"
 pygments = ">=2.7.1"
 pyyaml = ">=5.3.1"
 pyyaml-include = ">=1.2"
 questionary = ">=1.8.1"
 typing-extensions = { version = ">=3.7.4,<5.0.0", python = "<3.8" }
 
+[tool.poetry.group.dev]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
-autoflake = ">=1.4"
-black = ">=22.1"
-commitizen = ">=2.32.2"
-flake8 = ">=4.0.1"
-flake8-bugbear = ">=22.1.11"
-flake8-comprehensions = ">=3.8.0"
-flake8-debugger = ">=4.0.0"
-flake8-simplify = ">=0.19.3"
-isort = ">=5.10.1"
 mypy = ">=0.931"
 pexpect = ">=4.8.0"
 poethepoet = ">=0.12.3"
 pre-commit = ">=2.17.0"
-pytest = ">=7.0.1"
+pytest = ">=7.2.0"
 pytest-cov = ">=3.0.0"
 pytest-xdist = ">=2.5.0"
 types-backports = ">=0.1.3"
 types-pyyaml = ">=6.0.4"
+types-psutil = "*"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs-material = ">=8.2,<9.0.0"
+markdown-exec = ">=1.3.0"
+mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
 
 [tool.poe.tasks.clean]
 script = "devtasks:clean"
 help = "remove build/python artifacts"
 
 [tool.poe.tasks.coverage]
@@ -84,15 +81,15 @@
 help = "set up local development environment"
 
 [tool.poe.tasks.docs]
 cmd = "mkdocs serve"
 help = "start local docs server"
 
 [tool.poe.tasks.lint]
-cmd = "pre-commit run --all-files"
+script = "devtasks:lint"
 help = "check (and auto-fix) style with pre-commit"
 
 [tool.poe.tasks.test]
 cmd = "pytest --color=yes"
 help = "run tests"
 
 [tool.poe.tasks.types]
@@ -113,20 +110,27 @@
 known_first_party = ["copier"]
 
 [tool.mypy]
 ignore_missing_imports = true
 plugins = ["pydantic.mypy"]
 warn_no_return = false
 
+[tool.pydocstyle]
+match_dir = "^copier"
+add_ignore = ["D105", "D107"]
+
 [tool.pytest.ini_options]
 addopts = "-n auto -ra"
+markers = [
+    "impure: needs network or is not 100% reproducible"
+]
 
 [tool.commitizen]
 annotated_tag = true
 changelog_incremental = true
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "7.1.0a0"
+version = "7.2.0"
 
 [build-system]
-requires = ["poetry_core>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `copier-7.1.0a0/setup.py` & `copier-7.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,199 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: copier
+Version: 7.2.0
+Summary: A library for rendering project templates.
+Home-page: https://github.com/copier-org/copier
+License: MIT
+Author: Ben Felder
+Author-email: ben@felder.io
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: backports.cached-property (>=1.0.0) ; python_version < "3.8"
+Requires-Dist: colorama (>=0.4.3)
+Requires-Dist: dunamai (>=1.7.0)
+Requires-Dist: funcy (>=1.17)
+Requires-Dist: importlib-metadata (>=3.4,<7.0) ; python_version < "3.8"
+Requires-Dist: jinja2 (>=3.1.1)
+Requires-Dist: jinja2-ansible-filters (>=1.3.1)
+Requires-Dist: packaging (>=23.0)
+Requires-Dist: pathspec (>=0.9.0)
+Requires-Dist: plumbum (>=1.6.9)
+Requires-Dist: pydantic (>=1.10.2)
+Requires-Dist: pygments (>=2.7.1)
+Requires-Dist: pyyaml (>=5.3.1)
+Requires-Dist: pyyaml-include (>=1.2)
+Requires-Dist: questionary (>=1.8.1)
+Requires-Dist: typing-extensions (>=3.7.4,<5.0.0) ; python_version < "3.8"
+Project-URL: Bug Tracker, https://github.com/copier-org/copier/issues
+Project-URL: Repository, https://github.com/copier-org/copier
+Description-Content-Type: text/markdown
+
+# ![Copier](https://github.com/copier-org/copier/raw/master/img/copier-logotype.png)
+
+[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/copier-org/copier)
+[![codecov](https://codecov.io/gh/copier-org/copier/branch/master/graph/badge.svg)](https://codecov.io/gh/copier-org/copier)
+[![CI](https://github.com/copier-org/copier/workflows/CI/badge.svg)](https://github.com/copier-org/copier/actions?query=branch%3Amaster)
+[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+![Python](https://img.shields.io/pypi/pyversions/copier?logo=python&logoColor=%23959DA5)
+[![PyPI](https://img.shields.io/pypi/v/copier?logo=pypi&logoColor=%23959DA5)](https://pypi.org/project/copier/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Documentation Status](https://img.shields.io/readthedocs/copier/latest?logo=readthedocs)](https://copier.readthedocs.io/en/latest)
+
+A library and CLI app for rendering project templates.
+
+-   Works with **local** paths and **Git URLs**.
+-   Your project can include any file and Copier can dynamically replace values in any
+    kind of text file.
+-   It generates a beautiful output and takes care of not overwriting existing files
+    unless instructed to do so.
+
+![Sample output](https://github.com/copier-org/copier/raw/master/img/copier-output.png)
+
+## Installation
+
+1. Install Python 3.7 or newer (3.8 or newer if you're on Windows).
+1. Install Git 2.27 or newer.
+1. To use as a CLI app: `pipx install copier`
+1. To use as a library: `pip install copier` or `conda install -c conda-forge copier`
+1. To use with 100% reproducibility: `nix profile install github:copier-org/copier`
+
+## Quick start
+
+To create a template:
+
+```shell
+📁 my_copier_template                        # your template project
+├── 📄 copier.yml                            # your template configuration
+├── 📁 .git/                                 # your template is a Git repository
+├── 📁 {{project_name}}                      # a folder with a templated name
+│   └── 📄 {{module_name}}.py.jinja          # a file with a templated name
+└── 📄 {{_copier_conf.answers_file}}.jinja   # answers are recorded here
+```
+
+```yaml title="copier.yml"
+# questions
+project_name:
+    type: str
+    help: What is your project name?
+
+module_name:
+    type: str
+    help: What is your Python module name?
+```
+
+```python+jinja title="{{project_name}}/{{module_name}}.py.jinja"
+print("Hello from {{module_name}}!")
+```
+
+```yaml+jinja title="{{_copier_conf.answers_file}}.jinja"
+# Changes here will be overwritten by Copier
+{{ _copier_answers|to_nice_yaml -}}
+```
+
+To generate a project from the template:
+
+-   On the command-line:
+
+    ```shell
+    copier path/to/project/template path/to/destination
+    ```
+
+-   Or in Python code, programmatically:
+
+    ```python
+    from copier import run_auto
+
+    # Create a project from a local path
+    run_auto("path/to/project/template", "path/to/destination")
+
+    # Or from a Git URL.
+    run_auto("https://github.com/copier-org/copier.git", "path/to/destination")
+
+    # You can also use "gh:" as a shortcut of "https://github.com/"
+    run_auto("gh:copier-org/copier.git", "path/to/destination")
+
+    # Or "gl:" as a shortcut of "https://gitlab.com/"
+    run_auto("gl:copier-org/copier.git", "path/to/destination")
+    ```
+
+## Basic concepts
+
+Copier is composed of these main concepts:
+
+1. **Templates**. They lay out how to generate the subproject.
+1. **Questionaries**. They are configured in the template. Answers are used to generate
+   projects.
+1. **Projects**. This is where your real program lives. But it is usually generated
+   and/or updated from a template.
+
+Copier targets these main human audiences:
+
+1.  **Template creators**. Programmers that repeat code too much and prefer a tool to do
+    it for them.
+
+    !!! tip
+
+         Copier doesn't replace the DRY principle... but sometimes you simply can't be
+         DRY and you need a DRYing machine...
+
+1.  **Template consumers**. Programmers that want to start a new project quickly, or
+    that want to evolve it comfortably.
+
+Non-humans should be happy also by using Copier's CLI or API, as long as their
+expectations are the same as for those humans... and as long as they have feelings.
+
+Templates have these goals:
+
+1. **[Code scaffolding](<https://en.wikipedia.org/wiki/Scaffold_(programming)>)**. Help
+   consumers have a working source code tree as quickly as possible. All templates allow
+   scaffolding.
+1. **Code lifecycle management**. When the template evolves, let consumers update their
+   projects. Not all templates allow updating.
+
+Copier tries to have a smooth learning curve that lets you create simple templates that
+can evolve into complex ones as needed.
+
+## Browse or tag public templates
+
+You can browse public Copier templates on GitHub using
+[the `copier-template` topic](https://github.com/topics/copier-template). Use them as
+inspiration!
+
+If you want your template to appear in that list, just add the topic to it! 🏷
+
+## Credits
+
+Special thanks go to [jpsca](https://github.com/jpsca) for originally creating `Copier`.
+This project would not be a thing without him.
+
+Many thanks to [pykong](https://github.com/pykong) who took over maintainership on the
+project, promoted it, and laid out the bases of what the project is today.
+
+Big thanks also go to [yajo](https://github.com/yajo) for his relentless zest for
+improving `Copier` even further.
+
+Thanks a lot, [pawamoy](https://github.com/pawamoy) for polishing very important rough
+edges and improving the documentation and UX a lot.
+
+Also special thanks to [sisp](https://github.com/sisp) for being very helpful in
+polishing documentation, fixing bugs, helping the community and cleaning up the
+codebase.
 
-packages = \
-['copier']
+And thanks to all financial supporters and folks that give us a shiny star! ⭐
 
-package_data = \
-{'': ['*']}
+[![Star History Chart](https://api.star-history.com/svg?repos=copier-org/copier&type=Date)](https://star-history.com/#copier-org/copier&Date)
 
-install_requires = \
-['colorama>=0.4.3',
- 'dunamai>=1.7.0',
- 'funcy>=1.17',
- 'jinja2-ansible-filters>=1.3.1',
- 'jinja2>=3.1.1',
- 'packaging>=21.0',
- 'pathspec>=0.9.0',
- 'plumbum>=1.6.9',
- 'pydantic>=1.10.2',
- 'pygments>=2.7.1',
- 'pyyaml-include>=1.2',
- 'pyyaml>=5.3.1',
- 'questionary>=1.8.1']
-
-extras_require = \
-{':python_version < "3.8"': ['backports.cached-property>=1.0.0',
-                             'importlib-metadata>=3.4,<5.0',
-                             'typing-extensions>=3.7.4,<5.0.0']}
-
-entry_points = \
-{'console_scripts': ['copier = copier.cli:CopierApp.run']}
-
-setup_kwargs = {
-    'name': 'copier',
-    'version': '7.1.0a0',
-    'description': 'A library for rendering project templates.',
-    'long_description': '# ![Copier](https://github.com/copier-org/copier/raw/master/img/copier-logotype.png)\n\n[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/copier-org/copier)\n[![codecov](https://codecov.io/gh/copier-org/copier/branch/master/graph/badge.svg)](https://codecov.io/gh/copier-org/copier)\n[![CI](https://github.com/copier-org/copier/workflows/CI/badge.svg)](https://github.com/copier-org/copier/actions?query=branch%3Amaster)\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n![Python](https://img.shields.io/pypi/pyversions/copier?logo=python&logoColor=%23959DA5)\n[![PyPI](https://img.shields.io/pypi/v/copier?logo=pypi&logoColor=%23959DA5)](https://pypi.org/project/copier/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Documentation Status](https://img.shields.io/readthedocs/copier/latest?logo=readthedocs)](https://copier.readthedocs.io/en/latest)\n\nA library and CLI app for rendering project templates.\n\n-   Works with **local** paths and **Git URLs**.\n-   Your project can include any file and Copier can dynamically replace values in any\n    kind of text file.\n-   It generates a beautiful output and takes care of not overwriting existing files\n    unless instructed to do so.\n\n![Sample output](https://github.com/copier-org/copier/raw/master/img/copier-output.png)\n\n## Installation\n\n1. Install Python 3.7 or newer (3.8 or newer if you\'re on Windows).\n1. Install Git 2.27 or newer.\n1. To use as a CLI app: `pipx install copier`\n1. To use as a library: `pip install copier` or `conda install -c conda-forge copier`\n\n## Quick start\n\nTo create a template:\n\n```shell\n📁 my_copier_template ------------------------ # your template project\n├── 📄 copier.yml ---------------------------- # your template configuration\n├── 📁 .git ---------------------------------- # your template is a Git repository\n├── 📁 {{project_name}} ---------------------- # a folder with a templated name\n│   └── 📄 {{module_name}}.py.jinja ---------- # a file with a templated name\n└── 📄 {{_copier_conf.answers_file}}.jinja --- # answers are recorded here\n```\n\n```yaml title="copier.yml"\n# questions\nproject_name:\n    type: str\n    help: What is your project name?\n\nmodule_name:\n    type: str\n    help: What is your Python module name?\n```\n\n```python+jinja title="{{project_name}}/{{module_name}}.py.jinja"\nprint("Hello from {{module_name}}!")\n```\n\n```yaml+jinja title="{{_copier_conf.answers_file}}.jinja"\n# Changes here will be overwritten by Copier\n{{ _copier_answers|to_nice_yaml -}}\n```\n\nTo generate a project from the template:\n\n-   On the command-line:\n\n    ```shell\n    copier path/to/project/template path/to/destination\n    ```\n\n-   Or in Python code, programmatically:\n\n    ```python\n    from copier import run_auto\n\n    # Create a project from a local path\n    run_auto("path/to/project/template", "path/to/destination")\n\n    # Or from a Git URL.\n    run_auto("https://github.com/copier-org/copier.git", "path/to/destination")\n\n    # You can also use "gh:" as a shortcut of "https://github.com/"\n    run_auto("gh:copier-org/copier.git", "path/to/destination")\n\n    # Or "gl:" as a shortcut of "https://gitlab.com/"\n    run_auto("gl:copier-org/copier.git", "path/to/destination")\n    ```\n\n## Basic concepts\n\nCopier is composed of these main concepts:\n\n1. **Templates**. They lay out how to generate the subproject.\n1. **Questionaries**. They are configured in the template. Answers are used to generate\n   projects.\n1. **Projects**. This is where your real program lives. But it is usually generated\n   and/or updated from a template.\n\nCopier targets these main human audiences:\n\n1.  **Template creators**. Programmers that repeat code too much and prefer a tool to do\n    it for them.\n\n    !!! tip\n\n         Copier doesn\'t replace the DRY principle... but sometimes you simply can\'t be\n         DRY and you need a DRYing machine...\n\n1.  **Template consumers**. Programmers that want to start a new project quickly, or\n    that want to evolve it comfortably.\n\nNon-humans should be happy also by using Copier\'s CLI or API, as long as their\nexpectations are the same as for those humans... and as long as they have feelings.\n\nTemplates have these goals:\n\n1. **[Code scaffolding](<https://en.wikipedia.org/wiki/Scaffold_(programming)>)**. Help\n   consumers have a working source code tree as quickly as possible. All templates allow\n   scaffolding.\n1. **Code lifecycle management**. When the template evolves, let consumers update their\n   projects. Not all templates allow updating.\n\nCopier tries to have a smooth learning curve that lets you create simple templates that\ncan evolve into complex ones as needed.\n\n## Browse or tag public templates\n\nYou can browse public Copier templates on GitHub using\n[the `copier-template` topic](https://github.com/topics/copier-template). Use them as\ninspiration!\n\nIf you want your template to appear in that list, just add the topic to it! 🏷\n\n## Credits\n\nSpecial thanks go to [jpsca](https://github.com/jpsca) for originally creating `Copier`.\nThis project would not be a thing without him.\n\nMany thanks to [pykong](https://github.com/pykong) who took over maintainership on the\nproject, promoted it, and laid out the bases of what the project is today.\n\nBig thanks also go to [Yajo](https://github.com/Yajo) for his relentless zest for\nimproving `Copier` even further.\n\nThanks a lot, [pawamoy](https://github.com/pawamoy) for polishing very important rough\nedges and improving the documentation and UX a lot.\n',
-    'author': 'Ben Felder',
-    'author_email': 'ben@felder.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/copier-org/copier',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

