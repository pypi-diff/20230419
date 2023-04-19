# Comparing `tmp/hokusai-1.0.5.tar.gz` & `tmp/hokusai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hokusai-1.0.5.tar", max compression
+gzip compressed data, was "hokusai-1.1.0.tar", max compression
```

## Comparing `hokusai-1.0.5.tar` & `hokusai-1.1.0.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     1068 2023-03-06 17:27:08.094422 hokusai-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0    10166 2023-03-06 17:27:08.094422 hokusai-1.0.5/README.md
--rw-r--r--   0        0        0       96 2023-03-06 17:27:08.102422 hokusai-1.0.5/hokusai/__init__.py
--rw-r--r--   0        0        0      214 2023-03-06 17:27:50.946693 hokusai-1.0.5/hokusai/_version.py
--rw-r--r--   0        0        0      282 2023-03-06 17:27:08.102422 hokusai-1.0.5/hokusai/cli/__init__.py
--rw-r--r--   0        0        0     4692 2023-03-06 17:27:08.102422 hokusai-1.0.5/hokusai/cli/base.py
--rw-r--r--   0        0        0     3866 2023-03-06 17:27:08.102422 hokusai-1.0.5/hokusai/cli/dev.py
--rw-r--r--   0        0        0     2944 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/cli/pipeline.py
--rw-r--r--   0        0        0     8753 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/cli/production.py
--rw-r--r--   0        0        0     3430 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/cli/registry.py
--rw-r--r--   0        0        0     9575 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/cli/review_app.py
--rw-r--r--   0        0        0     8670 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/cli/staging.py
--rw-r--r--   0        0        0      175 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/command_line.py
--rw-r--r--   0        0        0     1086 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/__init__.py
--rw-r--r--   0        0        0      163 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/build.py
--rw-r--r--   0        0        0     3293 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/check.py
--rw-r--r--   0        0        0     1578 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/command_tree.py
--rw-r--r--   0        0        0     2011 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/configure.py
--rw-r--r--   0        0        0     1832 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/deployment.py
--rw-r--r--   0        0        0     3888 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/development.py
--rw-r--r--   0        0        0     1279 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/env.py
--rw-r--r--   0        0        0      768 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/gitcompare.py
--rw-r--r--   0        0        0      825 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/gitdiff.py
--rw-r--r--   0        0        0      848 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/gitlog.py
--rw-r--r--   0        0        0     1911 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/images.py
--rw-r--r--   0        0        0     5447 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/kubernetes.py
--rw-r--r--   0        0        0     1321 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/logs.py
--rw-r--r--   0        0        0     1531 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/namespace.py
--rw-r--r--   0        0        0      820 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/pull.py
--rw-r--r--   0        0        0     1727 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/push.py
--rw-r--r--   0        0        0      673 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/retag.py
--rw-r--r--   0        0        0      321 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/run.py
--rw-r--r--   0        0        0     3994 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/setup.py
--rw-r--r--   0        0        0     1894 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/test.py
--rw-r--r--   0        0        0      198 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/commands/version.py
--rw-r--r--   0        0        0        0 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/__init__.py
--rw-r--r--   0        0        0      447 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/branch_detection.py
--rw-r--r--   0        0        0     1404 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/command.py
--rw-r--r--   0        0        0     4193 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/common.py
--rw-r--r--   0        0        0     4840 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/config.py
--rw-r--r--   0        0        0     1322 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/config_loader.py
--rw-r--r--   0        0        0       22 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/constants.py
--rw-r--r--   0        0        0     1044 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/docker_compose_helpers.py
--rw-r--r--   0        0        0      532 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/environment.py
--rw-r--r--   0        0        0      182 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/exceptions.py
--rw-r--r--   0        0        0     1378 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/global_config.py
--rw-r--r--   0        0        0     1200 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/representers.py
--rw-r--r--   0        0        0      873 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/template_renderer.py
--rw-r--r--   0        0        0      660 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/lib/template_selector.py
--rw-r--r--   0        0        0        0 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/__init__.py
--rw-r--r--   0        0        0     2528 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/command_runner.py
--rw-r--r--   0        0        0     1861 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/configmap.py
--rw-r--r--   0        0        0    11054 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/deployment.py
--rw-r--r--   0        0        0      872 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/docker.py
--rw-r--r--   0        0        0     5075 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/ecr.py
--rw-r--r--   0        0        0     1001 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/kubectl.py
--rw-r--r--   0        0        0     1856 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/services/yaml_spec.py
--rw-r--r--   0        0        0      136 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/.dockerignore.j2
--rw-r--r--   0        0        0      313 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/Dockerfile.j2
--rw-r--r--   0        0        0       80 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/hokusai/build.yml.j2
--rw-r--r--   0        0        0      144 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/hokusai/development.yml.j2
--rw-r--r--   0        0        0     1193 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/hokusai/production.yml.j2
--rw-r--r--   0        0        0     1190 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/hokusai/staging.yml.j2
--rw-r--r--   0        0        0      152 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/templates/hokusai/test.yml.j2
--rw-r--r--   0        0        0     1275 2023-03-06 17:27:08.106422 hokusai-1.0.5/hokusai/version.py
--rw-r--r--   0        0        0     1148 2023-03-06 17:27:50.398690 hokusai-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    11547 1970-01-01 00:00:00.000000 hokusai-1.0.5/setup.py
--rw-r--r--   0        0        0    11223 1970-01-01 00:00:00.000000 hokusai-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-19 10:03:46.374651 hokusai-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0    10166 2023-04-19 10:03:46.374651 hokusai-1.1.0/README.md
+-rw-r--r--   0        0        0       96 2023-04-19 10:03:46.378651 hokusai-1.1.0/hokusai/__init__.py
+-rw-r--r--   0        0        0      214 2023-04-19 10:04:23.290901 hokusai-1.1.0/hokusai/_version.py
+-rw-r--r--   0        0        0      282 2023-04-19 10:03:46.378651 hokusai-1.1.0/hokusai/cli/__init__.py
+-rw-r--r--   0        0        0     4692 2023-04-19 10:03:46.378651 hokusai-1.1.0/hokusai/cli/base.py
+-rw-r--r--   0        0        0     3866 2023-04-19 10:03:46.378651 hokusai-1.1.0/hokusai/cli/dev.py
+-rw-r--r--   0        0        0     2944 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/cli/pipeline.py
+-rw-r--r--   0        0        0     8671 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/cli/production.py
+-rw-r--r--   0        0        0     3436 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/cli/registry.py
+-rw-r--r--   0        0        0     9575 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/cli/review_app.py
+-rw-r--r--   0        0        0     8588 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/cli/staging.py
+-rw-r--r--   0        0        0      175 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/command_line.py
+-rw-r--r--   0        0        0     1092 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/build.py
+-rw-r--r--   0        0        0     3293 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/check.py
+-rw-r--r--   0        0        0     1578 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/command_tree.py
+-rw-r--r--   0        0        0     2011 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/configure.py
+-rw-r--r--   0        0        0     1832 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/deployment.py
+-rw-r--r--   0        0        0     3888 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/development.py
+-rw-r--r--   0        0        0     1279 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/env.py
+-rw-r--r--   0        0        0      768 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/gitcompare.py
+-rw-r--r--   0        0        0      825 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/gitdiff.py
+-rw-r--r--   0        0        0      848 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/gitlog.py
+-rw-r--r--   0        0        0     1911 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/images.py
+-rw-r--r--   0        0        0     5445 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/kubernetes.py
+-rw-r--r--   0        0        0     1321 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/logs.py
+-rw-r--r--   0        0        0     1531 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/namespace.py
+-rw-r--r--   0        0        0      820 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/pull.py
+-rw-r--r--   0        0        0     2856 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/push.py
+-rw-r--r--   0        0        0      673 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/retag.py
+-rw-r--r--   0        0        0      321 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/run.py
+-rw-r--r--   0        0        0     3994 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/setup.py
+-rw-r--r--   0        0        0     1894 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/test.py
+-rw-r--r--   0        0        0      198 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/commands/version.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/__init__.py
+-rw-r--r--   0        0        0     1404 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/command.py
+-rw-r--r--   0        0        0     4193 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/common.py
+-rw-r--r--   0        0        0     4840 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/config.py
+-rw-r--r--   0        0        0     1322 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/config_loader.py
+-rw-r--r--   0        0        0       22 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/constants.py
+-rw-r--r--   0        0        0     1044 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/docker_compose_helpers.py
+-rw-r--r--   0        0        0      532 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/environment.py
+-rw-r--r--   0        0        0      182 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/exceptions.py
+-rw-r--r--   0        0        0     1378 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/global_config.py
+-rw-r--r--   0        0        0     1200 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/representers.py
+-rw-r--r--   0        0        0      873 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/template_renderer.py
+-rw-r--r--   0        0        0      660 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/lib/template_selector.py
+-rw-r--r--   0        0        0        0 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/__init__.py
+-rw-r--r--   0        0        0     2528 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/command_runner.py
+-rw-r--r--   0        0        0     1861 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/configmap.py
+-rw-r--r--   0        0        0    11054 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/deployment.py
+-rw-r--r--   0        0        0     1144 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/docker.py
+-rw-r--r--   0        0        0     5075 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/ecr.py
+-rw-r--r--   0        0        0     1001 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/kubectl.py
+-rw-r--r--   0        0        0     1856 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/services/yaml_spec.py
+-rw-r--r--   0        0        0      136 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/.dockerignore.j2
+-rw-r--r--   0        0        0      313 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/Dockerfile.j2
+-rw-r--r--   0        0        0       80 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/hokusai/build.yml.j2
+-rw-r--r--   0        0        0      144 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/hokusai/development.yml.j2
+-rw-r--r--   0        0        0     1193 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/hokusai/production.yml.j2
+-rw-r--r--   0        0        0     1190 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/hokusai/staging.yml.j2
+-rw-r--r--   0        0        0      152 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/templates/hokusai/test.yml.j2
+-rw-r--r--   0        0        0     1275 2023-04-19 10:03:46.382651 hokusai-1.1.0/hokusai/version.py
+-rw-r--r--   0        0        0     1148 2023-04-19 10:04:22.686897 hokusai-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11547 1970-01-01 00:00:00.000000 hokusai-1.1.0/setup.py
+-rw-r--r--   0        0        0    11223 1970-01-01 00:00:00.000000 hokusai-1.1.0/PKG-INFO
```

### Comparing `hokusai-1.0.5/LICENSE.txt` & `hokusai-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/README.md` & `hokusai-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/cli/base.py` & `hokusai-1.1.0/hokusai/cli/base.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/cli/dev.py` & `hokusai-1.1.0/hokusai/cli/dev.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/cli/pipeline.py` & `hokusai-1.1.0/hokusai/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/cli/production.py` & `hokusai-1.1.0/hokusai/cli/production.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import click
 
 import hokusai
 
 from hokusai.cli.base import base
 from hokusai.lib.common import set_verbosity, CONTEXT_SETTINGS
-from hokusai.lib.branch_detection import detect_branch
 
 KUBE_CONTEXT = 'production'
 
 @base.group()
 def production(context_settings=CONTEXT_SETTINGS):
   """Interact with the production Kubernetes environment
   defined by the `production` context in `~/.kube/config` and the 
@@ -32,15 +31,15 @@
   """Delete the Kubernetes resources defined in ./hokusai/production.yml"""
   set_verbosity(verbose)
   hokusai.k8s_delete(KUBE_CONTEXT, filename=filename)
 
 
 
 @production.command(context_settings=CONTEXT_SETTINGS)
-@click.option('--check-branch', type=click.STRING, default=detect_branch(), help='Check branch before updating (default: origin default or main)')
+@click.option('--check-branch', type=click.STRING, default="main", help='Check branch before updating (default: main)')
 @click.option('--check-remote', type=click.STRING, help='Check remotes before updating (otherwise check all remotes)')
 @click.option('--skip-checks', type=click.BOOL, is_flag=True, help='Skip all checks and update configuration recklessly')
 @click.option('-f', '--filename', type=click.STRING, help='Use the given Kubernetes Yaml file (default ./hokusai/production.yml)')
 @click.option('--dry-run', type=click.BOOL, is_flag=True, help='Perform a dry run of the configuration update')
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def update(check_branch, check_remote, skip_checks, filename, dry_run, verbose):
   """Update the Kubernetes resources defined in ./hokusai/production.yml"""
```

### Comparing `hokusai-1.0.5/hokusai/cli/registry.py` & `hokusai-1.1.0/hokusai/cli/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @click.option('--force', type=click.BOOL, is_flag=True, help='Push even if working directory is not clean')
 @click.option('--overwrite', type=click.BOOL, is_flag=True, help='Push even if the tag already exists')
 @click.option('--skip-latest', type=click.BOOL, is_flag=True, help="Don't update the 'latest' tag" )
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def push(tag, local_tag, build, filename, force, overwrite, skip_latest, verbose):
   """Build and push an image to the project's registry tagged as the git SHA1 of HEAD"""
   set_verbosity(verbose)
-  hokusai.push(tag, local_tag, build, filename, force, overwrite, skip_latest)
+  hokusai.push_image(tag, local_tag, build, filename, force, overwrite, skip_latest)
 
 
 @registry.command(context_settings=CONTEXT_SETTINGS)
 @click.option('--tag', type=click.STRING, default='latest', help='The remote tag to pull  (default: latest)')
 @click.option('--local-tag', type=click.STRING, default='latest', help='The local tag to pull to (default: latest)')
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def pull(tag, local_tag, verbose):
```

### Comparing `hokusai-1.0.5/hokusai/cli/review_app.py` & `hokusai-1.1.0/hokusai/cli/review_app.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/cli/staging.py` & `hokusai-1.1.0/hokusai/cli/staging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import click
 
 import hokusai
 
 from hokusai.cli.base import base
 from hokusai.lib.common import set_verbosity, CONTEXT_SETTINGS
-from hokusai.lib.branch_detection import detect_branch
 
 KUBE_CONTEXT = 'staging'
 
 @base.group()
 def staging(context_settings=CONTEXT_SETTINGS):
   """Interact with the staging Kubernetes environment
   defined by the `staging` context in `~/.kube/config` and the 
@@ -31,15 +30,15 @@
 def delete(filename, verbose):
   """Delete the Kubernetes resources defined in ./hokusai/staging.yml"""
   set_verbosity(verbose)
   hokusai.k8s_delete(KUBE_CONTEXT, filename=filename)
 
 
 @staging.command(context_settings=CONTEXT_SETTINGS)
-@click.option('--check-branch', type=click.STRING, default=detect_branch(), help='Check branch before updating (default: origin default or main)')
+@click.option('--check-branch', type=click.STRING, default="main", help='Check branch before updating (default: main)')
 @click.option('--check-remote', type=click.STRING, help='Check remotes before updating (otherwise check all remotes)')
 @click.option('--skip-checks', type=click.BOOL, is_flag=True, help='Skip all checks and update configuration recklessly')
 @click.option('-f', '--filename', type=click.STRING, help='Use the given Kubernetes Yaml file (default ./hokusai/staging.yml)')
 @click.option('--dry-run', type=click.BOOL, is_flag=True, help='Perform a dry run of the configuration update')
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def update(check_branch, check_remote, skip_checks, filename, dry_run, verbose):
   """Update the Kubernetes resources defined in ./hokusai/staging.yml"""
```

### Comparing `hokusai-1.0.5/hokusai/commands/__init__.py` & `hokusai-1.1.0/hokusai/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from hokusai.commands.development import dev_start, dev_stop, dev_status, dev_logs, dev_run, dev_clean
 from hokusai.commands.gitdiff import gitdiff
 from hokusai.commands.gitlog import gitlog
 from hokusai.commands.gitcompare import gitcompare
 from hokusai.commands.env import get_env, set_env, unset_env
 from hokusai.commands.images import images
 from hokusai.commands.logs import logs
-from hokusai.commands.push import push
+from hokusai.commands.push import push_image
 from hokusai.commands.pull import pull
 from hokusai.commands.run import run
 from hokusai.commands.setup import setup
 from hokusai.commands.kubernetes import k8s_create, k8s_update, k8s_delete, k8s_status, k8s_copy_config
 from hokusai.commands.namespace import create_new_app_yaml
 from hokusai.commands.retag import retag
 from hokusai.commands.test import test
```

### Comparing `hokusai-1.0.5/hokusai/commands/check.py` & `hokusai-1.1.0/hokusai/commands/check.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/command_tree.py` & `hokusai-1.1.0/hokusai/commands/command_tree.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/configure.py` & `hokusai-1.1.0/hokusai/commands/configure.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/deployment.py` & `hokusai-1.1.0/hokusai/commands/deployment.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/development.py` & `hokusai-1.1.0/hokusai/commands/development.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/env.py` & `hokusai-1.1.0/hokusai/commands/env.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/gitcompare.py` & `hokusai-1.1.0/hokusai/commands/gitcompare.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/gitdiff.py` & `hokusai-1.1.0/hokusai/commands/gitdiff.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/gitlog.py` & `hokusai-1.1.0/hokusai/commands/gitlog.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/images.py` & `hokusai-1.1.0/hokusai/commands/images.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/kubernetes.py` & `hokusai-1.1.0/hokusai/commands/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   yaml_spec = YamlSpec(yaml_template).to_file()
 
   shout(kctl.command("create --save-config -f %s" % yaml_spec), print_output=True)
   print_green("Created Kubernetes environment %s" % yaml_template)
 
 
 @command()
-def k8s_update(context, namespace=None, filename=None, check_branch="master",
+def k8s_update(context, namespace=None, filename=None, check_branch="main",
                 check_remote=None, skip_checks=False, dry_run=False):
   if filename is None:
     yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, context))
   else:
     yaml_template = TemplateSelector().get(filename)
 
   if not skip_checks:
```

### Comparing `hokusai-1.0.5/hokusai/commands/logs.py` & `hokusai-1.1.0/hokusai/commands/logs.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/namespace.py` & `hokusai-1.1.0/hokusai/commands/namespace.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/pull.py` & `hokusai-1.1.0/hokusai/commands/pull.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/retag.py` & `hokusai-1.1.0/hokusai/commands/retag.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/setup.py` & `hokusai-1.1.0/hokusai/commands/setup.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/commands/test.py` & `hokusai-1.1.0/hokusai/commands/test.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/command.py` & `hokusai-1.1.0/hokusai/lib/command.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/common.py` & `hokusai-1.1.0/hokusai/lib/common.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/config.py` & `hokusai-1.1.0/hokusai/lib/config.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/config_loader.py` & `hokusai-1.1.0/hokusai/lib/config_loader.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/docker_compose_helpers.py` & `hokusai-1.1.0/hokusai/lib/docker_compose_helpers.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/environment.py` & `hokusai-1.1.0/hokusai/lib/environment.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/global_config.py` & `hokusai-1.1.0/hokusai/lib/global_config.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/representers.py` & `hokusai-1.1.0/hokusai/lib/representers.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/template_renderer.py` & `hokusai-1.1.0/hokusai/lib/template_renderer.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/lib/template_selector.py` & `hokusai-1.1.0/hokusai/lib/template_selector.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/services/command_runner.py` & `hokusai-1.1.0/hokusai/services/command_runner.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/services/configmap.py` & `hokusai-1.1.0/hokusai/services/configmap.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/services/deployment.py` & `hokusai-1.1.0/hokusai/services/deployment.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/services/docker.py` & `hokusai-1.1.0/hokusai/services/docker.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,18 @@
   def build(self, filename=None):
     if filename is None:
       yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, BUILD_YAML_FILE))
     else:
       yaml_template = TemplateSelector().get(filename)
 
     docker_compose_yml = YamlSpec(yaml_template).to_file()
-    build_command = "docker-compose -f %s -p hokusai build" % docker_compose_yml
+
+    # docker-compose v2 switched to using '-' as separator in image name, resulting in 'hokusai-<project>'
+    # COMPOSE_COMPATIBILITY=true forces v2 to use '_', resulting in 'hokusai_<project>', matching v1
+    build_command = "DOCKER_DEFAULT_PLATFORM=linux/amd64 COMPOSE_COMPATIBILITY=true docker-compose -f %s -p hokusai build" % docker_compose_yml
 
     if config.pre_build:
       build_command = "%s && %s" % (config.pre_build, build_command)
 
     if config.post_build:
       build_command = "%s && %s" % (build_command, config.post_build)
```

### Comparing `hokusai-1.0.5/hokusai/services/ecr.py` & `hokusai-1.1.0/hokusai/services/ecr.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/services/kubectl.py` & `hokusai-1.1.0/hokusai/services/kubectl.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/services/yaml_spec.py` & `hokusai-1.1.0/hokusai/services/yaml_spec.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/templates/hokusai/production.yml.j2` & `hokusai-1.1.0/hokusai/templates/hokusai/production.yml.j2`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/templates/hokusai/staging.yml.j2` & `hokusai-1.1.0/hokusai/templates/hokusai/staging.yml.j2`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/hokusai/version.py` & `hokusai-1.1.0/hokusai/version.py`

 * *Files identical despite different names*

### Comparing `hokusai-1.0.5/pyproject.toml` & `hokusai-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "hokusai"
-version = "1.0.5"
+version = "1.1.0"
 description = "Artsy Docker development toolkit"
 authors = ["Isac Petruzzi <isac@artsymail.com>"]
 maintainers = ["Jian-Feng Xu <jian-feng@artsymail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/artsy/hokusai"
 include = ["hokusai/_version.py"]
```

### Comparing `hokusai-1.0.5/setup.py` & `hokusai-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'termcolor==1.1.0']
 
 entry_points = \
 {'console_scripts': ['hokusai = hokusai.command_line:main']}
 
 setup_kwargs = {
     'name': 'hokusai',
-    'version': '1.0.5',
+    'version': '1.1.0',
     'description': 'Artsy Docker development toolkit',
     'long_description': '## HOKUSAI [![CircleCI](https://circleci.com/gh/artsy/hokusai/tree/main.svg?style=svg)](https://circleci.com/gh/artsy/hokusai/tree/main)\n\n<a href="https://en.wikipedia.org/wiki/Hokusai"><img height="300" src="hokusai.jpg"></a>\n\nHokusai is a Docker + Kubernetes CLI for application developers.\n\nHokusai "dockerizes" applications and manages their lifecycle throughout development, testing, and release cycles.\n\nHokusai wraps calls to [Kubectl](https://kubernetes.io/), [Docker](https://www.docker.com/), [Docker-Compose](https://docs.docker.com/compose/) and [Git](https://git-scm.com/) with a CLI, and defines a CI workflow.\n\nHokusai currently only supports Kubernetes deployments on AWS, configured to pull from ECS container repositories (ECR), although other providers may be added in the future.\n\n### Why Hokusai?\n\nAt [Artsy](http://www.artsy.net), as we began working with Kubernetes, while impressed with its design, capabilities, and flexibility, we were in need of tooling we could deliver to agile development teams that addressed the day-to-day tasks of application development, delivery, introspection and maintenance, while providing a clean and uncomplicated interface.\n\nTransitioning teams to the Docker / Kubernetes ecosystem can be intimidating, and comes with a steep learning curve. We set out to create a Heroku-like CLI that would shepherd the application developer into the ecosystems of Docker and Kubernetes, and while introducing new tooling and concepts, outlining a clear practice for dependency management, local development, testing and CI, image repository structure, deployment and orchestration.\n\n## Installation\n\n### MacOS\n\nWe recommend installing via Homebrew:\n\n```\n$ brew update\n$ brew tap artsy/formulas\n$ brew install hokusai\n```\n\nIf you previously installed Hokusai via an alternate installation method, you may need to force the `link` step.\n\n```\n$ brew link --overwrite hokusai\n```\n\nIf you previously installed Hokusai via Pip, you may want to first uninstall it:\n\n```\n$ pip uninstall hokusai\n```\n\n### Linux\n\n```\ncurl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash\n```\n\nNote: This method installs Hokusai to `/usr/local/bin/hokusai`.\n\n### Pip\n\nHokusai can be installed via Pip, on MacOS or Linux. If you do so, please first go through [Pyenv](#Pyenv), [Python](#Python), and [Virtualenv](#Virtualenv) steps.\n\nPython 3.7+ is required.\n\n```\npip install hokusai\n```\n\nNote: If Pip fails at upgrading your system Python packages, try:\n\n```\npip install hokusai --ignore-installed\n```\n\n### Docker\n\nWe also maintain [Hokusai Docker images](https://hub.docker.com/r/artsy/hokusai) for running Hokusai in Docker.\n\n### Github\n\nRelease artifacts are available on [Github](https://github.com/artsy/hokusai/releases).\n\n### AWS S3\n\nRelease artifacts are also available in AWS S3. You can use this [convenience script](get-hokusai.sh) or Curl to fetch them.\n\n### A note on Python 2.x\n\nHokusai currently supports Python 3.7+ only. The last version that supported Python 2.x was [v0.5.18](https://github.com/artsy/hokusai/tree/v0.5.18).\n\n## Setup\n\nWe assume that you already have Kubernetes cluster, Git, Docker, and Docker-Compose set up, and that you have an AWS account. Perform the following steps to setup Hokusai:\n\n1. [Configure AWS credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#configuring-credentials).\n\n2. Configure Hokusai\n\n    ```\n    hokusai configure --kubectl-version <kubectl version> --s3-bucket <bucket name> --s3-key <file key>\n    ```\n\n    Provide the Kubectl version matching that of your Kubernetes clusters, as well as the S3 bucket name/key where your org\'s Kubectl config file is stored.\n\n    For system administrators: see [Administering Hokusai](./docs/Administering_Hokusai.md) for instructions on preparing AWS and Kubernetes, and on publishing a Kubectl config file.\n\n    For Artsy developers: see [artsy/README](https://github.com/artsy/README/blob/main/playbooks/hokusai.md) for the current way of installing and configuring hokusai.\n\n3. Enable Bash autocompletion:\n\n    ```\n    eval "$(_HOKUSAI_COMPLETE=source hokusai)"\n    ```\n\n## Getting Started\n\nSee [Getting Started](./docs/Getting_Started.md) to start using Hokusai for your project.\n\n## Command Reference\n\nA full command reference can be found in [Command Reference](./docs/Command_Reference.md).\n\n## Review Apps\n\nHokusai can be used to simplify the process of spinning up a "review app" instance of your project, based on a feature branch or pull request.\n\nFull details are in the [Review App reference](./docs/Review_Apps.md).\n\n## Developing Hokusai\n\nTo work on Hokusai itself, please set up:\n\n### Pyenv\n\nWe recommend using [Pyenv](https://github.com/pyenv/pyenv) to install the correct version of Python. For a tutorial of Pyenv, see [this guide](https://realpython.com/intro-to-pyenv/).\n\nWhen installing on MacOS, please make sure to use brew-installed `openssl` and `readline` libraries, and xcode-installed `zlib` library. And make sure these libraries are correctly linked. Like so:\n\n```\nbrew install openssl readline zlib\n\necho \'export PATH="/usr/local/opt/openssl@1.1/bin:$PATH"\' >> ~/.bash_profile\necho \'export LDFLAGS="-L/usr/local/opt/openssl@1.1/lib"\' >> ~/.bash_profile\necho \'export CPPFLAGS="-I/usr/local/opt/openssl@1.1/include"\' >> ~/.bash_profile\necho \'export PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig"\' >> ~/.bash_profile\n```\n\n### Python\n\nHokusai is currently tested on Python 3.9.10 so we recommend using that Python version.\n\nIf you use Pyenv to install Python, you should see an output similar to this:\n\n```\npyenv install 3.9.10\n\n    python-build: use openssl from homebrew\n    python-build: use readline from homebrew\n\n    Downloading Python-3.9.10.tar.xz...\n    -> https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz\n    Installing Python-3.9.10...\n    python-build: use tcl-tk from homebrew\n    python-build: use readline from homebrew\n    python-build: use zlib from xcode sdk\n\n    Installed Python-3.9.10 to $HOME/.pyenv/versions/3.9.10\n```\n\nWith the desired Python version installed, activate it globally:\n\n```\npyenv global 3.9.10\n```\n\nNote: If you want to create a PyInstaller distribution, Python must be installed with development libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv install`.\n\n### Virtualenv\n\nWe recommend using a virtual environment to isolate Hokusai\'s dependencies from that of other projects on your local environment.\n\nThe Pyenv install comes with [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) which can be used to create virtual environments.\n\n### Poetry\n\nUse [Poetry](https://python-poetry.org/) to install Hokusai\'s dependencies as well as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-installs). See [this guide](https://python-poetry.org/docs/basic-usage/) for working with Poetry.\n\nInstall Poetry:\n\n```\npip install poetry\n```\n\nInstall dependencies and Hokusai in editable mode:\n\n```\npoetry install\n```\n\nTo update dependencies:\n\n```\npoetry lock\n```\n\n## Testing\n\n### Install Minikube\n\n[Minikube](https://minikube.sigs.k8s.io/docs/start/) is used for integration tests.\n\n```\nbrew install minikube\nminikube start --kubernetes-version=<version of your Kubernetes clusters, example: v1.2.3>\n```\n\n### Run tests\n\nTo run all tests:\n\n```\nmake tests\n```\n\nTo run only unit tests:\n\n```\nmake test\n```\n\nOnly integration tests:\n\n```\nmake integration\n```\n\nOnly specific modules, TestClasses, or even methods:\n\n```\npython -m unittest test.unit.test_module.TestClass.test_method\n```\n\nTip: Set `DEBUG=1` environment variable to print boto logging\n\n\n## Distributing Hokusai\n\n### Beta Release\n\nMerging a branch into `main` automatically creates a beta version useful for testing.\n\nTo install the beta:\n\n#### MacOS\n\n```\n$ brew uninstall hokusai\n$ brew uninstall hokusai-beta\n$ brew update\n$ brew tap artsy/formulas\n$ brew install hokusai-beta\n```\n\n#### Linux\n\n```\ncurl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash -s beta\n```\n\n### Official Release\n\nTo create an official release, such as `v1.2.3`, perform the following:\n\n- Create a branch named `prepare-v1.2.3` and make the following changes:\n  - Bump version in [RELEASE_VERSION](./RELEASE_VERSION) file.\n  - Upate [CHANGELOG](./CHANGELOG.md).\n  - Open a PR to merge into `main`. Please see [past PRs](https://github.com/artsy/hokusai/pulls?q=is%3Apr+Release+is%3Aclosed+%22prepare+version%22) for example.\n\n- Open a PR to merge `main` into `release`. Please see [past PRs](https://github.com/artsy/hokusai/pulls?q=is%3Apr+is%3Aclosed+%22release+version%22) for example.\n\n## The Name\n\nThe project is named for the great Japanese artist [Katsushika Hokusai](https://www.artsy.net/article/artsy-editorial-7-things-hokusai-creator-great-wave) (1760-1849).\n\n## About Artsy\n\n<a href="https://www.artsy.net/">\n  <img align="left" src="https://avatars2.githubusercontent.com/u/546231?s=200&v=4"/>\n</a>\n\nThis project is the work of engineers at [Artsy][footer_website], the world\'s\nleading and largest online art marketplace and platform for discovering art.\nOne of our core [Engineering Principles][footer_principles] is being [Open\nSource by Default][footer_open] which means we strive to share as many details\nof our work as possible.\n\nYou can learn more about this work from [our blog][footer_blog] and by following\n[@ArtsyOpenSource][footer_twitter] or explore our public data by checking out\n[our API][footer_api]. If you\'re interested in a career at Artsy, read through\nour [job postings][footer_jobs]!\n\n[footer_website]: https://www.artsy.net/\n[footer_principles]: https://github.com/artsy/README/blob/main/culture/engineering-principles.md\n[footer_open]: https://github.com/artsy/README/blob/main/culture/engineering-principles.md\n[footer_blog]: https://artsy.github.io/\n[footer_twitter]: https://twitter.com/ArtsyOpenSource\n[footer_api]: https://developers.artsy.net/\n[footer_jobs]: https://www.artsy.net/jobs\n',
     'author': 'Isac Petruzzi',
     'author_email': 'isac@artsymail.com',
     'maintainer': 'Jian-Feng Xu',
     'maintainer_email': 'jian-feng@artsymail.com',
     'url': 'http://github.com/artsy/hokusai',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['hokusai',
 'hokusai.cli', 'hokusai.commands', 'hokusai.lib', 'hokusai.services']
 package_data = \ {'': ['*'], 'hokusai': ['templates/*', 'templates/hokusai/*']}
 install_requires = \ ['Jinja2==3.1.1', 'MarkupSafe==2.1.1', 'PyYAML==6.0',
 'boto3==1.21.28', 'click-repl==0.2.0', 'click==8.1.0', 'packaging==21.3',
 'prompt-toolkit==3.0.28', 'termcolor==1.1.0'] entry_points = \
 {'console_scripts': ['hokusai = hokusai.command_line:main']} setup_kwargs =
-{ 'name': 'hokusai', 'version': '1.0.5', 'description': 'Artsy Docker
+{ 'name': 'hokusai', 'version': '1.1.0', 'description': 'Artsy Docker
 development toolkit', 'long_description': '## HOKUSAI [![CircleCI](https://
 circleci.com/gh/artsy/hokusai/tree/main.svg?style=svg)](https://circleci.com/
 gh/artsy/hokusai/tree/main)\n\n[hokusai.jpg]\n\nHokusai is a Docker +
 Kubernetes CLI for application developers.\n\nHokusai "dockerizes" applications
 and manages their lifecycle throughout development, testing, and release
 cycles.\n\nHokusai wraps calls to [Kubectl](https://kubernetes.io/), [Docker]
 (https://www.docker.com/), [Docker-Compose](https://docs.docker.com/compose/
```

### Comparing `hokusai-1.0.5/PKG-INFO` & `hokusai-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hokusai
-Version: 1.0.5
+Version: 1.1.0
 Summary: Artsy Docker development toolkit
 Home-page: http://github.com/artsy/hokusai
 License: MIT
 Author: Isac Petruzzi
 Author-email: isac@artsymail.com
 Maintainer: Jian-Feng Xu
 Maintainer-email: jian-feng@artsymail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hokusai Version: 1.0.5 Summary: Artsy Docker
+Metadata-Version: 2.1 Name: hokusai Version: 1.1.0 Summary: Artsy Docker
 development toolkit Home-page: http://github.com/artsy/hokusai License: MIT
 Author: Isac Petruzzi Author-email: isac@artsymail.com Maintainer: Jian-Feng Xu
 Maintainer-email: jian-feng@artsymail.com Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

