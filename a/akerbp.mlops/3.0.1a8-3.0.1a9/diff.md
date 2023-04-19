# Comparing `tmp/akerbp.mlops-3.0.1a8.tar.gz` & `tmp/akerbp.mlops-3.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-5qlr_ntb/akerbp.mlops-3.0.1a8.tar", last modified: Fri Apr 14 11:53:09 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-cgfw_mfx/akerbp.mlops-3.0.1a9.tar", last modified: Wed Apr 19 11:13:16 2023, max compression
```

## Comparing `akerbp.mlops-3.0.1a8.tar` & `akerbp.mlops-3.0.1a9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.flake8
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.gitattributes
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35941 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1183 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/build.sh
--rw-rw-rw-   0 root         (0) root         (0)     3510 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/increment_package_version.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/install.sh
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/mlops_settings.yaml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/model_artifact/
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_artifact/README.md
--rw-rw-rw-   0 root         (0) root         (0)      531 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_artifact/dummy.joblib
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/model_code/
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_code/model.py
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_code/requirements.model
--rw-rw-rw-   0 root         (0) root         (0)     2850 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/model_code/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/promote_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)     1498 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/remove_dummy_artifacts.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.389257 akerbp.mlops-3.0.1a8/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.389257 akerbp.mlops-3.0.1a8/src/akerbp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/download_function_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/handler.py
--rw-rw-rw-   0 root         (0) root         (0)    38633 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/helpers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.401257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16951 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6474 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/mappings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     6555 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy_prediction_service.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy_training_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21689 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/platforms.py
--rw-rw-rw-   0 root         (0) root         (0)     5062 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22239 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/model_manager.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5919 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3160 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/test_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/training.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.397257 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)    49463 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-14 11:53:09.000000 akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11480 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_data_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_install_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)     1547 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_metadata_validation.py
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 11:53:09.405257 akerbp.mlops-3.0.1a8/test/test_settings/
--rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/installing_reqs_in_venv.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_all_required_fields.yaml
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_petrel_field.yaml
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_no_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_settings/single_model_required_input.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3549 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/test/test_version_increment.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-14 11:52:47.000000 akerbp.mlops-3.0.1a8/upload_dummy_artifacts.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.810010 akerbp.mlops-3.0.1a9/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/.gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-04-19 11:13:16.810010 akerbp.mlops-3.0.1a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35941 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1183 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3510 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/increment_package_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/mlops_settings.yaml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.798010 akerbp.mlops-3.0.1a9/model_artifact/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/model_artifact/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      531 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/model_artifact/dummy.joblib
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.798010 akerbp.mlops-3.0.1a9/model_code/
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/model_code/model.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/model_code/requirements.model
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/model_code/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      338 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/promote_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1498 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/remove_dummy_artifacts.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-19 11:13:16.810010 akerbp.mlops-3.0.1a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.794010 akerbp.mlops-3.0.1a9/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.794010 akerbp.mlops-3.0.1a9/src/akerbp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.802010 akerbp.mlops-3.0.1a9/src/akerbp/mlops/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.802010 akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/download_function_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/handler.py
+-rw-rw-rw-   0 root         (0) root         (0)    38633 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/helpers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.802010 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16951 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6474 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/logger_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/mappings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.806010 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6555 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/deploy_prediction_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/deploy_training_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    21689 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/platforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     5062 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.806010 akerbp.mlops-3.0.1a9/src/akerbp/mlops/model_manager/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/model_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22521 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/model_manager/model_manager.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.806010 akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3160 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/training.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.802010 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)    49463 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-19 11:13:16.000000 akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.806010 akerbp.mlops-3.0.1a9/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11480 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_data_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_install_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)     1547 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_metadata_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 11:13:16.810010 akerbp.mlops-3.0.1a9/test/test_settings/
+-rw-rw-rw-   0 root         (0) root         (0)      721 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/installing_reqs_in_venv.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/multiple_models_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1267 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/multiple_models_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      674 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/single_model_all_required_fields.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/single_model_missing_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/single_model_missing_petrel_field.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      636 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/single_model_no_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_settings/single_model_required_input.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3549 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/test/test_version_increment.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-04-19 11:12:50.000000 akerbp.mlops-3.0.1a9/upload_dummy_artifacts.py
```

### Comparing `akerbp.mlops-3.0.1a8/.flake8` & `akerbp.mlops-3.0.1a9/.flake8`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [flake8]
-ignore = E203, E266, E501, W503, B950, W605, B008, B006, C901
+ignore = E203, E266, E501, W503, B950, W605, B008, B006, C901, B907
 # line length is intentionally set to 88 here because black uses Bugbear
 # See https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html#line-length for more details
 # Also choosing to suppress B950 as black will try and handle line-length as
 # best it can.
 max-line-length = 88
 max-complexity = 18
 select = B,C,E,F,W,T4,B9
```

### Comparing `akerbp.mlops-3.0.1a8/.pre-commit-config.yaml` & `akerbp.mlops-3.0.1a9/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -7,16 +7,16 @@
       - id: check-yaml
         args: [--allow-multiple-documents]
       - id: check-added-large-files
   - repo: https://github.com/psf/black
     rev: 22.3.0
     hooks:
       - id: black
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: "3.9.2"
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v2.0.0
     hooks:
       - id: flake8
         additional_dependencies: [flake8-bugbear]
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.971
     hooks:
       - id: mypy
```

### Comparing `akerbp.mlops-3.0.1a8/LICENSE` & `akerbp.mlops-3.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/PKG-INFO` & `akerbp.mlops-3.0.1a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.0.1a8
+Version: 3.0.1a9
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.0.1a8/README.md` & `akerbp.mlops-3.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/bitbucket-pipelines.yml` & `akerbp.mlops-3.0.1a9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/build.sh` & `akerbp.mlops-3.0.1a9/build.sh`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/increment_package_version.py` & `akerbp.mlops-3.0.1a9/increment_package_version.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/mlops_settings.yaml` & `akerbp.mlops-3.0.1a9/mlops_settings.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/model_artifact/dummy.joblib` & `akerbp.mlops-3.0.1a9/model_artifact/dummy.joblib`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/model_code/model.py` & `akerbp.mlops-3.0.1a9/model_code/model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/model_code/test_model.py` & `akerbp.mlops-3.0.1a9/model_code/test_model.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/pyproject.toml` & `akerbp.mlops-3.0.1a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/handler.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/handler.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/cdf/helpers.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/cdf/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/config.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/exceptions.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/helpers.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/logger.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/logger_config.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/logger_config.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/core/mappings.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/core/mappings.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/bitbucket-pipelines.yml` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/deploy.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/helpers.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/helpers.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/platforms.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/platforms.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/deployment/setup.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/deployment/setup.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/model_manager/model_manager.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/model_manager/model_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,19 @@
         folder: (Path) path to folder whose content will be uploaded
         metadata: dictionary with metadata (it should not contain a 'version' key)
 
     Returns:
         (dict): model metadata
     """
     specified_version = kwargs.get("version", None)
+    # TODO: when migrating to dev->test->prod release cycle, add check for test as well
+    if env == "prod":
+        raise ValueError(
+            "You are not allowed to upload artifacts directly to prod, use promote_model instead to promote artifacts from test to prod"
+        )
     if specified_version is None:
         file_list = cdf.query_file_versions(
             external_id_prefix=f"{model_name}/{env}/",
             directory_prefix="/mlops",
             uploaded=None,  # count any file
             dataset_id=dataset_id,
         )
@@ -206,15 +211,14 @@
 def download_model_version(
     model_name: str,
     env: str,
     folder: Union[Path, str],
     metadata: Dict = {},
     version: Optional[str] = None,
 ) -> str:
-
     """
     Download a model version to a folder. First the model's external id is found
     (unless provided by the user), and then it is downloaded to the chosen
     folder (creating the folder if necessary).
 
     Args:
         model_name (str): name of the model
```

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/prediction.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/prediction.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/test_service.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/test_service.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp/mlops/services/training.py` & `akerbp.mlops-3.0.1a9/src/akerbp/mlops/services/training.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/PKG-INFO` & `akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akerbp.mlops
-Version: 3.0.1a8
+Version: 3.0.1a9
 Summary: MLOps framework
 Author-email: "Alfonso M. Canterla" <alfonso.canterla@soprasteria.com>
 Maintainer-email: "Christian N. Lehre" <christian.lehre@soprasteria.com>
 License:             Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `akerbp.mlops-3.0.1a8/src/akerbp.mlops.egg-info/SOURCES.txt` & `akerbp.mlops-3.0.1a9/src/akerbp.mlops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_data_validation.py` & `akerbp.mlops-3.0.1a9/test/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_install_requirements.py` & `akerbp.mlops-3.0.1a9/test/test_install_requirements.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_metadata_validation.py` & `akerbp.mlops-3.0.1a9/test/test_metadata_validation.py`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/installing_reqs_in_venv.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/installing_reqs_in_venv.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_all_required_fields.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/multiple_models_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/multiple_models_missing_field.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/multiple_models_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/single_model_all_required_fields.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/single_model_all_required_fields.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_field.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/single_model_missing_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/single_model_missing_petrel_field.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/single_model_missing_petrel_field.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/single_model_no_required_input.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/single_model_no_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_settings/single_model_required_input.yaml` & `akerbp.mlops-3.0.1a9/test/test_settings/single_model_required_input.yaml`

 * *Files identical despite different names*

### Comparing `akerbp.mlops-3.0.1a8/test/test_version_increment.py` & `akerbp.mlops-3.0.1a9/test/test_version_increment.py`

 * *Files identical despite different names*

