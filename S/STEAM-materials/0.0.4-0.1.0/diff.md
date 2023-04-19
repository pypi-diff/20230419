# Comparing `tmp/STEAM_materials-0.0.4.tar.gz` & `tmp/STEAM_materials-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "STEAM_materials-0.0.4.tar", last modified: Wed Apr 19 07:05:37 2023, max compression
+gzip compressed data, was "STEAM_materials-0.1.0.tar", last modified: Wed Apr 19 07:07:09 2023, max compression
```

## Comparing `STEAM_materials-0.0.4.tar` & `STEAM_materials-0.1.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:37.879750 STEAM_materials-0.0.4/
--rw-rw-rw-   0        0        0       37 2022-04-11 08:27:26.000000 STEAM_materials-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      462 2023-04-19 07:05:37.879750 STEAM_materials-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       68 2022-04-05 13:59:57.000000 STEAM_materials-0.0.4/README.md
--rw-rw-rw-   0        0        0       86 2022-04-05 14:02:07.000000 STEAM_materials-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 07:05:37.879750 STEAM_materials-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-04-19 07:04:07.000000 STEAM_materials-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:37.801643 STEAM_materials-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:37.817267 STEAM_materials-0.0.4/src/STEAM_materials.egg-info/
--rw-rw-rw-   0        0        0      462 2023-04-19 07:05:37.000000 STEAM_materials-0.0.4/src/STEAM_materials.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2800 2023-04-19 07:05:37.000000 STEAM_materials-0.0.4/src/STEAM_materials.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:05:37.000000 STEAM_materials-0.0.4/src/STEAM_materials.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 07:05:37.000000 STEAM_materials-0.0.4/src/STEAM_materials.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 07:05:37.000000 STEAM_materials-0.0.4/src/STEAM_materials.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:37.817267 STEAM_materials-0.0.4/src/steammaterials/
-drwxrwxrwx   0        0        0        0 2023-04-19 07:05:37.879750 STEAM_materials-0.0.4/src/steammaterials/CFUN/
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/BHAir_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/BHIron2_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvAg_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvAl_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll
--rw-rw-rw-   0        0        0   124928 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvCu_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvG10_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvHast_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvHe_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:13.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvTi_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
--rw-rw-rw-   0        0        0   129536 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:17.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAg_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
--rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kBrass_v1.dll
--rw-rw-rw-   0        0        0   105472 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kCu_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kG10_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kHast_v1.dll
--rw-rw-rw-   0        0        0   124416 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kHe_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kKapton_v1.dll
--rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kSteel_v1.dll
--rw-rw-rw-   0        0        0   124416 2023-04-19 07:02:15.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kStycast_v1.dll
--rw-rw-rw-   0        0        0   105984 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_quenchState_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll
--rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll
--rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll
--rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:16.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll
--rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:17.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll
--rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-0.0.4/src/steammaterials/CFUN/__init__.py
--rw-rw-rw-   0        0        0     2874 2023-04-19 07:04:52.000000 STEAM_materials-0.0.4/src/steammaterials/STEAM_materials.py
--rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-0.0.4/src/steammaterials/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:07:09.445312 STEAM_materials-0.1.0/
+-rw-rw-rw-   0        0        0       37 2022-04-11 08:27:26.000000 STEAM_materials-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      462 2023-04-19 07:07:09.445312 STEAM_materials-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2022-04-05 13:59:57.000000 STEAM_materials-0.1.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-05 14:02:07.000000 STEAM_materials-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:07:09.445312 STEAM_materials-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-04-19 07:06:57.000000 STEAM_materials-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:07:09.365153 STEAM_materials-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:07:09.391452 STEAM_materials-0.1.0/src/STEAM_materials.egg-info/
+-rw-rw-rw-   0        0        0      462 2023-04-19 07:07:09.000000 STEAM_materials-0.1.0/src/STEAM_materials.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2800 2023-04-19 07:07:09.000000 STEAM_materials-0.1.0/src/STEAM_materials.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:07:09.000000 STEAM_materials-0.1.0/src/STEAM_materials.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 07:07:09.000000 STEAM_materials-0.1.0/src/STEAM_materials.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-19 07:07:09.000000 STEAM_materials-0.1.0/src/STEAM_materials.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 07:07:09.392485 STEAM_materials-0.1.0/src/steammaterials/
+drwxrwxrwx   0        0        0        0 2023-04-19 07:07:09.445312 STEAM_materials-0.1.0/src/steammaterials/CFUN/
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/BHAir_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/BHIron2_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvAg_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvAl_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:12.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll
+-rw-rw-rw-   0        0        0   124928 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvCu_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvG10_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvHast_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvHe_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:13.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvTi_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll
+-rw-rw-rw-   0        0        0   129536 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:17.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAg_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:14.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll
+-rw-rw-rw-   0        0        0   123904 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kBrass_v1.dll
+-rw-rw-rw-   0        0        0   105472 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kCu_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kG10_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kHast_v1.dll
+-rw-rw-rw-   0        0        0   124416 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kHe_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kKapton_v1.dll
+-rw-rw-rw-   0        0        0   122880 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kSteel_v1.dll
+-rw-rw-rw-   0        0        0   124416 2023-04-19 07:02:15.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kStycast_v1.dll
+-rw-rw-rw-   0        0        0   105984 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_quenchState_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll
+-rw-rw-rw-   0        0        0   125440 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll
+-rw-rw-rw-   0        0        0   125952 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll
+-rw-rw-rw-   0        0        0   123392 2023-04-19 07:02:16.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll
+-rw-rw-rw-   0        0        0   122368 2023-04-19 07:02:17.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll
+-rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-0.1.0/src/steammaterials/CFUN/__init__.py
+-rw-rw-rw-   0        0        0     2874 2023-04-19 07:04:52.000000 STEAM_materials-0.1.0/src/steammaterials/STEAM_materials.py
+-rw-rw-rw-   0        0        0        0 2022-04-05 14:16:54.000000 STEAM_materials-0.1.0/src/steammaterials/__init__.py
```

### Comparing `STEAM_materials-0.0.4/setup.py` & `STEAM_materials-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="STEAM_materials",
-    version="0.0.4",
+    version="0.1.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Python wrapper for the steam materials package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.cern.ch/steam/steam-material-library",
     keywords={'STEAM', 'API', 'MATERIALS', 'CERN'},
```

### Comparing `STEAM_materials-0.0.4/src/STEAM_materials.egg-info/SOURCES.txt` & `STEAM_materials-0.1.0/src/STEAM_materials.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/BHAir_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/BHAir_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/BHIron2_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/BHIron2_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvAg_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvAg_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvAl5083_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvAl_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvAl_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvBSCCO2212_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvBeCu_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvBrass_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvCu_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvCu_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvG10_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvG10_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvHast_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvHast_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvHe_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvHe_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvKapton_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvNb3Sn_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvNbTi_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvSteel_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_CvTi_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_CvTi_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_fK_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_HTS_CurrentSharing_f_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_HTS_JcFit_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_HiLumi_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_WithStress_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNb3Sn_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_IcNbTi_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_JcNbTiLowCurrent_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_QHCircuit_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_TcsNbTi_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAg_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAg_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAl1350_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAl5083_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kAl6061_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kBrass_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kBrass_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kCu_Wiedermann_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kCu_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kCu_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kG10_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kG10_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kHast_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kHast_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kHe_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kHe_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kKapton_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kKapton_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kSteel_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kSteel_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_kStycast_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_kStycast_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_quenchState_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_quenchState_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAgMg_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAg_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl1350_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl5083_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl6061_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoAl_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoCu_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoHast_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll` & `STEAM_materials-0.1.0/src/steammaterials/CFUN/CFUN_rhoSS_v1.dll`

 * *Files identical despite different names*

### Comparing `STEAM_materials-0.0.4/src/steammaterials/STEAM_materials.py` & `STEAM_materials-0.1.0/src/steammaterials/STEAM_materials.py`

 * *Files identical despite different names*

