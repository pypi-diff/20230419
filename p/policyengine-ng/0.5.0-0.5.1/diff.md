# Comparing `tmp/policyengine-ng-0.5.0.tar.gz` & `tmp/policyengine-ng-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-ng-0.5.0.tar", last modified: Wed Apr 19 13:03:08 2023, max compression
+gzip compressed data, was "policyengine-ng-0.5.1.tar", last modified: Wed Apr 19 13:13:00 2023, max compression
```

## Comparing `policyengine-ng-0.5.0.tar` & `policyengine-ng-0.5.1.tar`

### file list

```diff
@@ -1,66 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/modelled_policies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/flat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/percent.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/exempt_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/main_rates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/minimum.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/parameters/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/simulation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/simulation/marginal_tax_rate_adults.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/integration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/tests/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/consolidated_relief_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/is_tax_exempt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/main_tax_rates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/minimum_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/taxable_income.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/age.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/employment_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/gross_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_benefits.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_market_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_net_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/input/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/input/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/input/demographic/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/input/demographic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/input/demographic/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/is_adult.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/market_income.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/consolidated_relief_allowance.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/is_tax_exempt.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/main_tax_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/minimum_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/taxable_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/setup.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.650379 policyengine-ng-0.5.1/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.629313 policyengine-ng-0.5.1/.github/
+-rw-r--r--   0 nikhil     (501) staff       (20)      189 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 nikhil     (501) staff       (20)      676 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 nikhil     (501) staff       (20)      267 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/changelog_template.md
+-rwxr-xr-x   0 nikhil     (501) staff       (20)      222 2023-02-11 13:17:10.000000 policyengine-ng-0.5.1/.github/get-changelog-diff.sh
+-rwxr-xr-x   0 nikhil     (501) staff       (20)      647 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/has-functional-changes.sh
+-rwxr-xr-x   0 nikhil     (501) staff       (20)     1013 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/is-version-number-acceptable.sh
+-rwxr-xr-x   0 nikhil     (501) staff       (20)      115 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/publish-git-tag.sh
+-rw-r--r--   0 nikhil     (501) staff       (20)      770 2023-04-19 13:12:12.000000 policyengine-ng-0.5.1/.github/update_api.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.629581 policyengine-ng-0.5.1/.github/workflows/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1518 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.github/workflows/pr.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)     4100 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/.github/workflows/push.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      135 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.gitignore
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.630121 policyengine-ng-0.5.1/.vscode/
+-rw-r--r--   0 nikhil     (501) staff       (20)      934 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.vscode/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)      496 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.vscode/launch.json
+-rw-r--r--   0 nikhil     (501) staff       (20)     1299 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.vscode/python.code-snippets
+-rw-r--r--   0 nikhil     (501) staff       (20)     1426 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/.vscode/yaml.code-snippets
+-rw-r--r--   0 nikhil     (501) staff       (20)     1761 2023-04-19 13:12:33.000000 policyengine-ng-0.5.1/CHANGELOG.md
+-rw-r--r--   0 nikhil     (501) staff       (20)     1859 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 nikhil     (501) staff       (20)    34523 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/LICENSE
+-rw-r--r--   0 nikhil     (501) staff       (20)       37 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/MANIFEST.in
+-rw-r--r--   0 nikhil     (501) staff       (20)      657 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/Makefile
+-rw-r--r--   0 nikhil     (501) staff       (20)     1314 2023-04-19 13:13:00.650112 policyengine-ng-0.5.1/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)      414 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)     1020 2023-04-19 13:12:33.000000 policyengine-ng-0.5.1/changelog.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)        0 2023-04-19 13:12:33.000000 policyengine-ng-0.5.1/changelog_entry.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.631294 policyengine-ng-0.5.1/docs/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.631440 policyengine-ng-0.5.1/docs/.streamlit/
+-rw-r--r--   0 nikhil     (501) staff       (20)      141 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/docs/.streamlit/config.toml
+-rw-r--r--   0 nikhil     (501) staff       (20)      573 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/docs/_config.yml
+-rw-r--r--   0 nikhil     (501) staff       (20)       28 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/docs/_toc.yml
+-rw-r--r--   0 nikhil     (501) staff       (20)     4287 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/docs/api_utils.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     1628 2023-02-11 13:17:55.000000 policyengine-ng-0.5.1/docs/demo.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      353 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/docs/intro.md
+-rw-r--r--   0 nikhil     (501) staff       (20)       37 2023-04-19 13:12:33.000000 policyengine-ng-0.5.1/docs/requirements.txt
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.632132 policyengine-ng-0.5.1/policyengine_ng/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1600 2023-03-25 14:11:40.000000 policyengine-ng-0.5.1/policyengine_ng/__init__.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.634535 policyengine-ng-0.5.1/policyengine_ng/__pycache__/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1834 2023-04-19 12:11:52.000000 policyengine-ng-0.5.1/policyengine_ng/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      241 2023-02-11 12:43:21.000000 policyengine-ng-0.5.1/policyengine_ng/__pycache__/constants.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)     2510 2023-02-11 12:43:21.000000 policyengine-ng-0.5.1/policyengine_ng/__pycache__/entities.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      242 2023-02-11 12:43:21.000000 policyengine-ng-0.5.1/policyengine_ng/__pycache__/model_api.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)       62 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/policyengine_ng/constants.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     2482 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/policyengine_ng/entities.py
+-rw-r--r--   0 nikhil     (501) staff       (20)       81 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/policyengine_ng/model_api.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      131 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/modelled_policies.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.625991 policyengine-ng-0.5.1/policyengine_ng/parameters/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.634772 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/
+-rw-r--r--   0 nikhil     (501) staff       (20)       13 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.636955 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/
+-rw-r--r--   0 nikhil     (501) staff       (20)        6 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.637297 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/
+-rw-r--r--   0 nikhil     (501) staff       (20)      383 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/flat.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      384 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/percent.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      365 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/exempt_threshold.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      884 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/main_rates.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      320 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/minimum.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.637592 policyengine-ng-0.5.1/policyengine_ng/parameters/simulation/
+-rw-r--r--   0 nikhil     (501) staff       (20)       12 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/simulation/README.md
+-rw-r--r--   0 nikhil     (501) staff       (20)      188 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/parameters/simulation/marginal_tax_rate_adults.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.637743 policyengine-ng-0.5.1/policyengine_ng/tests/
+-rw-r--r--   0 nikhil     (501) staff       (20)      378 2023-03-24 09:49:05.000000 policyengine-ng-0.5.1/policyengine_ng/tests/integration.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.639021 policyengine-ng-0.5.1/policyengine_ng/tests/tax/
+-rw-r--r--   0 nikhil     (501) staff       (20)      264 2023-02-11 13:17:10.000000 policyengine-ng-0.5.1/policyengine_ng/tests/tax/consolidated_relief_allowance.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      520 2023-02-11 15:17:00.000000 policyengine-ng-0.5.1/policyengine_ng/tests/tax/is_tax_exempt.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      457 2023-02-11 15:17:00.000000 policyengine-ng-0.5.1/policyengine_ng/tests/tax/main_tax_rates.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      118 2023-02-11 15:17:00.000000 policyengine-ng-0.5.1/policyengine_ng/tests/tax/minimum_tax.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      306 2023-02-11 15:17:00.000000 policyengine-ng-0.5.1/policyengine_ng/tests/tax/tax.yaml
+-rw-r--r--   0 nikhil     (501) staff       (20)      332 2023-02-11 15:17:00.000000 policyengine-ng-0.5.1/policyengine_ng/tests/tax/taxable_income.yaml
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.640637 policyengine-ng-0.5.1/policyengine_ng/variables/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.643896 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/
+-rw-r--r--   0 nikhil     (501) staff       (20)      553 2023-04-19 12:50:52.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/age.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      607 2023-04-19 12:14:02.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/employment_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      550 2023-02-11 13:17:21.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/gross_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      528 2023-02-11 13:17:35.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/household_benefits.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      623 2023-02-11 13:17:35.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/household_market_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      629 2023-02-11 13:17:35.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/household_net_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      527 2023-02-11 13:17:35.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/household_tax.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      710 2023-04-19 12:47:05.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/is_adult.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)     1882 2023-04-19 12:38:51.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/marginal_tax_rate.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      604 2023-02-11 12:43:21.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/market_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      756 2023-04-19 12:26:51.000000 policyengine-ng-0.5.1/policyengine_ng/variables/__pycache__/tax.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      244 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/age.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      282 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/employment_income.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      230 2023-02-11 13:17:10.000000 policyengine-ng-0.5.1/policyengine_ng/variables/gross_income.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      202 2023-02-11 13:17:26.000000 policyengine-ng-0.5.1/policyengine_ng/variables/household_benefits.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      292 2023-02-11 13:17:26.000000 policyengine-ng-0.5.1/policyengine_ng/variables/household_market_income.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      301 2023-02-11 13:17:26.000000 policyengine-ng-0.5.1/policyengine_ng/variables/household_net_income.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      211 2023-02-11 13:17:26.000000 policyengine-ng-0.5.1/policyengine_ng/variables/household_tax.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.644178 policyengine-ng-0.5.1/policyengine_ng/variables/input/
+-rw-r--r--   0 nikhil     (501) staff       (20)        7 2023-02-11 12:40:13.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.644888 policyengine-ng-0.5.1/policyengine_ng/variables/input/__pycache__/
+-rw-r--r--   0 nikhil     (501) staff       (20)      533 2023-04-19 12:13:26.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/__pycache__/age.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      613 2023-02-11 12:43:49.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/__pycache__/employment_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      714 2023-04-19 12:19:10.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/__pycache__/gender.cpython-39.pyc
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.646834 policyengine-ng-0.5.1/policyengine_ng/variables/input/demographic/
+-rw-r--r--   0 nikhil     (501) staff       (20)       15 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/demographic/README.md
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.646978 policyengine-ng-0.5.1/policyengine_ng/variables/input/demographic/__pycache__/
+-rw-r--r--   0 nikhil     (501) staff       (20)      726 2023-04-19 12:47:05.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/demographic/__pycache__/gender.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      300 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/input/demographic/gender.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      330 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/is_adult.py
+-rw-r--r--   0 nikhil     (501) staff       (20)     2223 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/marginal_tax_rate.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      283 2023-02-10 01:55:51.000000 policyengine-ng-0.5.1/policyengine_ng/variables/market_income.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.648292 policyengine-ng-0.5.1/policyengine_ng/variables/tax/
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.649647 policyengine-ng-0.5.1/policyengine_ng/variables/tax/__pycache__/
+-rw-r--r--   0 nikhil     (501) staff       (20)      822 2023-04-19 12:21:37.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/__pycache__/consolidated_relief_allowance.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      855 2023-04-19 12:21:37.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/__pycache__/is_tax_exempt.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      756 2023-04-19 12:21:37.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/__pycache__/main_tax_rates.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      731 2023-04-19 12:21:37.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/__pycache__/minimum_tax.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      774 2023-02-11 15:17:09.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/__pycache__/taxable_income.cpython-39.pyc
+-rw-r--r--   0 nikhil     (501) staff       (20)      451 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/consolidated_relief_allowance.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      678 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/is_tax_exempt.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      393 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/main_tax_rates.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      374 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/minimum_tax.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      480 2023-02-11 15:17:00.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax/taxable_income.py
+-rw-r--r--   0 nikhil     (501) staff       (20)      446 2023-04-19 13:12:06.000000 policyengine-ng-0.5.1/policyengine_ng/variables/tax.py
+drwxr-xr-x   0 nikhil     (501) staff       (20)        0 2023-04-19 13:13:00.633017 policyengine-ng-0.5.1/policyengine_ng.egg-info/
+-rw-r--r--   0 nikhil     (501) staff       (20)     1314 2023-04-19 13:13:00.000000 policyengine-ng-0.5.1/policyengine_ng.egg-info/PKG-INFO
+-rw-r--r--   0 nikhil     (501) staff       (20)     4338 2023-04-19 13:13:00.000000 policyengine-ng-0.5.1/policyengine_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)        1 2023-04-19 13:13:00.000000 policyengine-ng-0.5.1/policyengine_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       90 2023-04-19 13:13:00.000000 policyengine-ng-0.5.1/policyengine_ng.egg-info/entry_points.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)      222 2023-04-19 13:13:00.000000 policyengine-ng-0.5.1/policyengine_ng.egg-info/requires.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       16 2023-04-19 13:13:00.000000 policyengine-ng-0.5.1/policyengine_ng.egg-info/top_level.txt
+-rw-r--r--   0 nikhil     (501) staff       (20)       38 2023-04-19 13:13:00.650442 policyengine-ng-0.5.1/setup.cfg
+-rw-r--r--   0 nikhil     (501) staff       (20)     2076 2023-04-19 13:12:33.000000 policyengine-ng-0.5.1/setup.py
```

### Comparing `policyengine-ng-0.5.0/LICENSE` & `policyengine-ng-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/PKG-INFO` & `policyengine-ng-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-ng
-Version: 0.5.0
+Version: 0.5.1
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-ng-0.5.0/policyengine_ng/__init__.py` & `policyengine-ng-0.5.1/policyengine_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/policyengine_ng/entities.py` & `policyengine-ng-0.5.1/policyengine_ng/entities.py`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/main_rates.yaml` & `policyengine-ng-0.5.1/policyengine_ng/parameters/gov/tax/main_rates.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/policyengine_ng/tests/tax/is_tax_exempt.yaml` & `policyengine-ng-0.5.1/policyengine_ng/tests/tax/is_tax_exempt.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/policyengine_ng/variables/marginal_tax_rate.py` & `policyengine-ng-0.5.1/policyengine_ng/variables/marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/policyengine_ng/variables/tax/is_tax_exempt.py` & `policyengine-ng-0.5.1/policyengine_ng/variables/tax/is_tax_exempt.py`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.5.0/policyengine_ng.egg-info/PKG-INFO` & `policyengine-ng-0.5.1/policyengine_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-ng
-Version: 0.5.0
+Version: 0.5.1
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-ng-0.5.0/setup.py` & `policyengine-ng-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "sphinx>=4.5.0,<5",
     "sphinx-argparse>=0.3.2,<1",
     "sphinx-math-dollar>=1.2.1,<2",
 ]
 
 setup(
     name="policyengine-ng",
-    version="0.5.0",
+    version="0.5.1",
     author="PolicyEngine",
     author_email="hello@policyengine.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

