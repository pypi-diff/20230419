# Comparing `tmp/qmflows-0.13.0.tar.gz` & `tmp/qmflows-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmflows-0.13.0.tar", last modified: Wed Apr 19 17:43:05 2023, max compression
+gzip compressed data, was "dist/qmflows-0.2.1.tar", last modified: Thu Nov 16 15:20:19 2017, max compression
```

## Comparing `qmflows-0.13.0.tar` & `qmflows-0.2.1.tar`

### file list

```diff
@@ -1,100 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.229066 qmflows-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-19 17:42:47.000000 qmflows-0.13.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-19 17:42:47.000000 qmflows-0.13.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-19 17:43:05.229066 qmflows-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-19 17:42:47.000000 qmflows-0.13.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 17:42:48.000000 qmflows-0.13.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-19 17:43:05.233066 qmflows-0.13.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2886 2023-04-19 17:42:48.000000 qmflows-0.13.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.213066 qmflows-0.13.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.221066 qmflows-0.13.0/src/qmflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/_init_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/_version_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/backports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.221066 qmflows-0.13.0/src/qmflows/components/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/components/reactivity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21504 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/cp2k_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.221066 qmflows-0.13.0/src/qmflows/data/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.225066 qmflows-0.13.0/src/qmflows/data/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/generic2ADF.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/generic2CP2K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/generic2CP2KMM.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/generic2DFTB.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/generic2ORCA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/generic2PackageWrapper.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/propertiesADF.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/propertiesCP2K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/propertiesCP2KMM.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/propertiesDFTB.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/propertiesORCA.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/data/dictionaries/propertiesPackageWrapper.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.225066 qmflows-0.13.0/src/qmflows/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.225066 qmflows-0.13.0/src/qmflows/examples/Conditional_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/Conditional_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/Conditional_workflows/calc_freqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.225066 qmflows-0.13.0/src/qmflows/examples/Constrained_and_TS_optimizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/Constrained_and_TS_optimizations/H2O2_TS.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/Constrained_and_TS_optimizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/Constrained_and_TS_optimizations/generic_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/Constrained_and_TS_optimizations/partial_geometry_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/examples/_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/fileFunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.229066 qmflows-0.13.0/src/qmflows/packages/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/SCM.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_cp2k.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_cp2k_mm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     9480 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_package_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    30575 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/_serializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      434 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/cp2k_mm.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/cp2k_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/orca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/package_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/packages/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.229066 qmflows-0.13.0/src/qmflows/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/_cp2k_basis_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/_cp2k_orbital_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/_xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/adf.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/adf_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/cp2KParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/cp2k.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/generic_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/orca_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/parsers/xyzParser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.229066 qmflows-0.13.0/src/qmflows/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/templates/_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/templates/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8357 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/type_hints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/warnings_qmflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-19 17:42:48.000000 qmflows-0.13.0/src/qmflows/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:43:05.221066 qmflows-0.13.0/src/qmflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-19 17:43:05.000000 qmflows-0.13.0/src/qmflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-19 17:43:05.000000 qmflows-0.13.0/src/qmflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:43:05.000000 qmflows-0.13.0/src/qmflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-19 17:43:05.000000 qmflows-0.13.0/src/qmflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 17:43:05.000000 qmflows-0.13.0/src/qmflows.egg-info/top_level.txt
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows.egg-info/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        8 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows.egg-info/top_level.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2379 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     7975 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      207 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       57 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows.egg-info/dependency_links.txt
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/examples/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      114 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/examples/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      608 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/common.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/hdf5/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1036 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/hdf5/hdf5_functions.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       57 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/hdf5/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     4918 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/hdf5/quantumHDF5.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1157 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/draw_workflow.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/templates/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      140 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/templates/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1319 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/templates/templates.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/packages/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     7469 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/orca.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    19358 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/packages.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2018 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/dirac.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    14408 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/SCM.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      134 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     9665 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/cp2k_package.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     8172 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/packages/gamess.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      422 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/fileFunctions.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      263 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/__init__.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/data/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/data/templates/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2327 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/templates/singlepoint.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      784 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/templates/ts.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      857 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/templates/freq.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2002 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/templates/geometry.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/__init__.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        3 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/generic2gamess.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1715 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/propertiesADF.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1681 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/propertiesORCA.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      604 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/propertiesGAMESS.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       29 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      120 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/generic2DFTB.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      528 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/propertiesDIRAC.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       66 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/generic2CP2K.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      100 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/generic2Dirac.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1323 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/generic2ADF.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      164 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/warningsCP2K.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      141 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/generic2ORCA.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      944 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/propertiesDFTB.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      267 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/data/dictionaries/propertiesCP2K.json
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     4035 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/settings.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/components/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     6277 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/components/fde.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       71 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/components/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     6739 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/components/reactivity.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2618 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/components/operations.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/src/qmflows/parsers/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2911 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/parser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2236 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/xyzParser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     3973 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/turbomoleParser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      228 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      941 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/adf_parser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      985 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/dirac_xml_parser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    11463 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/cp2KParser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     3242 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/gamess_parser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2217 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/generic_parsers.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     8541 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/parsers/orca_parser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      191 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/warnings_qmflows.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    27072 2017-11-10 11:20:52.000000 qmflows-0.2.1/src/qmflows/molkit.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2850 2017-11-08 16:58:27.000000 qmflows-0.2.1/src/qmflows/utils.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2017-11-16 15:20:19.000000 qmflows-0.2.1/test/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     5048 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_special_keywords.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      470 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_templates.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1031 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_parser_gamess.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      895 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_parser_turbomole.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1195 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_utils.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      496 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_xyz_parser.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     2033 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_overlay.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      367 2017-11-08 16:58:27.000000 qmflows-0.2.1/test/test_molecule.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     7975 2017-11-16 15:20:19.000000 qmflows-0.2.1/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     5999 2017-11-08 16:58:27.000000 qmflows-0.2.1/README.rst
+-rwxrwxr-x   0 felipe    (1000) felipe    (1000)     1675 2017-11-16 15:17:36.000000 qmflows-0.2.1/setup.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       38 2017-11-16 15:20:19.000000 qmflows-0.2.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `qmflows-0.13.0/PKG-INFO` & `qmflows-0.2.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,144 +1,170 @@
-Metadata-Version: 2.1
-Name: qmflows
-Version: 0.13.0
-Summary: Automation of computations in quantum chemistry
-Home-page: https://github.com/SCM-NV/qmflows
-Author: Felipe Zapata
-Author-email: f.zapata@esciencecenter.nl
-License: LGPLv3
-Keywords: chemistry workflows simulation materials
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Typing :: Typed
-Requires-Python: >=3.6
-Provides-Extra: test
-Provides-Extra: test_no_optional
-Provides-Extra: doc
-License-File: LICENSE.md
-
-
-.. image:: https://github.com/SCM-NV/qmflows/workflows/build%20with%20conda/badge.svg
-   :target: https://github.com/SCM-NV/qmflows/actions
-.. image:: https://codecov.io/gh/SCM-NV/qmflows/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/SCM-NV/qmflows
-.. image:: https://readthedocs.org/projects/qmflows/badge/?version=latest
-   :target: https://qmflows.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3274284.svg
-   :target: https://doi.org/10.5281/zenodo.3274284
-.. image:: https://badge.fury.io/py/qmflows.svg
-   :target: https://badge.fury.io/py/qmflows
-.. image:: qmflows.png
+
+.. image:: https://img.shields.io/github/license/SCM-NV/qmflows.svg?maxAge=2592000
+   :target: https://github.com/SCM-NV/qmflows/blob/master/LICENSE.md
+.. image:: https://travis-ci.org/SCM-NV/qmflows.svg?branch=master
+   :target: https://travis-ci.org/SCM-NV/qmflows 
+.. image:: https://img.shields.io/badge/python-3.5-blue.svg
+.. image:: https://api.codacy.com/project/badge/Grade/7e95b6d4d873458daf0de5e4b3110885
+   :target: https://www.codacy.com/app/tifonzafel/qmflows?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=SCM-NV/qmflows&amp;utm_campaign=Badge_Grade	   
+.. image:: https://api.codacy.com/project/badge/Coverage/7e95b6d4d873458daf0de5e4b3110885
+   :target: https://www.codacy.com/app/tifonzafel/qmflows?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=SCM-NV/qmflows&amp;utm_campaign=Badge_Coverage	   
 
 QMFlows
 #######
-See documentation_ for tutorials and documentation.
+See http://scm-nv.github.io/qmflows/ for tutorials and documentation.
 
 Motivation
 ==========
 Research on modern computational quantum chemistry relies on a set of computational
-tools to carry out calculations. The complexity of the calculations usually requires
-intercommunication between the aforementioned tools, such communication is usually done
-through shell scripts that try to automate input/output actions like: launching
+tools to carry out calculations. The complexity of the calculations usually requires 
+intercommunication between the aforementioned tools, such communication is usually done 
+through shell scripts that try to automate input/output actions like: launching 
 the computations in a cluster, reading the resulting output and feeding the relevant
 numerical result to another program. Such scripts are difficult to maintain and extend,
 requiring a significant programming expertise to work with them. Being then desirable a
 set of automatic and extensible tools that allows to perform complex simulations in
 heterogeneous hardware platforms.
 
 This library tackles the construction and efficient execution of computational chemistry workflows.
 This allows computational chemists to use the emerging massively parallel compute environments in
 an easy manner and focus on interpretation of scientific data rather than on tedious job submission
-procedures and manual data processing.
+procedures and manual data processing. 
 
 Description
 ===========
-This library consists of a set of modules written in Python3 to
+This library consists of a set of modules written in Python 3.5 to
 automate the following tasks:
 
  1. Input generation.
  2. Handle tasks dependencies (Noodles_).
  3. Advanced molecular manipulation capabilities with (rdkit_).
- 4. Jobs failure detection and recovery.
- 5. Numerical data storage (h5py_).
+ 4. Numerical data storage and manipulation (HDF5_).
+ 5. Jobs failure detection and recovery.
+ 6. Distribution in heterogeneous hardware platforms.    
 
 Tutorial and Examples
 ---------------------
 A tutorial written as a jupyter-notebook_ is available from: tutorial-qmflows_. You can
 also access direclty more advanced examples_.
-
+    
+ 
 Installation
 ============
 
-- Download miniconda for python3: miniconda_ (also you can install the complete anaconda_ version).
+- Download miniconda for python >= 3.5: miniconda_ (also you can install the complete anaconda_ version).
+
+- Install according to: installConda_. 
 
-- Install according to: installConda_.
+- Reopen terminal (or type ``source ~/.bashrc``).
 
 - Create a new virtual environment using the following commands:
 
-  - ``conda create -n qmflows``
+  - ``conda create -n qmflows python=3.5`` 
 
 - Activate the new virtual environment
-
+  
   - ``source activate qmflows``
 
 To exit the virtual environment type  ``source deactivate``.
-
-
+    
+    
 .. _dependecies:
 
 Dependencies installation
 -------------------------
 
-- Type in your terminal:
+Using the conda environment the following packages should be installed:    
 
-  ``conda activate qmflows``
 
-Using the conda environment the following packages should be installed:
+- install rdkit_ using the following command:
 
+  - ``conda install -y -q --name qmflows -c https://conda.anaconda.org/rdkit rdkit``
 
-- install rdkit_ and h5py_ using conda:
+- install HDF5_ using conda:
 
-  - ``conda install -y -q -c conda-forge rdkit h5py``
-
-  - Note that ``rdkit`` is optional for Python 3.7 and later.
+  - ``conda install -y -q --name qmflows -c anaconda h5py``
+    
 
 .. _installation:
 
 Package installation
 --------------------
-Finally install the package:
+    
+- Type in your terminal,
+
+  ``source activate qmflows``  
+
+- Then
 
-- Install **QMFlows** using pip:
-  - ``pip install qmflows``
+  ``pip install qmflows --upgrade``
+  
+Now you are ready to use *qmflows*. 
+ 
 
-Now you are ready to use *qmflows*.
+Latest stable version
+---------------------
+If you want to install the latest stable version directly from github
+you can use the following command:
 
+``pip install https://github.com/SCM-NV/qmflows/tarball/master#egg=qmflows``
 
   **Notes:**
 
   - Once the libraries and the virtual environment are installed, you only need to type
-    ``conda activate qmflows`` each time that you want to use the software.
+    ``source activate qmflows`` each time that you want to use the software.
+
+
+.. _remote_setup:
+
+Remote/Xenon setup
+------------------
+
+Qmflows supports running jobs over a variety of cluster computing schedulers
+like Slurm and Torque. You program and run your workflows from your laptop, but
+the jobs are run at the remote site. For this to work you need to setup Qmflows
+both locally and remotely. In addition you need to add a Bash script that loads
+the VirtualEnv and starts the Noodles remote worker. This remote worker acts as
+a pilot job, reading job descriptions from input and returning the results. If
+you defined the remote VirtualEnv with the name `qmflows`, the following Bash
+script gives an idea of what you need:
+
+.. code-block:: bash
+
+    #!/bin/bash
+    # comment/uncomment lines that you need
+
+    # If you need ADF, and it is available in a module
+    module load adf/2016.102
+    # or if you installed it yourself
+    # ADFHOME=${HOME}/.local/opt/adf
+    # source ${ADFHOME}/bin/adfrc.sh
+
+    # Point PLAMS to its place
+    export PLAMSDEFAULTS="${HOME}/.local/src/plams/utils/plams_defaults.py"
+
+    # Go to the directory that contains this script
+    cd "$(dirname "${BASH_SOURCE[0]}")"
+
+    # Activate the VirtualEnv
+    source activate qmflows
+
+    # Start the remote worker
+    python -m noodles.worker ${@:2}
+
+    # Bye!
+    source deactivate
+
+
 
 
-.. _documentation: https://qmflows.readthedocs.io/en/latest/
-.. _miniconda: https://docs.conda.io/en/latest/miniconda.html
-.. _anaconda: https://www.anaconda.com/distribution/#download-section
-.. _installConda: https://conda.io/projects/conda/en/latest/user-guide/install/index.html
+.. _miniconda: http://conda.pydata.org/miniconda.html
+.. _anaconda: https://www.continuum.io/downloads
+.. _installConda: http://conda.pydata.org/docs/install/quick.html
 .. _Noodles: http://nlesc.github.io/noodles/
-.. _h5py: http://www.h5py.org/
+.. _HDF5: http://www.h5py.org/ 
 .. _here: https://www.python.org/downloads/
 .. _rdkit: http://www.rdkit.org
+.. _Plams: https://www.scm.com/documentation/Tutorials/Scripting/first_steps_with_plams/
 .. _jupyter-notebook: http://jupyter.org/
 .. _tutorial-qmflows: https://github.com/SCM-NV/qmflows/tree/master/jupyterNotebooks
 .. _examples: https://github.com/SCM-NV/qmflows/tree/master/src/qmflows/examples
-.. _PLAMS: https://github.com/SCM-NV/PLAMS
```

### Comparing `qmflows-0.13.0/setup.py` & `qmflows-0.2.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,50 @@
 #!/usr/bin/env python
 
 from setuptools import setup
-import os
 
-version_file = os.path.abspath(os.path.join(
-    os.path.dirname(__file__),
-    'src',
-    'qmflows',
-    '_version.py',
-))
-version: "dict[str, str]" = {}
-with open(version_file, 'r', encoding='utf8') as f:
-    exec(f.read(), version)
 
 def readme():
-    with open('README.rst', 'r', encoding='utf8') as f:
+    with open('README.rst') as f:
         return f.read()
 
-docs_require = [
-    'sphinx>=2.1,!=3.1.1',
-    'sphinx-autodoc-typehints',
-    'sphinx_rtd_theme',
-    'bleach<5; python_version<"3.7"',
-    'nbsphinx',
-    'jupyter',
-    'pandoc',
-]
-
-tests_no_optional_require = [
-    'assertionlib>=3.1.0',
-    'pytest>=5.4',
-    'pytest-cov',
-    'pytest-mock',
-    'typing_extensions'
-]
-
-tests_require = tests_no_optional_require.copy()
-tests_require += docs_require
-tests_require += [
-    'rdkit>=2018.03.1; python_version>="3.7"',
-    'rdkit-pypi>=2018.03.1; python_version=="3.6"',
-]
 
 setup(
     name='qmflows',
-    version=version['__version__'],
+    version='0.2.1',
     description='Automation of computations in quantum chemistry',
-    license='LGPLv3',
+    license='Apache 2.0',
     url='https://github.com/SCM-NV/qmflows',
-    author='Felipe Zapata',
+    author='felipe zapata',
     author_email='f.zapata@esciencecenter.nl',
     keywords='chemistry workflows simulation materials',
     long_description=readme(),
     package_dir={'': 'src'},
-    packages=["qmflows",
-              "qmflows.components",
+    packages=["qmflows", "qmflows.components",
               "qmflows.data",
               "qmflows.data.dictionaries",
               "qmflows.examples",
-              "qmflows.examples.Conditional_workflows",
-              "qmflows.examples.Constrained_and_TS_optimizations",
-              "qmflows.packages",
-              "qmflows.parsers",
+              "qmflows.hdf5",
+              "qmflows.packages", "qmflows.parsers",
               "qmflows.templates"],
     package_data={
-        "qmflows": ['data/dictionaries/*yaml',
-                    'py.typed']
+        "qmflows": ['data/templates/*json', 'data/dictionaries/*json']
     },
-    python_requires='>=3.6',
     classifiers=[
-        'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Intended Audience :: Science/Research',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.5',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
-        'Topic :: Scientific/Engineering :: Chemistry',
-        'Typing :: Typed',
-    ],
-    install_requires=[
-        'more-itertools',
-        'h5py',
-        'numpy',
-        'pandas',
-        'noodles>=0.3.3',
-        'plams>=1.5.1',
-        'pyparsing!=3.0.0,<3.1.0',
-        'pyyaml>=5.1',
-        'filelock',
-        'packaging>=1.16.8',
+        'Topic :: Scientific/Engineering :: Chemistry'
     ],
+    install_requires=['h5py', 'numpy', 'noodles', 'plams>=1.1.1',
+                      'pymonad', 'pyparsing', 'six', 'tinydb',
+                      'noodles[prov, xenon, numpy]', 'pyxenon',
+                      'filelock', 'msgpack-python',
+                      'sphinx_rtd_theme'],
     extras_require={
-        'test': tests_require,
-        'test_no_optional': tests_no_optional_require,
-        'doc': docs_require,
-    }
+        'test': ['nose', 'coverage', 'nbsphinx'],
+        'doc': ['sphinx', 'sphinx_rtd_theme', 'nbsphinx']
+    },
+    dependency_links=[
+        "https://github.com/SCM-NV/plams/tarball/master#egg=plams"]
 )
```

### Comparing `qmflows-0.13.0/src/qmflows/packages/_cp2k.py` & `qmflows-0.2.1/src/qmflows/packages/cp2k_package.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,264 +1,255 @@
-"""CP2K input/output handling."""
+__all__ = ['cp2k']
 
-import os
-from os.path import join
-from typing import Any, Dict, Iterable, ClassVar, Type, TYPE_CHECKING
-from warnings import warn
-
-import numpy as np
+from qmflows.data.dictionaries.warningsCP2K import cp2k_warnings
+from qmflows.packages.packages import (
+    Package, package_properties, parse_output_warnings, Result)
+from qmflows.parsers.cp2KParser import parse_cp2k_warnings
+from qmflows.settings import Settings
 from scm import plams
+from warnings import warn
 
-from ._packages import Package, Result, parse_output_warnings, load_properties
-from ..parsers.cp2k import parse_cp2k_warnings
-from .._settings import Settings
-from ..warnings_qmflows import cp2k_warnings, Key_Warning
-from ..type_hints import Final, _Settings, Generic2Special
-from ..common import CP2KInfoMO
-
-if TYPE_CHECKING:
-    from numpy.typing import NDArray
-    from numpy import float64 as f8
-
-__all__ = ['CP2K_Result', 'CP2K', 'cp2k']
-
-
-def _write_cell_angles(s: Settings, key: str, value: list, mol: plams.Molecule) -> None:
-    """Write the Angles for the cell.
-
-    The angles of the cell is a 3-dimensional list.
-    &SUBSYS
-        &CELL
-        ABC [angstrom] 5.958 7.596 15.610
-        ALPHA_BETA_GAMMA 81.250 86.560 89.800
-        &END CELL
-
-    """
-    if value is not None:
-        angles = '{} {} {}'.format(*value)
-        s.specific.cp2k.force_eval.subsys.cell.ALPHA_BETA_GAMMA = angles
-
-
-def _write_cell_parameters(s: Settings, key: str, value: list, mol: plams.Molecule) -> None:
-    """Write the cell parameters.
-
-    The cell parameter can be a list of lists containing the ABC parameter.
-
-    For example: ::
-
-    &SUBSYS
-        &CELL
-        A  16.11886919    0.07814137      -0.697284243
-        B  -0.215317662   4.389405268     1.408951791
-        C  -0.216126961   1.732808365     9.748961085
-        PERIODIC XYZ
-        &END
-    .....
-
-    The cell parameter can also be a scalar for ABC like ::
-
-    &SUBSYS
-    &CELL
-    ABC [angstrom] 12.74 12.74 12.74
-    PERIODIC NONE
-    &END CELL
-
-    """
-    def fun(xs: Iterable[Any]) -> str:
-        return '{:} {:} {:}'.format(*xs)
-
-    ar = np.asarray(value, dtype=np.float64)
-    if ar.ndim == 0:
-        abc = f' [angstrom] {fun(np.repeat(ar, 3))}'
-        s.specific.cp2k.force_eval.subsys.cell.ABC = abc
-    elif ar.ndim == 1:
-        abc = f' [angstrom] {fun(ar)}'
-        s.specific.cp2k.force_eval.subsys.cell.ABC = abc
-    elif ar.ndim == 2:
-        a, b, c = ar
-        s.specific.cp2k.force_eval.subsys.cell.A = fun(a)
-        s.specific.cp2k.force_eval.subsys.cell.B = fun(b)
-        s.specific.cp2k.force_eval.subsys.cell.C = fun(c)
-    else:
-        raise RuntimeError(
-            f"cell parameter:{value!r}\nformat not recognized")
-
-
-def _write_periodic(s: Settings, key: str, value: list, mol: plams.Molecule) -> None:
-    """Set the keyword for periodic calculations."""
-    s.specific.cp2k.force_eval.subsys.cell.periodic = value
-
-
-def _ignore_keyword(s: Settings, key: str, value: list, mol: plams.Molecule) -> None:
-    pass
-
-
-def _write_basis(s: Settings, key: str, value: list, mol: plams.Molecule) -> None:
-    """Write the basis set for all atoms in ``mol``.
-
-    .. code-block::
-
-        &SUBSYS
-            &KIND  C
-            BASIS_SET  DZVP-MOLOPT-SR-GTH
-            &END
-            &KIND  H
-            BASIS_SET  DZVP-MOLOPT-SR-GTH
-            &END
-    """
-    subsys = s.specific.cp2k.force_eval.subsys
-    symbol_set = {at.symbol for at in mol}
-    for symbol in symbol_set:
-        subsys[f'kind {symbol}'].basis_set = value
-
-
-def _write_potential(s: Settings, key: str, value: list, mol: plams.Molecule) -> None:
-    """Write the pseudopotential set for all atoms in ``mol``.
-
-    .. code-block::
-
-        &SUBSYS
-            &KIND  C
-            POTENTIAL  GTH-PBE
-            &END
-            &KIND  H
-            POTENTIAL  GTH-PBE
-            &END
-    """
-    subsys = s.specific.cp2k.force_eval.subsys
-    symbol_set = {at.symbol for at in mol}
-    for symbol in symbol_set:
-        subsys[f'kind {symbol}'].potential = value
-
-
-class CP2K_Result(Result):
-    """Class providing access to CP2K result."""
-
-    prop_mapping: ClassVar[_Settings] = load_properties('CP2K', prefix='properties')
-
-    # Attributes accessed via `__getattr__`
-    energy: "None | float"
-    frequencies: "None | NDArray[f8]"
-    geometry: "None | plams.Molecule"
-    enthalpy: "None | float"
-    free_energy: "None | float"
-    orbitals: "None | CP2KInfoMO | tuple[CP2KInfoMO, CP2KInfoMO]"
-    forces: "None | NDArray[f8]"
-    coordinates: "None | NDArray[f8]"
-    temperature: "None | NDArray[f8]"
-    volume: "None | NDArray[f8]"
-    lattice: "None | NDArray[f8]"
-    pressure: "None | NDArray[f8]"
-
-    @property
-    def molecule(self) -> "None | plams.Molecule":
-        """Return the current geometry.
 
-        If the job is an optimization, try to read the ` *-pos-1.xyz` file.
-        Otherwise return the input molecule.
-        """
-        try:
-            return self.get_property('geometry')
-        except FileNotFoundError:
-            return self._molecule
+# ====================================<>=======================================
+charge_dict = {
+    'H': 1, 'He': 2, 'Li': 3, 'Be': 4, 'B': 3, 'C': 4, 'N': 5, 'O': 6, 'F': 7,
+    'Ne': 8, 'Na': 9, 'Mg': 10, 'Al': 3, 'Si': 4, 'P': 5, 'S': 6, 'Cl': 7,
+    'Ar': 8, 'K': 9, 'Ca': 10, 'Sc': 11, 'Ti': 12, 'V': 13, 'Cr': 14, 'Mn': 15,
+    'Fe': 16, 'Co': 17, 'Ni': 18, 'Cu': 11, 'Zn': 12, 'Ga': 13, 'Ge': 4, 'As': 5,
+    'Se': 6, 'Br': 7, 'Kr': 8, 'Rb': 9, 'Sr': 10, 'Y': 11, 'Zr': 12, 'Nb': 13,
+    'Mo': 14, 'Tc': 15, 'Ru': 16, 'Rh': 17, 'Pd': 18, 'Ag': 11, 'Cd': 12,
+    'In': 13, 'Sn': 4, 'Sb': 5, 'Te': 6, 'I': 7, 'Xe': 8, 'Cs': 9, 'Ba': 10,
+    'Hf': 12, 'Ta': 13, 'W': 14, 'Re': 15, 'Os': 16, 'Ir': 17, 'Pt': 18,
+    'Au': 11, 'Hg': 12, 'Tl': 13, 'Pb': 4, 'Bi': 5, 'Po': 6, 'At': 7, 'Rn': 8}
+# ======================================<>====================================
+__all__ = ['cp2k']
 
 
 class CP2K(Package):
-    """A Package subclass for running `CP2K Jobs <https://www.cp2k.org/>`_.
-
+    """
+    This class setup the requirement to run a CP2K Job <https://www.cp2k.org/>.
     It uses plams together with the templates to generate the stucture input
     and also uses Plams to invoke the binary CP2K code.
     This class is not intended to be called directly by the user, instead the
-    :data:`cp2k` function should be called.
-
+    **cp2k** function should be called.
     """
-
-    generic_mapping: ClassVar[_Settings] = load_properties('CP2K', prefix='generic2')
-    result_type: ClassVar[Type[CP2K_Result]] = CP2K_Result
-
-    def __init__(self, pkg_name: str = "cp2k") -> None:
-        super().__init__(pkg_name)
-
-    @classmethod
-    def run_job(cls, settings: Settings, mol: plams.Molecule,
-                job_name: str = 'cp2k_job',
-                work_dir: "None | str | os.PathLike[str]" = None,
-                validate_output: bool = True,
-                **kwargs: Any) -> CP2K_Result:
-        """Call the Cp2K binary using plams interface.
+    def __init__(self):
+        super(CP2K, self).__init__("cp2k")
+        self.generic_dict_file = 'generic2CP2K.json'
+
+    def prerun(self):
+        pass
+
+    @staticmethod
+    def run_job(settings, mol, job_name='cp2k_job',
+                work_dir=None, terminate_job_in_case_of_warnings=None, **kwargs):
+        """
+        Call the Cp2K binary using plams interface.
 
         :param settings: Job Settings.
         :type settings: :class:`~qmflows.Settings`
         :param mol: molecular Geometry
         :type mol: plams Molecule
-        :param hdf5_file: Path to the HDF5 file that contains the numerical results.
+        :param hdf5_file: Path to the HDF5 file that contains the
+        numerical results.
         :type hdf5_file: String
         :param input_file_name: Optional name for the input.
         :type input_file_name: String
         :param out_file_name: Optional name for the output.
         :type out_file_name: String
         :param store_in_hdf5: wether to store the output arrays in HDF5 format.
         :type store_in_hdf5: Bool
-
         """
         # Yet another work directory
 
         # Input modifications
         cp2k_settings = Settings()
         cp2k_settings.input = settings.specific.cp2k
-        cp2k_settings.executable = settings.get("executable", "cp2k.ssmp")
+
+        # Add molecular coordinates
+        m = format_coord_xyz(mol) + '{:>8}'.format('&END')
+        cp2k_settings.input.force_eval.subsys['&COORD'] = m
 
         # Create a Plams job
-        job = plams.interfaces.thirdparty.cp2k.Cp2kJob(
-            name=job_name, settings=cp2k_settings, molecule=mol)
+        job = plams.interfaces.cp2k.Cp2kJob(name=job_name,
+                                            settings=cp2k_settings,
+                                            molecule=mol)
         r = job.run()
 
         work_dir = work_dir if work_dir is not None else job.path
 
-        if validate_output:
-            warnings = parse_output_warnings(
-                job_name, r.job.path, parse_cp2k_warnings, cp2k_warnings
-            )
-        else:
-            warnings = None
+        warnings = parse_output_warnings(job_name, r.job.path,
+                                         parse_cp2k_warnings, cp2k_warnings)
 
-        # Absolute path to the .dill file
-        dill_path = join(job.path, f'{job.name}.dill')
+        result = CP2K_Result(cp2k_settings, mol, job_name, r.job.path,
+                             work_dir, status=job.status, warnings=warnings)
 
-        result = cls.result_type(cp2k_settings, mol, job_name, dill_path=dill_path,
-                                 plams_dir=r.job.path, work_dir=work_dir,
-                                 status=job.status, warnings=warnings)
         return result
 
-    #: A :class:`dict` mapping special keywords to the appropiate function.
-    SPECIAL_FUNCS: ClassVar[Dict[str, Generic2Special]] = {
-        'cell_parameters': _write_cell_parameters,
-        'cell_angles': _write_cell_angles,
-        'periodic': _write_periodic,
-        'executable': _ignore_keyword,
-        'basis': _write_basis,
-        'potential': _write_potential,
-    }
+    def postrun(self):
+        pass
 
-    @classmethod
-    def handle_special_keywords(cls, settings: Settings, key: str, value: Any, mol: plams.Molecule) -> None:
-        """Create the settings input for complex cp2k keys.
+    @staticmethod
+    def handle_special_keywords(settings, key, value, mol):
+        """
+        Create the settings input for complex cp2k keys
 
         :param settings: Job Settings.
         :type settings: :class:`~qmflows.Settings`
         :param key: Special key declared in ``settings``.
         :param value: Value store in ``settings``.
         :param mol: molecular Geometry
         :type mol: plams Molecule
-
         """
+
+        def write_cell_angles(s, value, mol, key):
+            """
+            The angles of the cell is a 3-dimensional list ::
+
+            &SUBSYS
+              &CELL
+                ABC [angstrom] 5.958 7.596 15.610
+                ALPHA_BETA_GAMMA 81.250 86.560 89.800
+              &END CELL
+            """
+            angles = '{} {} {}'.format(*value)
+            s.specific.cp2k.force_eval.subsys.cell.alpha_beta_gamma = angles
+
+            return s
+
+        def write_cell_parameters(s, value, mol, key):
+            """
+            The cell parameter can be a list of lists containing the
+            ABC parameter like ::
+
+            &SUBSYS
+               &CELL
+               A  16.11886919    0.07814137      -0.697284243
+               B  -0.215317662   4.389405268     1.408951791
+               C  -0.216126961   1.732808365     9.748961085
+               PERIODIC XYZ
+               &END
+            .....
+
+            The cell parameter can also be a scalar for ABC like ::
+
+            &SUBSYS
+            &CELL
+            ABC [angstrom] 12.74 12.74 12.74
+            PERIODIC NONE
+            &END CELL
+            """
+            if not isinstance(value, list):
+                abc = [value] * 3
+                abc_cell = ' [angstrom] {} {} {}'.format(*abc)
+                s.specific.cp2k.force_eval.subsys.cell.ABC = abc_cell
+            elif isinstance(value, list):
+                abc = ' [angstrom] {} {} {}'.format(*value)
+                s.specific.cp2k.force_eval.subsys.cell.ABC = abc
+            elif isinstance(value[0], list):
+                a, b, c = value  #
+                fun = lambda xs: '{} {} {}'.format(*xs)
+                s.specific.cp2k.force_eval.subsys.cell.A = fun(a)
+                s.specific.cp2k.force_eval.subsys.cell.B = fun(b)
+                s.specific.cp2k.force_eval.subsys.cell.C = fun(c)
+            else:
+                msg = "cell parameter:{}\nformat not recognized"
+                RuntimeError(msg)
+
+            return s
+
+        def expand_basis_set(s, prefix, mol, key):
+            """
+            CP2k has a sspecial format for the basis set, For more
+            information have a look at
+            `basis <https://www.cp2k.org/basis_sets?s[]=basis>`.
+            For a Molecule that contains only carbon and oxygen atoms,
+            the basis set declaration is given by,
+            >>> &FORCE_EVAL
+                    .......
+                    &SUBSYS
+                        &KIND  C
+                            BASIS_SET  DZVP-MOLOPT-SR-GTH-q4
+                            POTENTIAL  GTH-PBE-q4
+                        &END C
+                        &KIND  H
+                            BASIS_SET  DZVP-MOLOPT-SR-GTH-q1
+                            POTENTIAL  GTH-PBE-q1
+                        &END H
+                    &END SUBSYS
+                & END FORCE_EVALXS
+            Where DZVP-MOLOPT-SR-GTH is the name of the basis and q4, q1
+            correspond to the charge associated with that atom
+            (e.g. 4 for carbon, 1 for hydrogen).
+            """
+
+            def symbols2charge(s):
+                q = charge_dict[s]
+                return 'q{}'.format(q)
+
+            symbols = set([at.symbol for at in mol.atoms])
+            qs = list(map(symbols2charge, symbols))
+            for symb, q in zip(symbols, qs):
+                name = '{}-{}'.format(prefix, q)
+                if key == 'basis':
+                    s.specific.cp2k.force_eval.subsys.kind[symb]["basis_set"] = name
+                elif key == 'potential':
+                    s.specific.cp2k.force_eval.subsys.kind[symb]["potential"] = name
+            return s
+
+        funs = {'basis': expand_basis_set, 'potential': expand_basis_set,
+                'cell_parameters': write_cell_parameters,
+                'cell_angles': write_cell_angles}
+
         # Function that handles the special keyword
-        f = cls.SPECIAL_FUNCS.get(key)
+        f = funs.get(key)
 
         if f is not None:
-            f(settings, key, value, mol)
+            return f(settings, value, mol, key)
         else:
-            warn(f'Generic keyword {key!r} not implemented for package CP2K',
-                 category=Key_Warning)
+            msg = 'Keyword ' + key + ' doesn\'t exist'
+            warn(msg)
+
+
+class CP2K_Result(Result):
+    """
+    Class providing access to CP2K result.
+    """
+    def __init__(self, settings, molecule, job_name, plams_dir, work_dir=None,
+                 properties=package_properties['cp2k'],
+                 status='successful', warnings=None):
+        super().__init__(settings, molecule, job_name, plams_dir,
+                         work_dir=work_dir, properties=properties,
+                         status=status, warnings=warnings)
+
+    @classmethod
+    def from_dict(cls, settings, molecule, job_name, archive, status, warnings):
+        """
+        Create a :class:`~CP2K_Result` instance using the data serialized in
+        a dictionary.
+
+        :param cls:
+        :param settings: Job Settings.
+        :param molecule: molecular Geometry.
+        :param job_name: Name of the job.
+        :param plams_dir: Absolute path to plams output folder
+        :param archive: dictionary containing the paths to the input/output
+        folders.
+        :param path_hdf5: Path to the HDF5 file that contains the numerical
+        results.
+        """
+        plams_dir, work_dir = list(map(archive.get, ["plams_dir", "work_dir"]))
+        return CP2K_Result(settings, molecule, job_name, plams_dir.path,
+                           work_dir=work_dir,
+                           properties=package_properties['cp2k'],
+                           status=status, warnings=warnings)
+
+
+def format_coord_xyz(mol):
+    """
+    """
+    xs  = ''.join('{}  {: 12.8e}  {: 12.8e}  {: 12.8e}\n'.format(at.symbol, *at.coords)
+                  for at in mol)
 
+    return '\n' + xs
 
-cp2k: Final[CP2K] = CP2K()
+cp2k = CP2K()
```

### Comparing `qmflows-0.13.0/src/qmflows/packages/_orca.py` & `qmflows-0.2.1/src/qmflows/packages/gamess.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,221 +1,210 @@
-"""Orca input/output bookkeeping."""
+__all__ = ['gamess']
 
-import os
-from os.path import join
-from warnings import warn
-from typing import Any, Union, Optional, ClassVar, List, Type, TYPE_CHECKING
-
-import numpy as np
+from qmflows.packages.packages import (Package, package_properties, Result)
+from qmflows.settings import Settings
 from scm import plams
+from warnings import warn
 
-from ._packages import Package, Result, load_properties
-from ..parsers.orca import parse_molecule
-from .._settings import Settings
-from ..type_hints import Final, _Settings
-from ..utils import get_tmpfile_name
-from ..warnings_qmflows import Key_Warning
-from ..common import InfoMO
-
-if TYPE_CHECKING:
-    from numpy.typing import NDArray
-    from numpy import float64 as f8
-
-__all__ = ['ORCA_Result', 'ORCA', 'orca']
-
-# ============================= Orca ==========================================
-
-
-class ORCA_Result(Result):
-    """Class providing access to PLAMS OrcaJob results."""
-
-    prop_mapping: ClassVar[_Settings] = load_properties('ORCA', prefix='properties')
-
-    # Attributes accessed via `__getattr__`
-    charges: "None | list[float]"
-    dipole: "None | list[float]"
-    energy: "None | float"
-    enthalpy: "None | float"
-    free_energy: "None | float"
-    frequencies: "None | NDArray[f8]"
-    hessian: "None | NDArray[f8]"
-    normal_modes: "None | NDArray[f8]"
-    optcycles: "None | int"
-    orbitals: "None | InfoMO"
-    runtime: "None | float"
-
-    @property
-    def molecule(self) -> Optional[plams.Molecule]:
-        """Retrieve the molecule from the output file."""
-        if self.status in {'crashed', 'failed'}:
-            return None
-
-        plams_dir = self.archive["plams_dir"]
-        if plams_dir is None:
-            return None
-        else:
-            file_name = join(plams_dir, f'{self.job_name}.out')
-            return parse_molecule(file_name, self._molecule)
-
-
-class ORCA(Package):
-    """A class for preparing the input for running a Orca job using both PLAMS and templates.
-
-    It also does the manangement of the input/output files resulting
-    from running Orca and returns a Results object that containing the methods
-    and data required to retrieve the output.
 
+class GAMESS(Package):
     """
+    This class setup the requirement to run a Gamess-US Job
+    <http://www.msg.ameslab.gov/gamess/>.
+    It uses plams together with the templates to generate the stucture input
+    and also uses Plams to invoke the ``rungms`` script.
+    This class is not intended to be called directly by the user, instead the
+    **gamess** function should be called.
+    """
+    def __init__(self):
+        super(GAMESS, self).__init__("gamess")
+        self.generic_dict_file = 'generic2gamess.json'
 
-    generic_mapping: ClassVar[_Settings] = load_properties('ORCA', prefix='generic2')
-    result_type: ClassVar[Type[ORCA_Result]] = ORCA_Result
-
-    def __init__(self, pkg_name: str = "orca") -> None:
-        super().__init__(pkg_name)
-
-    @classmethod
-    def run_job(cls, settings: Settings, mol: plams.Molecule,
-                job_name: str = "ORCAjob",
-                work_dir: "None | str | os.PathLike[str]" = None,
-                validate_output: bool = True,
-                **kwargs: Any) -> ORCA_Result:
-        """Call the ORCA binary using plams interface."""
-        orca_settings = Settings()
-        orca_settings.input = settings.specific.orca
-
-        # Running Orca with Plams
-        job = plams.interfaces.thirdparty.orca.ORCAJob(
-            molecule=mol, settings=orca_settings, name=job_name)
-        result = job.run()
-
-        # Relative job path
-        relative_plams_path = join(*str(result.job.path).split(os.sep)[-2:])
-
-        # Absolute path to the .dill file
-        dill_path = join(job.path, f'{job.name}.dill')
-
-        return cls.result_type(orca_settings, mol, result.job.name, dill_path,
-                               plams_dir=relative_plams_path, status=job.status)
+    def prerun(self):
+        pass
 
     @staticmethod
-    def handle_special_keywords(settings: Settings, key: str,
-                                value: Any, mol: plams.Molecule) -> None:
-        """Translate generic keywords to their corresponding Orca keywords."""
-        def inithess(value: Any) -> Settings:
-            """Generate an seperate file containing the initial Hessian matrix.
-
-            It is used as guess for the computation.
-
-            """
-            # Convert Hessian to numpy array
-            value = value if isinstance(value, np.ndarray) else np.array(value)
-
-            def format_atom(atom: plams.Atom) -> str:
-                symbol, mass, coords = atom.symbol, atom.mass, atom.coords
-                return '{:2s}{:12.4f}{:14.6f}{:14.6f}{:14.6f}\n'.format(symbol, mass, *coords)
-
-            def format_hessian(dim, hess: Union[List[List[float]], np.ndarray]) -> str:
-                """Format numpy array to Orca matrix format."""
-                ret = ''
-                for i in range((dim - 1) // 6 + 1):
-                    n_columns = min(6, dim - 6 * i)
-                    ret += '         '
-                    ret += ' '.join('{:10d}'.format(v + 6 * i)
-                                    for v in range(n_columns))
-                    ret += '\n'
-                    for j in range(dim):
-                        ret += '{:7d}     '.format(j)
-                        ret += ' '.join('{:10.6f}'.format(hess[v + 6 * i][j])
-                                        for v in range(n_columns))
-                        ret += '\n'
-                return ret
-
-            # Check Hessian dimension
-            if value.ndim == 1:
-                dim = int(value.size ** 0.5)
-                hess = np.reshape(value, (dim, dim))
-            else:
-                dim = value.shape[0]
-                hess = value
+    def run_job(settings, mol, job_name='gamess_job', work_dir=None):
+        """
+        Call the Cp2K binary using plams interface.
+
+        :param settings: Job Settings.
+        :type settings: :class:`~qmflows.Settings`
+        :param mol: molecular Geometry
+        :type mol: plams Molecule
+        :param input_file_name: Optional name for the input.
+        :type input_file_name: String
+        :param out_file_name: Optional name for the output.
+        :type out_file_name: String
+        :return: Package.Result
+        """
+        gamess_settings = Settings()
+        gamess_settings.input = settings.specific.gamess
+        job = plams.interfaces.gamess.GamessJob(molecule=mol, name=job_name,
+                                                settings=gamess_settings)
+        r = job.run()
 
-            # Header
-            hess_str = '\n$orca_hessian_file\n\n$hessian\n' + str(dim) + '\n'
-            # Actual Hessian
-            hess_str += format_hessian(dim, hess)
-            # Atoms header
-            hess_str += '\n$atoms\n'
-            # Atoms coordinates
-            hess_str += str(len(mol)) + '\n'
-            hess_str += ''.join(format_atom(atom) for atom in mol.atoms)
-            # The end
-            hess_str += '\n\n$end\n'
-
-            # Store the hessian in the plams_dir
-            hess_path = get_tmpfile_name("ORCA_hessian_")
-            with open(hess_path, "w") as hess_file:
-                hess_file.write(hess_str)
+        # Relative job path
+        relative_plams_path = '/'.join(r.job.path.split('/')[-2:])
 
-            settings.specific.orca.geom.InHess = "read"
-            settings.specific.orca.geom.InHessName = f'{hess_path.as_posix()}'
+        result = Gamess_Result(gamess_settings, mol, r.job.name,
+                               plams_dir=relative_plams_path, work_dir=work_dir,
+                               status=job.status)
 
-            return settings
+        return result
 
-        def constraint(value: Any) -> None:
-            cons = ''
-            if isinstance(value, Settings):
-                for k, v in value.items():
-                    ks = k.split()
-                    atoms = [int(a) - 1 for a in ks[1:]]
-                    if ks[0] == 'dist' and len(ks) == 3:
-                        cons += '{{ B {:d} {:d} {:.2f} C }}'.format(*atoms, v)
-                    elif ks[0] == 'angle' and len(ks) == 4:
-                        cons += '{{ A {:d} {:d} {:d} {:.2f} C }}'.format(
-                            *atoms, v)
-                    elif ks[0] == 'dihed' and len(ks) == 5:
-                        cons += '{{ D {:d} {:d} {:d} {:d} {:.2f} C }}'.format(
-                            *atoms, v)
-                    else:
-                        warn(
-                            f'Invalid constraint key: {k}', category=Key_Warning)
-            settings.specific.orca.geom.Constraints._end = cons
+    def postrun(self):
+        pass
 
-        def freeze(value: List[Union[int, str]]) -> None:
+    @staticmethod
+    def handle_special_keywords(settings, key, value, mol):
+        """
+        Create the settings input for complex gamess-us keys.
+        some keywords provided by the user do not have a straightforward
+        translation to *GAMESS* input and require some hooks that handle the
+        special behaviour of the following keywords:
+
+        * ``freeze``
+        * ``selected_atoms``
+
+        :param settings: Job Settings.
+        :type settings: :class:`~qmflows.Settings`
+        :param key: Special key declared in ``settings``.
+        :param value: Value store in ``settings``.
+        :param mol: molecular Geometry
+        :type mol: plams Molecule
+        """
+        def freeze():
             if not isinstance(value, list):
-                msg = f'selected_atoms {value} is not a list'
+                msg = 'selected_atoms ' + str(value) + ' is not a list'
                 raise RuntimeError(msg)
-            cons = ''
+            sel_coords = []
             if isinstance(value[0], int):
-                for a in value:
-                    cons += '{{ C {:d} C }}'.format(a - 1)
+                for v in value:
+                        a = v - 1
+                        sel_coords += [str(i) for i in range(a * 3 + 1, a * 3 + 4)]
             else:
                 for a in range(len(mol)):
                     if mol[a + 1].symbol in value:
-                        cons += '{{ C {:d} C }}'.format(a)
-            settings.specific.orca.geom.Constraints._end = cons
+                        sel_coords += [str(i) for i in range(a * 3 + 1, a * 3 + 4)]
+            ifreez = Settings()
+            ifreez.statpt = "IFREEZ(1)=" + ",".join(sel_coords)
+            settings.specific.gamess.update(ifreez)
 
-        def selected_atoms(value: List[Union[int, str]]) -> None:
+        def selected_atoms():
             if not isinstance(value, list):
-                raise RuntimeError(f'selected_atoms {value} is not a list')
-            cons = ''
+                msg = 'selected_atoms ' + str(value) + ' is not a list'
+                raise RuntimeError(msg)
+            sel_coords = []
             if isinstance(value[0], int):
                 for a in range(len(mol)):
                     if a + 1 not in value:
-                        cons += '{{ C {:d} C }}'.format(a)
+                        sel_coords += [str(i) for i in range(a * 3 + 1, a * 3 + 4)]
             else:
                 for a in range(len(mol)):
                     if mol[a + 1].symbol not in value:
-                        cons += '{{ C {:d} C }}'.format(a)
-            settings.specific.orca.geom.Constraints._end = cons
+                        sel_coords += [str(i) for i in range(a * 3 + 1, a * 3 + 4)]
+            ifreez = Settings()
+            ifreez.statpt = "IFREEZ(1)=" + ",".join(sel_coords)
+            settings.specific.gamess.update(ifreez)
 
+        def constraint():
+            if isinstance(value, Settings):
+                s = Settings()
+                if len(mol) == 2:
+                    degr = 1
+                    # s['izmat(1)'] = '1,1,2'
+                else:
+                    degr = 3 * len(mol) - 6
+                    s.auto = ".TRUE."
+                    s.dlc = ".TRUE."
+                settings.specific.gamess.contrl.nzvar = degr
+                i = 1
+                for k, v in value.items():
+                    ks = k.split()
+                    # print('--->', ks, type(ks[2]), type(value), v)
+                    if ks[0] == 'dist' and len(ks) == 3:
+                        n = 'ifzmat({:d})'.format(i)
+                        s[n] = "1,{},{}".format(int(ks[1]), int(ks[2]))
+                        n = 'fvalue({:d})'.format(i)
+                        s[n] = v
+                    elif ks[0] == 'angle' and len(ks) == 4:
+                        n = 'ifzmat({:d})'.format(i)
+                        s[n] = "2,{},{},{}".format(int(ks[1]),
+                                                   int(ks[2]),
+                                                   int(ks[3]))
+                        n = 'fvalue({:d})'.format(i)
+                        s[n] = v
+                    elif ks[0] == 'dihed' and len(ks) == 5:
+                        n = 'ifzmat({:d})'.format(i)
+                        s[n] = "3,{},{},{},{}".format(int(ks[1]), int(ks[2]),
+                                                      int(ks[3]), int(ks[4]))
+                        n = 'fvalue({:d})'.format(i)
+                        s[n] = v
+                    else:
+                        warn('Invalid constraint key: ' + k)
+                    i += 1
+                settings.specific.gamess.zmat = s
         # Available translations
-        functions = {'inithess': inithess,
-                     'freeze': freeze,
+        functions = {'freeze': freeze,
                      'selected_atoms': selected_atoms,
                      'constraint': constraint}
         if key in functions:
-            functions[key](value)
+            functions[key]()
         else:
-            warn(f'Generic keyword {key!r} not implemented for package ORCA',
-                 category=Key_Warning)
+            msg = 'Generic keyword "' + key + '" not implemented for package Gamess.'
+            warn(msg)
+
+
+class Gamess_Result(Result):
+    """
+    Class providing access to CP2K result.
+    """
+    def __init__(self, settings, molecule, job_name, plams_dir=None,
+                 work_dir=None, status='done', warnings=None):
+        properties = package_properties['gamess']
+        super().__init__(settings, molecule, job_name, plams_dir,
+                         work_dir=work_dir, properties=properties,
+                         status=status, warnings=warnings)
+
+    @classmethod
+    def from_dict(cls, settings, molecule, job_name, archive, status, warnings):
+        """
+        Create a :class:`~CP2K_Result` instance using the data serialized in
+        a dictionary.
+
+        :param cls:
+        :param settings: Job Settings.
+        :param molecule: molecular Geometry.
+        :param job_name: Name of the job.
+        :param plams_dir: Absolute path to plams output folder
+        :param archive: dictionary containing the paths to the input/output
+        folders.
+        """
+        plams_dir = archive.get("plams_dir").path
+        work_dir = archive.get("work_dir")
+        return Gamess_Result(settings, molecule, job_name,
+                             plams_dir=plams_dir, work_dir=work_dir,
+                             status=status, warnings=warnings)
+
+    def __getattr__(self, prop):
+        """Returns a section of the results.
+        The property is extracted from a  result file, which is recursively
+        search for in the GAMESS settings
+
+        Example:
+        ..
+            Hessian_matrix = result.hessian
+        """
+        result = super().__getattr__(prop)
+        if result is None:
+            msg = """
+            Maybe you need to provided to the gamess
+            function the optional keyword 'work_dir' containing the path
+            to the SCR folder where GAMESS stores the *.dat and other
+            output files"""
+            warn(msg)
+
+        return result
 
 
-orca: Final[ORCA] = ORCA()
+gamess = GAMESS()
```

### Comparing `qmflows-0.13.0/src/qmflows/parsers/_xyz.py` & `qmflows-0.2.1/src/qmflows/parsers/xyzParser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,87 @@
-"""XYZ file format readers."""
-
-__all__ = ['parse_string_xyz', 'readXYZ',
-           'manyXYZ', "string_to_plams_Molecule"]
-
-from typing import List, Iterable
-
-from pyparsing import (Group, LineEnd, OneOrMore, Suppress, Word, alphas,
-                       restOfLine, ParseResults)
-from scm.plams import Atom, Molecule
-
-from .utils import floatNumber, natural
-from ..common import AtomXYZ
-from ..type_hints import PathLike
+__author__ = "Felipe Zapata"
 
+__all__ = ['parse_string_xyz', 'readXYZ', 'manyXYZ', "string_to_plams_Molecule"]
 
+# ===================> Standard libraries and third-party <====================
+from scm.plams import (Atom, Molecule)
+from pyparsing   import (alphas, Group, LineEnd, OneOrMore, restOfLine,
+                         Suppress, Word)
+
+from qmflows.common import AtomXYZ
+from qmflows.parsers.parser import (floatNumber, natural)
+from qmflows.utils import zipWith
 # =============================================================================
 
-header = natural + LineEnd() + restOfLine
+header  = natural + LineEnd() + restOfLine
 
-label = Word(alphas, max=2)
+label   = Word(alphas, max=2)
 
-xyz = floatNumber * 3
+xyz     = floatNumber * 3
 
 atomParser = label.setResultsName("label") + xyz.setResultsName("xyz")
 
 parser_xyz = Suppress(header) + OneOrMore(Group(atomParser))
 
 # ==============================<>====================================
 
 
-def parse_string_xyz(xs: str) -> List[AtomXYZ]:
-    """Read a molecula geometry in XYZ format from a string.
+def parse_string_xyz(xs):
+    """
+    Read a molecula geometry in XYZ format from a string.
 
     :param: xs
     :type:  string
     :return: [AtomXYZ]
     """
     rs = parser_xyz.parseString(xs)
     return createAtoms(rs)
 
 
-def readXYZ(pathXYZ: PathLike) -> List[AtomXYZ]:
-    """Parse molecular geometry in XYZ format from a file.
+def readXYZ(pathXYZ):
+    """
+    Parse molecular geometry in XYZ format from a file.
 
     :param: pathXYZ
     :type:  string
     :return: [AtomXYZ]
     """
     xs = parser_xyz.parseFile(pathXYZ)
     return createAtoms(xs)
 
 
-def manyXYZ(pathXYZ: PathLike) -> List[List[AtomXYZ]]:
-    """Read one or more molecular geometries in XYZ format from a file.
+def manyXYZ(pathXYZ):
+    """
+    Read one or more molecular geometries in XYZ format from a file.
 
     :param: pathXYZ
     :type:  string
     :return: [[AtomXYZ]]
     """
     manyMol = OneOrMore(Group(parser_xyz))
-    xss = manyMol.parseFile(pathXYZ)
+    xss     = manyMol.parseFile(pathXYZ)
     return list(map(createAtoms, xss))
 
 
-def createAtoms(xs: ParseResults) -> List[AtomXYZ]:
-    """Create an AtomXYZ tuple from a string."""
-    ls = (a.label.lower() for a in xs)
-    rs = (tuple(map(float, a.xyz)) for a in xs)
-    return [AtomXYZ(symbol, xyz) for symbol, xyz in zip(ls, rs)]  # type: ignore
+def createAtoms(xs):
+    """
+    Create an AtomXYZ tuple from a string.
+    """
+    ls = [a.label.lower() for a in xs]
+    rs = [list(map(float, a.xyz)) for a in xs]
+    return zipWith(AtomXYZ)(ls)(rs)
 
 
-def tuplesXYZ_to_plams(xs: Iterable[AtomXYZ]) -> Molecule:
-    """Transform a list of namedTuples to a Plams molecule."""
+def tuplesXYZ_to_plams(xs):
+    """ Transform a list of namedTuples to a Plams molecule """
     plams_mol = Molecule()
     for at in xs:
         symb = at.symbol
         cs = at.xyz
         plams_mol.add_atom(Atom(symbol=symb, coords=tuple(cs)))
 
     return plams_mol
 
 
-def string_to_plams_Molecule(xs: str) -> Molecule:
-    """Convert a molecule stored in a string to a plams Molecule."""
-    return tuplesXYZ_to_plams(parse_string_xyz(xs))
+def string_to_plams_Molecule(xs):
+    """Convert a molecule stored in a string to a plams Molecule"""
+    return  tuplesXYZ_to_plams(parse_string_xyz(xs))
```

### Comparing `qmflows-0.13.0/src/qmflows/parsers/orca.py` & `qmflows-0.2.1/src/qmflows/parsers/orca_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,131 +1,140 @@
-"""Read Orca output files."""
+
 __all__ = [
-    'parse_hessian', 'parse_frequencies', 'parse_molecule',
+    'parse_basis_set', 'parse_hessian', 'parse_frequencies', 'parse_molecule',
     'parse_molecular_orbitals', 'parse_molecule_traj', 'parse_normal_modes']
 
-from typing import Sequence, Tuple
-from typing import Optional as Optional_
+from itertools import chain
+from scm.plams import (Atom, Molecule)
+from pyparsing import (alphanums, Group, OneOrMore, Word)
+from .parser import (floatNumber, natural, parse_file, parse_section, skipLine,
+                     skipSupress, string_array_to_molecule, try_search_pattern)
+from qmflows.common import (AtomBasisData, AtomBasisKey, InfoMO)
+from qmflows.utils import chunksOf
+from .xyzParser import manyXYZ
 
 import numpy as np
-from more_itertools import chunked
-from pyparsing import Group, OneOrMore, Word, alphanums
-from scm.plams import Atom, Molecule
-
-from .utils import (floatNumber, parse_file, parse_section, skipLine,
-                    skipSupress, string_array_to_molecule,
-                    try_search_pattern)
-from ._xyz import manyXYZ
-from ..common import InfoMO
-from ..type_hints import PathLike
+import pyparsing as pa
+
+# Type hints
+from typing import (List, Tuple)
 
 Vector = np.ndarray
+Matrix = np.ndarray
+
+vectorize_float = np.vectorize(float)
 
 
-def parse_molecule(file_name: PathLike, mol: Optional_[Molecule] = None) -> Molecule:
-    """Parse The Cartesian coordinates from the output file."""
+def parse_molecule(file_name, mol=None):
+    """
+    Parse The Cartesian coordinates from the output file.
+    """
     header = "CARTESIAN COORDINATES (ANGSTROEM)"
     p1 = skipSupress(header) + skipLine * 2
     parse_atoms = Group(Word(alphanums) + floatNumber * 3)
     parse_mol = p1 + Group(OneOrMore(parse_atoms))
 
     parse_many_mol = OneOrMore(parse_mol)
 
     return string_array_to_molecule(parse_many_mol, file_name, mol=mol)
 
 
-def parse_molecule_traj(file_traj: PathLike) -> Molecule:
-    """Read Molecules from the job_name.traj file."""
+def parse_molecule_traj(file_traj):
+    """
+    Read Molecules from the job_name.traj file.
+    """
     mols = manyXYZ(file_traj)
     # Last geometry corresponds to the optimized structure
     opt_mol = mols[-1]
 
     plams_mol = Molecule()
     for at in opt_mol:
         symb = at.symbol
         cs = at.xyz
         plams_mol.add_atom(Atom(symbol=symb, coords=tuple(cs)))
 
     return plams_mol
 
 
-def parse_hessian(file_hess: PathLike, start: str = '$hessian') -> np.ndarray:
-    """Read the hessian matrix in cartesian coordinates from the job_name.hess file.
-
+def parse_hessian(file_hess: str) -> Matrix:
+    """
+    Read the hessian matrix in cartesian coordinates from the job_name.hess file.
     :returns: Numpy array
     """
+    start = '$hessian'
     return read_blocks_from_file(start, '\n\n', file_hess)
 
 
-def parse_normal_modes(file_hess: PathLike) -> np.ndarray:
-    """Return the normal modes from the job_name.hess file."""
+def parse_normal_modes(file_hess: str) -> Matrix:
+    """
+    Returns the normal modes from the job_name.hess file
+    """
     start = '$normal_modes'
     return read_blocks_from_file(start, '\n\n', file_hess)
 
 
-def parse_frequencies(file_hess: PathLike) -> np.ndarray:
-    """Parse the vibrational frequencies from the job_name.hess file."""
+def parse_frequencies(file_hess: str) -> Matrix:
+    """
+    Parse the vibrational frequencies from the job_name.hess file.
+    """
     p = parse_section('$vibrational_frequencies', '\n\n')
     lines = parse_file(p, file_hess)[0].splitlines()
 
-    return np.array([x.split()[-1] for x in lines[1:]], dtype=float)
+    return vectorize_float([x.split()[-1] for x in lines[1:]])
 
 
-def read_blocks_from_file(start: str, end: str, file_name: PathLike) -> np.ndarray:
-    """Read a matrix printed in block format.
+def read_blocks_from_file(start: str, end: str, file_name: str) -> Matrix:
+    """
+    Read a matrix printed in block format
 
     :param  start: token identifying the start of the block.
     :param end: characters signaling end of block.
     :param file_name: Name of the file containing the matrix printed in blocks
     :returns: Numpy array
     """
     p = parse_section(start, end)
     raw = parse_file(p, file_name)[0].splitlines()
     number_of_basis = int(raw[0].split()[0])
     lines = raw[1:]
-
     # Matrix elements are printed in block of 6 columns
     nblocks = number_of_basis // 6
     rest = number_of_basis % 6
     nblocks = nblocks if rest == 0 else nblocks + 1
 
     # a block start with a line header then the data
     blocks = [read_block(block)
-              for block in chunked(lines, number_of_basis + 1)]
+              for block in chunksOf(lines, number_of_basis + 1)]
 
     return np.concatenate(blocks, axis=1)
 
 
-def read_block(lines: Sequence[str]) -> np.ndarray:
-    """Read a block containing the values of the block matrix.
-
-    The format is similar to:
+def read_block(lines):
+    """
+    Read a block containing the values of the block matrix in
+    a format similar to:
 
               0          1          2          3          4          5
       0   0.752994  0.078644   0.000000  -0.134007   0.156950  -0.000000
       1   0.078857  0.848881  -0.000000   0.162989  -0.312155   0.000000
       2   0.000000 -0.000000   0.074907  -0.000000   0.000000  -0.026031
       3  -0.133981  0.162928  -0.000000   0.133434  -0.164602   0.000000
 
     Read the matrix skiping the header and the first integer index
 
     :returns: Numpy array
     """
-    return np.array([x.split()[1:] for x in lines[1:]], dtype=float)
+    return np.stack(map(lambda x: vectorize_float(x.split()[1:]), lines[1:]))
 
 
-def parse_molecular_orbitals(file_name: PathLike) -> InfoMO:
-    """Read the Molecular orbital from the orca output."""
-    _n_contracted = try_search_pattern(
-        "# of contracted basis functions", file_name)
-    try:
-        n_contracted = _n_contracted.rsplit(maxsplit=1)[-1]  # type: ignore
-    except AttributeError as ex:  # _n_contracted can be None
-        raise RuntimeError(
-            "Failed to extract molecular orbials from {file_name!r}") from ex
+def parse_molecular_orbitals(file_name: str) -> Tuple:
+    """
+    Read the Molecular orbital from the orca output
+    """
+    n_contracted = try_search_pattern(
+        "# of contracted basis functions", file_name).split()[-1]
 
     # Parse the blocks of MOs
     start = 'MOLECULAR ORBITALS'
     end = '\n\n'
     block = parse_file(parse_section(start, end), file_name).asList()
 
     # split the block in lines  discarding the first line
@@ -133,32 +142,119 @@
 
     # Lines in each block
     n_contracted = int(n_contracted)
     block_lines = n_contracted + 4
 
     tuple_energies, tuple_coeffs = tuple(
         zip(*(read_column_orbitals(xs)
-              for xs in chunked(lines, block_lines))))
+              for xs in chunksOf(lines, block_lines))))
 
     return InfoMO(np.hstack(tuple_energies), np.hstack(tuple_coeffs))
 
 
-def read_column_orbitals(lines: Sequence[str]) -> Tuple[np.ndarray, np.ndarray]:
-    """Read a set of maximum 6 columns containing the Molecular orbitals.
-
-    the format similar to:
+def read_column_orbitals(lines: List) -> Tuple:
+    """
+    Read a set of maximum 6 columns containing the Molecular orbitals in a
+      format similar to:
                         0         1         2         3         4         5
                    -19.12661  -0.94591  -0.47899  -0.35256  -0.28216   0.00756
                      2.00000   2.00000   2.00000   2.00000   2.00000   0.00000
                     --------  --------  --------  --------  --------  --------
     0H   1s        -0.002625 -0.226108 -0.331594 -0.177649  0.000002 -0.074461
     0H   2s         0.002789 -0.015914 -0.107136 -0.054883  0.000001 -0.398168
     0H   1pz       -0.001404 -0.016000 -0.008447 -0.009195  0.027232  0.002729
     0H   1px        0.002631  0.023125  0.025515 -0.010664  0.005733  0.008004
     0H   1py       -0.001684 -0.022031 -0.006086 -0.022644 -0.013760  0.008735
     """
-    energies = np.array(lines[1].split(), dtype=np.float64)
+    energies = np.array(lines[1].split(), dtype=np.float)
 
     coefficients = np.array(
-        [z.split()[2:] for z in lines[4:]], dtype=np.float64)
+        [z.split()[2:] for z in lines[4:]], dtype=np.float)
 
     return energies, coefficients
+
+
+def parse_basis_set(file_name: str) -> Tuple:
+    """
+    Read the basis set used by Orca. It is printed by specifying the keyword:
+      !printbase
+    """
+    parse_basis_name = skipSupress('Your calculation utilizes the basis: ') + \
+        skipSupress(pa.Literal(':')) + pa.Suppress(pa.Literal(':')) + \
+        pa.SkipTo('\n')
+    header = skipSupress('BASIS SET IN INPUT FORMAT') + skipLine * 2
+    parserElements = create_parser_element()
+    parser = parse_basis_name + pa.Suppress(header) + \
+        pa.Group(pa.OneOrMore(parserElements))
+
+    basis = parse_file(parser, file_name).asList()
+
+    return create_basis_data(basis)
+
+
+def create_basis_data(basis: List) -> Tuple:
+    """
+    Convert the parse data into Contracted Gauss functions information
+    """
+    basis_name = basis[0]
+    atom_keys, atom_basis = zip(*[create_CGFs_per_atom(basis_name, xs)
+                                  for xs in basis[1]])
+
+    return atom_keys, atom_basis
+
+
+def create_CGFs_per_atom(basis_name: str, xs: List) -> Tuple:
+    """
+    Create the structure of the CGFs for each atom
+    """
+    atom_name = xs[0]
+    formats, primitives = zip(*[((x[0], int(x[1])), x[2:]) for x in xs[1:]])
+
+    # flatten de primitives
+    primitives = list(chain(*chain(*primitives)))
+
+    # order in coefficients and exponents the CGFs
+    nPrimitives = len(primitives) // 2
+    exponents, coefficients = np.array(
+        primitives, dtype=np.float).reshape(nPrimitives, 2).transpose()
+
+    atom_basis_key = AtomBasisKey(atom_name, basis_name, formats)
+    atom_basis_data = AtomBasisData(exponents, coefficients)
+
+    return atom_basis_key, atom_basis_data
+
+
+def create_parser_element():
+    """
+    Parser to read the basis set of a given element in
+    the following format:
+
+    # Basis set for element : O
+      NewGTO O
+      S 5
+        1    2266.1767785000     -0.0053893504
+        2     340.8701019100     -0.0402347214
+        3      77.3631351670     -0.1800818421
+        4      21.4796449400     -0.4682885766
+        5       6.6589433124     -0.4469261716
+      S 1
+        1       0.8097597567      1.0000000000
+      S 1
+        1       0.2553077223      1.0000000000
+      P 3
+        1      17.7215043170      0.0626302488
+        2       3.8635505440      0.3333113849
+        3       1.0480920883      0.7414863830
+      P 1
+        1       0.2764154441      1.0000000000
+      D 1
+        1       1.2000000000      1.0000000000
+       end;
+    """
+    header = pa.Suppress(pa.Literal('# Basis set for element :')) + \
+        pa.Word(pa.alphas) + skipLine
+
+    parseCGF = pa.Group(
+        pa.Word(pa.alphas, exact=1)  + natural +
+        pa.Group(pa.OneOrMore(pa.Suppress(natural) + floatNumber * 2)))
+
+    return pa.Group(header + pa.OneOrMore(parseCGF) + pa.Suppress(pa.Literal('end;')))
```

### Comparing `qmflows-0.13.0/src/qmflows/parsers/utils.py` & `qmflows-0.2.1/src/qmflows/parsers/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,102 @@
-"""General utilities to parse both input/out files."""
+__author__ = "Felipe Zapata"
 
 __all__ = ['anyChar', 'integer', 'natural', 'parse_file', 'parse_section',
            'skipAnyChar', 'skipLine', 'skipSupress', 'try_search_pattern']
 
 
-import re
-from typing import Optional as Optional_
-
+from scm.plams import (Atom, Molecule)
+from pyparsing import (CaselessKeyword, Combine, Literal, nums, Optional,
+                       ParseException, Regex, SkipTo, Suppress, Word)
 import numpy as np
-from pyparsing import (CaselessKeyword, Combine, Literal, Optional,
-                       ParseException, ParserElement, ParseResults, Regex,
-                       SkipTo, Suppress, Word, nums)
-from scm.plams import Atom, Molecule
-
-from ..type_hints import PathLike
+import re
 
 # Literals
 point = Literal('.')
 e = CaselessKeyword('E')
 minusOrplus = Literal('+') | Literal('-')
 
 # Parsing Floats
 natural = Word(nums)
 integer = Combine(Optional(minusOrplus) + natural)
 floatNumber = Regex(r'(\-)?\d+(\.)(\d*)?([eE][\-\+]\d+)?')
 
 floatNumberDot = Regex(r'(\-)?(\d+)?(\.)(\d*)?([eE][\-\+]\d+)?')
 
-# Parse Utilities
-
-
-def skipSupress(z: str) -> ParserElement:
-    """Skip until `z` and suppress the skipped values."""
-    return Suppress(SkipTo(z))
-
 
+# Parse Utilities
 anyChar = Regex('.')
 skipAnyChar = Suppress(anyChar)
+skipSupress = lambda z: Suppress(SkipTo(z))
 skipLine = Suppress(skipSupress('\n'))
 
-# Generic Functions
 
+# Generic Functions
 
-def parse_file(p: ParserElement, file_name: PathLike) -> ParseResults:
-    """Apply parser `p` on file `file_name`."""
+def parse_file(p, file_name):
+    """
+    Wrapper over the parseFile method
+    """
     try:
         return p.parseFile(file_name)
-    except ParseException as ex:
-        raise ParseException(f"Error Trying to parse: {p} in file: {file_name}") from ex
+    except ParseException:
+        msg = "Error Trying to parse: {} in file: {}".format(p, file_name)
+        print(msg)
+        raise
 
 
-def parse_section(start: str, end: str) -> ParserElement:
-    """Read the lines from `start` to `end`."""
+def parse_section(start, end):
+    """
+    Read the lines from `start` to `end`.
+    """
     s = Literal('{}'.format(start))
     e = Literal('{}'.format(end))
 
     return Suppress(SkipTo(s)) + skipLine + SkipTo(e)
 
 
-def string_array_to_molecule(parser_fun: ParserElement,
-                             file_name: PathLike,
-                             mol: Optional_[Molecule] = None) -> Molecule:
-    """Convert a Numpy string array.
+def string_array_to_molecule(parser_fun, file_name, mol=None):
+    """
+    Convert a Numpy string array like:
 
-    It takes an array like:
     [['C', '-1.487460', '-0.028670', '-0.000060'],
     ['O', '0.376340', '0.028670', '-0.000060'],
     ['H', '-1.818910', '-1.067060', '-0.000060'],
     ['H', '-1.866470', '0.473700', '0.889930'],
     ['H', '-1.866470', '0.473700', '-0.890040'],
     ['H', '0.756720', '-0.950010', '-0.000060']]
 
-    and covert it to a plams ``Molecule``.
+    To a plams ``Molecule``.
     """
+    string_array_to_float = np.vectorize(float)
     mols = parse_file(parser_fun, file_name).asList()
     last_mol = np.array(mols[-1])
     elems = last_mol[:, 0]
-    coords = np.array(last_mol[:, 1:], dtype=float)
-
+    coords = string_array_to_float(last_mol[:, 1:])
     if mol:
         if len(coords) == len(mol):
-            mol.from_array(coords)
+            plams_mol = mol
+            for i in range(len(plams_mol)):
+                plams_mol.atoms[i].coords = tuple([float(c) for c in coords[i]])
         else:
             raise RuntimeError('Output molecule does not match input molecule')
-
     else:
-        mol = Molecule()
+        plams_mol = Molecule()
         for e, c in zip(elems, coords):
-            mol.add_atom(Atom(symbol=e, coords=tuple(c)))
-    return mol
+            plams_mol.add_atom(Atom(symbol=e, coords=tuple(c)))
+    return plams_mol
 
 
-def try_search_pattern(pat: str, file_name: PathLike) -> Optional_[str]:
-    """Search for an specific pattern in  a file."""
+def try_search_pattern(pat, file_name):
+    """
+    Search for an specific pattern in  a file
+    """
     try:
         with open(file_name, 'r') as f:
             for line in f:
                 if re.search(pat, line):
                     return line
-            else:
-                return None
+    except NameError:
+        return None
     except FileNotFoundError:
-        msg2 = f'There is not a file: {file_name}\n'
+        msg2 = 'There is not a file: {}\n'.format(file_name)
         raise RuntimeError(msg2)
```

