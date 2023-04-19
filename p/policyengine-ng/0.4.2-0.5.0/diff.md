# Comparing `tmp/policyengine-ng-0.4.2.tar.gz` & `tmp/policyengine-ng-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "policyengine-ng-0.4.2.tar", last modified: Sat Mar 25 14:40:04 2023, max compression
+gzip compressed data, was "policyengine-ng-0.5.0.tar", last modified: Wed Apr 19 13:03:08 2023, max compression
```

## Comparing `policyengine-ng-0.4.2.tar` & `policyengine-ng-0.5.0.tar`

### file list

```diff
@@ -1,60 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.075682 policyengine-ng-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-25 14:40:04.075682 policyengine-ng-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/model_api.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/modelled_policies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.067682 policyengine-ng-0.4.2/policyengine_ng/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/parameters/gov/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/parameters/gov/tax_rate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/consolidated_relief_allowance/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/consolidated_relief_allowance/flat.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/consolidated_relief_allowance/percent.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/exempt_threshold.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/main_rates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/parameters/tax/minimum.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/integration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/tests/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/tax/consolidated_relief_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/tax/is_tax_exempt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/tax/main_tax_rates.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/tax/minimum_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/tax/tax.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/tests/tax/taxable_income.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/gross_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/household_benefits.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/household_market_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/household_net_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/household_tax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng/variables/input/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/input/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.075682 policyengine-ng-0.4.2/policyengine_ng/variables/input/household/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/input/household/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/input/household/age.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/input/household/employment_income.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/market_income.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.075682 policyengine-ng-0.4.2/policyengine_ng/variables/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/tax/consolidated_relief_allowance.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/tax/is_tax_exempt.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/tax/main_tax_rates.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/tax/minimum_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/tax/taxable_income.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/policyengine_ng/variables/tax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 14:40:04.071682 policyengine-ng-0.4.2/policyengine_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-25 14:40:03.000000 policyengine-ng-0.4.2/policyengine_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-25 14:40:03.000000 policyengine-ng-0.4.2/policyengine_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 14:40:03.000000 policyengine-ng-0.4.2/policyengine_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-25 14:40:03.000000 policyengine-ng-0.4.2/policyengine_ng.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-25 14:40:03.000000 policyengine-ng-0.4.2/policyengine_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-25 14:40:03.000000 policyengine-ng-0.4.2/policyengine_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 14:40:04.075682 policyengine-ng-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-25 14:39:18.000000 policyengine-ng-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/model_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/modelled_policies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/flat.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/percent.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/exempt_threshold.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/main_rates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/minimum.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/parameters/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/simulation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/parameters/simulation/marginal_tax_rate_adults.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/integration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/tests/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/consolidated_relief_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/is_tax_exempt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/main_tax_rates.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/minimum_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/tests/tax/taxable_income.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/age.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/employment_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/gross_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_benefits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_market_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_net_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/household_tax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/input/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/input/demographic/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/input/demographic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/input/demographic/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/is_adult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/market_income.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/policyengine_ng/variables/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/consolidated_relief_allowance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/is_tax_exempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/main_tax_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/minimum_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax/taxable_income.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/policyengine_ng/variables/tax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:03:08.580114 policyengine-ng-0.5.0/policyengine_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 13:03:08.000000 policyengine-ng-0.5.0/policyengine_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:03:08.584114 policyengine-ng-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-19 13:02:17.000000 policyengine-ng-0.5.0/setup.py
```

### Comparing `policyengine-ng-0.4.2/LICENSE` & `policyengine-ng-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.4.2/PKG-INFO` & `policyengine-ng-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-ng
-Version: 0.4.2
+Version: 0.5.0
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-ng-0.4.2/policyengine_ng/__init__.py` & `policyengine-ng-0.5.0/policyengine_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.4.2/policyengine_ng/entities.py` & `policyengine-ng-0.5.0/policyengine_ng/entities.py`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.4.2/policyengine_ng/parameters/tax/main_rates.yaml` & `policyengine-ng-0.5.0/policyengine_ng/parameters/gov/tax/main_rates.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,8 @@
 description: Nigeria taxes taxable income at these rates.
-# 1. First N300,000 @ 7 per cent [threshold: 0]
-# 2. Next N300,000 @ 11 per cent [threshold: 300_000]
-# 3. Next N500,000 @ 15 per cent [threshold: 600_000]
-# 4. Next N500,000 @ 19 per cent [threshold: 1_100_000]
-# 5. Next N 1, 600,000 @ 21 per cent [threshold: 1_600_000]
-# 6. Above N3, 200,000 @ 24 per cent [threshold: 3_200_000]
 brackets:
   - threshold:
       2011-01-01: 0
     rate:
       2011-01-01: 0.07
   - threshold:
       2011-01-01: 300_000 # "Next N300,000"
```

### Comparing `policyengine-ng-0.4.2/policyengine_ng/tests/tax/is_tax_exempt.yaml` & `policyengine-ng-0.5.0/policyengine_ng/tests/tax/is_tax_exempt.yaml`

 * *Files identical despite different names*

### Comparing `policyengine-ng-0.4.2/policyengine_ng/variables/marginal_tax_rate.py` & `policyengine-ng-0.5.0/policyengine_ng/variables/marginal_tax_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         mtr_values = np.zeros(person.count, dtype=np.float32)
         simulation = person.simulation
         adult_index_values = person("adult_index", period)
         DELTA = 1_000
         mtr_adult_count = parameters(
             period
         ).simulation.marginal_tax_rate_adults
+        print(simulation.input_variables)
         for adult_index in range(1, 1 + mtr_adult_count):
             alt_simulation = simulation.get_branch(
                 f"adult_{adult_index}_pay_rise"
             )
             mask = adult_index_values == adult_index
             for variable in simulation.tax_benefit_system.variables:
                 if variable not in simulation.input_variables:
@@ -36,14 +37,18 @@
             household_net_income_higher_earnings = alt_person.household(
                 "household_net_income", period
             )
             increase = (
                 household_net_income_higher_earnings - household_net_income
             )
             mtr_values += where(mask, 1 - increase / DELTA, 0)
+            print(household_net_income)
+            print(household_net_income_higher_earnings)
+            print(increase)
+            print(mtr_values)
         return mtr_values
 
 
 class adult_index(Variable):
     value_type = int
     entity = Person
     label = "Index of adult in household"
```

### Comparing `policyengine-ng-0.4.2/policyengine_ng/variables/tax/is_tax_exempt.py` & `policyengine-ng-0.5.0/policyengine_ng/variables/tax/is_tax_exempt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     label = "is tax exempt"
     entity = Person
     definition_period = YEAR
     value_type = bool
 
     def formula(person, period, parameters):
         employment_income = person("employment_income", period)
-        p = parameters(period).tax
+        p = parameters(period).gov.tax
         employment_income_at_or_below_threshold = (
             employment_income <= p.exempt_threshold
         )
         gross_income = person("gross_income", period)
         has_non_employment_income = gross_income > employment_income
         return (
             employment_income_at_or_below_threshold
```

### Comparing `policyengine-ng-0.4.2/policyengine_ng.egg-info/PKG-INFO` & `policyengine-ng-0.5.0/policyengine_ng.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: policyengine-ng
-Version: 0.4.2
+Version: 0.5.0
 Summary: Core microsimulation engine enabling country-specific policy models.
 Home-page: https://github.com/policyengine/policyengine-core
 Author: PolicyEngine
 Author-email: hello@policyengine.org
 License: https://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: tax benefit microsimulation framework
 Platform: UNKNOWN
```

### Comparing `policyengine-ng-0.4.2/policyengine_ng.egg-info/SOURCES.txt` & `policyengine-ng-0.5.0/policyengine_ng.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,37 +9,42 @@
 policyengine_ng/modelled_policies.yaml
 policyengine_ng.egg-info/PKG-INFO
 policyengine_ng.egg-info/SOURCES.txt
 policyengine_ng.egg-info/dependency_links.txt
 policyengine_ng.egg-info/entry_points.txt
 policyengine_ng.egg-info/requires.txt
 policyengine_ng.egg-info/top_level.txt
-policyengine_ng/parameters/gov/tax_rate.yaml
-policyengine_ng/parameters/tax/exempt_threshold.yaml
-policyengine_ng/parameters/tax/main_rates.yaml
-policyengine_ng/parameters/tax/minimum.yaml
-policyengine_ng/parameters/tax/consolidated_relief_allowance/flat.yaml
-policyengine_ng/parameters/tax/consolidated_relief_allowance/percent.yaml
+policyengine_ng/parameters/gov/README.md
+policyengine_ng/parameters/gov/tax/README.md
+policyengine_ng/parameters/gov/tax/exempt_threshold.yaml
+policyengine_ng/parameters/gov/tax/main_rates.yaml
+policyengine_ng/parameters/gov/tax/minimum.yaml
+policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/flat.yaml
+policyengine_ng/parameters/gov/tax/consolidated_relief_allowance/percent.yaml
+policyengine_ng/parameters/simulation/README.md
+policyengine_ng/parameters/simulation/marginal_tax_rate_adults.yaml
 policyengine_ng/tests/integration.yaml
 policyengine_ng/tests/tax/consolidated_relief_allowance.yaml
 policyengine_ng/tests/tax/is_tax_exempt.yaml
 policyengine_ng/tests/tax/main_tax_rates.yaml
 policyengine_ng/tests/tax/minimum_tax.yaml
 policyengine_ng/tests/tax/tax.yaml
 policyengine_ng/tests/tax/taxable_income.yaml
+policyengine_ng/variables/age.py
+policyengine_ng/variables/employment_income.py
 policyengine_ng/variables/gross_income.py
 policyengine_ng/variables/household_benefits.py
 policyengine_ng/variables/household_market_income.py
 policyengine_ng/variables/household_net_income.py
 policyengine_ng/variables/household_tax.py
+policyengine_ng/variables/is_adult.py
 policyengine_ng/variables/marginal_tax_rate.py
 policyengine_ng/variables/market_income.py
 policyengine_ng/variables/tax.py
 policyengine_ng/variables/input/README.md
-policyengine_ng/variables/input/household/README.md
-policyengine_ng/variables/input/household/age.py
-policyengine_ng/variables/input/household/employment_income.py
+policyengine_ng/variables/input/demographic/README.md
+policyengine_ng/variables/input/demographic/gender.py
 policyengine_ng/variables/tax/consolidated_relief_allowance.py
 policyengine_ng/variables/tax/is_tax_exempt.py
 policyengine_ng/variables/tax/main_tax_rates.py
 policyengine_ng/variables/tax/minimum_tax.py
 policyengine_ng/variables/tax/taxable_income.py
```

### Comparing `policyengine-ng-0.4.2/setup.py` & `policyengine-ng-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "sphinx>=4.5.0,<5",
     "sphinx-argparse>=0.3.2,<1",
     "sphinx-math-dollar>=1.2.1,<2",
 ]
 
 setup(
     name="policyengine-ng",
-    version="0.4.2",
+    version="0.5.0",
     author="PolicyEngine",
     author_email="hello@policyengine.org",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

