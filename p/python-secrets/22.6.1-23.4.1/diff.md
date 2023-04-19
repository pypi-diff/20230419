# Comparing `tmp/python_secrets-22.6.1.tar.gz` & `tmp/python_secrets-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_secrets-22.6.1.tar", last modified: Wed Jun 22 06:34:43 2022, max compression
+gzip compressed data, was "python_secrets-23.4.1.tar", last modified: Wed Apr 19 21:52:37 2023, max compression
```

## Comparing `python_secrets-22.6.1.tar` & `python_secrets-23.4.1.tar`

### file list

```diff
@@ -1,152 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.905385 python_secrets-22.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.889385 python_secrets-22.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.893385 python_secrets-22.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     4494 2022-06-22 06:25:28.000000 python_secrets-22.6.1/.github/workflows/test-build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)      893 2022-06-22 06:25:28.000000 python_secrets-22.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      404 2022-06-22 06:25:28.000000 python_secrets-22.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1262 2022-06-22 06:25:28.000000 python_secrets-22.6.1/.travis.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.893385 python_secrets-22.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (116)    31531 2022-06-22 06:25:28.000000 python_secrets-22.6.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (116)      528 2022-06-22 06:25:28.000000 python_secrets-22.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4108 2022-06-22 06:25:28.000000 python_secrets-22.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)    12679 2022-06-22 06:25:28.000000 python_secrets-22.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (116)      611 2022-06-22 06:25:28.000000 python_secrets-22.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)      265 2022-06-22 06:25:28.000000 python_secrets-22.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     6723 2022-06-22 06:25:28.000000 python_secrets-22.6.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)    78571 2022-06-22 06:34:43.905385 python_secrets-22.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    65524 2022-06-22 06:25:28.000000 python_secrets-22.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-06-22 06:25:28.000000 python_secrets-22.6.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (116)       25 2022-06-22 06:25:28.000000 python_secrets-22.6.1/bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.893385 python_secrets-22.6.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (116)      502 2022-06-22 06:25:28.000000 python_secrets-22.6.1/bin/psec
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.893385 python_secrets-22.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)       14 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     6794 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.893385 python_secrets-22.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1997 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/advanced.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (116)     8728 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       33 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      647 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1212 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)       52 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6475 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (116)      560 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     9602 2022-06-22 06:25:28.000000 python_secrets-22.6.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.897385 python_secrets-22.6.1/psec/
--rwxr-xr-x   0 runner    (1001) docker     (116)      718 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12422 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3879 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/about.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.897385 python_secrets-22.6.1/psec/cli/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.897385 python_secrets-22.6.1/psec/cli/environments/
--rw-r--r--   0 runner    (1001) docker     (116)       76 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5301 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (116)     5363 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/default.py
--rw-r--r--   0 runner    (1001) docker     (116)     5112 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     3760 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/list.py
--rw-r--r--   0 runner    (1001) docker     (116)     4533 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     2467 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/rename.py
--rw-r--r--   0 runner    (1001) docker     (116)     3412 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/environments/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.897385 python_secrets-22.6.1/psec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (116)       75 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4234 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/groups/create.py
--rw-r--r--   0 runner    (1001) docker     (116)     3518 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/groups/delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     1101 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/groups/list.py
--rw-r--r--   0 runner    (1001) docker     (116)      904 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/groups/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     1466 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/groups/show.py
--rw-r--r--   0 runner    (1001) docker     (116)     2579 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (116)     4287 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/run.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/psec/cli/secrets/
--rw-r--r--   0 runner    (1001) docker     (116)      196 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2075 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/backup.py
--rw-r--r--   0 runner    (1001) docker     (116)    10647 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/create.py
--rw-r--r--   0 runner    (1001) docker     (116)     5067 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/delete.py
--rw-r--r--   0 runner    (1001) docker     (116)     4081 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/describe.py
--rw-r--r--   0 runner    (1001) docker     (116)     3889 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/generate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1756 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/get.py
--rw-r--r--   0 runner    (1001) docker     (116)     1050 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/path.py
--rw-r--r--   0 runner    (1001) docker     (116)     2816 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/restore.py
--rw-r--r--   0 runner    (1001) docker     (116)     5292 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/send.py
--rw-r--r--   0 runner    (1001) docker     (116)     9947 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/set.py
--rw-r--r--   0 runner    (1001) docker     (116)     5473 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/show.py
--rw-r--r--   0 runner    (1001) docker     (116)     1715 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/secrets/tree.py
--rw-r--r--   0 runner    (1001) docker     (116)    48131 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/ssh.py
--rw-r--r--   0 runner    (1001) docker     (116)     2635 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/template.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/psec/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (116)      224 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6301 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/myip.py
--rw-r--r--   0 runner    (1001) docker     (116)     1311 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/netblock.py
--rw-r--r--   0 runner    (1001) docker     (116)     2099 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/set_aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (116)     2172 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/tfbackend.py
--rw-r--r--   0 runner    (1001) docker     (116)     4391 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/tfoutput.py
--rw-r--r--   0 runner    (1001) docker     (116)     7459 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/cli/utils/yaml_to_json.py
--rw-r--r--   0 runner    (1001) docker     (116)     3003 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    17834 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/google_oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/psec/secrets_environment/
--rw-r--r--   0 runner    (1001) docker     (116)    30549 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/psec/secrets_environment/factory/
--rw-r--r--   0 runner    (1001) docker     (116)     2401 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/factory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/psec/secrets_environment/handlers/
--rw-r--r--   0 runner    (1001) docker     (116)      392 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      461 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/boolean.py
--rw-r--r--   0 runner    (1001) docker     (116)      759 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/crypt_6.py
--rw-r--r--   0 runner    (1001) docker     (116)     4945 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/password.py
--rw-r--r--   0 runner    (1001) docker     (116)      846 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/sha256_digest.py
--rw-r--r--   0 runner    (1001) docker     (116)      393 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/string.py
--rw-r--r--   0 runner    (1001) docker     (116)      730 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/token_base64.py
--rw-r--r--   0 runner    (1001) docker     (116)      522 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/token_hex.py
--rw-r--r--   0 runner    (1001) docker     (116)      522 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/token_urlsafe.py
--rw-r--r--   0 runner    (1001) docker     (116)      458 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/secrets_environment/handlers/uuid4.py
--rw-r--r--   0 runner    (1001) docker     (116)    32031 2022-06-22 06:25:28.000000 python_secrets-22.6.1/psec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/python_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    78571 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3325 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2117 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-06-22 06:29:04.000000 python_secrets-22.6.1/python_secrets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      219 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)      176 2022-06-22 06:34:43.000000 python_secrets-22.6.1/python_secrets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       55 2022-06-22 06:25:28.000000 python_secrets-22.6.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      105 2022-06-22 06:25:28.000000 python_secrets-22.6.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      219 2022-06-22 06:25:28.000000 python_secrets-22.6.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.901385 python_secrets-22.6.1/secrets.d/
--rw-r--r--   0 runner    (1001) docker     (116)     1845 2022-06-22 06:25:28.000000 python_secrets-22.6.1/secrets.d/hypriot.json
--rw-r--r--   0 runner    (1001) docker     (116)     3630 2022-06-22 06:34:43.905385 python_secrets-22.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     2148 2022-06-22 06:25:28.000000 python_secrets-22.6.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      375 2022-06-22 06:25:28.000000 python_secrets-22.6.1/test-environment.bash
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.905385 python_secrets-22.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      600 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/00_usage.bats
--rwxr-xr-x   0 runner    (1001) docker     (116)       24 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1530 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/gosecure.json
--rw-r--r--   0 runner    (1001) docker     (116)     1047 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/runtime_00_initialization.bats
--rw-r--r--   0 runner    (1001) docker     (116)     9024 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/runtime_05_environments.bats
--rw-r--r--   0 runner    (1001) docker     (116)     3371 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/runtime_10_groups.bats
--rw-r--r--   0 runner    (1001) docker     (116)     6909 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/runtime_20_secrets.bats
--rw-r--r--   0 runner    (1001) docker     (116)     3145 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/runtime_30_utils.bats
--rw-r--r--   0 runner    (1001) docker     (116)     1713 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/runtime_40_run.bats
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.905385 python_secrets-22.6.1/tests/secrets.d/
--rw-r--r--   0 runner    (1001) docker     (116)      109 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/secrets.d/consul.json
--rw-r--r--   0 runner    (1001) docker     (116)     1845 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/secrets.d/hypriot.json
--rw-r--r--   0 runner    (1001) docker     (116)      131 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/secrets.d/jenkins.json
--rw-r--r--   0 runner    (1001) docker     (116)     1040 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/secrets.d/myapp.json
--rw-r--r--   0 runner    (1001) docker     (116)      469 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/secrets.d/oauth.json
--rw-r--r--   0 runner    (1001) docker     (116)      254 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/secrets.d/trident.json
--rw-r--r--   0 runner    (1001) docker     (116)     2132 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1285 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (116)     1167 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/test_helper.bash
--rw-r--r--   0 runner    (1001) docker     (116)     9069 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/test_secrets.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1076 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.889385 python_secrets-22.6.1/tests/yamlsecrets/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-06-22 06:34:43.905385 python_secrets-22.6.1/tests/yamlsecrets/secrets.d/
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/yamlsecrets/secrets.d/jenkins.yml
--rw-r--r--   0 runner    (1001) docker     (116)      637 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/yamlsecrets/secrets.d/myapp.yml
--rw-r--r--   0 runner    (1001) docker     (116)      384 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/yamlsecrets/secrets.d/oauth.yml
--rw-r--r--   0 runner    (1001) docker     (116)      224 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tests/yamlsecrets/secrets.d/trident.yml
--rw-r--r--   0 runner    (1001) docker     (116)     3176 2022-06-22 06:25:28.000000 python_secrets-22.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.360944 python_secrets-23.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.364944 python_secrets-23.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     4224 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.github/workflows/test-build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.travis.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.364944 python_secrets-23.4.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)    31952 2023-04-19 21:46:29.000000 python_secrets-23.4.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-19 21:46:29.000000 python_secrets-23.4.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4108 2023-04-19 21:46:29.000000 python_secrets-23.4.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    13073 2023-04-19 21:46:29.000000 python_secrets-23.4.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-04-19 21:46:29.000000 python_secrets-23.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-19 21:46:29.000000 python_secrets-23.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7052 2023-04-19 21:46:29.000000 python_secrets-23.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    78965 2023-04-19 21:52:37.380944 python_secrets-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    65524 2023-04-19 21:46:29.000000 python_secrets-23.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-19 21:46:29.000000 python_secrets-23.4.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-19 21:46:29.000000 python_secrets-23.4.1/bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      502 2023-04-19 21:46:29.000000 python_secrets-23.4.1/bin/psec
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     6794 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1997 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8728 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      647 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1212 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6475 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-04-19 21:46:29.000000 python_secrets-23.4.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/psec/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      718 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12422 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/about.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.368944 python_secrets-23.4.1/psec/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/environments/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5301 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5363 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/default.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5112 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3760 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4533 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/rename.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3412 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/environments/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3518 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/list.py
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/groups/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/secrets/
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/backup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11324 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5067 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/delete.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4081 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/describe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/find.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3889 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1756 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1050 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/restore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5292 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/send.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/set.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5473 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/secrets/tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48131 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2635 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.372944 python_secrets-23.4.1/psec/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6301 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/myip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/netblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2099 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/set_aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2172 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/tfbackend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/tfoutput.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7459 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/cli/utils/yaml_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17834 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/google_oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/psec/secrets_environment/
+-rw-r--r--   0 runner    (1001) docker     (122)    30739 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/psec/secrets_environment/factory/
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/factory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/psec/secrets_environment/handlers/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/crypt_6.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4945 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/password.py
+-rw-r--r--   0 runner    (1001) docker     (122)      846 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/sha256_digest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/string.py
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/token_base64.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/token_hex.py
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/token_urlsafe.py
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/secrets_environment/handlers/uuid4.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32045 2023-04-19 21:46:29.000000 python_secrets-23.4.1/psec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/python_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    78965 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2166 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 21:48:55.000000 python_secrets-23.4.1/python_secrets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-19 21:52:37.000000 python_secrets-23.4.1/python_secrets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-19 21:46:29.000000 python_secrets-23.4.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-19 21:46:29.000000 python_secrets-23.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-19 21:46:29.000000 python_secrets-23.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.376944 python_secrets-23.4.1/secrets.d/
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-04-19 21:46:29.000000 python_secrets-23.4.1/secrets.d/hypriot.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-19 21:52:37.380944 python_secrets-23.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2148 2023-04-19 21:46:29.000000 python_secrets-23.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-19 21:46:29.000000 python_secrets-23.4.1/test-environment.bash
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/00_usage.bats
+-rwxr-xr-x   0 runner    (1001) docker     (122)       24 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/gosecure.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1047 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_00_initialization.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     9024 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_05_environments.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_10_groups.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     6909 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_20_secrets.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     3145 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_30_utils.bats
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/runtime_40_run.bats
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/tests/secrets.d/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/consul.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1845 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/hypriot.json
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/jenkins.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/myapp.json
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/oauth.json
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/secrets.d/trident.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1285 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1167 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_helper.bash
+-rw-r--r--   0 runner    (1001) docker     (122)     9069 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_secrets.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1076 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.364944 python_secrets-23.4.1/tests/yamlsecrets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 21:52:37.380944 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/jenkins.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/myapp.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/oauth.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tests/yamlsecrets/secrets.d/trident.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3160 2023-04-19 21:46:29.000000 python_secrets-23.4.1/tox.ini
```

### Comparing `python_secrets-22.6.1/.github/workflows/test-build-publish.yml` & `python_secrets-23.4.1/.github/workflows/test-build-publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 name: Test Build and Publish
 on: [ push, pull_request ]
 
 jobs:
   build-test:
     name: Test and Build
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     env:
       PY_COLORS: 1
       TOX_PARALLEL_NO_SPINNER: 1
     steps:
     - name: Dump select GitHub event context
       run: |
         echo "github.ref=${{ github.ref }}"
         echo "github.event.head_commit=$HEAD_COMMIT"
       env:
         HEAD_COMMIT: ${{ toJson(github.event.head_commit) }}
     - name: Check out src from GitHub
       uses: actions/checkout@v2
       with:
         fetch-depth: 0
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+    - name: Set up Python
+      uses: actions/setup-python@v3
       with:
-        python-version: 3.8
+        python-version: 3.9.16
     - uses: conda-incubator/setup-miniconda@v2
       with:
         auto-activate-base: true
-        python-version: 3.8
+        python-version: 3.9.16
         auto-update-conda: true
     - name: Install dependencies
       run: |
         conda config --set always_yes yes --set changeps1 no
         python3 -m pip install tox setuptools>=42 setuptools_scm wheel twine
         [ -f requirements.txt ] && python3 -m pip install -Ur requirements.txt
         [ -f test-requirements.txt ] && python3 -m pip install -Ur test-requirements.txt
@@ -38,32 +38,27 @@
         make bats-libraries
         # Useful for debugging any issues with conda
         conda info -a
     - name: Get variables
       id: get_vars
       run: |
         REPO=$(basename ${{ github.repository }})
-        echo "REPO=${REPO}"
-        echo ::set-output name=REPO::${REPO}
+        echo "REPO=${REPO}" >> $GITHUB_OUTPUT
 
         BRANCH=${GITHUB_REF##*/}
-        echo "BRANCH=${BRANCH}"
-        echo ::set-output name=BRANCH::${BRANCH}
+        echo "BRANCH=${BRANCH}" >> $GITHUB_OUTPUT
 
         VERSION=$(python3 setup.py --version 2>/dev/null)
-        echo "VERSION=${VERSION}"
-        echo ::set-output name=VERSION::${VERSION}
+        echo "VERSION=${VERSION}" >> $GITHUB_OUTPUT
 
         TAG_VERSION=$(git describe --abbrev=0 --tags 2>/dev/null || true)
-        echo "TAG_VERSION=${TAG_VERSION}"
-        echo ::set-output name=TAG_VERSION::${TAG_VERSION}
+        echo "TAG_VERSION=${TAG_VERSION}" >> $GITHUB_OUTPUT
 
         ARTIFACT="${REPO}-${BRANCH}"
-        echo "ARTIFACT=${ARTIFACT}"
-        echo ::set-output name=ARTIFACT::${REPO}-${BRANCH}
+        echo "ARTIFACT=${ARTIFACT}" >> $GITHUB_OUTPUT
     # [1-test-build-publish]
     - name: Run tests
       run: make test
     # ![1-test-build-publish]
     - name: Build artifacts
       run: make bdist_wheel sdist twine-check
       if: >-
@@ -86,35 +81,32 @@
   deploy:
     name: Publish
     if: >-
       github.event_name == 'push' &&
       startsWith(github.ref, 'refs/tags')
     needs:
       - build-test
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-20.04
     env:
       PY_COLORS: 1
       TOX_PARALLEL_NO_SPINNER: 1
     steps:
     - name: Download artifacts
       uses: actions/download-artifact@v2
     - name: Get variables
       id: get_vars
       run: |
         REPO=$(basename ${{ github.repository }})
-        echo "REPO=${REPO}"
-        echo ::set-output name=REPO::${REPO}
+        echo "REPO=${REPO}" >> $GITHUB_OUTPUT
 
         BRANCH=${GITHUB_REF##*/}
-        echo "BRANCH=${BRANCH}"
-        echo ::set-output name=BRANCH::${BRANCH}
+        echo "BRANCH=${BRANCH}" >> $GITHUB_OUTPUT
 
         ARTIFACT="${REPO}-${BRANCH}"
-        echo "ARTIFACT=${ARTIFACT}"
-        echo ::set-output name=ARTIFACT::${REPO}-${BRANCH}
+        echo "ARTIFACT=${ARTIFACT}" >> $GITHUB_OUTPUT
     - name: Display artifacts
       run: |
         ls -lR
     # [2-test-build-publish]
     - name: Publish release candidate artifacts to TestPyPI
       if: >-
         github.event_name == 'push' &&
```

### Comparing `python_secrets-22.6.1/.gitignore` & `python_secrets-23.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/.travis.yml` & `python_secrets-23.4.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/.vscode/launch.json` & `python_secrets-23.4.1/.vscode/launch.json`

 * *Files 0% similar despite different names*

```diff
@@ -465,14 +465,28 @@
                 "describe",
                 "jenkins_admin_password"
             ],
             "stopOnEntry": false,
             "console": "integratedTerminal"
         },
         {
+            "name": "psec secrets find jenkins_admin_password",
+            "type": "python",
+            "request": "launch",
+            "module": "psec.__main__",
+            "args": [
+                "--debug",
+                "secrets",
+                "find",
+                "jenkins_admin_password"
+            ],
+            "stopOnEntry": false,
+            "console": "integratedTerminal"
+        },
+        {
             "name": "psec secrets get jenkins_admin_password",
             "type": "python",
             "request": "launch",
             "module": "psec.__main__",
             "args": [
                 "--debug",
                 "secrets",
```

### Comparing `python_secrets-22.6.1/AUTHORS.rst` & `python_secrets-23.4.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/CONTRIBUTING.rst` & `python_secrets-23.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/HISTORY.rst` & `python_secrets-23.4.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,31 @@
 .. Added for new features.
 .. Changed for changes in existing functionality.
 .. Deprecated for soon-to-be removed features.
 .. Removed for now removed features.
 .. Fixed for any bug fixes.
 .. Security in case of vulnerabilities.
 
+23.4.1 (2023-04-19)
+~~~~~~~~~~~~~~~~~~~
+
+Added
+^^^^^
+
+- Added `secrets find` command.
+- Added support for new variable type `boolean`.
+
+Changed
+^^^^^^^
+
+- Updated GitHub Actions workflows (default to Python 3.9.16).
+- Drop Python 3.7, 3.8, add Python 3.11 (default to 3.10) for `tox`.
+- Fixed downstream dependency and `pip` installation problems.
+- Resolved new `pep8` and `bandit` findings.
+
 22.6.1 (2022-06-21)
 ~~~~~~~~~~~~~~~~~~~
 
 Added
 ^^^^^
 
 - Added `--ignore-missing` option to continue when settings variables.
```

### Comparing `python_secrets-22.6.1/LICENSE.txt` & `python_secrets-23.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/Makefile` & `python_secrets-23.4.1/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Makefile for python_secrets
 
 SHELL=bash
 VERSION=$(shell cat VERSION)
 REQUIRED_VENV:=python_secrets
 VENV_DIR=$(HOME)/.virtualenvs/$(REQUIRED_VENV)
 PROJECT:=$(shell basename `pwd`)
-PYTHON=python3
 
 .PHONY: default
 default: all
 
 .PHONY: all
 all: install-active
 
@@ -20,42 +19,51 @@
 	@echo 'test - generic target for both "test-tox" and "test-bats"'
 	@echo 'test-tox - run tox tests'
 	@echo 'test-bats - run Bats unit tests'
 	@echo 'test-bats-runtime - run Bats runtime integration/system tests'
 	@echo 'release - produce a pypi production release'
 	@echo 'release-test - produce a pypi test release'
 	@echo 'release-prep - final documentation preparations for release'
-	@echo 'sdist - run "$(PYTHON) setup.py sdist"'
+	@echo 'sdist - run "python3 setup.py sdist"'
 	@echo 'bdist_wheel - build a universal binary wheel'
 	@echo 'twine-check - run "twine check"'
 	@echo 'clean - remove build artifacts'
 	@echo 'spotless - deep clean'
 	@echo 'build-packet-cafe - Build and bring up packet_cafe containers'
 	@echo 'up-packet-cafe - Bring up packet_cafe containers'
 	@echo 'down-packet-cafe - Bring up packet_cafe containers'
 	@echo 'clean-packet-cafe - remove packet_cafe contents'
 	@echo 'spotless-packet-cafe - Remove all packet_cafe files and containers'
 	@echo 'install - install pip package'
-	@echo 'install-active - run "$(PYTHON) -m pip install -U ."'
+	@echo 'install-active - run "python3 -m pip install -U ."'
 	@echo 'docs-tests - generate bats test output for documentation'
 	@echo 'docs-help - generate "lim help" output for documentation'
 	@echo 'docs - build Sphinx docs'
 
 
 #HELP test - run 'tox' for testing
 .PHONY: test
 test: test-tox
 	@echo '[+] test: All tests passed'
 
+# [Makefile-test-tox]
+# The following target rules are optimized by splitting up `tox` tests so they
+# fail early on syntax and security checks before running more lengthy unit
+# tests against Python versions (with coverage reporting).  This is designed to
+# more easily focus on code quality first and foremost.
 .PHONY: test-tox
 test-tox:
 	@if [ -f .python_secrets_environment ]; then (echo '[!] Remove .python_secrets_environment prior to testing'; exit 1); fi
 	touch docs/psec_help.txt
-	@# See comment in tox.ini file.
-	tox -e pep8 && tox -e bandit,docs,bats && tox -e clean,py37,py38,py39,py310,pypi,report && echo '[+] test-tox: All tests passed'
+	@# See also comment in tox.ini file.
+	tox -e pep8
+	tox -e bandit,docs,bats
+	tox -e clean,py39,py310,py311,pypi,report
+	echo '[+] test-tox: All tests passed'
+# ![Makefile-test-tox]
 
 .PHONY: test-bats
 test-bats: bats-libraries
 	@if [ "$(TRAVIS)" != "true" ]; then \
 		if ! type bats 2>/dev/null >/dev/null; then \
 			echo "[-] Skipping bats tests"; \
 		else \
@@ -94,43 +102,43 @@
 	$(MAKE) no-diffs
 	twine upload $(shell cat dist/.LATEST_*) -r testpypi
 
 #HELP sdist - build a source package
 .PHONY: sdist
 sdist: clean-docs docs
 	rm -f dist/.LATEST_SDIST
-	$(PYTHON) setup.py sdist
+	python3 setup.py sdist
 	ls -t dist/*.tar.gz 2>/dev/null | head -n 1 > dist/.LATEST_SDIST
 	ls -l dist/*.tar.gz
 
 #HELP bdist_egg - build an egg package
 .PHONY: bdist_egg
 bdist_egg:
 	rm -f dist/.LATEST_EGG
-	$(PYTHON) setup.py bdist_egg
+	python3 setup.py bdist_egg
 	ls -t dist/*.egg 2>/dev/null | head -n 1 > dist/.LATEST_EGG
 	ls -lt dist/*.egg
 
 #HELP bdist_wheel - build a wheel package
 .PHONY: bdist_wheel
 bdist_wheel:
 	rm -f dist/.LATEST_WHEEL
-	$(PYTHON) setup.py bdist_wheel
+	python3 setup.py bdist_wheel
 	ls -t dist/*.whl 2>/dev/null | head -n 1 > dist/.LATEST_WHEEL
 	ls -lt dist/*.whl
 
 #HELP twine-check
 .PHONY: twine-check
 twine-check: sdist bdist_egg bdist_wheel
 	twine check $(shell cat dist/.LATEST_*)
 
 #HELP clean - remove build artifacts
 .PHONY: clean
 clean: clean-docs
-	$(PYTHON) setup.py clean
+	python3 setup.py clean
 	rm -rf dist build *.egg-info
 	find . -name '*.pyc' -delete
 
 .PHONY: clean-docs
 clean-docs:
 	cd docs && make clean
 
@@ -141,29 +149,30 @@
 #HELP install - install in required Python virtual environment (default $(REQUIRED_VENV))
 .PHONY: install
 install:
 	@if [ ! -d $(VENV_DIR) ]; then \
 		echo "Required virtual environment '$(REQUIRED_VENV)' not found."; \
 		exit 1; \
 	fi
-	@if [ ! -e "$(VENV_DIR)/bin/python" ]; then \
-		echo "Cannot find $(VENV_DIR)/bin/python"; \
+	@if [ ! -e "$(VENV_DIR)/bin/python3" ]; then \
+		echo "Cannot find $(VENV_DIR)/bin/python3"; \
 		exit 1; \
 	else \
 		echo "Installing into $(REQUIRED_VENV) virtual environment"; \
-		$(VENV_DIR)/bin/$(PYTHON) -m pip uninstall -y $(PROJECT); \
-		$(VENV_DIR)/bin/$(PYTHON) setup.py install; \
+		$(VENV_DIR)/bin/python3 -m pip uninstall -y $(PROJECT); \
+		$(VENV_DIR)/bin/python3 setup.py install; \
 	fi
 
 #HELP install-active - install in the active Python virtual environment
 .PHONY: i
 .PHONY: install-active
 i install-active: bdist_wheel
-	$(PYTHON) -m pip uninstall -y $(PROJECT)
-	$(PYTHON) -m pip install -U "$(shell cat dist/.LATEST_WHEEL)" | grep -v ' already '
+	python3 -m pip uninstall -y $(PROJECT)
+	@# python3 -m pip install -U "$(shell cat dist/.LATEST_WHEEL)" | grep -v ' already '
+	python3 setup.py install
 
 #HELP docs-tests - generate bats test output for documentation
 .PHONY: docs-tests
 PR=pr --omit-header --omit-pagination --page-width 80
 docs-tests:
 	$(MAKE) -B docs/test-tox.txt
 	$(MAKE) -B docs/test-bats.txt
@@ -182,20 +191,20 @@
 
 #HELP docs - build Sphinx docs (NOT INTEGRATED YET FROM OPENSTACK CODE BASE)
 .PHONY: docs
 docs: docs/psec_help.txt
 	cd docs && make html
 
 docs/psec_help.txt: install-active
-	PYTHONPATH=$(shell pwd) python -m psec help | tee docs/psec_help.txt
+	PYTHONPATH=$(shell pwd) python3 -m psec help | tee docs/psec_help.txt
 
 #HELP examples - produce some example output for docs
 .PHONY: examples
 examples:
-	@PYTHONPATH=$(shell pwd) python -m psec --help
+	@PYTHONPATH=$(shell pwd) python3 -m psec --help
 
 # Git submodules and subtrees are both a huge PITA. This is way simpler.
 
 .PHONY: bats-libraries
 bats-libraries: bats bats-support bats-assert
 
 bats:
```

### Comparing `python_secrets-22.6.1/PKG-INFO` & `python_secrets-23.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_secrets
-Version: 22.6.1
+Version: 23.4.1
 Home-page: https://github.com/davedittrich/python_secrets
 Download-URL: https://github.com/davedittrich/python_secrets/tarball/master
 Author: Dave Dittrich
 Author-email: dave.dittrich@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -25,15 +25,15 @@
         :alt: Documentation Status
 
 
 Python command line app for managing groups of secrets (passwords, API keys, etc) and
 other project variables. Reduces security risks from things like weak default passwords,
 secrets stored in files in the source code repository directory.
 
-Version: 22.6.1
+Version: 23.4.1
 
 * Free software: `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_
 * Documentation: https://python_secrets.readthedocs.org.
 
 Features
 --------
 
@@ -1226,15 +1226,15 @@
     To: dittrich@u.washington.edu
 
     The following secret is being shared with you:
 
     myapp_app_password=brunt.outclass.alike.turbine
 
     --
-    Sent using psec version 22.6.1
+    Sent using psec version 23.4.1
     https://pypi.org/project/python-secrets/
     https://github.com/davedittrich/python_secrets
 
 ..
 
 A group of secrets required for Google's `OAuth 2.0 Mechanism`_  is provided
 and must be set according to Google's instructions. See also:
@@ -1712,14 +1712,31 @@
 .. Added for new features.
 .. Changed for changes in existing functionality.
 .. Deprecated for soon-to-be removed features.
 .. Removed for now removed features.
 .. Fixed for any bug fixes.
 .. Security in case of vulnerabilities.
 
+23.4.1 (2023-04-19)
+~~~~~~~~~~~~~~~~~~~
+
+Added
+^^^^^
+
+- Added `secrets find` command.
+- Added support for new variable type `boolean`.
+
+Changed
+^^^^^^^
+
+- Updated GitHub Actions workflows (default to Python 3.9.16).
+- Drop Python 3.7, 3.8, add Python 3.11 (default to 3.10) for `tox`.
+- Fixed downstream dependency and `pip` installation problems.
+- Resolved new `pep8` and `bandit` findings.
+
 22.6.1 (2022-06-21)
 ~~~~~~~~~~~~~~~~~~~
 
 Added
 ^^^^^
 
 - Added `--ignore-missing` option to continue when settings variables.
```

### Comparing `python_secrets-22.6.1/README.rst` & `python_secrets-23.4.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         :alt: Documentation Status
 
 
 Python command line app for managing groups of secrets (passwords, API keys, etc) and
 other project variables. Reduces security risks from things like weak default passwords,
 secrets stored in files in the source code repository directory.
 
-Version: 22.6.1
+Version: 23.4.1
 
 * Free software: `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_
 * Documentation: https://python_secrets.readthedocs.org.
 
 Features
 --------
 
@@ -1214,15 +1214,15 @@
     To: dittrich@u.washington.edu
 
     The following secret is being shared with you:
 
     myapp_app_password=brunt.outclass.alike.turbine
 
     --
-    Sent using psec version 22.6.1
+    Sent using psec version 23.4.1
     https://pypi.org/project/python-secrets/
     https://github.com/davedittrich/python_secrets
 
 ..
 
 A group of secrets required for Google's `OAuth 2.0 Mechanism`_  is provided
 and must be set according to Google's instructions. See also:
```

### Comparing `python_secrets-22.6.1/docs/Makefile` & `python_secrets-23.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/advanced.rst` & `python_secrets-23.4.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/conf.py` & `python_secrets-23.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/index.rst` & `python_secrets-23.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/installation.rst` & `python_secrets-23.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/make.bat` & `python_secrets-23.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/reference.rst` & `python_secrets-23.4.1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/docs/usage.rst` & `python_secrets-23.4.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/__init__.py` & `python_secrets-23.4.1/psec/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __version__ = None
-__release__ = '22.6.1'
+__release__ = '23.4.1'
 
 # Get development version from repository tags.
 try:
     from setuptools_scm import get_version
     __version__ = get_version(root='..', relative_to=__file__)
 except (ImportError, LookupError):
     pass
```

### Comparing `python_secrets-22.6.1/psec/__main__.py` & `python_secrets-23.4.1/psec/__main__.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/about.py` & `python_secrets-23.4.1/psec/about.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/create.py` & `python_secrets-23.4.1/psec/cli/environments/create.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/default.py` & `python_secrets-23.4.1/psec/cli/environments/default.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/delete.py` & `python_secrets-23.4.1/psec/cli/environments/delete.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/list.py` & `python_secrets-23.4.1/psec/cli/environments/list.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/path.py` & `python_secrets-23.4.1/psec/cli/environments/path.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/rename.py` & `python_secrets-23.4.1/psec/cli/environments/rename.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/environments/tree.py` & `python_secrets-23.4.1/psec/cli/environments/tree.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/groups/create.py` & `python_secrets-23.4.1/psec/cli/groups/create.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/groups/delete.py` & `python_secrets-23.4.1/psec/cli/groups/delete.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/groups/list.py` & `python_secrets-23.4.1/psec/cli/groups/list.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/groups/path.py` & `python_secrets-23.4.1/psec/cli/groups/path.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/groups/show.py` & `python_secrets-23.4.1/psec/cli/groups/show.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/init.py` & `python_secrets-23.4.1/psec/cli/init.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/run.py` & `python_secrets-23.4.1/psec/cli/run.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/backup.py` & `python_secrets-23.4.1/psec/cli/secrets/backup.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/create.py` & `python_secrets-23.4.1/psec/cli/secrets/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,53 @@
 # -*- coding: utf-8 -*-
 
 """
 Create a new secret definition.
 """
 
 # External imports
+# from ctypes.wintypes import BOOL
 import logging
 import os
 
 from sys import stdin
 
 # TODO(dittrich): https://github.com/Mckinsey666/bullet/issues/2
 # Workaround until bullet has Windows missing 'termios' fix.
 try:
-    from bullet import colors
-    from bullet import Input
-    from bullet import YesNo
+    from bullet import (
+        colors,
+        Input,
+        YesNo,
+    )
 except ModuleNotFoundError:
     pass
 from cliff.command import Command
 from prettytable import PrettyTable
 
 # Local imports
-from psec.secrets_environment import SECRET_TYPES
+from psec.secrets_environment import (
+    BOOLEAN_OPTIONS,
+    SECRET_TYPES,
+)
 from psec.utils import (
     find,
+    prompt_options_dict,
     prompt_options_list,
 )
 
 
+def ordered_boolean_options(result):
+    """Return a string with boolean options ordered based on result"""
+    boolean_idents = [i.get('ident') for i in BOOLEAN_OPTIONS]
+    first = boolean_idents.pop(boolean_idents.index(result))
+    second = boolean_idents.pop()
+    return ",".join([first, second])
+
+
 def get_description(name=None, defaults=None):
     """Prompt user for description fields and return results."""
     new_description = dict()
     # Variable name is required (obviously)
     new_description['Variable'] = defaults['Variable']
     # Variable type is required (obviously)
     original_type = defaults.get('Type', None)
@@ -46,25 +61,32 @@
     prompt = ("Descriptive string to prompt user when "
               "setting value: ")
     cli = Input(prompt,
                 default=defaults.get('Prompt'),
                 word_color=colors.foreground["yellow"])
     result = cli.launch()
     new_description['Prompt'] = result
-    # Alternative option set is (no pun intended) optional
+    if new_description['Type'] == 'boolean':
+        # This is going to go one of two ways!
+        result = prompt_options_dict(
+            prompt="Choose default state: ",
+            options=BOOLEAN_OPTIONS,
+        )
+        new_description['Options'] = ordered_boolean_options(result)
+    # Alternative option set is (no pun intended) optional.
     if new_description['Type'] in ['string']:
         prompt = "Acceptable options from which to chose: "
         cli = Input(prompt,
                     default=defaults.get('Options'),
                     word_color=colors.foreground["yellow"])
         result = cli.launch()
         # TODO(dittrich): BUG or ISSUE in waiting.
         # Items in an Options list can't end in '.*' without
         # causing confusion with ',*' wildcard feature.
-        # Maybe switch to using '|' for alternaives instead?
+        # Maybe switch to using '|' for alternatives instead?
         if '.*' in result:
             if result == '.*':
                 msg = "[-] '.*' is not valid: did you mean '*'?"
             else:
                 msg = ("[-] options list items can't have '.*' "
                        "wildcards: did you mean to end with ',*'?")
             raise RuntimeError(msg)
```

### Comparing `python_secrets-22.6.1/psec/cli/secrets/delete.py` & `python_secrets-23.4.1/psec/cli/secrets/delete.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/describe.py` & `python_secrets-23.4.1/psec/cli/secrets/describe.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/generate.py` & `python_secrets-23.4.1/psec/cli/secrets/generate.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/get.py` & `python_secrets-23.4.1/psec/cli/secrets/get.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/path.py` & `python_secrets-23.4.1/psec/cli/secrets/path.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/restore.py` & `python_secrets-23.4.1/psec/cli/secrets/restore.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/send.py` & `python_secrets-23.4.1/psec/cli/secrets/send.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/set.py` & `python_secrets-23.4.1/psec/cli/secrets/set.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Set values manually for secrets.
 """
 
 import logging
 import os
+import shlex
 
 from subprocess import run, PIPE  # nosec
 from cliff.command import Command
 
 from psec.secrets_environment import (
     BOOLEAN_OPTIONS,
     SecretsEnvironment,
@@ -229,24 +230,30 @@
                 if v is not None:
                     # Is the value indirectly referenced?
                     if v.startswith('@'):
                         if v[1] == '~':
                             _path = os.path.expanduser(v[1:])
                         else:
                             _path = v[1:]
-                        with open(_path, 'r') as f:
+                        with open(_path, 'r', encoding='utf-8') as f:
                             v = f.read().strip()
                     elif v.startswith('!'):
                         # >> Issue: [B603:subprocess_without_shell_equals_true] subprocess call - check for execution of untrusted input.  # noqa
                         #    Severity: Low   Confidence: High
-                        #    Location: psec/secrets.py:641
-                        p = run(v[1:].split(),
-                                stdout=PIPE,
-                                stderr=PIPE,
-                                shell=False)
+                        #    Location: psec/cli/set.py:246
+                        # >>> v = "!echo this is a $SHELL `command`"
+                        # >>> shlex.split(v[1:])
+                        # ['echo', 'this', 'is', 'a', '$SHELL', '`command`']
+                        p = run(
+                            shlex.split(v[1:]),  # nosec
+                            stdout=PIPE,
+                            stderr=PIPE,
+                            shell=False,
+                            check=True,
+                        )
                         v = p.stdout.decode('UTF-8').strip()
             # After all that, did we get a value?
             if v is None:
                 self.logger.info("[-] could not obtain value for '%s'", k)
             else:
                 self.logger.debug("[+] setting variable '%s'", k)
                 se.set_secret(k, v)
```

### Comparing `python_secrets-22.6.1/psec/cli/secrets/show.py` & `python_secrets-23.4.1/psec/cli/secrets/show.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/secrets/tree.py` & `python_secrets-23.4.1/psec/cli/secrets/tree.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/ssh.py` & `python_secrets-23.4.1/psec/cli/ssh.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/template.py` & `python_secrets-23.4.1/psec/cli/template.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/utils/myip.py` & `python_secrets-23.4.1/psec/cli/utils/myip.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/utils/netblock.py` & `python_secrets-23.4.1/psec/cli/utils/netblock.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/utils/set_aws_credentials.py` & `python_secrets-23.4.1/psec/cli/utils/set_aws_credentials.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/utils/tfbackend.py` & `python_secrets-23.4.1/psec/cli/utils/tfbackend.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/utils/tfoutput.py` & `python_secrets-23.4.1/psec/cli/utils/tfoutput.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/cli/utils/yaml_to_json.py` & `python_secrets-23.4.1/psec/cli/utils/yaml_to_json.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/exceptions.py` & `python_secrets-23.4.1/psec/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/google_oauth2.py` & `python_secrets-23.4.1/psec/google_oauth2.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/__init__.py` & `python_secrets-23.4.1/psec/secrets_environment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,17 +509,17 @@
             values = []
         return (
             values[0]
             if len(values) > 0 and values[0] != '*'
             else ''
         )
 
-    def read_secrets_and_descriptions(self):
+    def read_secrets_and_descriptions(self, ignore_errors=False):
         """Read secrets descriptions and secrets."""
-        self.read_secrets_descriptions()
+        self.read_secrets_descriptions(ignore_errors=ignore_errors)
         self.read_secrets(from_descriptions=True)
         self.find_new_secrets()
 
     def find_new_secrets(self):
         """
         Ensure that any new secrets defined in description files are
         called out and/or become new undefined secrets.
@@ -692,31 +692,37 @@
             for d in data:
                 v = d.get('Variable')
                 if v in self._secrets:
                     raise RuntimeError(
                         f"[-] variable '{v}' duplicates an existing variable"
                     )
 
-    def read_secrets_descriptions(self):
+    def read_secrets_descriptions(
+        self,
+        ignore_errors=False,
+    ):
         """Load the descriptions of groups of secrets from a .d directory"""
         groups_dir = self.get_descriptions_path()
         if not groups_dir.exists():
-            self.logger.info('[-] secrets descriptions directory not found')
+            if not ignore_errors:
+                self.logger.info(
+                    '[-] secrets descriptions directory not found'
+                )
         else:
             # Ignore .order file and any other file extensions
             extensions = ['.json']
             file_names = [
                 fn for fn in groups_dir.iterdir()
                 if fn.suffix in extensions
             ]
             self.logger.debug(
                 "[+] reading secrets descriptions from '%s'", groups_dir)
             # Iterate over files in directory, loading them into
             # dictionaries as dictionary keyed on group name.
-            if len(file_names) == 0:
+            if len(file_names) == 0 and not ignore_errors:
                 self.logger.info('[-] no secrets descriptions files found')
             for fname in file_names:
                 group = fname.stem
                 if '.' in group:
                     raise RuntimeError(
                         f"[-] group name cannot include '.': '{group}'")
                 descriptions = self.read_descriptions(group=group)
```

### Comparing `python_secrets-22.6.1/psec/secrets_environment/factory/__init__.py` & `python_secrets-23.4.1/psec/secrets_environment/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/handlers/crypt_6.py` & `python_secrets-23.4.1/psec/secrets_environment/handlers/crypt_6.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/handlers/password.py` & `python_secrets-23.4.1/psec/secrets_environment/handlers/password.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/handlers/sha256_digest.py` & `python_secrets-23.4.1/psec/secrets_environment/handlers/sha256_digest.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/handlers/token_base64.py` & `python_secrets-23.4.1/psec/secrets_environment/handlers/token_base64.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/handlers/token_hex.py` & `python_secrets-23.4.1/psec/secrets_environment/handlers/token_hex.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/secrets_environment/handlers/token_urlsafe.py` & `python_secrets-23.4.1/psec/secrets_environment/handlers/token_urlsafe.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/psec/utils.py` & `python_secrets-23.4.1/psec/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -984,15 +984,15 @@
 
 
 def myip_http(arg=None):
     """Use an HTTP service that only returns IP address."""
     # Return type if no argument for use in Lister.
     if arg is None:
         return 'https'
-    page = requests.get(arg, stream=True)
+    page = requests.get(arg, stream=True, timeout=3.05)
     soup = BeautifulSoup(page.text, 'html.parser')
     if page.status_code != 200:
         raise RuntimeError(
             f"[-] error: {page.reason}\n{soup.body.text}")
     logger.debug('[-] got page: "%s"', page.text)
     interface = ipaddress.ip_interface(str(soup).strip())
     return interface
```

### Comparing `python_secrets-22.6.1/python_secrets.egg-info/PKG-INFO` & `python_secrets-23.4.1/python_secrets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-secrets
-Version: 22.6.1
+Version: 23.4.1
 Home-page: https://github.com/davedittrich/python_secrets
 Download-URL: https://github.com/davedittrich/python_secrets/tarball/master
 Author: Dave Dittrich
 Author-email: dave.dittrich@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
@@ -25,15 +25,15 @@
         :alt: Documentation Status
 
 
 Python command line app for managing groups of secrets (passwords, API keys, etc) and
 other project variables. Reduces security risks from things like weak default passwords,
 secrets stored in files in the source code repository directory.
 
-Version: 22.6.1
+Version: 23.4.1
 
 * Free software: `Apache 2.0 License <https://www.apache.org/licenses/LICENSE-2.0>`_
 * Documentation: https://python_secrets.readthedocs.org.
 
 Features
 --------
 
@@ -1226,15 +1226,15 @@
     To: dittrich@u.washington.edu
 
     The following secret is being shared with you:
 
     myapp_app_password=brunt.outclass.alike.turbine
 
     --
-    Sent using psec version 22.6.1
+    Sent using psec version 23.4.1
     https://pypi.org/project/python-secrets/
     https://github.com/davedittrich/python_secrets
 
 ..
 
 A group of secrets required for Google's `OAuth 2.0 Mechanism`_  is provided
 and must be set according to Google's instructions. See also:
@@ -1712,14 +1712,31 @@
 .. Added for new features.
 .. Changed for changes in existing functionality.
 .. Deprecated for soon-to-be removed features.
 .. Removed for now removed features.
 .. Fixed for any bug fixes.
 .. Security in case of vulnerabilities.
 
+23.4.1 (2023-04-19)
+~~~~~~~~~~~~~~~~~~~
+
+Added
+^^^^^
+
+- Added `secrets find` command.
+- Added support for new variable type `boolean`.
+
+Changed
+^^^^^^^
+
+- Updated GitHub Actions workflows (default to Python 3.9.16).
+- Drop Python 3.7, 3.8, add Python 3.11 (default to 3.10) for `tox`.
+- Fixed downstream dependency and `pip` installation problems.
+- Resolved new `pep8` and `bandit` findings.
+
 22.6.1 (2022-06-21)
 ~~~~~~~~~~~~~~~~~~~
 
 Added
 ^^^^^
 
 - Added `--ignore-missing` option to continue when settings variables.
```

### Comparing `python_secrets-22.6.1/python_secrets.egg-info/SOURCES.txt` & `python_secrets-23.4.1/python_secrets.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 psec/cli/groups/path.py
 psec/cli/groups/show.py
 psec/cli/secrets/__init__.py
 psec/cli/secrets/backup.py
 psec/cli/secrets/create.py
 psec/cli/secrets/delete.py
 psec/cli/secrets/describe.py
+psec/cli/secrets/find.py
 psec/cli/secrets/generate.py
 psec/cli/secrets/get.py
 psec/cli/secrets/path.py
 psec/cli/secrets/restore.py
 psec/cli/secrets/send.py
 psec/cli/secrets/set.py
 psec/cli/secrets/show.py
```

### Comparing `python_secrets-22.6.1/python_secrets.egg-info/entry_points.txt` & `python_secrets-23.4.1/python_secrets.egg-info/entry_points.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 groups show = psec.cli.groups.show:GroupsShow
 init = psec.cli.init:Init
 run = psec.cli.run:Run
 secrets backup = psec.cli.secrets.backup:SecretsBackup
 secrets create = psec.cli.secrets.create:SecretsCreate
 secrets delete = psec.cli.secrets.delete:SecretsDelete
 secrets describe = psec.cli.secrets.describe:SecretsDescribe
+secrets find = psec.cli.secrets.find:SecretsFind
 secrets generate = psec.cli.secrets.generate:SecretsGenerate
 secrets get = psec.cli.secrets.get:SecretsGet
 secrets path = psec.cli.secrets.path:SecretsPath
 secrets restore = psec.cli.secrets.restore:SecretsRestore
 secrets send = psec.cli.secrets.send:SecretsSend
 secrets set = psec.cli.secrets.set:SecretsSet
 secrets show = psec.cli.secrets.show:SecretsShow
```

### Comparing `python_secrets-22.6.1/secrets.d/hypriot.json` & `python_secrets-23.4.1/secrets.d/hypriot.json`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/setup.cfg` & `python_secrets-23.4.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 22.6.1
+current_version = 23.4.1
 commit = False
 tag = False
 
 [bumpversion:file:VERSION]
 
 [bumpversion:file:README.rst]
 
@@ -27,19 +27,17 @@
 	Intended Audience :: Other Audience
 	Intended Audience :: Science/Research
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Security
 	Topic :: Software Development
 	Topic :: Software Development :: Build Tools
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Installation/Setup
 	Topic :: Utilities
 include_package_data = True
@@ -68,14 +66,15 @@
 	groups path = psec.cli.groups.path:GroupsPath
 	groups show = psec.cli.groups.show:GroupsShow
 	run = psec.cli.run:Run
 	secrets backup = psec.cli.secrets.backup:SecretsBackup
 	secrets create = psec.cli.secrets.create:SecretsCreate
 	secrets delete = psec.cli.secrets.delete:SecretsDelete
 	secrets describe = psec.cli.secrets.describe:SecretsDescribe
+	secrets find = psec.cli.secrets.find:SecretsFind
 	secrets generate = psec.cli.secrets.generate:SecretsGenerate
 	secrets get = psec.cli.secrets.get:SecretsGet
 	secrets path = psec.cli.secrets.path:SecretsPath
 	secrets restore = psec.cli.secrets.restore:SecretsRestore
 	secrets send = psec.cli.secrets.send:SecretsSend
 	secrets set = psec.cli.secrets.set:SecretsSet
 	secrets show = psec.cli.secrets.show:SecretsShow
```

### Comparing `python_secrets-22.6.1/setup.py` & `python_secrets-23.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/00_usage.bats` & `python_secrets-23.4.1/tests/00_usage.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/gosecure.json` & `python_secrets-23.4.1/tests/gosecure.json`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/runtime_00_initialization.bats` & `python_secrets-23.4.1/tests/runtime_00_initialization.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/runtime_05_environments.bats` & `python_secrets-23.4.1/tests/runtime_05_environments.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/runtime_10_groups.bats` & `python_secrets-23.4.1/tests/runtime_10_groups.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/runtime_20_secrets.bats` & `python_secrets-23.4.1/tests/runtime_20_secrets.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/runtime_30_utils.bats` & `python_secrets-23.4.1/tests/runtime_30_utils.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/runtime_40_run.bats` & `python_secrets-23.4.1/tests/runtime_40_run.bats`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/secrets.d/hypriot.json` & `python_secrets-23.4.1/tests/secrets.d/hypriot.json`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/secrets.d/myapp.json` & `python_secrets-23.4.1/tests/secrets.d/myapp.json`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/test_exceptions.py` & `python_secrets-23.4.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/test_groups.py` & `python_secrets-23.4.1/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/test_helper.bash` & `python_secrets-23.4.1/tests/test_helper.bash`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/test_secrets.py` & `python_secrets-23.4.1/tests/test_secrets.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/test_utils.py` & `python_secrets-23.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tests/yamlsecrets/secrets.d/myapp.yml` & `python_secrets-23.4.1/tests/yamlsecrets/secrets.d/myapp.yml`

 * *Files identical despite different names*

### Comparing `python_secrets-22.6.1/tox.ini` & `python_secrets-23.4.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tox]
 # In practice, you can optimize by first running basic tests
 # 'pep8,bandit,docs' and only after those succeed go on to
 # run the remaining (default) tests. E.g.,
-# $ tox -e pep8,bandit,docs && tox -e clean,py37,py38,py39,py310,bats,pypi,report
+# $ tox -e pep8,bandit,docs && tox -e clean,py39,py310,py311,bats,pypi,report
 
-envlist = clean,pep8,bandit,docs,py37,py38,py39,py310,bats,pypi,report
+envlist = clean,pep8,bandit,docs,py39,py310,py311,bats,pypi,report
 skip_missing_interpreters = True
 skipsdists = True
 requires = tox-conda
            setuptools>=40.9.0
            setuptools_scm
 
 [testenv]
@@ -19,16 +19,16 @@
 install_command = python -m pip install {opts} {packages}
 conda_deps =
        pytest
        pytest-cov
 conda_channels =
        conda-forge
 depends =
-   {py37,py38,py39,py310}: clean
-   report: py37,py38,py39,py310
+   {py39,py310,py311}: clean
+   report: py39,py310,py311
 # Make sure these match setup.py!
 deps = -r{toxinidir}/requirements-dev.txt
        -r{toxinidir}/requirements.txt
 commands = pytest {posargs} --cov=psec --cov-append --cov-report=term-missing
 
 [testenv:report]
 deps = coverage
```

