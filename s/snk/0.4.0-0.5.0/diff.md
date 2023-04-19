# Comparing `tmp/snk-0.4.0.tar.gz` & `tmp/snk-0.5.0.tar.gz`

## Comparing `snk-0.4.0.tar` & `snk-0.5.0.tar`

### file list

```diff
@@ -1,68 +1,31 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.4.0/snk/__about__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.4.0/snk/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.4.0/snk/errors.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 snk-0.4.0/snk/main.py
--rw-r--r--   0        0        0     8624 2020-02-02 00:00:00.000000 snk-0.4.0/snk/nest.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 snk-0.4.0/snk/cli/__init__.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 snk-0.4.0/snk/cli/config.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 snk-0.4.0/snk/cli/gui.py
--rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 snk-0.4.0/snk/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.4.0/snk/cli/options.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 snk-0.4.0/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.4.0/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 snk-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 snk-0.4.0/tests/test_cli.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 snk-0.4.0/tests/test_nest.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.4.0/tests/test_snk
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.4.0/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/cov.fasta
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.editorconfig
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.gitattributes
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.gitignore
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.gitmodules
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.snakemake-workflow-catalog.yml
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/LICENSE
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.github/workflows/main.yml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.test/config/config.yaml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.test/config/samples.tsv
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/.test/config/units.tsv
--rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/bin/rna-seq-star-deseq2
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/config/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/config/config.yaml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/config/samples.tsv
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/config/units.tsv
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/Snakefile
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/envs/biomart.yaml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/envs/deseq2.yaml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/envs/gffutils.yaml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/envs/pandas.yaml
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/envs/rseqc.yaml
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/report/diffexp.rst
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/report/ma.rst
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/report/pca.rst
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/report/workflow.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/rules/align.smk
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/rules/common.smk
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/rules/diffexp.smk
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/rules/qc.smk
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/rules/ref.smk
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/rules/trim.smk
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/schemas/config.schema.yaml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/schemas/samples.schema.yaml
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/schemas/units.schema.yaml
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/count-matrix.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/deseq2-init.R
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/deseq2.R
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/gene2symbol.R
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/gtf2bed.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/plot-pca.R
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/workflow/scripts/common/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk-0.4.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 snk-0.4.0/README.md
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 snk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 snk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.5.0/Dockerfile
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.5.0/snk/__about__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.5.0/snk/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.5.0/snk/errors.py
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 snk-0.5.0/snk/main.py
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 snk-0.5.0/snk/nest.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/__init__.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/config.py
+-rw-r--r--   0        0        0    12284 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/options.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/pipeline.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 snk-0.5.0/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.5.0/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 snk-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 snk-0.5.0/tests/test_nest.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 snk-0.5.0/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.5.0/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.5.0/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/pipeline/Snakefile
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.5.0/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 snk-0.5.0/README.md
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 snk-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 snk-0.5.0/PKG-INFO
```

### Comparing `snk-0.4.0/snk/main.py` & `snk-0.5.0/snk/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typer
 from pathlib import Path
 import os
-from typing import Optional
+from typing import Optional, List
 from rich.pretty import pprint
 from .nest import Nest
 from .errors import PipelineExistsError, PipelineNotFoundError
 
 app = typer.Typer()
 
 SNK_HOME = None
@@ -51,15 +51,15 @@
     SNK_HOME = home
     
 
 
 @app.command()
 def install(
         pipeline: str = typer.Argument(
-            ..., help="URL or Github name (user/repo) of the pipeline to install."
+            ..., help="Path, URL or Github name (user/repo) of the pipeline to install."
         ),
         name: Optional[str] = typer.Option(
             None, 
             help="Rename the pipeline (this name will be used to call the CLI.)"
         ),
         tag: Optional[str] = typer.Option(
             None,
@@ -67,33 +67,36 @@
             "-t",
             help="Tag (version) of the pipeline to install. Can specify a branch name, or tag. If None the latest commit will be installed."
         ),
         config: Optional[Path] = typer.Option(
             None, 
             help="Specify a non-standard config location."
         ),
+        resource: Optional[List[Path]] = typer.Option(
+            [], 
+            help="Specify a resource required to run the pipeline (copied to working dir at runtime)."
+        ),
     ):
     """
     Install a pipeline.
     """
-    
     nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
-    if not pipeline.startswith('http'):
+    if not Path(pipeline).exists() and not pipeline.startswith('http'):
         pipeline = f"https://github.com/{pipeline}.git"
     try:
-        installl_pipeline = nest.install(repo_url=pipeline, name=name, tag=tag, config=config)
+        installed_pipeline = nest.install(pipeline, name=name, tag=tag, config=config, resources=resource)
     except PipelineExistsError as e:
         typer.secho(e, fg='red')
         raise typer.Exit()
     except PipelineNotFoundError as e:
         typer.secho(e, fg='red')
         raise typer.Exit()
-    v = installl_pipeline.version
+    v = installed_pipeline.version
     v = v if v else 'latest'
-    typer.secho(f"Successfully installed {installl_pipeline.name} ({v})!", fg='green')
+    typer.secho(f"Successfully installed {installed_pipeline.name} ({v})!", fg='green')
 
 
 @app.command()
 def uninstall(
         name: str = typer.Argument(..., help="Name of the pipeline to uninstall."),
         force: Optional[bool] = typer.Option(False, '--force', '-f', help="Force uninstall without asking."),
     ):
```

### Comparing `snk-0.4.0/snk/nest.py` & `snk-0.5.0/snk/nest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,20 @@
 from pathlib import Path
-from git import Repo, GitCommandError
+from git import InvalidGitRepositoryError, Repo, GitCommandError
 import sys
 import stat
 import inspect
 import os
 from typing import List
 import shutil
+import yaml
 
-from .errors import PipelineExistsError, PipelineNotFoundError
-
-class Pipeline:
-    def __init__(self, path:Path) -> None:
-        self.path = path
-        self.repo = Repo(path)
-        self.name = self.path.name
-    
-    @property
-    def version(self):
-        try:
-            # TODO: default to commit
-            version = self.repo.git.describe(['--tags','--exact-match']) 
-        except GitCommandError:
-            version = None
-        return version
-
-    @property
-    def executable(self):
-        pipeline_bin_dir = self.path / 'bin'
-        name = self.name
-        if sys.platform.startswith('win'):
-            name += '.exe'
-        return pipeline_bin_dir / name
-        
+from .errors import PipelineExistsError, PipelineNotFoundError, InvalidPipelineRepositoryError
+from .cli.config import SnkConfig
+from .cli.pipeline import Pipeline
 
 
 class Nest:
     """Class for managing Snk pipelines"""
 
     def __init__(self, snk_home: Path = None, bin_dir: Path = None) -> None:
         self.python_interpreter_path = Path(sys.executable) # needs to be the same python that has snk
@@ -59,47 +38,64 @@
         self.bin_dir = Path(bin_dir).absolute()
         
         # Create dirs
         self.snk_home.mkdir(parents=True, exist_ok=True)
         self.pipelines_dir.mkdir(parents=True, exist_ok=True)
         self.bin_dir.mkdir(parents=True, exist_ok=True)
 
-    def _check_repo_url_format(self, repo):
+    def _check_repo_url_format(self, repo: str):
+        if not repo.startswith('http'):
+            raise InvalidPipelineRepositoryError('Repo url must start with http')
         if not repo.endswith('.git'):
-            raise ValueError('Repo url must end in .git')
+            raise InvalidPipelineRepositoryError('Repo url must end in .git')
 
-    def install(self, repo_url: str, name = None, tag = None, config: Path = None, force = False, resources=[]) -> Pipeline:
+    def install(self, pipeline: str, editable = False, name = None, tag = None, config: Path = None, force = False, resources=[]) -> Pipeline:
         """
         Install a Snakemake pipeline as a CLI. 
         They must be standards compliant*, public, Snakemake workflows.
         https://snakemake.github.io/snakemake-workflow-catalog/
         """
-        self._check_repo_url_format(repo_url)
-        if not name:
-            name = self._get_name_from_git_url(repo_url)
-        if name in os.listdir(self.pipelines_dir):
-            raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.pipelines_dir}")
-        if name in os.listdir(self.bin_dir):
-            raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.bin_dir}")
-        repo = self.download(repo_url, name, tag_name=tag)
+        try:
+            self._check_repo_url_format(pipeline)
+            if not name:
+                name = self._get_name_from_git_url(pipeline)
+            if name in os.listdir(self.pipelines_dir):
+                raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.pipelines_dir}")
+            if name in os.listdir(self.bin_dir):
+                raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.bin_dir}")
+            repo = self.download(pipeline, name, tag_name=tag)
+        except InvalidPipelineRepositoryError:
+            pipeline = Path(pipeline)
+            if pipeline.suffix == '.snk':
+                pipeline = pipeline.parent
+            if not name:
+                name = pipeline.name
+            repo = self.local(pipeline, name, editable)
         try:
             pipeline = Pipeline(path=Path(repo.git_dir).parent)
             pipeline_executable = self.create_package(pipeline.path)
             self.link_pipeline_executable_to_bin(pipeline_executable)
             if config:
                 self.copy_nonstandard_config(pipeline.path, config)
             if resources:
-                self.copy_additional_resources(pipeline.path, config)
+                self.additional_resources(pipeline.path, resources)
             self._confirm_installation(name)
         except Exception as e:
             # remove any half completed steps 
             to_remove = self.get_paths_to_delete(name)
             self.delete_paths(to_remove)
             raise e
         return pipeline
+    
+    def additional_resources(self, pipeline_dir: Path, resources: List[Path]):
+        """Modify the .snk file so that resources will be copied at runtime."""
+        # validate_resources(resources)
+        snk_config = SnkConfig.from_path(pipeline_dir / '.snk')
+        snk_config.resources += [r for r in resources if r not in snk_config.resources]
+        snk_config.to_yaml(pipeline_dir / '.snk')
 
     def copy_nonstandard_config(self, pipeline_dir: Path, config_path: Path):
         config_dir = pipeline_dir / 'config'
         config_dir.mkdir()
         shutil.copyfile(pipeline_dir / config_path, config_dir / 'config.yaml')
 
     def get_paths_to_delete(self, pipeline_name: str) -> List[Path]:
@@ -176,14 +172,27 @@
                 raise PipelineExistsError(f"Pipeline '{name}' already exists in {self.pipelines_dir}")
             elif f"Remote branch {tag_name}" in e.stderr:
                 raise PipelineNotFoundError(f"Pipeline tag '{tag_name}' not found")
             elif "not found" in e.stderr:
                 raise PipelineNotFoundError(f"Pipeline repository '{repo_url}' not found")
             raise e
         return repo
+    
+    def local(self, path: Path, name: str, editable=False):
+        location  = self.pipelines_dir / name
+        if editable:
+            os.symlink(path, location)
+        else:
+            shutil.copytree(path, location)
+        try:
+            return Repo(location)
+        except InvalidGitRepositoryError:
+            return Repo.init(location, mkdir=False)
+        
+
 
     def create_package(self, pipeline_dir: Path) -> Path:
         """Convert a SnakeMake pipeline repo into a snk CLI"""
         self.validate_SnakeMake_repo(pipeline_dir)
         
         template = inspect.cleandoc(f"""
             #!/bin/sh
```

### Comparing `snk-0.4.0/snk/cli/utils.py` & `snk-0.5.0/snk/cli/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,20 @@
     'int': int,
     'integer': int,
     'str': str,
     'string': str,
     'path': Path,
     'bool': bool,
     'boolean': bool,
-    'list': List[str]
+    'list': List[str],
+    'list[path]': List[Path],
+    'list[int]': List[int],
 }
 
 def create_cli_parameter(option):
-
     return Parameter(
         option['name'], 
         kind=Parameter.POSITIONAL_OR_KEYWORD, 
         default=typer.Option(... if option['required'] else option['default'], help=f"[CONFIG] {option['help']}"), 
         annotation=types.get(option['type'].lower(), str))
 
 def add_dynamic_options(options: List[dict]):
```

### Comparing `snk-0.4.0/tests/.DS_Store` & `snk-0.5.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.4.0/tests/test_nest.py` & `snk-0.5.0/tests/test_nest.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 def test_init(bin_dir, snk_home):
     nest = Nest(snk_home, bin_dir=bin_dir)
     assert nest.pipelines_dir == Path(snk_home) / 'pipelines'
     for path in [nest.pipelines_dir, nest.bin_dir, nest.snk_home]:
         assert path.exists()
 
 def test_download(nest: Nest):
-    repo = nest.download('https://github.com/snakemake-workflows/rna-seq-star-deseq2.git', 'rna-seq-star-deseq2')
+    repo = nest.download('https://github.com/Wytamma/snk-basic-pipeline.git', 'rna-seq-star-deseq2')
     expected_location = nest.pipelines_dir / 'rna-seq-star-deseq2'
     assert (expected_location).exists()
     assert Path(repo.git_dir).parent == expected_location
 
 def test_create_package(nest: Nest):
     test_pipeline_path = nest.pipelines_dir / 'pipeline-name'
     test_pipeline_path.mkdir()
     path = nest.create_package(pipeline_dir=test_pipeline_path)
     assert path == test_pipeline_path / 'bin' / 'pipeline-name'
 
 def test_link_pipeline_executable_to_bin(nest: Nest):
-    pipeline_executable_path = Path('tests/data/snk/pipelines/rna-seq-star-deseq2/bin/rna-seq-star-deseq2')
+    pipeline_executable_path = Path('tests/data/bin/snk-basic-pipeline')
     executable_path = nest.link_pipeline_executable_to_bin(pipeline_executable_path)
     assert executable_path.exists() == True and executable_path.is_symlink() == True
 
 def test_uninstall(nest:Nest):
-    pass
+    pass
```

### Comparing `snk-0.4.0/tests/utils.py` & `snk-0.5.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.4.0/tests/data/artic_v4.1.bed` & `snk-0.5.0/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.4.0/tests/data/config.yaml` & `snk-0.5.0/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.4.0/tests/data/cov.fasta` & `snk-0.5.0/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.4.0/tests/data/snk/pipelines/rna-seq-star-deseq2/LICENSE` & `snk-0.5.0/LICENSE.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 MIT License
 
-Copyright (c) 2017, Johannes Köster
+Copyright (c) 2022-present Wytamma Wirth <wytamma.wirth@me.com>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `snk-0.4.0/README.md` & `snk-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 ```console
 pip install snk
 ```
 
 ## About
 
-Snk is a SnakeMake pipeline management system. Snk allows you to install SnakeMake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases it's interoperability and allows complex pipelines to be used as modular components in a larger system.
+Snk is a SnakeMake pipeline management system. Snk allows you to install SnakeMake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system.
 
 ## Basic Use
 
 ### Install a pipeline as a CLI
 
 ```
 snk install snakemake-workflows/rna-seq-star-deseq2
```

### Comparing `snk-0.4.0/pyproject.toml` & `snk-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -44,21 +44,27 @@
 path = "snk/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
 ]
+
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=snk --cov=tests"
-no-cov = "cov --no-cov"
+test = "cov --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
 
+# requires hatch-containers
+[tool.hatch.envs.docker]
+type = "container"
+image = "wytamma/snk"
+
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "snk/__about__.py",
 ]
```

### Comparing `snk-0.4.0/PKG-INFO` & `snk-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.4.0
+Version: 0.5.0
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,15 @@
 
 ```console
 pip install snk
 ```
 
 ## About
 
-Snk is a SnakeMake pipeline management system. Snk allows you to install SnakeMake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases it's interoperability and allows complex pipelines to be used as modular components in a larger system.
+Snk is a SnakeMake pipeline management system. Snk allows you to install SnakeMake pipelines as Command Line Interfaces (CLIs). Using a pipeline as a CLI increases its interoperability and allows complex pipelines to be used as modular components in a larger system.
 
 ## Basic Use
 
 ### Install a pipeline as a CLI
 
 ```
 snk install snakemake-workflows/rna-seq-star-deseq2
```

