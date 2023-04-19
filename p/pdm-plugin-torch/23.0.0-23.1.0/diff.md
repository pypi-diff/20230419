# Comparing `tmp/pdm-plugin-torch-23.0.0.tar.gz` & `tmp/pdm-plugin-torch-23.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-plugin-torch-23.0.0.tar", last modified: Wed Mar  1 14:11:13 2023, max compression
+gzip compressed data, was "pdm-plugin-torch-23.1.0.tar", last modified: Wed Apr 19 14:11:32 2023, max compression
```

## Comparing `pdm-plugin-torch-23.0.0.tar` & `pdm-plugin-torch-23.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      474 2023-03-01 14:10:13.379344 pdm-plugin-torch-23.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    10841 2023-03-01 14:10:13.379344 pdm-plugin-torch-23.0.0/LICENSE-APACHE
--rw-r--r--   0        0        0     1074 2023-03-01 14:10:13.379344 pdm-plugin-torch-23.0.0/LICENSE-MIT
--rw-r--r--   0        0        0     2885 2023-03-01 14:10:13.379344 pdm-plugin-torch-23.0.0/README.md
--rw-r--r--   0        0        0        9 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/pdm-plugin-torch/pdm_plugin_torch/__init__.py
--rw-r--r--   0        0        0     1295 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/pdm-plugin-torch/pdm_plugin_torch/config.py
--rw-r--r--   0        0        0    12653 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/pdm-plugin-torch/pdm_plugin_torch/main.py
--rw-r--r--   0        0        0     1590 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2370 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/tests/conftest.py
--rw-r--r--   0        0        0      574 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/tests/fixtures/cpu-only/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-03-01 14:10:13.383344 pdm-plugin-torch-23.0.0/tests/test_lock.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 pdm-plugin-torch-23.0.0/PKG-INFO
+-rw-r--r--   0        0        0      614 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    10841 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/LICENSE-APACHE
+-rw-r--r--   0        0        0     1074 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/LICENSE-MIT
+-rw-r--r--   0        0        0     2885 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/README.md
+-rw-r--r--   0        0        0        9 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/__init__.py
+-rw-r--r--   0        0        0     1295 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/config.py
+-rw-r--r--   0        0        0    16668 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/main.py
+-rw-r--r--   0        0        0     1590 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2370 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      574 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/fixtures/cpu-only/pyproject.toml
+-rw-r--r--   0        0        0     2018 2023-04-19 14:10:59.681309 pdm-plugin-torch-23.1.0/tests/test_lock.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 pdm-plugin-torch-23.1.0/PKG-INFO
```

### Comparing `pdm-plugin-torch-23.0.0/LICENSE-APACHE` & `pdm-plugin-torch-23.1.0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.0.0/LICENSE-MIT` & `pdm-plugin-torch-23.1.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.0.0/README.md` & `pdm-plugin-torch-23.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.0.0/pdm-plugin-torch/pdm_plugin_torch/config.py` & `pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/config.py`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.0.0/pdm-plugin-torch/pdm_plugin_torch/main.py` & `pdm-plugin-torch-23.1.0/pdm-plugin-torch/pdm_plugin_torch/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,97 +3,197 @@
 import sys
 
 from typing import Iterable
 
 import tomlkit
 
 from pdm import __version__, termui
-from pdm._types import Source
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.utils import fetch_hashes, format_lockfile, format_resolution_impossible
 from pdm.core import Core
 from pdm.models.candidates import Candidate
 from pdm.models.repositories import BaseRepository, LockedRepository
 from pdm.models.requirements import Requirement, parse_requirement
 from pdm.models.specifiers import PySpecSet, get_specifier
 from pdm.project import Project
 from pdm.project.config import ConfigItem
 from pdm.resolver import resolve
 from pdm.resolver.providers import BaseProvider
 from pdm.termui import Verbosity
-from pdm.utils import atomic_open_for_write
+from pdm.utils import atomic_open_for_write, expand_env_vars_in_auth
 from resolvelib.reporters import BaseReporter
 from resolvelib.resolvers import ResolutionImpossible, ResolutionTooDeep, Resolver
 
 from pdm_plugin_torch.config import Configuration
 
 
 is_pdm22 = PySpecSet("<2.3").contains(__version__.__version__)
+is_pdm24 = PySpecSet("<2.5").contains(__version__.__version__)
 
+if is_pdm24:
+    from pdm._types import Source as RepositoryConfig
 
-def sources(project: Project, sources: list) -> list[Source]:
-    if all(source.get("name") != "pypi" for source in sources):
-        sources.insert(0, project.default_source)
-    expanded_sources: list[Source] = [
-        Source(
-            url=s["url"],
-            verify_ssl=s.get("verify_ssl", True),
-            name=s.get("name"),
-            type=s.get("type", "index"),
+    def sources(project: Project, sources: list) -> list[RepositoryConfig]:
+        if all(source.get("name") != "pypi" for source in sources):
+            sources.insert(0, project.default_source)
+
+        expanded_sources: list[RepositoryConfig] = [
+            RepositoryConfig(
+                url=s["url"],
+                verify_ssl=s.get("verify_ssl", True),
+                name=s.get("name"),
+                type=s.get("type", "index"),
+            )
+            for s in sources
+        ]
+        return expanded_sources
+
+    def get_provider(
+        project: Project,
+        raw_sources: list,
+        strategy: str = "all",
+        for_install: bool = False,
+        lockfile: dict = None,
+    ) -> BaseProvider:
+        """Build a provider class for resolver.
+        :param strategy: the resolve strategy
+        :param tracked_names: the names of packages that needs to update
+        :param for_install: if the provider is for install
+        :returns: The provider object
+        """
+
+        from pdm.resolver.providers import BaseProvider
+
+        repository = get_repository(
+            project, raw_sources, for_install=for_install, lockfile=lockfile
+        )
+        allow_prereleases = False
+
+        return BaseProvider(repository, allow_prereleases, [])
+
+else:
+    from pdm._types import RepositoryConfig
+
+    def sources(project: Project, sources: list) -> list[RepositoryConfig]:
+        result: dict[str, RepositoryConfig] = {}
+        for source in project.pyproject.settings.get("source", []):
+            result[source["name"]] = RepositoryConfig(**source)
+
+        for source in sources:
+            result[source["name"]] = RepositoryConfig(**source)
+
+        def merge_sources(
+            other_sources: Iterable[tuple[str, RepositoryConfig]]
+        ) -> None:
+            for name, source in other_sources:
+                source.name = name
+                if name in result:
+                    result[name].passive_update(source)
+                else:
+                    result[name] = source
+
+        if not project.config.get("pypi.ignore_stored_index", False):
+            if "pypi" not in result:  # put pypi source at the beginning
+                result = {"pypi": project.default_source, **result}
+            else:
+                result["pypi"].passive_update(project.default_source)
+            merge_sources(project.project_config.iter_sources())
+            merge_sources(project.global_config.iter_sources())
+
+        for source in result.values():
+            assert source.url, "Source URL must not be empty"
+            source.url = expand_env_vars_in_auth(source.url)
+
+        return list(result.values())
+
+    def get_provider(
+        project: Project,
+        raw_sources: list,
+        strategy: str = "all",
+        for_install: bool = False,
+        lockfile: dict = None,
+        tracked_names: Iterable[str] | None = None,
+        allow_prereleases: bool = False,
+    ) -> BaseProvider:
+        """Build a provider class for resolver.
+        :param strategy: the resolve strategy
+        :param tracked_names: the names of packages that needs to update
+        :param for_install: if the provider is for install
+        :returns: The provider object
+        """
+        from pdm.models.requirements import strip_extras
+        from pdm.resolver.providers import (
+            BaseProvider,
+            EagerUpdateProvider,
+            ReusePinProvider,
+        )
+        from pdm.utils import normalize_name
+
+        repository = get_repository(
+            project, raw_sources, for_install=for_install, lockfile=lockfile
+        )
+
+        overrides = {
+            normalize_name(k): v
+            for k, v in project.pyproject.resolution_overrides.items()
+        }
+
+        locked_repository: LockedRepository | None = None
+        if strategy != "all" or for_install:
+            try:
+                locked_repository = LockedRepository(
+                    lockfile, sources, project.environment
+                )
+            except Exception:
+                if for_install:
+                    raise
+                project.core.ui.echo(
+                    "Unable to reuse the lock file as it is not compatible with PDM",
+                    style="warning",
+                    err=True,
+                )
+
+        if locked_repository is None:
+            return BaseProvider(repository, allow_prereleases, overrides)
+
+        if for_install:
+            return BaseProvider(locked_repository, allow_prereleases, overrides)
+
+        provider_class = (
+            ReusePinProvider if strategy == "reuse" else EagerUpdateProvider
+        )
+        tracked_names = [strip_extras(name)[0] for name in tracked_names or ()]
+
+        return provider_class(
+            locked_repository.all_candidates,
+            tracked_names,
+            repository,
+            allow_prereleases,
+            overrides,
         )
-        for s in sources
-    ]
-    return expanded_sources
 
 
 def get_repository(
     project: Project,
     raw_sources: list,
     cls: type[BaseRepository] | None = None,
     for_install: bool = False,
     lockfile: dict = None,
 ) -> BaseRepository:
     """Get the repository object"""
     if cls is None:
         cls = project.core.repository_class
 
     fixed_sources = sources(project, raw_sources)
-    if for_install:
-        return LockedRepository(lockfile, fixed_sources, project.environment)
-
     return cls(
         fixed_sources,
         project.environment,
     )
 
 
-def get_provider(
-    project: Project,
-    raw_sources: list,
-    strategy: str = "all",
-    for_install: bool = False,
-    lockfile: dict = None,
-) -> BaseProvider:
-    """Build a provider class for resolver.
-    :param strategy: the resolve strategy
-    :param tracked_names: the names of packages that needs to update
-    :param for_install: if the provider is for install
-    :returns: The provider object
-    """
-
-    from pdm.resolver.providers import BaseProvider
-
-    repository = get_repository(
-        project, raw_sources, for_install=for_install, lockfile=lockfile
-    )
-    allow_prereleases = False
-
-    return BaseProvider(repository, allow_prereleases, [])
-
-
 def do_lock(
     project: Project,
     raw_sources: list,
     strategy: str = "all",
     requirements: list[Requirement] | None = None,
 ) -> dict[str, Candidate]:
     """Performs the locking process and update lockfile."""
@@ -104,21 +204,22 @@
     with ui.logging("lock"):
         # The context managers are nested to ensure the spinner is stopped before
         # any message is thrown to the output.
         try:
             with ui.open_spinner(title="Resolving dependencies") as spin:
                 reporter = project.get_reporter(requirements, None, spin)
                 resolver: Resolver = project.core.resolver_class(provider, reporter)
-
                 mapping, dependencies = resolve(
                     resolver,
                     requirements,
                     project.environment.python_requires,
                     resolve_max_rounds,
                 )
+
+                spin.update("Fetching hashes for resolved packages...")
                 fetch_hashes(provider.repository, mapping)
 
         except ResolutionTooDeep:
             ui.echo(f"{termui.Emoji.LOCK} Lock failed", err=True)
             ui.echo(
                 "The dependency resolution exceeds the maximum loop depth of "
                 f"{resolve_max_rounds}, there may be some circular dependencies "
@@ -159,26 +260,27 @@
     resolve_max_rounds = int(project.config["strategy.resolve_max_rounds"])
     reqs = [
         req
         for req in requirements
         if not req.marker or req.marker.evaluate(project.environment.marker_environment)
     ]
     with ui.logging("install-resolve"):
-        with ui.open_spinner("Resolving packages from lockfile..."):
+        with ui.open_spinner("Resolving packages from lockfile...") as spinner:
             reporter = BaseReporter()
             provider = get_provider(
                 project, raw_sources, for_install=True, lockfile=lockfile
             )
             resolver: Resolver = project.core.resolver_class(provider, reporter)
             mapping, *_ = resolve(
                 resolver,
                 reqs,
                 project.environment.python_requires,
                 resolve_max_rounds,
             )
+            spinner.update("Fetching hashes for resolved packages...")
             fetch_hashes(provider.repository, mapping)
 
     return mapping
 
 
 def do_sync(
     project: Project,
@@ -201,15 +303,16 @@
         no_editable=True,
         install_self=False,
         use_install_cache=project.config["install.cache"],
         reinstall=True,
         only_keep=False,
     )
 
-    handler.synchronize()
+    with project.core.ui.logging("install"):
+        handler.synchronize()
 
 
 def read_lockfile(project: Project, lock_name: str) -> None:
     lockfile_file = project.root / lock_name
 
     data = tomlkit.parse(lockfile_file.read_text("utf-8"))
     return data
@@ -281,45 +384,18 @@
     if is_pdm22:
         return project.pyproject["tool"]["pdm"]["plugins"]["torch"]
 
     else:
         return project.pyproject.settings["plugins"]["torch"]
 
 
-class TorchCommand(BaseCommand):
-    """Generate a lockfile for torch specifically."""
-
-    def add_arguments(self, parser):
-        subparsers = parser.add_subparsers(help="sub-command help", dest="command")
-        subparsers.required = True
-
-        parser_install = subparsers.add_parser(
-            "install", help="install a torch variant"
-        )
-        parser_install.add_argument(
-            "api", help="the api to use, e.g. cuda version or rocm"
-        )
-        parser_install.set_defaults(command="install")
-
-        parser_lock = subparsers.add_parser("lock", help="update lockfile")
-        parser_lock.add_argument(
-            "--check",
-            help="validate that the lockfile is up to date",
-            action="store_true",
-        )
-        parser_lock.set_defaults(command="lock")
-
-    def handle(self, project, options):
-        if options.command == "install":
-            self.handle_install(project, options)
-
-        elif options.command == "lock":
-            self.handle_lock(project, options)
+class InstallCommand:
+    name = "install"
 
-    def handle_install(self, project, options):
+    def handle(self, project: Project, options: dict):
         plugin_config = Configuration.from_toml(get_settings(project))
 
         resolves = plugin_config.variants
         if options.api not in resolves:
             raise ValueError(
                 f"unknown API {options.api}, expected one of {[v for v in resolves]}"
             )
@@ -336,21 +412,26 @@
         do_sync(
             project,
             raw_sources=[
                 {
                     "name": "torch",
                     "url": source,
                     "type": "index",
+                    "verify_ssl": True,
                 }
             ],
             requirements=reqs,
             lockfile=spec_for_version,
         )
 
-    def handle_lock(self, project, options):
+
+class LockCommand:
+    name = "lock"
+
+    def handle(self, project: Project, options: dict):
         plugin_config = Configuration.from_toml(get_settings(project))
 
         if options.check:
             is_updated = check_lockfile(project, plugin_config.lockfile)
             if not is_updated:
                 project.core.ui.echo(
                     "Lockfile is [error]out of date[/].",
@@ -376,18 +457,47 @@
             results[api] = do_lock(
                 project,
                 [
                     {
                         "name": "torch",
                         "url": url,
                         "type": "index",
+                        "verify_ssl": True,
                     }
                 ],
                 requirements=reqs,
             )
 
         write_lockfile(project, plugin_config.lockfile, results)
 
 
+class TorchCommand(BaseCommand):
+    """Generate a lockfile for torch specifically."""
+
+    name = "torch"
+
+    def add_arguments(self, parser):
+        subparsers = parser.add_subparsers(help="sub-command help", dest="command")
+        subparsers.required = True
+
+        parser_install = subparsers.add_parser(
+            "install", help="install a torch variant"
+        )
+        parser_install.add_argument(
+            "api", help="the api to use, e.g. cuda version or rocm"
+        )
+        parser_install.set_defaults(command=InstallCommand())
+
+        parser_lock = subparsers.add_parser("lock", help="update lockfile")
+        parser_lock.add_argument(
+            "--check",
+            help="validate that the lockfile is up to date",
+            action="store_true",
+        )
+        parser_lock.set_defaults(command=LockCommand())
+
+    def handle(self, project, options):
+        options.command.handle(project, options)
+
+
 def torch_plugin(core: Core):
     core.register_command(TorchCommand, "torch")
-    core.add_config("hello.name", ConfigItem("The person's name", "John"))
```

### Comparing `pdm-plugin-torch-23.0.0/pyproject.toml` & `pdm-plugin-torch-23.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pdm-plugin-torch"
-version = "23.0.0"
+version = "23.1.0"
 description = "A plugin to help installing torch versions"
 authors = [
     { name = "Embark Studios", email = "python@embark-studios.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = []
```

### Comparing `pdm-plugin-torch-23.0.0/tests/conftest.py` & `pdm-plugin-torch-23.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-plugin-torch-23.0.0/tests/test_lock.py` & `pdm-plugin-torch-23.1.0/tests/test_lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,28 +53,28 @@
 
     @staticmethod
     def test_lock_check_fails(tmpdir, pdm):
         import subprocess
 
         tmpdir_project("cpu-only", tmpdir)
         with pytest.raises(subprocess.CalledProcessError):
-            pdm(["torch", "lock", "--check"], tmpdir)
+            pdm(["torch", "-v", "lock", "--check"], tmpdir)
 
     @staticmethod
     def test_lock_plugin_check_succeeds(tmpdir, pdm):
         tmpdir_project("cpu-only", tmpdir)
-        pdm(["torch", "lock"], tmpdir)
-        pdm(["torch", "lock", "--check"], tmpdir)
+        pdm(["torch", "-v", "lock"], tmpdir)
+        pdm(["torch", "-v", "lock", "--check"], tmpdir)
 
     @staticmethod
     def test_install_fails(tmpdir, pdm):
         import subprocess
 
         tmpdir_project("cpu-only", tmpdir)
         with pytest.raises(subprocess.CalledProcessError):
-            pdm(["torch", "install", "cpu"], tmpdir)
+            pdm(["torch", "-v", "install", "cpu"], tmpdir)
 
     @staticmethod
     def test_install_succeeds(tmpdir, pdm):
         tmpdir_project("cpu-only", tmpdir)
-        pdm(["torch", "lock"], tmpdir)
-        pdm(["torch", "install", "cpu"], tmpdir)
+        pdm(["torch", "-v", "lock"], tmpdir)
+        pdm(["torch", "-v", "install", "cpu"], tmpdir)
```

### Comparing `pdm-plugin-torch-23.0.0/PKG-INFO` & `pdm-plugin-torch-23.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-plugin-torch
-Version: 23.0.0
+Version: 23.1.0
 Summary: A plugin to help installing torch versions
 License: MIT
 Author-email: Embark Studios <python@embark-studios.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/EmbarkStudios/pdm-plugin-torch
 Description-Content-Type: text/markdown
```

