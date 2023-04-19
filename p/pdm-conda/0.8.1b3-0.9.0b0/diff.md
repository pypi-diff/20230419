# Comparing `tmp/pdm_conda-0.8.1b3.tar.gz` & `tmp/pdm_conda-0.9.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.8.1b3.tar", last modified: Sun Apr 16 21:55:24 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.0b0.tar", last modified: Wed Apr 19 17:38:17 2023, max compression
```

## Comparing `pdm_conda-0.8.1b3.tar` & `pdm_conda-0.9.0b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b3/LICENSE
--rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b3/README.md
--rw-r--r--   0        0        0     1962 2023-04-16 21:55:24.322209 pdm_conda-0.8.1b3/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-16 21:54:51.001898 pdm_conda-0.8.1b3/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b3/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b3/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    11223 2023-04-15 17:34:37.904070 pdm_conda-0.8.1b3/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b3/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b3/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2311 2023-04-15 20:38:24.832128 pdm_conda-0.8.1b3/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b3/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b3/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b3/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b3/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-15 01:10:11.358619 pdm_conda-0.8.1b3/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b3/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3606 2023-04-16 21:54:51.005272 pdm_conda-0.8.1b3/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b3/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    10806 2023-04-15 17:37:15.580889 pdm_conda-0.8.1b3/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b3/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b3/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b3/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b3/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5455 2023-04-15 17:36:44.693219 pdm_conda-0.8.1b3/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b3/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.0b0/LICENSE
+-rw-r--r--   0        0        0     5649 2023-04-19 17:36:40.659039 pdm_conda-0.9.0b0/README.md
+-rw-r--r--   0        0        0     1979 2023-04-19 17:38:17.553059 pdm_conda-0.9.0b0/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-19 17:38:08.385052 pdm_conda-0.9.0b0/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.0b0/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 15:05:35.481829 pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.9.0b0/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    14551 2023-04-19 16:29:34.284850 pdm_conda-0.9.0b0/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.0b0/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.9.0b0/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2307 2023-04-18 22:35:19.397503 pdm_conda-0.9.0b0/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3043 2023-04-18 01:05:14.781588 pdm_conda-0.9.0b0/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.0b0/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.0b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7946 2023-04-18 23:13:02.100650 pdm_conda-0.9.0b0/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-18 01:05:14.782254 pdm_conda-0.9.0b0/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8612 2023-04-18 23:02:22.362754 pdm_conda-0.9.0b0/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3095 2023-04-19 17:13:01.223457 pdm_conda-0.9.0b0/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6581 2023-04-19 14:41:57.331734 pdm_conda-0.9.0b0/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11268 2023-04-18 23:02:59.727692 pdm_conda-0.9.0b0/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.0b0/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8246 2023-04-19 16:32:27.859361 pdm_conda-0.9.0b0/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.0b0/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-18 22:33:52.217660 pdm_conda-0.9.0b0/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8575 2023-04-19 16:34:29.164097 pdm_conda-0.9.0b0/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.0b0/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.0b0/PKG-INFO
```

### Comparing `pdm_conda-0.8.1b3/LICENSE` & `pdm_conda-0.9.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/README.md` & `pdm_conda-0.9.0b0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # pdm-conda
 
-A PDM plugin to install project dependencies with Conda.
+A PDM plugin to resolve/install/uninstall project dependencies with Conda.
 
 ## Configuration
 
 | Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
 |-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
 | `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
+| `conda.solver`                    | Solver to use for Conda resolution                                                                   | `conda`             | `conda`, `libmamba`            | `CONDA_SOLVER`              |
 | `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
 | `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
 | `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
 | `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
 | `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
 | `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
 | `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
@@ -21,14 +22,15 @@
 
 ```toml
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
+solver = "libmamba"
 excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
 batched-commands = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
@@ -57,23 +59,31 @@
     * With flag `-r` or `--runner` you can specify the Conda runner to use.
 * `pdm remove`
 * `pdm list`
 * `pdm info`
 
 ### How it works
 
-When PDM detects a Conda managed package, it gets candidates with Conda and then tries to resolve the environment as
-with any other requirement.
+#### Using conda/libmamba solver
 
-To keep the resolution consistent with Conda, PDM follows resolution rules from Conda as good as possible.
+PDM invokes Conda solver to resolve conda packages each time a PDM candidate makes a change in the last Conda
+resolution.
+
+If only Conda packages are used (i.e. setting `conda.as-default-manager` to `true` and no `conda.excludes`) then Conda
+solver is invoked only once.
 
 ### Settings overriden
 
 In order to use Conda to install packages some settings were overriden:
 
+* `python.use_venv` if conda settings detected in `pyproject.toml` this setting is set to `True`.
+* `python.use_pyenv` if conda settings detected in `pyproject.toml` this setting is set to `False`.
+* `venv.backend` if conda settings detected in `pyproject.toml` this setting is set to `conda.runner`.
+* `venv.location` if conda settings detected in `pyproject.toml` and `VIRTUAL_ENV` or `CONDA_PREFIX` environment
+  variables are set then this setting is set to the value of the environment variable.
 * `install.parallel` if some Conda managed packages are to be uninstalled or updated this option is disabled
   momentarily.
 
 ## Development
 
 For development `docker-compose` files exist in `deploy` directory, helper script `deploy/docker-compose.sh` can be used
 for executing docker.
```

### Comparing `pdm_conda-0.8.1b3/pyproject.toml` & `pdm_conda-0.9.0b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "pdm-conda"
-description = " A PDM plugin to install project dependencies with Conda"
+description = "A PDM plugin to resolve/install/uninstall project dependencies with Conda"
 requires-python = ">=3.10"
 authors = [
     { name = "Marcos Pastorini" },
 ]
 keywords = [
     "pdm",
     "plugin",
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.8.1b3"
+version = "0.9.0b0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/__init__.py` & `pdm_conda-0.9.0b0/src/pdm_conda/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.8.1b3"
+__version__ = "0.9.0b0"
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,17 +41,14 @@
     description = BaseCommand.__doc__
     name = "add"
     arguments = BaseCommand.arguments + [conda_group]
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:
         project = cast(CondaProject, project)
         config = project.conda_config
-        if config.as_default_manager:
-            options.conda_packages.extend(options.packages)
-            options.packages = []
 
         if conda_packages := options.conda_packages:
             channel = options.conda_channel
 
             existing_channels = config.channels
             if options.conda_runner:
                 config.runner = options.conda_runner
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.0b0/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.0b0/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/conda.py` & `pdm_conda-0.9.0b0/src/pdm_conda/conda.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import contextlib
 import json
 import subprocess
 from functools import lru_cache
+from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import Iterable
-from urllib.parse import urlparse
 
-from packaging.version import Version
 from pdm import termui
-from pdm.exceptions import RequirementError
+from pdm.cli.commands.venv.backends import VirtualenvCreateError
+from pdm.exceptions import PdmException, RequirementError
 from pdm.models.setup import Setup
 from pdm.termui import Verbosity
 
-from pdm_conda.models.candidates import CondaCandidate
+from pdm_conda.models.candidates import CondaCandidate, parse_channel
 from pdm_conda.models.conda import ChannelSorter
 from pdm_conda.models.config import CondaRunner
 from pdm_conda.models.requirements import (
     CondaRequirement,
     parse_conda_version,
     parse_requirement,
 )
@@ -25,125 +25,171 @@
 from pdm_conda.utils import normalize_name
 
 logger = termui.logger
 
 
 @contextlib.contextmanager
 def _optional_temporary_file(environment: dict):
+    """
+    If environment contains data then creates temporary file else yield None
+    :param environment: environment data
+    :return: Temporary file or None
+    """
     if environment:
         with NamedTemporaryFile(mode="w+", suffix=".yml") as f:
             yield f
     else:
         yield
 
 
-def run_conda(cmd, **environment) -> dict:
+def run_conda(
+    cmd,
+    exception_cls: type[PdmException] = RequirementError,
+    exception_msg: str = "Error locking dependencies",
+    **environment,
+) -> dict:
     """
-    Creates temporary environment file and run conda command
+    Optionally creates temporary environment file and run conda command
     :param cmd: conda command
+    :param exception_cls: exception to raise on error
+    :param exception_msg: base message to show on error
     :param environment: environment data
     :return: conda command response
     """
     with _optional_temporary_file(environment) as f:
         if environment:
             for name, options in environment.items():
                 if options:
-                    f.write(f"{name}:\n")
+                    f.write(f"{name}:")
+                    if isinstance(options, str):
+                        f.write(f" {options}\n")
+                        continue
+                    else:
+                        f.write("\n")
                     for v in options:
                         f.write(f"  - {v}\n")
             f.seek(0)
             cmd = cmd + ["-f", f.name]
         logger.debug(f"cmd: {' '.join(cmd)}")
         if environment:
             logger.debug(f"env: {environment}")
         process = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding="utf-8")
     if "--json" in cmd:
         try:
             response = json.loads(process.stdout)
         except:
             response = {}
     else:
-        response = {"message": process.stdout}
+        response = {"message": f"{process.stdout}\n{process.stderr}"}
     try:
         process.check_returncode()
     except subprocess.CalledProcessError as e:
-        msg = "Error locking dependencies\n"
+        msg = f"{exception_msg}\n"
         if isinstance(response, dict) and not response.get("success", False):
-            if err := response.get("solver_problems", response.get("error", response.get("message", []))):
+            if err := response.get("solver_problems", response.get("error", response.get("message", process.stderr))):
                 if isinstance(err, str):
                     err = [err]
                 msg += "\n".join(err)
         else:
             msg += process.stderr
         if environment:
             msg += f"\n{environment}"
-        raise RequirementError(msg) from e
+        raise exception_cls(msg) from e
     return response
 
 
 @lru_cache(maxsize=None)
 def _get_channel_sorter(platform: str, channels: tuple[str]) -> ChannelSorter:
     """
     Get channel sorter
     :param channels: list of conda channels used to determine priority
     :param platform: env platform
     :return: channel sorter
     """
     return ChannelSorter(platform, channels)
 
 
-def _sort_packages(packages: list[dict], channels: Iterable[str], platform: str) -> Iterable[dict]:
+def sort_candidates(project: CondaProject, packages: list[CondaCandidate]) -> Iterable[CondaCandidate]:
     """
-    Sort packages following mamba specification
+    Sort candidates following mamba specification
     (https://mamba.readthedocs.io/en/latest/advanced_usage/package_resolution.html).
-    :param packages: list of conda packages
-    :param channels: list of conda channels used to determine priority
-    :param platform: env platform
-    :return: sorted conda packages
+    :param project: PDM project
+    :param packages: list of conda candidates
+    :return: sorted conda candidates
     """
     if len(packages) <= 1:
         return packages
+    channels_sorter = _get_channel_sorter(project.platform, tuple(project.conda_config.channels))
 
-    channels_sorter = _get_channel_sorter(platform, tuple(channels))
-
-    def get_preference(package):
+    def get_preference(candidate: CondaCandidate):
         return (
-            not package.get("track_feature", ""),
-            Version(parse_conda_version(package["version"], inverse=package.get("name", "") == "openssl")),
-            package.get("build_number", 0),
-            -channels_sorter.get_priority(package["channel"]),
-            package.get("timestamp", 0),
+            not candidate.track_feature,
+            candidate.version,
+            candidate.build_number,
+            -channels_sorter.get_priority(candidate.channel or ""),
+            candidate.timestamp,
         )
 
     return sorted(packages, key=get_preference, reverse=True)
 
 
-@lru_cache(maxsize=None)
-def _parse_channel(channel_url: str) -> str:
+def _parse_candidates(project: CondaProject, packages: list[dict], requirement=None) -> list[CondaCandidate]:
+    """
+    Convert conda packages to candidates
+    :param project: PDM project
+    :param packages: conda packages
+    :param requirement: requirement linked to packages
+    :return: list of candidates
     """
-    Parse channel from channel url
-    :param channel_url: channel url from package
-    :return: channel
-    """
-    channel = urlparse(channel_url).path
-    if channel.startswith("/"):
-        channel = channel[1:]
-    return channel
+    candidates = []
+    for p in packages:
+        dependencies = p.get("depends", None) or []
+        valid_candidate = True
+        for d in dependencies:
+            if d.startswith("__"):
+                d = parse_requirement(f"conda:{d}")
+                if not any(d.is_compatible(v) for v in project.virtual_packages):
+                    valid_candidate = False
+                    break
+        if valid_candidate:
+            candidates.append(CondaCandidate.from_conda_package(p, requirement))
+
+    return candidates
+
+
+def _ensure_channels(
+    project: CondaProject,
+    channels: list[str],
+    log_message: str = "No channels specified, using defaults if exist.",
+) -> list[str]:
+    """
+    Ensure channels and if empty use defaults
+    :param project: PDM project
+    :param channels: channels to validate
+    :param log_message: log message to display if using defaults
+    :return: list of channels
+    """
+    channels = channels or project.conda_config.channels
+    if not channels:
+        project.core.ui.echo(log_message, verbosity=Verbosity.DEBUG)
+        channels.append("defaults")
+
+    return list(dict.fromkeys(channels))
 
 
 @lru_cache(maxsize=None)
 def _conda_search(
-    requirement: str,
     project: CondaProject,
+    requirement: str,
     channels: tuple[str],
 ) -> list[CondaCandidate]:
     """
     Search conda candidates for a requirement
-    :param requirement: requirement
     :param project: PDM project
+    :param requirement: requirement
     :param channels: requirement channels
     :return: list of conda candidates
     """
     config = project.conda_config
     command = config.command("search")
     command.append(requirement)
 
@@ -156,150 +202,198 @@
         result = run_conda(command)
     except RequirementError as e:
         if "PackagesNotFoundError:" in str(e):
             result = dict()
         else:
             raise
 
-    candidates = []
     if config.runner == CondaRunner.CONDA:
         packages = result.get(parse_requirement(f"conda:{requirement}").name, [])
     else:
         packages = result.get("result", dict()).get("pkgs", [])
 
-    for p in packages:
-        p["channel"] = _parse_channel(p["channel"])
-
-    for p in _sort_packages(packages, channels, project.platform):
-        dependencies = p.get("depends", [])
-        valid_candidate = True
-        for d in dependencies:
-            if d.startswith("__"):
-                d = parse_requirement(f"conda:{d}")
-                if not any(d.is_compatible(v) for v in project.virtual_packages):
-                    valid_candidate = False
-                    break
-        if valid_candidate:
-            candidates.append(CondaCandidate.from_conda_package(p))
-
-    return candidates
+    return _parse_candidates(project, packages=packages)
 
 
 def conda_search(
-    requirement: CondaRequirement | str,
     project: CondaProject,
+    requirement: CondaRequirement | str,
     channel: str | None = None,
 ) -> list[CondaCandidate]:
     """
     Search conda candidates for a requirement
-    :param requirement: requirement
     :param project: PDM project
+    :param requirement: requirement
     :param channel: requirement channel
     :return: list of conda candidates
     """
     if isinstance(requirement, CondaRequirement):
         channel = channel or requirement.channel
         requirement = requirement.as_line(with_build_string=True, conda_compatible=True).replace(" ", "=")
     if "::" in requirement:
         channel, requirement = requirement.split("::", maxsplit=1)
-    channels = [channel] if channel else project.conda_config.channels
-    if not channels:
-        project.core.ui.echo(
-            f"No channel specified for searching [success]{requirement}[/] using defaults if exist.",
-            verbosity=Verbosity.DEBUG,
-        )
-        channels.append("defaults")
+    channels = _ensure_channels(
+        project,
+        [channel] if channel else [],
+        f"No channel specified for searching [req]{requirement}[/] using defaults if exist.",
+    )
+    return _conda_search(project, requirement, tuple(channels))
 
-    # set defaults if exist
-    try:
-        idx = channels.index("defaults")
-        channels = channels[:idx] + project.default_channels + channels[idx + 1 :]
-    except ValueError:
-        pass
 
-    return _conda_search(requirement, project, tuple(channels))
+def conda_create(
+    project: CondaProject,
+    requirements: list[CondaRequirement],
+    channels: list[str] | None = None,
+    prefix: Path | str | None = None,
+    name: str = "",
+    dry_run: bool = False,
+) -> dict[str, list[CondaCandidate]]:
+    """
+    Creates environment using conda
+    :param project: PDM project
+    :param requirements: conda requirements
+    :param channels: requirement channels
+    :param prefix: environment prefix
+    :param name: environment name
+    :param dry_run: don't install if dry run
+    """
+    config = project.conda_config
+    if not config.is_initialized:
+        raise VirtualenvCreateError("Error creating environment, no pdm-conda configs were found on pyproject.toml.")
+    candidates = dict()
+    channels = channels or []
+    for req in requirements:
+        if req.channel:
+            channels.append(req.channel)
+    channels = _ensure_channels(
+        project,
+        channels,
+        "No channels specified for creating environment, using defaults if exist.",
+    )
+    command = config.command("create")
+    command.append("--json")
+    if prefix is not None:
+        command.extend(["--prefix", str(prefix)])
+    elif name:
+        command.extend(["--name", name])
+    else:
+        raise VirtualenvCreateError("Error creating environment, name or prefix must be specified.")
+
+    if dry_run:
+        command.append("--dry-run")
+
+    for req in requirements:
+        command.append(req.as_line(with_build_string=True, conda_compatible=True, with_channel=True).replace(" ", "="))
+
+    if channels:
+        for c in channels:
+            command.extend(["-c", c])
+        command.append("--override-channels")
+
+    result = run_conda(
+        command,
+        exception_cls=VirtualenvCreateError,
+        exception_msg="Error creating environment",
+    )
+
+    actions = result.get("actions", dict())
+    fetch_packages = {pkg["name"]: pkg for pkg in actions.get("FETCH", [])}
+    packages = actions.get("LINK", [])
+    for i, pkg in enumerate(packages):
+        pkg = fetch_packages.get(pkg["name"], pkg)
+        if any(True for n in ("constrains", "depends") if n not in pkg):
+            pkg = conda_search(
+                project,
+                f'{pkg["name"]} {pkg["version"]} {pkg["build_string"]}',
+                parse_channel(pkg["channel"]),
+            )[0]
+        packages[i] = pkg
+
+    _requirements = {req.conda_name: req for req in requirements}
+    for pkg in packages:
+        name = pkg["name"]
+        candidates[name] = _parse_candidates(
+            project,
+            packages=[pkg],
+            requirement=_requirements.get(name, None),
+        )
+    return candidates
 
 
 def _conda_install(
     project: CondaProject,
     command: list[str],
     packages: str | list[str] | None = None,
-    verbose: bool = False,
+    dry_run: bool = False,
 ):
     if isinstance(packages, str):
         packages = [packages]
-    kwargs = dict()
     if packages:
-        kwargs["dependencies"] = packages
-    response = run_conda(command + ["--json"], **kwargs)
-    if verbose:
-        project.core.ui.echo(response)
+        command.extend(packages)
+    if dry_run:
+        command.append("--dry-run")
+    response = run_conda(command + ["--json"])
+    project.core.ui.echo(response, verbosity=Verbosity.DEBUG)
 
 
 def conda_install(
     project: CondaProject,
     packages: str | list[str],
-    verbose: bool = False,
     dry_run: bool = False,
     no_deps: bool = False,
 ):
     """
     Install resolved packages using conda
     :param project: PDM project
     :param packages: resolved packages
-    :param verbose: show conda response if true
     :param dry_run: don't install if dry run
     :param no_deps: don't install dependencies if true
     """
     config = project.conda_config
-    command = config.command()
+    command = config.command("install")
     if no_deps:
         command.append("--no-deps")
-    if dry_run:
-        command.append("--dry-run")
+        if config.runner != CondaRunner.MICROMAMBA:
+            command.append("--no-update-deps")
+
     if config.installation_method == "copy":
         _copy = "copy"
         if config.runner == CondaRunner.MICROMAMBA:
             _copy = f"always-{_copy}"
         command.append(f"--{_copy}")
 
-    _conda_install(project, command, packages, verbose)
+    _conda_install(project, command, packages, dry_run=dry_run)
 
 
 def conda_uninstall(
     project: CondaProject,
     packages: str | list[str],
-    verbose: bool = False,
     dry_run: bool = False,
     no_deps: bool = False,
 ):
     """
     Uninstall resolved packages using conda
     :param project: PDM project
     :param packages: resolved packages
-    :param verbose: show conda response if true
     :param dry_run: don't uninstall if dry run
     :param no_deps: don't uninstall dependencies if true
     """
     config = project.conda_config
-    command = config.command("remove")
+
+    with config.with_config(
+        runner=CondaRunner.CONDA if no_deps and config.runner == CondaRunner.MAMBA else config.runner,
+    ):
+        command = config.command("remove")
+
     if no_deps:
         if config.runner == CondaRunner.MICROMAMBA:
             command.append("--no-prune")
-        elif config.runner == CondaRunner.MAMBA:
-            command[0] = "conda"
         command.append("--force")
-    if dry_run:
-        command.append("--dry-run")
-    if isinstance(packages, str):
-        packages = [packages]
-    command.extend(packages)
-    command.append("--json")
 
-    _conda_install(project, command, verbose=verbose)
+    _conda_install(project, command, packages, dry_run=dry_run)
 
 
 def not_initialized_warning(project):
     project.core.ui.echo(
         "[warning]Tried to execute a conda command but no pdm-conda configs were found on pyproject.toml.[/]",
     )
 
@@ -317,15 +411,15 @@
         if config.runner != CondaRunner.MICROMAMBA:
             virtual_packages = {"=".join(p) for p in info["virtual_pkgs"]}
         else:
             virtual_packages = set(info["virtual packages"])
 
         res["virtual_packages"] = {parse_requirement(f"conda:{p.replace('=', '==', 1)}") for p in virtual_packages}
         res["platform"] = info["platform"]
-        res["channels"] = [_parse_channel(channel) for channel in (info["channels"] or [])]
+        res["channels"] = [parse_channel(channel) for channel in (info["channels"] or [])]
     else:
         not_initialized_warning(project)
     return res
 
 
 def conda_list(project: CondaProject) -> dict[str, CondaSetupDistribution]:
     """
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.0b0/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.0b0/src/pdm_conda/installers/synchronizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,25 +40,25 @@
     def compare_with_working_set(self) -> tuple[list[str], list[str], list[str]]:
         to_add, to_update, to_remove = super().compare_with_working_set()
 
         # deactivate parallel execution if uninstall
         self.parallel = self.environment.project.config["install.parallel"]
         if to_remove:
             to_remove = [p for p in to_remove if p not in self.environment.python_dependencies]
-     
+
         num_update, num_remove = (
             len([p for p in pks if isinstance(self.working_set[p], CondaSetupDistribution)])
             for pks in (to_update, to_remove)
         )
         if self.parallel and (num_update + num_remove > 0):
             self.environment.project.core.ui.echo("Deactivating parallel uninstall.")
             self.parallel = False
 
         if self.environment.project.conda_config.batched_commands:
             num_adds = len([p for p in to_add if isinstance(self.candidates[p], CondaCandidate)])
 
             self.manager.prepare_batch_operations(
                 num_install=num_adds + num_update,
-                num_remove=num_remove + num_update
+                num_remove=num_remove + num_update,
             )
 
         return to_add, to_update, to_remove
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/mapping.py` & `pdm_conda-0.9.0b0/src/pdm_conda/mapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,33 +66,30 @@
 
 
 @lru_cache
 def get_conda_mapping() -> dict[str, str]:
     return {v: k for k, v in get_pypi_mapping().items()}
 
 
-def _requirement_map(requirement: str, mapping: dict, exclude: set | None = None):
+def _requirement_map(requirement: str, mapping: dict):
     requirement = requirement.strip()
     name = requirement
     for s in (">", "<", "=", "!", "~", " ", "["):
         name = name.split(s, maxsplit=1)[0]
     name = name.split("::")[-1].strip()
-    if exclude is not None and name in exclude:
-        return name
-
     return mapping.get(name, name)
 
 
 def pypi_to_conda(requirement: str) -> str:
     """
     Map PyPI requirement to Conda version
     :param requirement: PyPI requirement
     :return: Conda requirement
     """
-    return _requirement_map(requirement, get_pypi_mapping())
+    return _requirement_map(requirement, get_pypi_mapping()).lower()
 
 
 def conda_to_pypi(requirement: str) -> str:
     """
     Map Conda requirement to PyPI version
     :param requirement: Conda requirement
     :return: PyPI requirement
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.0b0/src/pdm_conda/models/candidates.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 import functools
 import re
 from importlib.metadata import Distribution
 from pathlib import Path
 from typing import Any, cast
+from urllib.parse import urlparse
 
 from pdm.models.candidates import Candidate, PreparedCandidate
 from pdm.models.environment import Environment
 from pdm.models.setup import Setup
 from unearth import Link
 
 from pdm_conda.models.requirements import (
     CondaRequirement,
     Requirement,
+    as_conda_requirement,
     parse_conda_version,
     parse_requirement,
 )
 from pdm_conda.models.setup import CondaSetupDistribution
 
 _patched = False
 
 
+def parse_channel(channel_url: str) -> str:
+    """
+    Parse channel from channel url
+    :param channel_url: channel url from package
+    :return: channel
+    """
+    channel = urlparse(channel_url).path
+    if channel.startswith("/"):
+        channel = channel[1:]
+    return channel
+
+
 class CondaPreparedCandidate(PreparedCandidate):
     def __init__(self, candidate: Candidate, environment: Environment) -> None:
         super().__init__(candidate, environment)
         self.candidate = cast(CondaCandidate, self.candidate)  # type: ignore
 
     def get_dependencies_from_metadata(self) -> list[str]:
         # if conda candidate return already obtained dependencies
@@ -40,29 +54,35 @@
         req: Requirement,
         name: str | None = None,
         version: str | None = None,
         link: Link | None = None,
         dependencies: list[str] | None = None,
         constrains: list[str] | None = None,
         build_string: str | None = None,
+        build_number: int = 0,
+        timestamp: int = 0,
         channel: str | None = None,
+        track_feature: str = "",
     ):
         super().__init__(req, name, version, link)
         self._req = cast(CondaRequirement, req)  # type: ignore
         self._preferred = None
         self._prepared: CondaPreparedCandidate | None = None
         self.dependencies: list[CondaRequirement] = [parse_requirement(f"conda:{r}") for r in (dependencies or [])]
         self.constrains: dict[str, CondaRequirement] = dict()
         for r in constrains or []:
             c = cast(CondaRequirement, parse_requirement(f"conda:{r}"))
             self.constrains[str(c.conda_name)] = c
         self.build_string = build_string
+        self.build_number = build_number
+        self.timestamp = timestamp
         self.channel = channel
+        self.track_feature = track_feature
         self.conda_version = version
-        self.version = parse_conda_version(version, name == "openssl")
+        self.version = parse_conda_version(version)
 
     @property
     def req(self):
         return self._req
 
     @req.setter
     def req(self, value):
@@ -90,14 +110,17 @@
         result["conda_managed"] = True
         if self.link is None:
             raise ValueError("Uninitialized conda requirement")
         result["url"] = self.link.url
         result["channel"] = self.channel
         if self.build_string is not None:
             result["build_string"] = self.build_string
+        result["build_number"] = self.build_number
+        if self.track_feature:
+            result["track_feature"] = self.track_feature
         if self.constrains:
             result["constrains"] = [c.as_line(with_build_string=True) for c in self.constrains.values()]
         result["version"] = self.conda_version
         return result
 
     def prepare(self, environment: Environment) -> CondaPreparedCandidate:
         """Prepare the candidate for installation."""
@@ -115,18 +138,19 @@
         requires_python = package.get("requires_python", "")
         dependencies = package.get("dependencies", [])
         if requires_python:
             dependencies.append(f"python {requires_python}")
         return CondaCandidate.from_conda_package(package | {"depends": dependencies})
 
     @classmethod
-    def from_conda_package(cls, package: dict) -> "CondaCandidate":
+    def from_conda_package(cls, package: dict, requirement: CondaRequirement | None = None) -> "CondaCandidate":
         """
         Create conda candidate from conda package.
         :param package: conda package
+        :param requirement: conda requirement associated with conda package
         :return: conda candidate
         """
         dependencies: list = package["depends"] or []
         requires_python = None
         to_delete = []
         for d in dependencies:
             if d.startswith("__"):
@@ -139,30 +163,38 @@
             dependencies.remove(d)
         hashes = {h: package[h] for h in ["sha256", "md5"] if h in package}
         url = package["url"]
         for k, v in hashes.items():
             url += f"#{k}={v}"
         name, version = package["name"], package["version"]
         build_string = package.get("build", package.get("build_string", ""))
-        channel = package["channel"]
-        req = parse_requirement(f"conda:{name} {version} {build_string}")
-        req.is_python_package = requires_python is not None
+        channel = parse_channel(package["channel"])
+        if requirement is not None:
+            requirement = as_conda_requirement(requirement)
+        else:
+            requirement = parse_requirement(f"conda:{name} {version} {build_string}")
+
+        assert requirement is not None
+        requirement.is_python_package = requires_python is not None
         return CondaCandidate(
-            req=req,
+            req=requirement,
             name=name,
             version=version,
             link=Link(
                 url,
                 requires_python=requires_python,
                 comes_from=channel,
             ),
             channel=channel,
             dependencies=dependencies,
-            constrains=package.get("constrains", []),
+            constrains=package.get("constrains", None) or [],
             build_string=build_string,
+            build_number=package.get("build_number", 0),
+            track_feature=package.get("track_feature", ""),
+            timestamp=package.get("timestamp", 0),
         )
 
     def __str__(self) -> str:
         if self.req.is_named:
             return f"{self.name}@{self.conda_version}"
         return super().__str__()
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.0b0/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/models/config.py` & `pdm_conda-0.9.0b0/src/pdm_conda/models/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,32 @@
 from typing import Any
 
 from pdm.exceptions import ProjectError
 from pdm.project import ConfigItem, Project
 
 from pdm_conda.mapping import DOWNLOAD_DIR_ENV_VAR
 
+
+class CondaRunner(str, Enum):
+    CONDA = "conda"
+    MAMBA = "mamba"
+    MICROMAMBA = "micromamba"
+
+
+class CondaSolver(str, Enum):
+    CONDA = "conda"
+    MAMBA = "libmamba"
+
+
 _CONFIG_MAP = {"pypi-mapping.download-dir": "mapping_download_dir"}
 _CONFIG_MAP |= {v: k for k, v in _CONFIG_MAP.items()}
+
 CONFIGS = [
-    ("runner", ConfigItem("Conda runner executable", "conda", env_var="CONDA_RUNNER")),
+    ("runner", ConfigItem("Conda runner executable", CondaRunner.CONDA.value, env_var="CONDA_RUNNER")),
+    ("solver", ConfigItem("Solver to use for Conda resolution", CondaSolver.CONDA.value, env_var="CONDA_SOLVER")),
     ("channels", ConfigItem("Conda channels to use")),
     (
         "as-default-manager",
         ConfigItem("Use Conda to install all possible requirements", False, env_var="CONDA_AS_DEFAULT_MANAGER"),
     ),
     (
         "batched-commands",
@@ -41,63 +55,69 @@
         ConfigItem(
             "PyPI-Conda mapping download directory",
             Path().home() / ".pdm-conda/",
             env_var=DOWNLOAD_DIR_ENV_VAR,
         ),
     ),
 ]
+
 CONFIGS = [(f"conda.{name}", config) for name, config in CONFIGS]
 
 
 def is_decorated(func):
     return hasattr(func, "__wrapped__")
 
 
 def is_conda_config_initialized(project: Project):
     return "conda" in project.pyproject.settings
 
 
-class CondaRunner(str, Enum):
-    CONDA = "conda"
-    MAMBA = "mamba"
-    MICROMAMBA = "micromamba"
-
-
 @dataclass
 class PluginConfig:
     _project: Project = field(repr=False, default=None)
     _initialized: bool = field(repr=False, default=False, compare=False)
     _set_project_config: bool = field(repr=False, default=False, compare=False)
 
     channels: list[str] = field(default_factory=list)
-    runner: str = "conda"
+    runner: str = CondaRunner.CONDA
+    solver: str = CondaSolver.CONDA
     as_default_manager: bool = False
     batched_commands: bool = False
     installation_method: str = "hard-link"
     excludes: list[str] = field(default_factory=list, repr=False)
     dependencies: list[str] = field(default_factory=list, repr=False)
     optional_dependencies: dict[str, list] = field(default_factory=dict)
     dev_dependencies: dict[str, list] = field(default_factory=dict)
     mapping_download_dir: Path = field(repr=False, default=Path())
 
     def __post_init__(self):
         if self.runner not in list(CondaRunner):
             raise ProjectError(f"Invalid Conda runner: {self.runner}")
+        if self.solver not in list(CondaSolver):
+            raise ProjectError(f"Invalid Conda solver: {self.solver}")
         if self.installation_method not in ["hard-link", "copy"]:
             raise ProjectError(f"Invalid Conda installation method: {self.installation_method}")
         to_suscribe = [
             (self._project.pyproject._data, "update"),
             (self._project.pyproject, "write"),
             (self._project.pyproject, "reload"),
         ]
         for obj, name in to_suscribe:
             func = getattr(obj, name)
             if not is_decorated(func):
                 setattr(obj, name, self.suscribe(self, func))
         self._set_project_config = True
+        if self.is_initialized:
+            config = self._project.project_config
+            config["python.use_venv"] = True
+            config["python.use_pyenv"] = False
+            config["venv.backend"] = self.runner
+            if (venv_location := os.getenv("VIRTUAL_ENV", os.getenv("CONDA_PREFIX", None))) is not None:
+                self._project.global_config["venv.location"] = str(Path(venv_location).parent)
+                os.environ["PDM_IGNORE_SAVED_PYTHON"] = "true"
 
     def __setattr__(self, name: str, value: Any) -> None:
         super().__setattr__(name, value)
         # if plugin config is set then maybe update pyproject settings
         if not name.startswith("_") and not callable(getattr(self, name)):
             name = f"conda.{_CONFIG_MAP.get(name, name)}".replace("_", "-")
             name, config_item = next(filter(lambda n: name == n[0], CONFIGS))
@@ -132,25 +152,37 @@
             result = func(*args, **kwargs)
             config.reload()
             return result
 
         return wrapper
 
     @contextmanager
-    def omit_set_project_config(self):
+    def with_config(self, **kwargs):
         """
-        Context manager that deactivates updating pyproject settings
-        :return:
+        Context manager that temporarily updates configs without updating pyproject settings
         """
-        old_value = self._set_project_config
-        self._set_project_config = False
+        configs = ["_set_project_config"] + list(kwargs)
+        kwargs["_set_project_config"] = False
+        old_values = {}
+        for name in configs:
+            old_values[name] = getattr(self, name)
+            setattr(self, name, kwargs[name])
         try:
             yield
         finally:
-            self._set_project_config = old_value
+            for name in reversed(configs):
+                setattr(self, name, old_values[name])
+
+    @contextmanager
+    def omit_set_project_config(self):
+        """
+        Context manager that deactivates updating pyproject settings
+        """
+        with self.with_config():
+            yield
 
     @property
     def is_initialized(self):
         return self._initialized
 
     @classmethod
     def load_config(cls, project: Project, **kwargs) -> "PluginConfig":
@@ -176,16 +208,18 @@
 
     def command(self, cmd="install"):
         """
         Get runner command args
         :param cmd: command, install by default
         :return: args list
         """
-        _command = [self.runner, cmd]
+        _command = [self.runner, *cmd.split(" ")]
         if self.runner != CondaRunner.CONDA and cmd == "search":
             _command.insert(1, "repoquery")
 
-        if cmd in ("install", "create", "remove"):
+        if cmd in ("install", "remove", "create"):
             _command.append("-y")
         if cmd in ("install", "create") or (cmd == "search" and self.runner == CondaRunner.MICROMAMBA):
             _command.append("--strict-channel-priority")
+        if self.runner == CondaRunner.CONDA and self.solver == CondaSolver.MAMBA and cmd in ("create", "install"):
+            _command.extend(["--solver", self.solver])
         return _command
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.0b0/src/pdm_conda/models/environment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import functools
 import os
 import sysconfig
 from copy import copy
 from pathlib import Path
 from typing import cast
 
-from pdm.exceptions import NoPythonVersion, ProjectError
+from pdm.exceptions import ProjectError
 from pdm.models.environment import Environment, PrefixEnvironment
 from pdm.models.requirements import Requirement
+from pdm.models.specifiers import PySpecSet
 from pdm.models.working_set import WorkingSet
 from pdm.project import Project
 
-from pdm_conda.conda import conda_list, conda_search, logger
+from pdm_conda.conda import conda_list, conda_search
 from pdm_conda.mapping import pypi_to_conda
-from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
 _patched = False
 
 
 def ensure_conda_env():
@@ -27,56 +27,46 @@
 
 
 class CondaEnvironment(Environment):
     def __init__(self, project: Project) -> None:
         super().__init__(project)
         self.project = cast(CondaProject, project)
         self._python_dependencies: dict[str, Requirement] | None = None
-        self._python_candidate: CondaCandidate | None = None
+        self.python_requires &= PySpecSet(f"=={self.interpreter.version}")
 
     @property
     def packages_path(self) -> Path:
         return Path(ensure_conda_env())
 
     def get_paths(self) -> dict[str, str]:
         prefix = ensure_conda_env()
         paths = sysconfig.get_paths(vars={k: prefix for k in ("base", "platbase", "installed_base")}, expand=True)
         paths.setdefault("prefix", prefix)
-        logger.debug(f"paths: {paths}")
         return paths
 
     def get_working_set(self) -> WorkingSet:
         """
         Get the working set based on local packages directory, include Conda managed packages.
         """
         working_set = super().get_working_set()
         working_set._dist_map = conda_list(self.project) | {
             normalize_name(pypi_to_conda(dist.metadata["Name"])): dist for dist in working_set._dist_map.values()
         }
         return working_set
 
     @property
-    def python_candidate(self) -> CondaCandidate:
-        if self._python_candidate is None:
-            python_package = conda_list(self.project).get("python", None)
-            if python_package is None:
-                raise NoPythonVersion("No python found in Conda environment.")
-            self._python_candidate = conda_search(python_package.as_line().replace(" ", "="), self.project)[0]
-        return self._python_candidate
-
-    @property
     def python_dependencies(self) -> dict[str, Requirement]:
         if self._python_dependencies is None:
             self._python_dependencies = dict()
 
             def load_dependencies(name: str, packages: dict, dependencies: dict):
                 if name not in packages and name not in dependencies:
                     return
                 package = packages[name].as_line().replace(" ", "=")
-                candidate = conda_search(package, self.project)[0]
+                candidate = conda_search(self.project, package)[0]
                 dependencies[name] = candidate.req
                 for d in candidate.dependencies:
                     load_dependencies(d.name, packages, dependencies)
 
             load_dependencies("python", conda_list(self.project), self._python_dependencies)
 
         return self._python_dependencies
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.0b0/src/pdm_conda/models/requirements.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import re
 from copy import copy
 from typing import Any
 
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version
+from pdm.models.candidates import Candidate
 from pdm.models.requirements import NamedRequirement, Requirement, T
 from pdm.models.requirements import parse_requirement as _parse_requirement
 from pdm.models.requirements import strip_extras
 
 from pdm_conda.mapping import conda_to_pypi, pypi_to_conda
 from pdm_conda.utils import normalize_name
 
@@ -82,24 +83,34 @@
             self.key,
             frozenset(self.specifier),
         )
 
     def as_named_requirement(self) -> NamedRequirement:
         return NamedRequirement.create(name=conda_to_pypi(self.name), specifier=self.specifier)
 
-    def is_compatible(self, requirement: Requirement):
+    def is_compatible(self, requirement_or_candidate: Requirement | Candidate):
         _compatible = True
-        if (build_string := getattr(requirement, "build_string", "")) and self.build_string:
+        # test build string compatible
+        if (build_string := getattr(requirement_or_candidate, "build_string", "")) and self.build_string:
             _compatible &= re.match(rf"{self.build_string.replace('*', r'.*')}", build_string) is not None
-        return (
-            _compatible
-            and self.conda_name == requirement.conda_name
-            and all(self.specifier.contains(s.version) for s in requirement.specifier)
+
+        # test equal name
+        _compatible &= self.conda_name == getattr(
+            requirement_or_candidate,
+            "conda_name",
+            getattr(requirement_or_candidate, "name", ""),
         )
 
+        # test version/specifier compatible
+        if (version := getattr(requirement_or_candidate, "version", None)) is not None:
+            _compatible &= self.specifier.contains(version)
+        else:
+            _compatible &= all(self.specifier.contains(s.version) for s in requirement_or_candidate.specifier)
+        return _compatible
+
     def merge(self, requirement: Requirement) -> "CondaRequirement":
         """
         Merge with other requirement to get more specific
         :param requirement: other requirement
         :return: merged requirement
         """
         _req = copy(self)
@@ -221,15 +232,15 @@
                                 s = "="
                             conda_version_or = f"{s}={conda_version_or}"
                         _version = conda_version_or
                         if not _version.startswith("=="):
                             _version = _conda_specifier_star_re.sub(correct_specifier_star, _version)
                             if _version.startswith("~") and "." not in _version:
                                 _version += ".0"
-                        _version = parse_conda_version(_version, name == "openssl")
+                        _version = parse_conda_version(_version)
                         version_mapping[remove_operator(_version)] = remove_operator(conda_version_or)
                     version_or[j] = _version
             version_and[i] = max((v for v in version_or if v), key=comparable_version, default="")
         version = ",".join(version_and)
         req = CondaRequirement.create(
             name=strip_extras(name.strip())[0],
             specifier=SpecifierSet(version),
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/models/setup.py` & `pdm_conda-0.9.0b0/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/project.py` & `pdm_conda-0.9.0b0/src/pdm_conda/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from pathlib import Path
 from typing import Iterable, cast
 
 from pdm.core import Core
 from pdm.exceptions import ProjectError
 from pdm.models.environment import Environment
 from pdm.models.repositories import LockedRepository
-from pdm.models.specifiers import PySpecSet
 from pdm.project import Project
 from pdm.resolver.providers import BaseProvider
 from pdm.utils import get_venv_like_prefix
 from tomlkit.items import Array
 
 from pdm_conda.models.config import PluginConfig
 from pdm_conda.models.requirements import (
@@ -73,20 +72,14 @@
         try:
             lockfile = self.lockfile._data.unwrap()
         except ProjectError:
             lockfile = {}
 
         return self.locked_repository_class(lockfile, self.sources, self.environment)
 
-    @property
-    def python_requires(self) -> PySpecSet:
-        if not self._python:
-            return super().python_requires
-        return PySpecSet(f"=={self.python.version}")
-
     def _get_conda_info(self):
         from pdm_conda.conda import conda_info
 
         info = conda_info(self)
         self._virtual_packages = info["virtual_packages"]
         self._platform = info["platform"]
         self._default_channels = info["channels"]
@@ -160,15 +153,17 @@
         show_message: bool = True,
     ) -> None:
         conda_requirements = {n: r for n, r in requirements.items() if isinstance(r, CondaRequirement)}
         requirements = {n: r for n, r in requirements.items() if n not in conda_requirements} | {
             n: r.as_named_requirement() for n, r in conda_requirements.items() if r.is_python_package
         }
         if self.conda_config.as_default_manager:
-            conda_requirements = {n: r for n, r in conda_requirements.items() if not r.is_python_package}
+            conda_requirements = {
+                n: r for n, r in conda_requirements.items() if not r.is_python_package or r.channel or r.build_string
+            }
         if conda_requirements:
             deps = self.get_conda_pyproject_dependencies(to_group, dev, set_defaults=True)
             cast(Array, deps).multiline(True)
             for _, dep in conda_requirements.items():
                 matched_index = next((i for i, r in enumerate(deps) if dep.matches(f"conda:{r}")), None)
                 req = dep.as_line(with_channel=True)
                 if matched_index is None:
```

### Comparing `pdm_conda-0.8.1b3/src/pdm_conda/utils.py` & `pdm_conda-0.9.0b0/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b3/PKG-INFO` & `pdm_conda-0.9.0b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.8.1b3
-Summary:  A PDM plugin to install project dependencies with Conda
+Version: 0.9.0b0
+Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,21 +33,22 @@
 Requires-Python: >=3.10
 Requires-Dist: pdm~=2.4.0
 Requires-Dist: requests>=2.28.1
 Description-Content-Type: text/markdown
 
 # pdm-conda
 
-A PDM plugin to install project dependencies with Conda.
+A PDM plugin to resolve/install/uninstall project dependencies with Conda.
 
 ## Configuration
 
 | Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
 |-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
 | `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
+| `conda.solver`                    | Solver to use for Conda resolution                                                                   | `conda`             | `conda`, `libmamba`            | `CONDA_SOLVER`              |
 | `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
 | `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
 | `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
 | `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
 | `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
 | `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
 | `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
@@ -58,14 +59,15 @@
 
 ```toml
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
 dependencies = ["pdm"]
 as-default-manager = true
+solver = "libmamba"
 excludes = ["pytest-cov"] # don't install with conda even if it's a dependency from other packages
 installation-method = "copy"
 batched-commands = true
 
 [tool.pdm.conda.pypi-mapping]
 download-dir = "/tmp"
 
@@ -94,23 +96,31 @@
     * With flag `-r` or `--runner` you can specify the Conda runner to use.
 * `pdm remove`
 * `pdm list`
 * `pdm info`
 
 ### How it works
 
-When PDM detects a Conda managed package, it gets candidates with Conda and then tries to resolve the environment as
-with any other requirement.
+#### Using conda/libmamba solver
 
-To keep the resolution consistent with Conda, PDM follows resolution rules from Conda as good as possible.
+PDM invokes Conda solver to resolve conda packages each time a PDM candidate makes a change in the last Conda
+resolution.
+
+If only Conda packages are used (i.e. setting `conda.as-default-manager` to `true` and no `conda.excludes`) then Conda
+solver is invoked only once.
 
 ### Settings overriden
 
 In order to use Conda to install packages some settings were overriden:
 
+* `python.use_venv` if conda settings detected in `pyproject.toml` this setting is set to `True`.
+* `python.use_pyenv` if conda settings detected in `pyproject.toml` this setting is set to `False`.
+* `venv.backend` if conda settings detected in `pyproject.toml` this setting is set to `conda.runner`.
+* `venv.location` if conda settings detected in `pyproject.toml` and `VIRTUAL_ENV` or `CONDA_PREFIX` environment
+  variables are set then this setting is set to the value of the environment variable.
 * `install.parallel` if some Conda managed packages are to be uninstalled or updated this option is disabled
   momentarily.
 
 ## Development
 
 For development `docker-compose` files exist in `deploy` directory, helper script `deploy/docker-compose.sh` can be used
 for executing docker.
```

