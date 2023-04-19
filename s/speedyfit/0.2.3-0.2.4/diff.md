# Comparing `tmp/speedyfit-0.2.3.tar.gz` & `tmp/speedyfit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/speedyfit-0.2.3.tar", last modified: Sun Oct 23 13:08:34 2022, max compression
+gzip compressed data, was "dist/speedyfit-0.2.4.tar", last modified: Wed Apr 19 09:04:45 2023, max compression
```

## Comparing `speedyfit-0.2.3.tar` & `speedyfit-0.2.4.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:08:34.000000 speedyfit-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-23 13:08:25.000000 speedyfit-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-10-23 13:08:34.000000 speedyfit-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-10-23 13:08:25.000000 speedyfit-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 13:08:34.000000 speedyfit-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-10-23 13:08:25.000000 speedyfit-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:08:34.000000 speedyfit-0.2.3/speedyfit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1622 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/calibration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/default_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15448 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/fileio.py
--rw-r--r--   0 runner    (1001) docker     (121)     7247 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/filters.py
--rw-r--r--   0 runner    (1001) docker     (121)    13734 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/integrate_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5142 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/interpol.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20094 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/main.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7239 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/mcmc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15773 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/model.py
--rw-r--r--   0 runner    (1001) docker     (121)    14160 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/photometry_query.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11257 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11903 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/reddening.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:08:34.000000 speedyfit-0.2.3/speedyfit/redlaws/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6135 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Chiar2006.red
--rwxr-xr-x   0 runner    (1001) docker     (121)   466871 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick1999_Rv_2_1.red
--rwxr-xr-x   0 runner    (1001) docker     (121)   466849 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick1999_Rv_3_1.red
--rwxr-xr-x   0 runner    (1001) docker     (121)   466860 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick1999_Rv_5_0.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.1.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.2.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.3.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.4.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.5.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.6.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.7.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.8.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.9.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.0.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.1.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.2.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.3.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.4.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.5.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.6.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.7.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.8.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.9.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.0.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.1.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.2.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.3.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.4.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.5.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.6.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.7.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.8.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.9.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.0.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.1.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.2.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.3.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.4.red
--rwxr-xr-x   0 runner    (1001) docker     (121)     2475 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.5.red
--rw-r--r--   0 runner    (1001) docker     (121)     6568 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/speedyfit_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14504 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/statfunc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1505 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tap_cats_phot.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:08:34.000000 speedyfit-0.2.3/speedyfit/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)        2 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1673 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/test_fileio.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2761 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/test_mcmc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9353 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/test_photometry_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/test_speedyfit_batch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1893 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/tests/test_statfunc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16864 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/vizier_cats_phot.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)    68312 2022-10-23 13:08:25.000000 speedyfit-0.2.3/speedyfit/zeropoints.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 13:08:34.000000 speedyfit-0.2.3/speedyfit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-10-23 13:08:33.000000 speedyfit-0.2.3/speedyfit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-23 13:08:34.000000 speedyfit-0.2.3/speedyfit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 13:08:33.000000 speedyfit-0.2.3/speedyfit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-10-23 13:08:33.000000 speedyfit-0.2.3/speedyfit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-10-23 13:08:33.000000 speedyfit-0.2.3/speedyfit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-23 13:08:33.000000 speedyfit-0.2.3/speedyfit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:04:45.000000 speedyfit-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 09:04:35.000000 speedyfit-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-19 09:04:45.000000 speedyfit-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-19 09:04:35.000000 speedyfit-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 09:04:45.000000 speedyfit-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-19 09:04:35.000000 speedyfit-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/default_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15448 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/integrate_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5149 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/interpol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20080 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7239 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/mcmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15773 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/photometry_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11273 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11903 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/reddening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit/redlaws/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6135 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Chiar2006.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)   466871 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick1999_Rv_2_1.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)   466849 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick1999_Rv_3_1.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)   466860 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick1999_Rv_5_0.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.1.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.2.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.3.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.4.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.5.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.6.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.7.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.8.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.9.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.0.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.1.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.2.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.3.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.4.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.5.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.6.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.7.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.8.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.9.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.0.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.1.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.2.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.3.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.4.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.5.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.6.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.7.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.8.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.9.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.0.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.1.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.2.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.3.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.4.red
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.5.red
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/speedyfit_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14504 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/statfunc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tap_cats_phot.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        2 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1673 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/test_fileio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2761 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/test_mcmc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9353 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/test_photometry_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/test_speedyfit_batch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1893 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/tests/test_statfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16864 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/vizier_cats_phot.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68312 2023-04-19 09:04:35.000000 speedyfit-0.2.4/speedyfit/zeropoints.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 09:04:45.000000 speedyfit-0.2.4/speedyfit.egg-info/top_level.txt
```

### Comparing `speedyfit-0.2.3/PKG-INFO` & `speedyfit-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyfit
-Version: 0.2.3
+Version: 0.2.4
 Summary: MC approach to fit photometric SEDs
 Home-page: https://github.com/vosjo/speedyfit
 Author: Joris Vos
 Author-email: joris.vos@uv.cl
 License: UNKNOWN
 Description: ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/speedyfit)
         [![PyPI](https://img.shields.io/pypi/v/speedyfit?color=blue)](https://pypi.org/project/speedyfit/)
```

### Comparing `speedyfit-0.2.3/README.md` & `speedyfit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/calibration.py` & `speedyfit-0.2.4/speedyfit/calibration.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/default_setup.py` & `speedyfit-0.2.4/speedyfit/default_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 default_binary = """
 # photometry file with index to the columns containing the photbands, observations and errors
 objectname: <objectname>
 photometryfile: <photfilename>
 photband_index: band
 obs_index: flux
 err_index: eflux
-photband_exclude: ['GALEX', 'SDSS', 'WISE.W3', 'WISE.W4']
+photband_exclude: ['GALEX', 'SDSS', 'WISE.W3', 'WISE.W4', 'GAIA2']
 # parameters to fit and the limits on them in same order as parameters
 pnames: [teff, logg, rad, teff2, logg2, rad2, ebv]
 limits:
 - [3500, 10000]
 - [4.31, 4.31]
 - [0.01, 2.5]
 - [20000, 80000]
```

### Comparing `speedyfit-0.2.3/speedyfit/fileio.py` & `speedyfit-0.2.4/speedyfit/fileio.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/filters.py` & `speedyfit-0.2.4/speedyfit/filters.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/integrate_grid.py` & `speedyfit-0.2.4/speedyfit/integrate_grid.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/interpol.py` & `speedyfit-0.2.4/speedyfit/interpol.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
    
    # We put np.inf as default value. If we get an inf, that means we tried to access
    # a region of the pixelgrid that is not populated by the data table
    pixelgrid[pixelgrid==1] = np.inf
    
    # now populate the multiDgrid
    indices = [uv[1] for uv in uniques]
-   pixelgrid[indices] = grid_data.T
+   pixelgrid[tuple(indices)] = grid_data.T
    
    return axis_values, pixelgrid
 
 def interpolate(p, axis_values, pixelgrid):
    """
    Interpolates in a grid prepared by create_pixeltypegrid().
```

### Comparing `speedyfit-0.2.3/speedyfit/main.py` & `speedyfit-0.2.4/speedyfit/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             if setup[pindex].get('show_best', False):
                 truths = [results[p][0] for p in data.dtype.names]
             else:
                 truths = None
 
             fig = corner.corner(data.view(np.float64).reshape(data.shape + (-1,)),
                                 labels=data.dtype.names,
-                                quantiles=setup[pindex].get('quantiles', [0.025, 0.16, 0.5, 0.84, 0.975]),
+                                quantiles=setup[pindex].get('quantiles', [0.16, 0.5, 0.84]),
                                 levels=setup[pindex].get('levels', [0.393, 0.865, 0.95]),
                                 truths=truths,
                                 show_titles=True, title_kwargs={"fontsize": 12}, )
 
             if not setup[pindex].get('path', None) is None:
                 pl.savefig(setup[pindex].get('path', 'distribution.png'))
```

### Comparing `speedyfit-0.2.3/speedyfit/mcmc.py` & `speedyfit-0.2.4/speedyfit/mcmc.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/model.py` & `speedyfit-0.2.4/speedyfit/model.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/photometry_query.py` & `speedyfit-0.2.4/speedyfit/photometry_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,21 +384,24 @@
 
     if filename is not None:
         ascii.write(photometry, filename, format='fixed_width', overwrite=True)
 
     return photometry
 
 
-def get_parallax(objectname, radius=5):
+def get_parallax(objectname, ra=None, dec=None, radius=5):
 
     v_gaia = Vizier(columns=["Plx", "e_Plx", '+_r', 'Gmag', 'nueff', 'pscol', 'ELAT', 'Solved'])
 
+    # try the query with the objectname first
     data = v_gaia.query_object(objectname, catalog=['I/350/gaiaedr3'], radius=radius*u.arcsec)
 
-    if len(data) == 0:
+    # if no data is returned retry the query with the coordinates if possible
+    if len(data) == 0 and ra is not None and dec is not None:
+
         return None, None
 
     data = data['I/350/gaiaedr3'][0]
 
     plx, plx_e = data['Plx'], data['e_Plx']
 
     if not data['pscol']:
```

### Comparing `speedyfit-0.2.3/speedyfit/plotting.py` & `speedyfit-0.2.4/speedyfit/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,22 +238,22 @@
     
    ascii.write([wave, flux, error, band], 'observations.txt', names=['wave', 'flux', 'error', 'band'], overwrite=True)
    
       
    pl.xlim(abs_xlim)
    pl.ylim([0.9*np.min(obs[~colors]), 1.1*np.max(obs[~colors])])
    pl.legend(loc='best', prop={'size': 9}, numpoints=1)
-   ax1.set_xscale("log", nonposx='clip')
-   ax1.set_yscale("log", nonposy='clip')
+   ax1.set_xscale("log", nonpositive='clip')
+   ax1.set_yscale("log", nonpositive='clip')
    
    pl.ylabel('Absolute Flux')
    
    #-- add band names to top of axis
    ax2 = ax1.twiny()
-   ax2.set_xscale("log", nonposx='clip')
+   ax2.set_xscale("log", nonpositive='clip')
    ax2.set_xlim(abs_xlim)
    waves = np.array([filters.eff_wave(p) for p in photbands[~colors]])
    bandnames = np.array([b.split('.')[-1] for b in photbands[~colors]])
    ax2.set_xticks(waves)
    ax2.set_xticklabels(bandnames)
    ax2.xaxis.tick_top()
    pl.minorticks_off()
@@ -281,15 +281,15 @@
       pl.errorbar(w, -y , yerr=yerr, ls='', marker='o', color=system_colors[system])
    
    pl.figtext(0.96, 0.96, '$\chi^2$ = {:0.2f}'.format(pars['chi2']), ha='right')
    
    pl.axhline(y=0, color='k', ls='--')
    
    pl.xlim(abs_xlim)
-   pl.gca().set_xscale('log',nonposx='clip')
+   pl.gca().set_xscale('log',nonpositive='clip')
    
    pl.ylabel('(O-C) (mag)')
    pl.xlabel('Wavelength (AA)')
    
 
    # plot O-C of the color fits
    #====================================
```

### Comparing `speedyfit-0.2.3/speedyfit/reddening.py` & `speedyfit-0.2.4/speedyfit/reddening.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Chiar2006.red` & `speedyfit-0.2.4/speedyfit/redlaws/Chiar2006.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick1999_Rv_2_1.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick1999_Rv_2_1.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick1999_Rv_3_1.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick1999_Rv_3_1.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick1999_Rv_5_0.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick1999_Rv_5_0.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.1.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.1.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.2.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.2.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.3.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.3.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.4.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.4.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.5.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.5.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.6.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.6.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.7.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.7.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.8.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.8.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_2.9.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_2.9.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.0.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.0.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.1.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.1.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.2.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.2.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.3.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.3.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.4.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.4.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.5.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.5.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.6.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.6.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.7.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.7.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.8.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.8.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_3.9.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_3.9.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.0.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.0.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.1.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.1.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.2.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.2.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.3.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.3.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.4.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.4.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.5.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.5.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.6.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.6.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.7.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.7.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.8.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.8.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_4.9.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_4.9.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.0.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.0.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.1.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.1.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.2.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.2.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.3.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.3.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.4.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.4.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/redlaws/Fitzpatrick2004_Rv_5.5.red` & `speedyfit-0.2.4/speedyfit/redlaws/Fitzpatrick2004_Rv_5.5.red`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/speedyfit_batch.py` & `speedyfit-0.2.4/speedyfit/speedyfit_batch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,122 @@
 import copy
 import os
 import argparse
 
 import yaml
 
 import pandas as pd
-
-from astropy.coordinates import Angle
+import numpy as np
 
 from speedyfit import photometry_query
 from speedyfit.main import fit_sed, get_observations, write_results, plot_results
 from speedyfit.default_setup import default_tmap, default_binary
+from speedyfit.utils import get_name_from_coordinates
 
+def extract_constraint_names(data):
+    columns = data.columns.values
+    constraint_names = []
+    for name in columns:
+        if 'constraint_' in name:
+            cname = name.split('_')[1]
+            constraint_names.append(cname)
 
-def process_objects(data):
+    return constraint_names
 
-    def convert_ra(ra):
-        if ' ' in str(ra).strip() or ':' in str(ra).strip():
-            ra = str(ra).strip()
-            ra = ra.replace(' ', '').replace(':', '')
-        else:
-            a = Angle(ra, unit='degree').hms
-            ra = '{:02.0f}{:02.0f}{:05.2f}'.format(*a)
-        return ra
-
-    def convert_dec(dec):
-        if ' ' in str(dec).strip() or ':' in str(dec).strip():
-            dec = str(dec).strip()
-            dec = dec.replace(' ', '').replace(':', '')
-            if not '-' in dec and not '+' in dec:
-                dec = '+' + dec
-        else:
-            a = Angle(dec, unit='degree').dms
-            dec = '{:+03.0f}{:02.0f}{:05.2f}'.format(a[0], abs(a[1]), abs(a[2]))
-        return dec
 
+def process_objects(data):
+
+    # check if we are working with names or if we need to make names from the coordinates
     if 'name' in data.columns.values:
-        object_list = data['name'].apply(lambda x: x.replace(' ', '_')).values
+        object_list = data['name'].apply(lambda x: x.replace(' ', '_').strip()).values
+        object_list = pd.DataFrame({'name': object_list})
     else:
-        # deal with coordinates
-        ra_ = data['ra'].apply(convert_ra)
-        dec_ = data['dec'].apply(convert_dec)
-
-        name = ['J{}{}'.format(r, d) for r, d in zip(ra_, dec_)]
-
-        object_list = pd.Series(data=name)
+        # convert coordinates into a name if no name was given.
+        name = get_name_from_coordinates(data['ra'].values, data['dec'].values)
+        object_list = pd.DataFrame({'name': name})
+
+    if 'ra' in data and 'dec' in data:
+        object_list['ra'] = data['ra']
+        object_list['dec'] = data['dec']
+
+    # now check for constraints
+    constraint_cols = extract_constraint_names(data)
+    for cname in constraint_cols:
+        object_list[cname] = data['constraint_'+cname]
 
     return object_list
 
 
 def read_setup(setup):
 
     if os.path.isfile(setup):
         infile = open(setup, 'r')
         setup = infile.readlines()
         infile.close()
         setup = ''.join(setup)
 
     elif setup == 'single':
         setup = default_tmap
-    elif setup == 'double':
+    elif setup == 'binary':
         setup = default_binary
     else:
         print('Setup not recognized! Using single as default')
         setup = default_tmap
 
     return setup
 
 
 def prepare_setup(object_list, basedir, default_setup):
 
-    for objectname in object_list:
+    constraint_names = list(object_list.columns.values)
+    constraint_names.remove('name')
+    constraint_names.remove('ra')
+    constraint_names.remove('dec')
+
+    for i, row in object_list.iterrows():
+        objectname = row['name']
+        ra, dec = row['ra'], row['dec']
+        print(f'Preparing setup files for object: {objectname} ({ra}  {dec})')
 
         if not os.path.isdir(basedir+'/'+objectname):
             os.mkdir(basedir+'/'+objectname)
 
         plx, e_plx = photometry_query.get_parallax(objectname)
 
         out = copy.copy(default_setup)
         if '<photfilename>' in out:
             photfilename_ = basedir + '/' + objectname + '/' + objectname + '.phot'
             out = out.replace('<photfilename>', photfilename_)
         if '<objectname>' in out:
             objectname_ = basedir + '/' + objectname + '/' + objectname
             out = out.replace('<objectname>', objectname_)
         if '<constraints>' in out:
-            constraints = "\n  parallax: [{:0.4f}, {:0.4f}]".format(plx, e_plx)
+            constraints = f"\n  parallax: [{plx:0.4f}, {e_plx:0.4f}]"
+            for cname in constraint_names:
+                val = row[cname]
+                try:
+                    val = val.replace('(', '').replace(')', '')
+                except:
+                    continue
+                if val.strip() == '':
+                    continue
+                constraints += f"\n  {cname}: [{val}]"
             out = out.replace('<constraints>', constraints)
 
         filename = basedir + '/' + objectname + '/' + objectname + '_setup.yaml'
 
         ofile = open(filename, 'w')
         ofile.write(out)
         ofile.close()
 
 
 def prepare_photometry(object_list, basedir, skip_existing=True):
 
-    for objectname in object_list:
+    for i, row  in object_list.iterrows():
+        objectname = row['name']
 
         if os.path.isfile(basedir+'/'+objectname+'/'+objectname+'.phot') and skip_existing:
             continue
 
         if not os.path.isdir(basedir+'/'+objectname):
             os.mkdir(basedir+'/'+objectname)
 
@@ -109,19 +124,24 @@
             filename = basedir + '/' + objectname + '/' + objectname + '.phot'
             photometry = photometry_query.get_photometry(objectname, filename=filename)
         except Exception as e:
             print("Failed to obtain photometry for {}".format(objectname))
             print(e)
 
 
-def fit_seds(object_list, basedir):
+def fit_seds(object_list, basedir, start_index=0, stop_index=None):
 
     all_results = {}
 
-    for objectname in object_list:
+    stop_index = len(object_list) if stop_index is None else stop_index
+    object_list_sel = object_list[start_index:stop_index+1]
+
+    for i, row in object_list_sel.iterrows():
+        objectname = row['name']
+        print(f"Starting fit {i}/{len(object_list)} for object: {objectname}")
 
         # read the setup
         filename = basedir + '/' + objectname + '/' + objectname + '_setup.yaml'
         try:
             infile = open(filename)
             setup = yaml.safe_load(infile)
             infile.close()
@@ -160,24 +180,26 @@
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filename', action="store", type=str,
                         help='file containing a list with the names or coordinates of the systems to fit')
     parser.add_argument("-setup", dest='setup', type=str, default='single',
-                        help="The path to the setup file to use, or a standard: 'single' or 'double'. "
+                        help="The path to the setup file to use, or a standard: 'single' or 'binary'. "
                              "(default = 'single'")
     parser.add_argument("-basedir", dest='basedir', type=str, default='./',
                         help="The directory where all photometry, setup and results will be stored. (default = ./)")
     parser.add_argument("--fit", dest='fit', action='store_true',
                         help="Fit the systems")
     parser.add_argument('--phot', dest='phot', action='store_true',
                         help='Obtain photometry of the systems')
-    parser.add_argument('--noplot', dest='noplot', action='store_true',
-                        help="Don't show any plots, only store to disk.")
+    parser.add_argument('-start', dest='start_index', type=int, default=0,
+                        help='Index of the object with which to start the fit, defaults to 0')
+    parser.add_argument('-stop', dest='stop_index', type=int, default=None,
+                        help='Index of the object with which to end the fitting, defaults to None (all objects are fitted).')
     args, variables = parser.parse_known_args()
 
     basedir = args.basedir
     default_setup = read_setup(args.setup)
 
     if not os.path.isdir(basedir):
         os.mkdir(basedir)
@@ -190,8 +212,8 @@
 
     # try to obtain photometry for all systems if requested
     if args.phot:
         prepare_photometry(object_list, basedir)
 
     # fit all systems if requested
     if args.fit:
-        fit_seds(object_list, basedir)
+        fit_seds(object_list, basedir, start_index=args.start_index, stop_index=args.stop_index)
```

### Comparing `speedyfit-0.2.3/speedyfit/statfunc.py` & `speedyfit-0.2.4/speedyfit/statfunc.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/tap_cats_phot.cfg` & `speedyfit-0.2.4/speedyfit/tap_cats_phot.cfg`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/tests/test_fileio.py` & `speedyfit-0.2.4/speedyfit/tests/test_fileio.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/tests/test_mcmc.py` & `speedyfit-0.2.4/speedyfit/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/tests/test_model.py` & `speedyfit-0.2.4/speedyfit/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/tests/test_speedyfit_batch.py` & `speedyfit-0.2.4/speedyfit/tests/test_speedyfit_batch.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/tests/test_statfunc.py` & `speedyfit-0.2.4/speedyfit/tests/test_statfunc.py`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/vizier_cats_phot.cfg` & `speedyfit-0.2.4/speedyfit/vizier_cats_phot.cfg`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit/zeropoints.dat` & `speedyfit-0.2.4/speedyfit/zeropoints.dat`

 * *Files identical despite different names*

### Comparing `speedyfit-0.2.3/speedyfit.egg-info/PKG-INFO` & `speedyfit-0.2.4/speedyfit.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedyfit
-Version: 0.2.3
+Version: 0.2.4
 Summary: MC approach to fit photometric SEDs
 Home-page: https://github.com/vosjo/speedyfit
 Author: Joris Vos
 Author-email: joris.vos@uv.cl
 License: UNKNOWN
 Description: ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/speedyfit)
         [![PyPI](https://img.shields.io/pypi/v/speedyfit?color=blue)](https://pypi.org/project/speedyfit/)
```

### Comparing `speedyfit-0.2.3/speedyfit.egg-info/SOURCES.txt` & `speedyfit-0.2.4/speedyfit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 speedyfit/model.py
 speedyfit/photometry_query.py
 speedyfit/plotting.py
 speedyfit/reddening.py
 speedyfit/speedyfit_batch.py
 speedyfit/statfunc.py
 speedyfit/tap_cats_phot.cfg
+speedyfit/utils.py
 speedyfit/vizier_cats_phot.cfg
 speedyfit/zeropoints.dat
 speedyfit.egg-info/PKG-INFO
 speedyfit.egg-info/SOURCES.txt
 speedyfit.egg-info/dependency_links.txt
 speedyfit.egg-info/entry_points.txt
 speedyfit.egg-info/requires.txt
```

