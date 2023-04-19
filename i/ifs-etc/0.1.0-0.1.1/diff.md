# Comparing `tmp/ifs_etc-0.1.0.tar.gz` & `tmp/ifs_etc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ifs_etc-0.1.0.tar", last modified: Wed Apr 19 03:23:14 2023, max compression
+gzip compressed data, was "dist/ifs_etc-0.1.1.tar", last modified: Wed Apr 19 05:54:44 2023, max compression
```

## Comparing `ifs_etc-0.1.0.tar` & `ifs_etc-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/
--rw-r--r--   0 linlin     (501) staff       (20)      246 2022-08-15 07:47:55.000000 ifs_etc-0.1.0/MANIFEST.in
--rw-r--r--   0 linlin     (501) staff       (20)     3788 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/PKG-INFO
--rw-r--r--   0 linlin     (501) staff       (20)     2703 2022-05-29 14:50:14.000000 ifs_etc-0.1.0/README.md
--rw-r--r--   0 linlin     (501) staff       (20)       58 2022-03-27 06:45:13.000000 ifs_etc-0.1.0/README.rst
--rw-r--r--   0 linlin     (501) staff       (20)       38 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/setup.cfg
--rw-r--r--   0 linlin     (501) staff       (20)     1160 2023-03-07 09:05:59.000000 ifs_etc-0.1.0/setup.py
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/
--rw-r--r--   0 linlin     (501) staff       (20)       21 2023-04-19 03:22:02.000000 ifs_etc-0.1.0/src/ifs_etc/__init__.py
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/etc1d/
--rw-r--r--   0 linlin     (501) staff       (20)       56 2022-01-10 07:33:09.000000 ifs_etc-0.1.0/src/ifs_etc/etc1d/__init__.py
--rw-r--r--   0 linlin     (501) staff       (20)     4120 2023-03-22 07:02:36.000000 ifs_etc-0.1.0/src/ifs_etc/etc1d/config.py
--rw-r--r--   0 linlin     (501) staff       (20)    23653 2023-03-22 07:02:36.000000 ifs_etc-0.1.0/src/ifs_etc/etc1d/perform_calculation.py
--rw-r--r--   0 linlin     (501) staff       (20)     9616 2023-03-12 07:10:28.000000 ifs_etc-0.1.0/src/ifs_etc/etc1d/source.py
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/
--rw-r--r--   0 linlin     (501) staff       (20)       67 2023-03-07 08:50:28.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/__init__.py
--rw-r--r--   0 linlin     (501) staff       (20)     5995 2023-03-22 07:02:37.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/config.py
--rw-r--r--   0 linlin     (501) staff       (20)    21704 2023-03-22 06:54:12.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/ifs_etc.py
--rw-r--r--   0 linlin     (501) staff       (20)    24404 2023-04-04 06:32:34.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/perform_calculation.py
--rw-r--r--   0 linlin     (501) staff       (20)    28823 2022-03-29 14:45:03.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/snpp.py
--rw-r--r--   0 linlin     (501) staff       (20)    16330 2023-04-19 02:31:07.000000 ifs_etc-0.1.0/src/ifs_etc/etc2d/source.py
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/
--rw-r--r--   0 linlin     (501) staff       (20)      968 2022-04-06 04:29:28.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/earthshine_spec.csv
--rw-r--r--   0 linlin     (501) staff       (20)    85785 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/skybg_50_10.dat
--rw-r--r--   0 linlin     (501) staff       (20)     1005 2022-04-06 04:29:44.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/zodi_spec.csv
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/ifs/
--rw-r--r--   0 linlin     (501) staff       (20)      653 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/ifs/IFU_throughput.dat
--rw-r--r--   0 linlin     (501) staff       (20)      229 2023-03-12 06:20:02.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/ifs/uv_throughtput.dat
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/telescope/
--rw-r--r--   0 linlin     (501) staff       (20)       76 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/csst/telescope/config.json
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/
--rw-r--r--   0 linlin     (501) staff       (20)    15744 2023-03-12 07:09:45.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/GALEX_fuv.par
--rw-r--r--   0 linlin     (501) staff       (20)    42784 2023-03-12 07:09:41.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/GALEX_nuv.par
--rw-r--r--   0 linlin     (501) staff       (20)    33010 2023-03-12 06:55:26.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_B.txt
--rw-r--r--   0 linlin     (501) staff       (20)    32832 2022-08-15 07:41:16.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_I.txt
--rw-r--r--   0 linlin     (501) staff       (20)    32753 2022-08-15 07:41:09.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_R.txt
--rw-r--r--   0 linlin     (501) staff       (20)    33166 2022-08-18 09:37:49.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_U.txt
--rw-r--r--   0 linlin     (501) staff       (20)    32964 2022-08-18 09:37:38.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_V.txt
--rw-r--r--   0 linlin     (501) staff       (20)     4682 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_g.par
--rw-r--r--   0 linlin     (501) staff       (20)     4682 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_i.par
--rw-r--r--   0 linlin     (501) staff       (20)     4482 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_r.par
--rw-r--r--   0 linlin     (501) staff       (20)     4782 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_u.par
--rw-r--r--   0 linlin     (501) staff       (20)     5033 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_z.par
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/sed/
--rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH-2_tau10_Ew50.fits
--rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau1_Ewd.fits
--rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew10_AGN1.fits
--rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew5.fits
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/source/
--rw-r--r--   0 linlin     (501) staff       (20)      413 2022-01-10 06:07:14.000000 ifs_etc-0.1.0/src/ifs_etc/refdata/source/config.json
-drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 03:23:14.000000 ifs_etc-0.1.0/src/ifs_etc.egg-info/
--rw-r--r--   0 linlin     (501) staff       (20)     3788 2023-04-19 03:23:13.000000 ifs_etc-0.1.0/src/ifs_etc.egg-info/PKG-INFO
--rw-r--r--   0 linlin     (501) staff       (20)     1770 2023-04-19 03:23:13.000000 ifs_etc-0.1.0/src/ifs_etc.egg-info/SOURCES.txt
--rw-r--r--   0 linlin     (501) staff       (20)        1 2023-04-19 03:23:13.000000 ifs_etc-0.1.0/src/ifs_etc.egg-info/dependency_links.txt
--rw-r--r--   0 linlin     (501) staff       (20)      137 2023-04-19 03:23:13.000000 ifs_etc-0.1.0/src/ifs_etc.egg-info/requires.txt
--rw-r--r--   0 linlin     (501) staff       (20)        8 2023-04-19 03:23:13.000000 ifs_etc-0.1.0/src/ifs_etc.egg-info/top_level.txt
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/
+-rw-r--r--   0 linlin     (501) staff       (20)      246 2022-08-15 07:47:55.000000 ifs_etc-0.1.1/MANIFEST.in
+-rw-r--r--   0 linlin     (501) staff       (20)     3788 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/PKG-INFO
+-rw-r--r--   0 linlin     (501) staff       (20)     2703 2022-05-29 14:50:14.000000 ifs_etc-0.1.1/README.md
+-rw-r--r--   0 linlin     (501) staff       (20)       58 2022-03-27 06:45:13.000000 ifs_etc-0.1.1/README.rst
+-rw-r--r--   0 linlin     (501) staff       (20)       38 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/setup.cfg
+-rw-r--r--   0 linlin     (501) staff       (20)     1160 2023-03-07 09:05:59.000000 ifs_etc-0.1.1/setup.py
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/
+-rw-r--r--   0 linlin     (501) staff       (20)       21 2023-04-19 05:54:30.000000 ifs_etc-0.1.1/src/ifs_etc/__init__.py
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/etc1d/
+-rw-r--r--   0 linlin     (501) staff       (20)       56 2022-01-10 07:33:09.000000 ifs_etc-0.1.1/src/ifs_etc/etc1d/__init__.py
+-rw-r--r--   0 linlin     (501) staff       (20)     4122 2023-04-19 05:45:24.000000 ifs_etc-0.1.1/src/ifs_etc/etc1d/config.py
+-rw-r--r--   0 linlin     (501) staff       (20)    23653 2023-03-22 07:02:36.000000 ifs_etc-0.1.1/src/ifs_etc/etc1d/perform_calculation.py
+-rw-r--r--   0 linlin     (501) staff       (20)     9616 2023-03-12 07:10:28.000000 ifs_etc-0.1.1/src/ifs_etc/etc1d/source.py
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/
+-rw-r--r--   0 linlin     (501) staff       (20)       67 2023-03-07 08:50:28.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/__init__.py
+-rw-r--r--   0 linlin     (501) staff       (20)     5995 2023-03-22 07:02:37.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/config.py
+-rw-r--r--   0 linlin     (501) staff       (20)    21704 2023-03-22 06:54:12.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/ifs_etc.py
+-rw-r--r--   0 linlin     (501) staff       (20)    24404 2023-04-04 06:32:34.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/perform_calculation.py
+-rw-r--r--   0 linlin     (501) staff       (20)    28823 2022-03-29 14:45:03.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/snpp.py
+-rw-r--r--   0 linlin     (501) staff       (20)    16330 2023-04-19 02:31:07.000000 ifs_etc-0.1.1/src/ifs_etc/etc2d/source.py
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/
+-rw-r--r--   0 linlin     (501) staff       (20)      968 2022-04-06 04:29:28.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/earthshine_spec.csv
+-rw-r--r--   0 linlin     (501) staff       (20)    85785 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/skybg_50_10.dat
+-rw-r--r--   0 linlin     (501) staff       (20)     1005 2022-04-06 04:29:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/zodi_spec.csv
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/ifs/
+-rw-r--r--   0 linlin     (501) staff       (20)      653 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/ifs/IFU_throughput.dat
+-rw-r--r--   0 linlin     (501) staff       (20)      229 2023-03-12 06:20:02.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/ifs/uv_throughtput.dat
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/telescope/
+-rw-r--r--   0 linlin     (501) staff       (20)       76 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/csst/telescope/config.json
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/
+-rw-r--r--   0 linlin     (501) staff       (20)    15744 2023-03-12 07:09:45.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/GALEX_fuv.par
+-rw-r--r--   0 linlin     (501) staff       (20)    42784 2023-03-12 07:09:41.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/GALEX_nuv.par
+-rw-r--r--   0 linlin     (501) staff       (20)    33010 2023-03-12 06:55:26.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_B.txt
+-rw-r--r--   0 linlin     (501) staff       (20)    32832 2022-08-15 07:41:16.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_I.txt
+-rw-r--r--   0 linlin     (501) staff       (20)    32753 2022-08-15 07:41:09.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_R.txt
+-rw-r--r--   0 linlin     (501) staff       (20)    33166 2022-08-18 09:37:49.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_U.txt
+-rw-r--r--   0 linlin     (501) staff       (20)    32964 2022-08-18 09:37:38.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_V.txt
+-rw-r--r--   0 linlin     (501) staff       (20)     4682 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_g.par
+-rw-r--r--   0 linlin     (501) staff       (20)     4682 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_i.par
+-rw-r--r--   0 linlin     (501) staff       (20)     4482 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_r.par
+-rw-r--r--   0 linlin     (501) staff       (20)     4782 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_u.par
+-rw-r--r--   0 linlin     (501) staff       (20)     5033 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_z.par
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/sed/
+-rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH-2_tau10_Ew50.fits
+-rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau1_Ewd.fits
+-rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew10_AGN1.fits
+-rw-r--r--   0 linlin     (501) staff       (20)    95040 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew5.fits
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/source/
+-rw-r--r--   0 linlin     (501) staff       (20)      413 2022-01-10 06:07:14.000000 ifs_etc-0.1.1/src/ifs_etc/refdata/source/config.json
+drwxr-xr-x   0 linlin     (501) staff       (20)        0 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc.egg-info/
+-rw-r--r--   0 linlin     (501) staff       (20)     3788 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc.egg-info/PKG-INFO
+-rw-r--r--   0 linlin     (501) staff       (20)     1770 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc.egg-info/SOURCES.txt
+-rw-r--r--   0 linlin     (501) staff       (20)        1 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc.egg-info/dependency_links.txt
+-rw-r--r--   0 linlin     (501) staff       (20)      137 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc.egg-info/requires.txt
+-rw-r--r--   0 linlin     (501) staff       (20)        8 2023-04-19 05:54:44.000000 ifs_etc-0.1.1/src/ifs_etc.egg-info/top_level.txt
```

### Comparing `ifs_etc-0.1.0/PKG-INFO` & `ifs_etc-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifs_etc
-Version: 0.1.0
+Version: 0.1.1
 Summary: exposure time calculator
 Home-page: UNKNOWN
 Author: linlin
 Author-email: linlin@shao.ac.cn
 License: UNKNOWN
 Description: # CSST-IFS ETC
```

### Comparing `ifs_etc-0.1.0/README.md` & `ifs_etc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/setup.py` & `ifs_etc-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc1d/config.py` & `ifs_etc-0.1.1/src/ifs_etc/etc1d/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     return dict
 
 
 
 def build_default_calc():
 
     calc = {}
-    calc['telescope'] = get_telescope_config()
+    # calc['telescope'] = get_telescope_config()
     calc['configuration'] = get_instrument_config()
     calc['source'] = build_default_source()
     calc['zodiacal_level'] = 'med'
     calc['earthshine_level'] = 'med'
     calc['repn'] = 20.
     calc['obst'] = 300.
```

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc1d/perform_calculation.py` & `ifs_etc-0.1.1/src/ifs_etc/etc1d/perform_calculation.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc1d/source.py` & `ifs_etc-0.1.1/src/ifs_etc/etc1d/source.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc2d/config.py` & `ifs_etc-0.1.1/src/ifs_etc/etc2d/config.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc2d/ifs_etc.py` & `ifs_etc-0.1.1/src/ifs_etc/etc2d/ifs_etc.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc2d/perform_calculation.py` & `ifs_etc-0.1.1/src/ifs_etc/etc2d/perform_calculation.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc2d/snpp.py` & `ifs_etc-0.1.1/src/ifs_etc/etc2d/snpp.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/etc2d/source.py` & `ifs_etc-0.1.1/src/ifs_etc/etc2d/source.py`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/earthshine_spec.csv` & `ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/earthshine_spec.csv`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/skybg_50_10.dat` & `ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/skybg_50_10.dat`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/csst/background/zodi_spec.csv` & `ifs_etc-0.1.1/src/ifs_etc/refdata/csst/background/zodi_spec.csv`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/csst/ifs/IFU_throughput.dat` & `ifs_etc-0.1.1/src/ifs_etc/refdata/csst/ifs/IFU_throughput.dat`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/GALEX_fuv.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/GALEX_fuv.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/GALEX_nuv.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/GALEX_nuv.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_B.txt` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_B.txt`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_I.txt` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_I.txt`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_R.txt` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_R.txt`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_U.txt` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_U.txt`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/Johnson_V.txt` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/Johnson_V.txt`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_g.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_g.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_i.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_i.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_r.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_r.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_u.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_u.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/normalization/filters/sdss_z.par` & `ifs_etc-0.1.1/src/ifs_etc/refdata/normalization/filters/sdss_z.par`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH-2_tau10_Ew50.fits` & `ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH-2_tau10_Ew50.fits`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau1_Ewd.fits` & `ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau1_Ewd.fits`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew10_AGN1.fits` & `ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew10_AGN1.fits`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew5.fits` & `ifs_etc-0.1.1/src/ifs_etc/refdata/sed/SFgal_texp_FeH0_tau5_Ew5.fits`

 * *Files identical despite different names*

### Comparing `ifs_etc-0.1.0/src/ifs_etc.egg-info/PKG-INFO` & `ifs_etc-0.1.1/src/ifs_etc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifs-etc
-Version: 0.1.0
+Version: 0.1.1
 Summary: exposure time calculator
 Home-page: UNKNOWN
 Author: linlin
 Author-email: linlin@shao.ac.cn
 License: UNKNOWN
 Description: # CSST-IFS ETC
```

### Comparing `ifs_etc-0.1.0/src/ifs_etc.egg-info/SOURCES.txt` & `ifs_etc-0.1.1/src/ifs_etc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

