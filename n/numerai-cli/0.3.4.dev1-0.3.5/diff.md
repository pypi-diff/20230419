# Comparing `tmp/numerai-cli-0.3.4.dev1.tar.gz` & `tmp/numerai-cli-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/numerai-cli-0.3.4.dev1.tar", last modified: Tue Mar 29 00:11:27 2022, max compression
+gzip compressed data, was "dist/numerai-cli-0.3.5.tar", last modified: Wed Apr 19 01:47:13 2023, max compression
```

## Comparing `numerai-cli-0.3.4.dev1.tar` & `numerai-cli-0.3.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/
--rw-r--r--   0 root         (0) root         (0)     1064 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8137 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7798 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/
--rw-r--r--   0 root         (0) root         (0)       68 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/cli/
--rw-r--r--   0 root         (0) root         (0)      790 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1912 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/constants.py
--rw-r--r--   0 root         (0) root         (0)     4188 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/doctor.py
--rw-r--r--   0 root         (0) root         (0)     1626 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/cli/node/
--rw-r--r--   0 root         (0) root         (0)     1882 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/node/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4636 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/node/config.py
--rw-r--r--   0 root         (0) root         (0)      934 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/node/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2174 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/node/destroy.py
--rw-r--r--   0 root         (0) root         (0)    12401 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/node/test.py
--rw-r--r--   0 root         (0) root         (0)     1798 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/setup.py
--rw-r--r--   0 root         (0) root         (0)     2701 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/uninstall.py
--rw-r--r--   0 root         (0) root         (0)     4846 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/cli/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6494 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/util/debug.py
--rw-r--r--   0 root         (0) root         (0)     7284 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/util/docker.py
--rw-r--r--   0 root         (0) root         (0)     2597 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/util/files.py
--rw-r--r--   0 root         (0) root         (0)     5182 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/cli/util/keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/
--rw-r--r--   0 root         (0) root         (0)     1359 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     5732 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/data.py
--rw-r--r--   0 root         (0) root         (0)     5533 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/predict.py
--rw-r--r--   0 root         (0) root         (0)      164 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      227 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-python3/
--rw-r--r--   0 root         (0) root         (0)     1359 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-python3/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     3750 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-python3/predict.py
--rw-r--r--   0 root         (0) root         (0)       63 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-python3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      312 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-python3/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-rlang/
--rw-r--r--   0 root         (0) root         (0)     1546 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-rlang/Dockerfile
--rw-r--r--   0 root         (0) root         (0)       58 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-rlang/install_packages.R
--rw-r--r--   0 root         (0) root         (0)     1087 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/examples/tournament-rlang/main.R
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/terraform/
--rw-r--r--   0 root         (0) root         (0)      663 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/-inputs.tf
--rw-r--r--   0 root         (0) root         (0)      573 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/-main.tf
--rw-r--r--   0 root         (0) root         (0)      121 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/-outputs.tf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/
--rw-r--r--   0 root         (0) root         (0)      663 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/-inputs.tf
--rw-r--r--   0 root         (0) root         (0)       48 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/-locals.tf
--rw-r--r--   0 root         (0) root         (0)      484 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/-outputs.tf
--rw-r--r--   0 root         (0) root         (0)     2048 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/cluster.tf
--rw-r--r--   0 root         (0) root         (0)     1240 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/network.tf
--rw-r--r--   0 root         (0) root         (0)     6806 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/aws/webhook.tf
--rw-r--r--   0 root         (0) root         (0)     2275 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/lambda.zip
--rw-r--r--   0 root         (0) root         (0)  5680699 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/numerai/terraform/layer.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8137 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1593 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/numerai_cli.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-03-29 00:11:27.000000 numerai-cli-0.3.4.dev1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      900 2022-03-29 00:11:20.000000 numerai-cli-0.3.4.dev1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9163 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8829 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/cli/
+-rw-r--r--   0 root         (0) root         (0)      790 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/constants.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/doctor.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/cli/node/
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/node/config.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/node/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/node/destroy.py
+-rw-r--r--   0 root         (0) root         (0)    12407 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/node/test.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/setup.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/uninstall.py
+-rw-r--r--   0 root         (0) root         (0)     4846 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/cli/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6494 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/util/debug.py
+-rw-r--r--   0 root         (0) root         (0)     7339 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/util/docker.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     5182 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/cli/util/keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/examples/signals-python3/
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/signals-python3/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     5732 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/signals-python3/data.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/signals-python3/predict.py
+-rw-r--r--   0 root         (0) root         (0)      180 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/signals-python3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      227 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/signals-python3/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/examples/tournament-python3/
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-python3/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-python3/predict.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-python3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      312 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-python3/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/examples/tournament-rlang/
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-rlang/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-rlang/install_packages.R
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/examples/tournament-rlang/main.R
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/terraform/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/-inputs.tf
+-rw-r--r--   0 root         (0) root         (0)      551 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/-main.tf
+-rw-r--r--   0 root         (0) root         (0)      121 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/-outputs.tf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai/terraform/aws/
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/aws/-inputs.tf
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/aws/-locals.tf
+-rw-r--r--   0 root         (0) root         (0)      484 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/aws/-outputs.tf
+-rw-r--r--   0 root         (0) root         (0)     2069 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/aws/cluster.tf
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/aws/network.tf
+-rw-r--r--   0 root         (0) root         (0)     6806 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/aws/webhook.tf
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/lambda.zip
+-rw-r--r--   0 root         (0) root         (0)  5680699 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/numerai/terraform/layer.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9163 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/numerai_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 01:47:13.000000 numerai-cli-0.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      895 2023-04-19 01:47:06.000000 numerai-cli-0.3.5/setup.py
```

### Comparing `numerai-cli-0.3.4.dev1/LICENSE` & `numerai-cli-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/PKG-INFO` & `numerai-cli-0.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,28 @@
-Metadata-Version: 2.1
-Name: numerai-cli
-Version: 0.3.4.dev1
-Summary: A library for deploying Numer.ai Prediction Nodes.
-Home-page: https://github.com/numerai/numerai-cli
-Author: Numer.ai
-Author-email: contact@numer.ai
-License: MIT
-Platform: UNKNOWN
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # numerai-cli
 
 [![CircleCI](https://circleci.com/gh/numerai/numerai-cli.svg?style=svg)](https://circleci.com/gh/numerai/numerai-cli)
 [![PyPI](https://img.shields.io/pypi/v/numerai-cli.svg?color=brightgreen)](https://pypi.org/project/numerai-cli/)
 
-Welcome to Numerai CLI, if you haven't heard of Numerai [see our docs](https://docs.numer.ai/tournament/learn)
-to learn more. Currently, this CLI configures a Numerai Prediction Node in Amazon Web Services 
-(AWS) that you can deploy your models to. This solution is architected to cost less than 
-$5/mo on average, but actual costs may vary. It has been tested and found working on 
-MacOS/OSX, Windows 8/10, and Ubuntu 18/20, but should theoretically work anywhere that
-Docker and Python 3 are available.
+Welcome to the Numerai CLI for the [Numerai Tournament](https://docs.numer.ai/tournament/learn).
+This CLI runs on your local computer to configure a Numerai Prediction Node in the cloud.
+This solution is architected to cost less than $5/mo on average, but actual costs may vary.
+It has been tested and found working on MacOS/OSX, Windows 8/10, and Ubuntu 18/20,
+but should theoretically work anywhere that Docker and Python 3 are available.
 
 If you have any problems, questions, comments, concerns, or general feedback, please refer to the
 [Troubleshooting and Feedback](#troubleshooting-and-feedback) before posting anywhere.
 
 
 ## Contents
 - [Getting Started](#getting-started)
-- [Upgrading to 0.3.0](#upgrading-to-030)
 - [Node Configuration Tutorial](#node-configuration)
 - [List of Commands](#list-of-commands)
 - [Troubleshooting and Feedback](#troubleshooting-and-feedback)
+- [Upgrading to 0.3.0](#upgrading-to-030)
 - [Uninstall](#uninstall)
 
 
 ## Getting Started
 
 1.  Sign up a Numerai Account, get your Numerai API Keys, and your first Model:
     1.  Sign up at https://numer.ai/signup and log in to your new account
@@ -71,61 +57,68 @@
     ```
     pip3 install --upgrade numerai-cli --user
     ```
     NOTES:
     - This command will also work to update to new versions of the package in the future.
     - If you are using python venv then drop the --user option. 
       If you don't know what that is, disregard this note.
-      
-## Upgrading
-Upgrading numerai-cli will always require you to update the package itself using pip:
+  
+
+## Node Configuration Tutorial
+
+If you know you have all the prerequisites and have your AWS and Numerai API Keys at hand,
+you can run these commands on your local computer to get an example node running in minutes:
+
 ```
-pip install --upgrade numerai-cli --user
+numerai setup
+numerai node config --example tournament-python3
+numerai node deploy
+numerai node test
 ```
 
-#### 0.1/0.2 -> 0.3.0
-CLI 0.3.0 uses a new configuration format that is incompatible with versions 0.1 and 0.2,
-but a command to migrate you configuration is provided for you. Run this in the directory
-you ran `numerai setup` from the previous version:
+If you want to use larger instances to generate your predictions first run `numerai list-constants`
+to list the vCPU/mem presets available, then you can configure a node to use one of the presets via:
 ```
-numerai upgrade
+numerai node config -s mem-lg
 ```
 
-#### Beyond
-Some updates will make changes to configuration files used by Numerai CLI. These will
-require you to re-run some commands to upgrade your nodes to the newest versions:
-- `numerai setup` will copy over changes to files in the `$HOME/.numerai` directory
-- `numerai node config` will apply those changes to a node
+Your compute node is now setup and ready to run! 
 
-## Node Configuration Tutorial
+**VERY IMPORTANT**
+These commands have stored configuration files in `$USER_HOME/.numerai/`.
+If you lose this directory without destroying your nodes,
+you will have to manually (and painfully) delete every cloud resource by hand,
+so make sure you backup these files regularly! 
+DO NOT USE THESE COMMANDS FROM A TEMPORARY INSTANCE!!!!
 
-If you know you have all the prerequisites and have your AWS and Numerai API Keys at hand,
-you can run these commands to get an example node running in minutes:
+
+The example node will train and predict in the cloud, but this is inefficient.
+It's usually best to train your model locally (ensuring that the trained model is 
+stored in the same folder as your code) and then deploy the trained model.
+When you make changes to your code or re-train your model, simply deploy and test your node again:
 
 ```
-numerai setup
-numerai node config --example tournament-python3
 numerai node deploy
 numerai node test
 ```
 
-Your compute node is now setup and ready to run. It saves important configuration 
-information in `$USER_HOME/.numerai/nodes.json` including the url for your Node Trigger.
+The `nodes.json` file also includes the url for your Node Trigger.
 This trigger is registered with whichever model you specified during configuration.
 Each trigger will be called Saturday morning right after a new round opens, 
 and if the related job fails it will be triggered again around 24 hours later.
+You can opt into compute for daily tournaments via the website (go to numer.ai/models,
+click the 3 dots next to your model, click "compute", and click the switch to opt in).
 
 NOTES:
 - The default example does _not_ make stake changes; you will still have to do that manually.
   Please refer to the [numerapi docs](https://numerapi.readthedocs.io/en/latest/api/numerapi.html#module-numerapi.numerapi)
   for the methods you must call to do this.
 - You can view resources and logs in the AWS Console (region us-east-1) for your
   [ECS Cluster](https://console.aws.amazon.com/ecs/home?region=us-east-1#/clusters/numerai-submission-ecs-cluster/tasks)
   and [other resources](https://console.aws.amazon.com/cloudwatch/home?region=us-east-1#logsV2:log-groups)
-- If you're getting
 
 NEXT: [read the Prediction Nodes wiki](https://github.com/numerai/numerai-cli/wiki/Prediction-Nodes)
 to learn about Numerai Examples and how to customize Prediction Nodes.
 
 ## List of Commands
 Use the `--help` option on any command or sub-command to get a full description of it:
 ```
@@ -149,36 +142,55 @@
 ## Troubleshooting and Feedback
 Before messaging the Rocketchat channel or creating a Github issue, 
 please read through the following (especially the "Troubleshooting" section in the wiki):
 - [Github Wiki](https://github.com/numerai/numerai-cli/wiki)
 - [Github Issues](https://github.com/numerai/numerai-cli/issues)
 
 If you still cannot find a solution or answer, please join us on the 
-[RocketChat #compute Channel](https://community.numer.ai/channel/compute) 
+[RocketChat #support Channel](https://rocketchat.numer.ai/channel/support) 
 and include the following information with your issue/message:
 
 - The commands you ran that caused the error (even previous commands)
 - Version information from running:
     - `pip3 show numerai-cli`
     - `python -V`
     - `docker -v`
 - System Information from running
     - Mac: `system_profiler SPSoftwareDataType && system_profiler SPHardwareDataType`
     - Linux: `lsb_release -a && uname -a`
     - Windows: `powershell -command "Get-ComputerInfo"`
   
 If you do not include this information, we cannot help you.
+
+
+## Upgrading and Updating
+Upgrading numerai-cli will always require you to update the package itself using pip:
+```
+pip install --upgrade numerai-cli --user
+```
+
+#### 0.1/0.2 -> 0.3.0
+CLI 0.3.0 uses a new configuration format that is incompatible with versions 0.1 and 0.2,
+but a command to migrate you configuration is provided for you. Run this in the directory
+you ran `numerai setup` from the previous version:
+```
+numerai upgrade
+```
+
+#### Beyond
+Some updates will make changes to configuration files used by Numerai CLI. These will
+require you to re-run some commands to upgrade your nodes to the newest versions:
+- `numerai setup` will copy over changes to files in the `$HOME/.numerai` directory
+- `numerai node config` will apply those changes to a node
       
 
 ## Uninstall
 ```
 numerai uninstall
 ```
 
 
 ## Contributions
 
 - Thanks to [uuazed](https://github.com/uuazed) for their work on [numerapi](https://github.com/uuazed/numerapi)
 - Thanks to [hellno](https://github.com/hellno) for starting the Signals [ticker map](https://github.com/hellno/numerai-signals-tickermap)
 - Thanks to tit_BTCQASH ([numerai profile](https://numer.ai/tit_btcqash) and [twitter profile](https://twitter.com/tit_BTCQASH)) for debugging the environment setup process on Windows 8
-
-
```

### Comparing `numerai-cli-0.3.4.dev1/README.md` & `numerai-cli-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,41 @@
+Metadata-Version: 2.1
+Name: numerai-cli
+Version: 0.3.5
+Summary: A library for deploying Numer.ai Prediction Nodes.
+Home-page: https://github.com/numerai/numerai-cli
+Author: Numer.ai
+Author-email: contact@numer.ai
+License: MIT
+Platform: UNKNOWN
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # numerai-cli
 
 [![CircleCI](https://circleci.com/gh/numerai/numerai-cli.svg?style=svg)](https://circleci.com/gh/numerai/numerai-cli)
 [![PyPI](https://img.shields.io/pypi/v/numerai-cli.svg?color=brightgreen)](https://pypi.org/project/numerai-cli/)
 
-Welcome to Numerai CLI, if you haven't heard of Numerai [see our docs](https://docs.numer.ai/tournament/learn)
-to learn more. Currently, this CLI configures a Numerai Prediction Node in Amazon Web Services 
-(AWS) that you can deploy your models to. This solution is architected to cost less than 
-$5/mo on average, but actual costs may vary. It has been tested and found working on 
-MacOS/OSX, Windows 8/10, and Ubuntu 18/20, but should theoretically work anywhere that
-Docker and Python 3 are available.
+Welcome to the Numerai CLI for the [Numerai Tournament](https://docs.numer.ai/tournament/learn).
+This CLI runs on your local computer to configure a Numerai Prediction Node in the cloud.
+This solution is architected to cost less than $5/mo on average, but actual costs may vary.
+It has been tested and found working on MacOS/OSX, Windows 8/10, and Ubuntu 18/20,
+but should theoretically work anywhere that Docker and Python 3 are available.
 
 If you have any problems, questions, comments, concerns, or general feedback, please refer to the
 [Troubleshooting and Feedback](#troubleshooting-and-feedback) before posting anywhere.
 
 
 ## Contents
 - [Getting Started](#getting-started)
-- [Upgrading to 0.3.0](#upgrading-to-030)
 - [Node Configuration Tutorial](#node-configuration)
 - [List of Commands](#list-of-commands)
 - [Troubleshooting and Feedback](#troubleshooting-and-feedback)
+- [Upgrading to 0.3.0](#upgrading-to-030)
 - [Uninstall](#uninstall)
 
 
 ## Getting Started
 
 1.  Sign up a Numerai Account, get your Numerai API Keys, and your first Model:
     1.  Sign up at https://numer.ai/signup and log in to your new account
@@ -58,61 +70,68 @@
     ```
     pip3 install --upgrade numerai-cli --user
     ```
     NOTES:
     - This command will also work to update to new versions of the package in the future.
     - If you are using python venv then drop the --user option. 
       If you don't know what that is, disregard this note.
-      
-## Upgrading
-Upgrading numerai-cli will always require you to update the package itself using pip:
+  
+
+## Node Configuration Tutorial
+
+If you know you have all the prerequisites and have your AWS and Numerai API Keys at hand,
+you can run these commands on your local computer to get an example node running in minutes:
+
 ```
-pip install --upgrade numerai-cli --user
+numerai setup
+numerai node config --example tournament-python3
+numerai node deploy
+numerai node test
 ```
 
-#### 0.1/0.2 -> 0.3.0
-CLI 0.3.0 uses a new configuration format that is incompatible with versions 0.1 and 0.2,
-but a command to migrate you configuration is provided for you. Run this in the directory
-you ran `numerai setup` from the previous version:
+If you want to use larger instances to generate your predictions first run `numerai list-constants`
+to list the vCPU/mem presets available, then you can configure a node to use one of the presets via:
 ```
-numerai upgrade
+numerai node config -s mem-lg
 ```
 
-#### Beyond
-Some updates will make changes to configuration files used by Numerai CLI. These will
-require you to re-run some commands to upgrade your nodes to the newest versions:
-- `numerai setup` will copy over changes to files in the `$HOME/.numerai` directory
-- `numerai node config` will apply those changes to a node
+Your compute node is now setup and ready to run! 
 
-## Node Configuration Tutorial
+**VERY IMPORTANT**
+These commands have stored configuration files in `$USER_HOME/.numerai/`.
+If you lose this directory without destroying your nodes,
+you will have to manually (and painfully) delete every cloud resource by hand,
+so make sure you backup these files regularly! 
+DO NOT USE THESE COMMANDS FROM A TEMPORARY INSTANCE!!!!
 
-If you know you have all the prerequisites and have your AWS and Numerai API Keys at hand,
-you can run these commands to get an example node running in minutes:
+
+The example node will train and predict in the cloud, but this is inefficient.
+It's usually best to train your model locally (ensuring that the trained model is 
+stored in the same folder as your code) and then deploy the trained model.
+When you make changes to your code or re-train your model, simply deploy and test your node again:
 
 ```
-numerai setup
-numerai node config --example tournament-python3
 numerai node deploy
 numerai node test
 ```
 
-Your compute node is now setup and ready to run. It saves important configuration 
-information in `$USER_HOME/.numerai/nodes.json` including the url for your Node Trigger.
+The `nodes.json` file also includes the url for your Node Trigger.
 This trigger is registered with whichever model you specified during configuration.
 Each trigger will be called Saturday morning right after a new round opens, 
 and if the related job fails it will be triggered again around 24 hours later.
+You can opt into compute for daily tournaments via the website (go to numer.ai/models,
+click the 3 dots next to your model, click "compute", and click the switch to opt in).
 
 NOTES:
 - The default example does _not_ make stake changes; you will still have to do that manually.
   Please refer to the [numerapi docs](https://numerapi.readthedocs.io/en/latest/api/numerapi.html#module-numerapi.numerapi)
   for the methods you must call to do this.
 - You can view resources and logs in the AWS Console (region us-east-1) for your
   [ECS Cluster](https://console.aws.amazon.com/ecs/home?region=us-east-1#/clusters/numerai-submission-ecs-cluster/tasks)
   and [other resources](https://console.aws.amazon.com/cloudwatch/home?region=us-east-1#logsV2:log-groups)
-- If you're getting
 
 NEXT: [read the Prediction Nodes wiki](https://github.com/numerai/numerai-cli/wiki/Prediction-Nodes)
 to learn about Numerai Examples and how to customize Prediction Nodes.
 
 ## List of Commands
 Use the `--help` option on any command or sub-command to get a full description of it:
 ```
@@ -136,34 +155,57 @@
 ## Troubleshooting and Feedback
 Before messaging the Rocketchat channel or creating a Github issue, 
 please read through the following (especially the "Troubleshooting" section in the wiki):
 - [Github Wiki](https://github.com/numerai/numerai-cli/wiki)
 - [Github Issues](https://github.com/numerai/numerai-cli/issues)
 
 If you still cannot find a solution or answer, please join us on the 
-[RocketChat #compute Channel](https://community.numer.ai/channel/compute) 
+[RocketChat #support Channel](https://rocketchat.numer.ai/channel/support) 
 and include the following information with your issue/message:
 
 - The commands you ran that caused the error (even previous commands)
 - Version information from running:
     - `pip3 show numerai-cli`
     - `python -V`
     - `docker -v`
 - System Information from running
     - Mac: `system_profiler SPSoftwareDataType && system_profiler SPHardwareDataType`
     - Linux: `lsb_release -a && uname -a`
     - Windows: `powershell -command "Get-ComputerInfo"`
   
 If you do not include this information, we cannot help you.
+
+
+## Upgrading and Updating
+Upgrading numerai-cli will always require you to update the package itself using pip:
+```
+pip install --upgrade numerai-cli --user
+```
+
+#### 0.1/0.2 -> 0.3.0
+CLI 0.3.0 uses a new configuration format that is incompatible with versions 0.1 and 0.2,
+but a command to migrate you configuration is provided for you. Run this in the directory
+you ran `numerai setup` from the previous version:
+```
+numerai upgrade
+```
+
+#### Beyond
+Some updates will make changes to configuration files used by Numerai CLI. These will
+require you to re-run some commands to upgrade your nodes to the newest versions:
+- `numerai setup` will copy over changes to files in the `$HOME/.numerai` directory
+- `numerai node config` will apply those changes to a node
       
 
 ## Uninstall
 ```
 numerai uninstall
 ```
 
 
 ## Contributions
 
 - Thanks to [uuazed](https://github.com/uuazed) for their work on [numerapi](https://github.com/uuazed/numerapi)
 - Thanks to [hellno](https://github.com/hellno) for starting the Signals [ticker map](https://github.com/hellno/numerai-signals-tickermap)
 - Thanks to tit_BTCQASH ([numerai profile](https://numer.ai/tit_btcqash) and [twitter profile](https://twitter.com/tit_BTCQASH)) for debugging the environment setup process on Windows 8
+
+
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/__init__.py` & `numerai-cli-0.3.5/numerai/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/constants.py` & `numerai-cli-0.3.5/numerai/cli/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,43 +19,51 @@
 PROVIDERS = [
     PROVIDER_AWS,
     # PROVIDER_GCP
 ]
 
 LOG_TYPE_WEBHOOK = 'webhook'
 LOG_TYPE_CLUSTER = 'cluster'
-LOG_TYPES = [
-    LOG_TYPE_WEBHOOK,
-    LOG_TYPE_CLUSTER
-]
+LOG_TYPES = [LOG_TYPE_WEBHOOK, LOG_TYPE_CLUSTER]
 
 SIZE_PRESETS = {
+    # balanced cpu/mem
+    "gen-xs": (512, 2048),
     "gen-sm": (1024, 4096),
     "gen-md": (2048, 8192),
     "gen-lg": (4096, 16384),
-
+    "gen-xl": (8192, 30720),
+    "gen-2xl": (16384, 61440),
+    # cpu heavy
     "cpu-xs": (512, 1024),
     "cpu-sm": (1024, 2048),
     "cpu-md": (2048, 4096),
     "cpu-lg": (4096, 8192),
-
+    "cpu-xl": (8192, 16384),
+    "cpu-2xl": (16384, 30720),
+    # mem heavy
+    "mem-xs": (512, 4096),
     "mem-sm": (1024, 8192),
     "mem-md": (2048, 16384),
     "mem-lg": (4096, 30720),
+    "mem-xl": (8192, 61440),
+    "mem-2xl": (16384, 81920),
+    "mem-3xl": (16384, 102400),
+    "mem-4xl": (16384, 122880),
 }
 
 DEFAULT_EXAMPLE = 'tournament-python3'
 DEFAULT_SIZE = "mem-md"
 DEFAULT_PROVIDER = PROVIDER_AWS
 DEFAULT_PATH = os.getcwd()
 DEFAULT_SETTINGS = {
     'provider': DEFAULT_PROVIDER,
     'cpu': SIZE_PRESETS[DEFAULT_SIZE][0],
     'memory': SIZE_PRESETS[DEFAULT_SIZE][1],
-    'path': DEFAULT_PATH
+    'path': DEFAULT_PATH,
 }
 
 CONSTANTS_STR = f'''Default values (not your configured node values):
 
 ---Tournament Numbers---
 TOURNAMENT_NUMERAI: {TOURNAMENT_NUMERAI}
 TOURNAMENT_SIGNALS: {TOURNAMENT_SIGNALS}
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/doctor.py` & `numerai-cli-0.3.5/numerai/cli/doctor.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/misc.py` & `numerai-cli-0.3.5/numerai/cli/misc.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/node/__init__.py` & `numerai-cli-0.3.5/numerai/cli/node/__init__.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/node/config.py` & `numerai-cli-0.3.5/numerai/cli/node/config.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/node/deploy.py` & `numerai-cli-0.3.5/numerai/cli/node/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     model = ctx.obj['model']
     node = model['name']
     node_config = files.load_or_init_nodes(node)
 
     docker.check_for_dockerfile(node_config['path'])
 
     click.echo('building container image (this may take several minutes)...')
-    docker.build(node_config, verbose)
+    docker.build(node_config, node, verbose)
 
     click.echo('logging into container registry...')
     docker.login(node_config, verbose)
 
     click.echo('pushing image to registry (this may take several minutes)...')
     docker.push(node_config['docker_repo'], verbose)
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/node/destroy.py` & `numerai-cli-0.3.5/numerai/cli/node/destroy.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/node/test.py` & `numerai-cli-0.3.5/numerai/cli/node/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     model = ctx.obj['model']
     node = model['name']
     is_signals = model['is_signals']
     node_config = load_or_init_nodes(node)
 
     if local:
         click.secho("starting local test; building container...")
-        docker.build(node_config, verbose)
+        docker.build(node_config, node, verbose)
         click.secho("running container...")
         docker.run(node_config, verbose, command=command)
 
     api = base_api.Api(*get_numerai_keys())
     trigger_id = None
     try:
         if 'cron' in node_config:
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/setup.py` & `numerai-cli-0.3.5/numerai/cli/setup.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/uninstall.py` & `numerai-cli-0.3.5/numerai/cli/uninstall.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/upgrade.py` & `numerai-cli-0.3.5/numerai/cli/upgrade.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/util/debug.py` & `numerai-cli-0.3.5/numerai/cli/util/debug.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/util/docker.py` & `numerai-cli-0.3.5/numerai/cli/util/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     if b'ResourceNotFoundException' in stdout or b'NoSuchEntity' in stdout:
         refresh = build_tf_cmd('refresh', env_vars, inputs, version, verbose)
         execute(refresh, verbose)
         stdout, stderr = execute(cmd, verbose)
     return stdout
 
 
-def build(node_config, verbose):
+def build(node_config, node, verbose):
     numerai_keys = load_or_init_keys()['numerai']
 
     node_path = node_config["path"]
     curr_path = os.path.abspath('.')
     if curr_path not in node_path:
         raise RuntimeError(
             f'Current directory invalid, you must run this command either from'
@@ -143,14 +143,15 @@
         click.secho(f'Using relative path to node: {path}')
 
     build_arg_str = ''
     for arg in numerai_keys:
         build_arg_str += f' --build-arg {arg}={numerai_keys[arg]}'
     build_arg_str += f' --build-arg MODEL_ID={node_config["model_id"]}'
     build_arg_str += f' --build-arg SRC_PATH={path}'
+    build_arg_str += f' --build-arg NODE={node}'
 
     cmd = f'docker build --platform=linux/amd64 -t {node_config["docker_repo"]}' \
           f'{build_arg_str} -f {path}/Dockerfile .'
 
     execute(cmd, verbose)
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/util/files.py` & `numerai-cli-0.3.5/numerai/cli/util/files.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/cli/util/keys.py` & `numerai-cli-0.3.5/numerai/cli/util/keys.py`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/Dockerfile` & `numerai-cli-0.3.5/numerai/examples/signals-python3/Dockerfile`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/data.py` & `numerai-cli-0.3.5/numerai/examples/signals-python3/data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 def generate_rsi_features(full_data, num_days):
     # add Relative Strength Index
     logging.info('generating RSI for each price...')
     ticker_groups = full_data.groupby("ticker")
     full_data["RSI"] = ticker_groups["price"].transform(
         lambda x: relative_strength_index(x)
     )
+    full_data.dropna(inplace=True)
 
     # group by era (date)
     logging.info('grouping by dates...')
     date_groups = full_data.groupby(full_data.index)
 
     # create quintile labels within each era, useful for learning relative ranking
     logging.info('generating RSI quintiles...')
     full_data["RSI_quintile"] = date_groups["RSI"].transform(
         lambda group: pd.qcut(group, 5, labels=False, duplicates="drop")
     )
-    full_data.dropna(inplace=True)
 
     feat_quintile_lag, feat_rsi_diff, feat_rsi_diff_abs = get_rsi_feature_names(num_days)
 
     # create lagged features grouped by ticker
     logging.info('grouping by ticker...')
     ticker_groups = full_data.groupby("ticker")
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/examples/signals-python3/predict.py` & `numerai-cli-0.3.5/numerai/examples/signals-python3/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import joblib
 import numerapi
 import pandas as pd
 from sklearn.ensemble import GradientBoostingRegressor
 from dateutil.relativedelta import relativedelta, FR
 
-TARGET_NAME = "target"
+TARGET_NAME = "target_4d"
 PREDICTION_NAME = "signal"
 TRAINED_MODEL_PREFIX = './trained_model'
 
 # Pull model id from "MODEL_ID" environment variable
 # defaults to None, change to a model id from
 MODEL_ID = os.getenv('MODEL_ID', None)
 MODEL = GradientBoostingRegressor(subsample=0.1)
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/examples/tournament-python3/Dockerfile` & `numerai-cli-0.3.5/numerai/examples/tournament-python3/Dockerfile`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/examples/tournament-rlang/Dockerfile` & `numerai-cli-0.3.5/numerai/examples/tournament-rlang/Dockerfile`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/examples/tournament-rlang/main.R` & `numerai-cli-0.3.5/numerai/examples/tournament-rlang/main.R`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/-inputs.tf` & `numerai-cli-0.3.5/numerai/terraform/-inputs.tf`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/-main.tf` & `numerai-cli-0.3.5/numerai/terraform/-main.tf`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 terraform {
   required_version = "~> 0.14.0"
 }
 
 # Specify the provider and access details
 provider "aws" {
-  profile = "default"
   region  = var.region
 }
 
 locals {
   nodes = jsondecode(file(var.node_config_file))
   aws_nodes = {
     for node, config in local.nodes:
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/aws/-inputs.tf` & `numerai-cli-0.3.5/numerai/terraform/aws/-inputs.tf`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/aws/cluster.tf` & `numerai-cli-0.3.5/numerai/terraform/aws/cluster.tf`

 * *Files 10% similar despite different names*

```diff
@@ -12,32 +12,32 @@
   requires_compatibilities = ["FARGATE"]
   cpu                      = each.value.cpu
   memory                   = each.value.memory
   execution_role_arn       = aws_iam_role.ecsTaskExecutionRole.arn
 
   container_definitions = jsonencode([
     {
-      cpu: parseint(each.value.cpu, 10),
-      image: aws_ecr_repository.node[each.key].repository_url,
-      memory: parseint(each.value.memory, 10),
-      name: each.key,
-      networkMode: "awsvpc",
-      portMappings: [
+      cpu : parseint(each.value.cpu, 10),
+      image : aws_ecr_repository.node[each.key].repository_url,
+      memory : parseint(each.value.memory, 10),
+      name : each.key,
+      networkMode : "awsvpc",
+      portMappings : [
         {
-          containerPort: var.node_container_port,
-          hostPort: var.node_container_port
+          containerPort : var.node_container_port,
+          hostPort : var.node_container_port
         }
       ],
-      logConfiguration: {
-          "logDriver": "awslogs",
-          "options": {
-              "awslogs-group": aws_cloudwatch_log_group.ecs[each.key].name,
-              "awslogs-region": var.aws_region,
-              "awslogs-stream-prefix": "ecs"
-          }
+      logConfiguration : {
+        "logDriver" : "awslogs",
+        "options" : {
+          "awslogs-group" : aws_cloudwatch_log_group.ecs[each.key].name,
+          "awslogs-region" : var.aws_region,
+          "awslogs-stream-prefix" : "ecs"
+        }
       }
     }
   ])
 }
 
 
 ### Cloudwatch
@@ -47,30 +47,30 @@
   name              = "/fargate/service/${each.key}"
   retention_in_days = "14"
 }
 
 
 ### ECR
 resource "aws_ecr_repository" "node" {
-  for_each = { for name, config in var.nodes : name => config }
-
-  name = each.key
+  for_each     = { for name, config in var.nodes : name => config }
+  force_delete = true
+  name         = each.key
 }
 
 
 ### IAM
 resource "aws_iam_role" "ecsTaskExecutionRole" {
-  name               = "${local.node_prefix}-ecs"
+  name = "${local.node_prefix}-ecs"
   assume_role_policy = jsonencode({
-    Version: "2012-10-17",
-    Statement: [{
-      Effect: "Allow",
-      Action: "sts:AssumeRole",
-      Principal: {
-        Service: [
+    Version : "2012-10-17",
+    Statement : [{
+      Effect : "Allow",
+      Action : "sts:AssumeRole",
+      Principal : {
+        Service : [
           "ecs-tasks.amazonaws.com"
         ]
       }
     }]
   })
 }
```

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/aws/network.tf` & `numerai-cli-0.3.5/numerai/terraform/aws/network.tf`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/aws/webhook.tf` & `numerai-cli-0.3.5/numerai/terraform/aws/webhook.tf`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/lambda.zip` & `numerai-cli-0.3.5/numerai/terraform/lambda.zip`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai/terraform/layer.zip` & `numerai-cli-0.3.5/numerai/terraform/layer.zip`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/numerai_cli.egg-info/PKG-INFO` & `numerai-cli-0.3.5/numerai_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numerai-cli
-Version: 0.3.4.dev1
+Version: 0.3.5
 Summary: A library for deploying Numer.ai Prediction Nodes.
 Home-page: https://github.com/numerai/numerai-cli
 Author: Numer.ai
 Author-email: contact@numer.ai
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6.0
@@ -12,31 +12,30 @@
 License-File: LICENSE
 
 # numerai-cli
 
 [![CircleCI](https://circleci.com/gh/numerai/numerai-cli.svg?style=svg)](https://circleci.com/gh/numerai/numerai-cli)
 [![PyPI](https://img.shields.io/pypi/v/numerai-cli.svg?color=brightgreen)](https://pypi.org/project/numerai-cli/)
 
-Welcome to Numerai CLI, if you haven't heard of Numerai [see our docs](https://docs.numer.ai/tournament/learn)
-to learn more. Currently, this CLI configures a Numerai Prediction Node in Amazon Web Services 
-(AWS) that you can deploy your models to. This solution is architected to cost less than 
-$5/mo on average, but actual costs may vary. It has been tested and found working on 
-MacOS/OSX, Windows 8/10, and Ubuntu 18/20, but should theoretically work anywhere that
-Docker and Python 3 are available.
+Welcome to the Numerai CLI for the [Numerai Tournament](https://docs.numer.ai/tournament/learn).
+This CLI runs on your local computer to configure a Numerai Prediction Node in the cloud.
+This solution is architected to cost less than $5/mo on average, but actual costs may vary.
+It has been tested and found working on MacOS/OSX, Windows 8/10, and Ubuntu 18/20,
+but should theoretically work anywhere that Docker and Python 3 are available.
 
 If you have any problems, questions, comments, concerns, or general feedback, please refer to the
 [Troubleshooting and Feedback](#troubleshooting-and-feedback) before posting anywhere.
 
 
 ## Contents
 - [Getting Started](#getting-started)
-- [Upgrading to 0.3.0](#upgrading-to-030)
 - [Node Configuration Tutorial](#node-configuration)
 - [List of Commands](#list-of-commands)
 - [Troubleshooting and Feedback](#troubleshooting-and-feedback)
+- [Upgrading to 0.3.0](#upgrading-to-030)
 - [Uninstall](#uninstall)
 
 
 ## Getting Started
 
 1.  Sign up a Numerai Account, get your Numerai API Keys, and your first Model:
     1.  Sign up at https://numer.ai/signup and log in to your new account
@@ -71,61 +70,68 @@
     ```
     pip3 install --upgrade numerai-cli --user
     ```
     NOTES:
     - This command will also work to update to new versions of the package in the future.
     - If you are using python venv then drop the --user option. 
       If you don't know what that is, disregard this note.
-      
-## Upgrading
-Upgrading numerai-cli will always require you to update the package itself using pip:
+  
+
+## Node Configuration Tutorial
+
+If you know you have all the prerequisites and have your AWS and Numerai API Keys at hand,
+you can run these commands on your local computer to get an example node running in minutes:
+
 ```
-pip install --upgrade numerai-cli --user
+numerai setup
+numerai node config --example tournament-python3
+numerai node deploy
+numerai node test
 ```
 
-#### 0.1/0.2 -> 0.3.0
-CLI 0.3.0 uses a new configuration format that is incompatible with versions 0.1 and 0.2,
-but a command to migrate you configuration is provided for you. Run this in the directory
-you ran `numerai setup` from the previous version:
+If you want to use larger instances to generate your predictions first run `numerai list-constants`
+to list the vCPU/mem presets available, then you can configure a node to use one of the presets via:
 ```
-numerai upgrade
+numerai node config -s mem-lg
 ```
 
-#### Beyond
-Some updates will make changes to configuration files used by Numerai CLI. These will
-require you to re-run some commands to upgrade your nodes to the newest versions:
-- `numerai setup` will copy over changes to files in the `$HOME/.numerai` directory
-- `numerai node config` will apply those changes to a node
+Your compute node is now setup and ready to run! 
 
-## Node Configuration Tutorial
+**VERY IMPORTANT**
+These commands have stored configuration files in `$USER_HOME/.numerai/`.
+If you lose this directory without destroying your nodes,
+you will have to manually (and painfully) delete every cloud resource by hand,
+so make sure you backup these files regularly! 
+DO NOT USE THESE COMMANDS FROM A TEMPORARY INSTANCE!!!!
 
-If you know you have all the prerequisites and have your AWS and Numerai API Keys at hand,
-you can run these commands to get an example node running in minutes:
+
+The example node will train and predict in the cloud, but this is inefficient.
+It's usually best to train your model locally (ensuring that the trained model is 
+stored in the same folder as your code) and then deploy the trained model.
+When you make changes to your code or re-train your model, simply deploy and test your node again:
 
 ```
-numerai setup
-numerai node config --example tournament-python3
 numerai node deploy
 numerai node test
 ```
 
-Your compute node is now setup and ready to run. It saves important configuration 
-information in `$USER_HOME/.numerai/nodes.json` including the url for your Node Trigger.
+The `nodes.json` file also includes the url for your Node Trigger.
 This trigger is registered with whichever model you specified during configuration.
 Each trigger will be called Saturday morning right after a new round opens, 
 and if the related job fails it will be triggered again around 24 hours later.
+You can opt into compute for daily tournaments via the website (go to numer.ai/models,
+click the 3 dots next to your model, click "compute", and click the switch to opt in).
 
 NOTES:
 - The default example does _not_ make stake changes; you will still have to do that manually.
   Please refer to the [numerapi docs](https://numerapi.readthedocs.io/en/latest/api/numerapi.html#module-numerapi.numerapi)
   for the methods you must call to do this.
 - You can view resources and logs in the AWS Console (region us-east-1) for your
   [ECS Cluster](https://console.aws.amazon.com/ecs/home?region=us-east-1#/clusters/numerai-submission-ecs-cluster/tasks)
   and [other resources](https://console.aws.amazon.com/cloudwatch/home?region=us-east-1#logsV2:log-groups)
-- If you're getting
 
 NEXT: [read the Prediction Nodes wiki](https://github.com/numerai/numerai-cli/wiki/Prediction-Nodes)
 to learn about Numerai Examples and how to customize Prediction Nodes.
 
 ## List of Commands
 Use the `--help` option on any command or sub-command to get a full description of it:
 ```
@@ -149,28 +155,49 @@
 ## Troubleshooting and Feedback
 Before messaging the Rocketchat channel or creating a Github issue, 
 please read through the following (especially the "Troubleshooting" section in the wiki):
 - [Github Wiki](https://github.com/numerai/numerai-cli/wiki)
 - [Github Issues](https://github.com/numerai/numerai-cli/issues)
 
 If you still cannot find a solution or answer, please join us on the 
-[RocketChat #compute Channel](https://community.numer.ai/channel/compute) 
+[RocketChat #support Channel](https://rocketchat.numer.ai/channel/support) 
 and include the following information with your issue/message:
 
 - The commands you ran that caused the error (even previous commands)
 - Version information from running:
     - `pip3 show numerai-cli`
     - `python -V`
     - `docker -v`
 - System Information from running
     - Mac: `system_profiler SPSoftwareDataType && system_profiler SPHardwareDataType`
     - Linux: `lsb_release -a && uname -a`
     - Windows: `powershell -command "Get-ComputerInfo"`
   
 If you do not include this information, we cannot help you.
+
+
+## Upgrading and Updating
+Upgrading numerai-cli will always require you to update the package itself using pip:
+```
+pip install --upgrade numerai-cli --user
+```
+
+#### 0.1/0.2 -> 0.3.0
+CLI 0.3.0 uses a new configuration format that is incompatible with versions 0.1 and 0.2,
+but a command to migrate you configuration is provided for you. Run this in the directory
+you ran `numerai setup` from the previous version:
+```
+numerai upgrade
+```
+
+#### Beyond
+Some updates will make changes to configuration files used by Numerai CLI. These will
+require you to re-run some commands to upgrade your nodes to the newest versions:
+- `numerai setup` will copy over changes to files in the `$HOME/.numerai` directory
+- `numerai node config` will apply those changes to a node
       
 
 ## Uninstall
 ```
 numerai uninstall
 ```
```

### Comparing `numerai-cli-0.3.4.dev1/numerai_cli.egg-info/SOURCES.txt` & `numerai-cli-0.3.5/numerai_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `numerai-cli-0.3.4.dev1/setup.py` & `numerai-cli-0.3.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='numerai-cli',
-    version='0.3.4.dev01',
+    version='0.3.5',
     description='A library for deploying Numer.ai Prediction Nodes.',
     url='https://github.com/numerai/numerai-cli',
     author='Numer.ai',
     author_email='contact@numer.ai',
     license='MIT',
     packages=['numerai'],
     include_package_data=True,
@@ -25,9 +25,9 @@
         "boto3",
         "numerapi>=2.4.5",
         "colorama",
         "requests",
     ],
     entry_points={
         'console_scripts': ['numerai=numerai:main'],
-    }
+    },
 )
```

