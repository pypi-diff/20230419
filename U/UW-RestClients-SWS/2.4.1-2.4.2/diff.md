# Comparing `tmp/UW-RestClients-SWS-2.4.1.tar.gz` & `tmp/UW-RestClients-SWS-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-SWS-2.4.1.tar", last modified: Mon Mar 20 20:39:25 2023, max compression
+gzip compressed data, was "UW-RestClients-SWS-2.4.2.tar", last modified: Wed Apr 19 20:30:28 2023, max compression
```

## Comparing `UW-RestClients-SWS-2.4.1.tar` & `UW-RestClients-SWS-2.4.2.tar`

### file list

```diff
@@ -1,1198 +1,1198 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.455561 UW-RestClients-SWS-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-20 20:39:25.455561 UW-RestClients-SWS-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.311561 UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-20 20:39:25.000000 UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    77597 2023-03-20 20:39:25.000000 UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-20 20:39:25.000000 UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-03-20 20:39:25.000000 UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-20 20:39:25.000000 UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-20 20:39:25.455561 UW-RestClients-SWS-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.315561 UW-RestClients-SWS-2.4.1/uw_sws/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-20 20:39:24.000000 UW-RestClients-SWS-2.4.1/uw_sws/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/adviser.py
--rw-r--r--   0 runner    (1001) docker     (122)      868 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/campus.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/college.py
--rw-r--r--   0 runner    (1001) docker     (122)     6685 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/course.py
--rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/curriculum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4595 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/degree.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/department.py
--rw-r--r--   0 runner    (1001) docker     (122)     4426 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)      787 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/financial.py
--rw-r--r--   0 runner    (1001) docker     (122)    62197 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/notice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/person.py
--rw-r--r--   0 runner    (1001) docker     (122)    12563 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.271561 UW-RestClients-SWS-2.4.1/uw_sws/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.271561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.271561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.315561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/index.html
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/just_test.xhtml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.323561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/campus.json
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/college.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.295561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.323561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W/
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W/status.json
--rwxr-xr-x   0 runner    (1001) docker     (122)     3748 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_555/
--rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_555/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/
--rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/AD.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_M%20SCI_201/
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_M%20SCI_201/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/
--rw-r--r--   0 runner    (1001) docker     (122)     4347 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/CA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_O%20S_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_O%20S_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALB_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALB_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_545/
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_545/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_640/
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PEDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PEDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_640/
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PROS_640/
--rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PROS_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_510/
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_510/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_574/
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_574/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_581/
--rw-r--r--   0 runner    (1001) docker     (122)     3663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_581/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.327561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_585/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_585/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_591/
--rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_591/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_640/
--rw-r--r--   0 runner    (1001) docker     (122)     9077 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_650/
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_650/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.331561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9490 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2809 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_548/
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_548/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_555/
--rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_555/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_EDC_I_461/
--rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_EDC_I_461/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/
--rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/AD.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json
--rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/CA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.335561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_O%20S_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_O%20S_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALB_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3666 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALB_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3577 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_545/
--rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_545/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_640/
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PEDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PEDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3585 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.339561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_640/
--rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9463 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PROS_640/
--rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PROS_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/
--rw-r--r--   0 runner    (1001) docker     (122)     4458 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/
--rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/
--rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/
--rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_640/
--rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_650/
--rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_650/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_T%20BUS_310/
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_T%20BUS_310/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TEST_098/
--rw-r--r--   0 runner    (1001) docker     (122)     5133 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TEST_098/T.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_CSS_161/
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_CSS_161/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.343561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_EDC_I_461/
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_EDC_I_461/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ELCBUS_451/
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ELCBUS_451/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_101/
--rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_102/
--rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_102/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_495/
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_495/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.347561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9462 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_T%20BUS_310/
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_T%20BUS_310/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEDADM_572/
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEDADM_572/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEST_098/
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEST_098/T.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TMATH_110/
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TMATH_110/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_102/
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_102/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_103/
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_103/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_104/
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_104/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_EDC_I_461/
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_EDC_I_461/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_ELCBUS_451/
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_ELCBUS_451/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.351561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.355561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.355561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_495/
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_495/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.355561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_600/
--rw-r--r--   0 runner    (1001) docker     (122)     2841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_600/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.355561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEDADM_572/
--rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEDADM_572/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEST_098/
--rw-r--r--   0 runner    (1001) docker     (122)     5131 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEST_098/T.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TMATH_110/
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TMATH_110/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_102/
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_102/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_103/
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_103/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_104/
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_104/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ASIAN_203/
--rw-r--r--   0 runner    (1001) docker     (122)     3595 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ASIAN_203/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_C%20LIT_396/
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_C%20LIT_396/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DENT_552/
--rw-r--r--   0 runner    (1001) docker     (122)     3955 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DENT_552/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_503/
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_503/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_533/
--rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_533/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_590/
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_590/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_535/
--rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_535/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3701 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_530/
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_530/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_630/
--rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ORALM_532/
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ORALM_532/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.359561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PEDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PEDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.363561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_531/
--rw-r--r--   0 runner    (1001) docker     (122)     4059 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_531/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.363561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_631/
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_631/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.363561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PROS_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PROS_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.363561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_531/
--rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_531/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.363561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_630/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/curriculum.json_department_abbreviation_EDUC_future_terms_0
--rw-r--r--   0 runner    (1001) docker     (122)    88163 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/curriculum.json_quarter_winter_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/department.json_college_abbreviation_MED
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.363561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/enrollment/
--rw-r--r--   0 runner    (1001) docker     (122)     7034 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)     6837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.375561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_A_course_number_100_year_2013_quarter_winter
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_B_course_number_100_year_2013_quarter_winter
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active_on_section_id_A_course_number_100_year_2013_quarter_winter
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active_on_section_id_B_course_number_100_year_2013_quarter_winter
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     4222 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_on_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.375561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2012_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2012_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2012_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2014_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2014_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/current.json
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/next.json
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/previous.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.387561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/campus.json
--rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/college.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.387561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.387561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.387561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.387561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W/
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W/status.json
--rwxr-xr-x   0 runner    (1001) docker     (122)     3748 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.387561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_199/
--rwxr-xr-x   0 runner    (1001) docker     (122)     4080 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_199/W.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_555/
--rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_555/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/
--rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/AD.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_M%20SCI_201/
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_M%20SCI_201/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/
--rw-r--r--   0 runner    (1001) docker     (122)     4347 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/CA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_O%20S_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_O%20S_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALB_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALB_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_545/
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_545/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_640/
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PEDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PEDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_640/
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PROS_640/
--rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PROS_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_510/
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_510/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_574/
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_574/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_581/
--rw-r--r--   0 runner    (1001) docker     (122)     3663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_581/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_585/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_585/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_591/
--rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_591/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_640/
--rw-r--r--   0 runner    (1001) docker     (122)     9077 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.391561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_650/
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_650/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.395561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.395561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.395561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9490 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.395561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.395561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_101/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013,spring,ATMO%20S,142.json
--rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013,spring,CSE,142.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2809 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_548/
--rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_548/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_555/
--rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_555/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_EDC_I_461/
--rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_EDC_I_461/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/
--rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/AD.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/
--rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/
--rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json
--rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/CA.json
--rw-r--r--   0 runner    (1001) docker     (122)     4001 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/ZZ.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_O%20S_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_O%20S_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALB_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3666 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALB_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3577 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_545/
--rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_545/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_640/
--rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.399561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PEDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PEDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.403561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3585 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.403561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_640/
--rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9463 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PROS_640/
--rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PROS_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/
--rw-r--r--   0 runner    (1001) docker     (122)     4458 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/
--rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/
--rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/
--rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/
--rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json
--rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/C.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_540/
--rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_540/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_640/
--rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_640/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_650/
--rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_650/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_T%20BUS_310/
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_T%20BUS_310/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TEST_098/
--rw-r--r--   0 runner    (1001) docker     (122)     5133 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TEST_098/T.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.407561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_BIGDATA_230/
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_BIGDATA_230/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSHP_230/
--rw-r--r--   0 runner    (1001) docker     (122)     5386 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSHP_230/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSS_161/
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSS_161/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_EDC_I_461/
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_EDC_I_461/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_EFS_FAILT_101/
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_EFS_FAILT_101/AQ.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ELCBUS_451/
--rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ELCBUS_451/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ESS_107/
--rw-r--r--   0 runner    (1001) docker     (122)     5441 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ESS_107/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_101/
--rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_102/
--rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_102/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/GA.json
--rw-r--r--   0 runner    (1001) docker     (122)     3417 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/H.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_495/
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_495/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.411561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     2991 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.415561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9156 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.415561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_T%20BUS_310/
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_T%20BUS_310/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.415561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEDADM_572/
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEDADM_572/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.415561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEST_098/
--rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEST_098/T.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.415561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TMATH_110/
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TMATH_110/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_102/
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_102/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_103/
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_103/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_104/
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_104/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/AA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A/
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_EDC_I_461/
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_EDC_I_461/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_ELCBUS_451/
--rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_ELCBUS_451/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G/
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G/status.json
--rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G.json
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/GA.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.419561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHIL_495/
--rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHIL_495/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/
--rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AB.json
--rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AC.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AD.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AE.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AF.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AG.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AH.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AI.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AJ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AK.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AM.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AN.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AO.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AP.json
--rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AQ.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AR.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AS.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AT.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AU.json
--rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AV.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEDADM_572/
--rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEDADM_572/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEST_098/
--rw-r--r--   0 runner    (1001) docker     (122)     5131 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEST_098/T.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TMATH_110/
--rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TMATH_110/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AA.json
--rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AB.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_101/
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_101/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_102/
--rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_102/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.423561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_103/
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_103/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_104/
--rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_104/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ASIAN_203/
--rw-r--r--   0 runner    (1001) docker     (122)     3595 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ASIAN_203/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_BIGDATA_220/
--rw-r--r--   0 runner    (1001) docker     (122)     5328 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_BIGDATA_220/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_C%20LIT_396/
--rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_C%20LIT_396/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_COM_201/
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_COM_201/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DENT_552/
--rw-r--r--   0 runner    (1001) docker     (122)     3955 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DENT_552/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_503/
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_503/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_533/
--rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_533/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_590/
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_590/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_535/
--rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_535/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3701 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_JAVA_125/
--rw-r--r--   0 runner    (1001) docker     (122)     8279 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_JAVA_125/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_530/
--rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_530/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_630/
--rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ORALM_532/
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ORALM_532/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PEDO_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PEDO_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_531/
--rw-r--r--   0 runner    (1001) docker     (122)     4059 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_531/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_631/
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_631/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PROS_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PROS_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_531/
--rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_531/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_630/
--rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_630/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2017_autumn_EDC%26I_552/
--rw-r--r--   0 runner    (1001) docker     (122)     7809 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2017_autumn_EDC%26I_552/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/
--rw-r--r--   0 runner    (1001) docker     (122)     8280 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     7307 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.427561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_autumn_E%20E_233/
--rw-r--r--   0 runner    (1001) docker     (122)     9125 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_autumn_E%20E_233/A.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_summer_EDIT_120/
--rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_summer_EDIT_120/B.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_summer_PHIL_600/
--rw-r--r--   0 runner    (1001) docker     (122)     6666 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_summer_PHIL_600/A.json
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/curriculum.json_department_abbreviation_EDUC_future_terms_0_view_unpublished_false
--rw-r--r--   0 runner    (1001) docker     (122)    88163 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_false
--rw-r--r--   0 runner    (1001) docker     (122)    88163 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_true
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/department.json_college_abbreviation_MED
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_00000000000000000000000000000001.json
--rw-r--r--   0 runner    (1001) docker     (122)     7034 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)    10069 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_FE36CCB8F66711D5BE060004AC494FCD.json
--rw-r--r--   0 runner    (1001) docker     (122)     6837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_winter_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_00000000000000000000000000000001_verbose_true_transcriptable_course_all_changed_since_date_
--rw-r--r--   0 runner    (1001) docker     (122)    54400 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_verbose_true_transcriptable_course_all_changed_since_date_
--rw-r--r--   0 runner    (1001) docker     (122)    13273 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_verbose_true_transcriptable_course_all_changed_since_date_
--rw-r--r--   0 runner    (1001) docker     (122)    13436 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_verbose_true_transcriptable_course_all_changed_since_date_
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/00000000000000000000000000000001.json
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494F31.json
--rw-r--r--   0 runner    (1001) docker     (122)    10779 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)    11996 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494F31.json
--rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494FCD.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001/advisers.json.http-headers
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001/financial.json
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/advisers.json
--rw-r--r--   0 runner    (1001) docker     (122)      534 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/degree.json_deg_status_all
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/financial.json
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012.json
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/24A20F50AE3511D68CBC0004AC494FFE.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.431562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31/financial.json
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.435562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/advisers.json
--rw-r--r--   0 runner    (1001) docker     (122)      540 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/degree.json_deg_status_all
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/financial.json
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/registrationblock.json
--rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.435562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494F31/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494F31/financial.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.435562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494FCD/
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494FCD/financial.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.443561 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      838 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      842 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      837 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_ESS_107_A_FE36CCB8F66711D5BE060004AC494FCE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      667 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_BIGDATA_220_A_FE36CCB8F66711D5BE060004AC494F31_.json
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)      689 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json
--rw-r--r--   0 runner    (1001) docker     (122)     3787 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_A
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B
--rw-r--r--   0 runner    (1001) docker     (122)     8553 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B_transcriptable_course_all
--rw-r--r--   0 runner    (1001) docker     (122)      649 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_A
--rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_B
--rw-r--r--   0 runner    (1001) docker     (122)     4006 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_EDC_I_instructor_reg_id__course_number_552_verbose_true_year_2017_quarter_autumn_is_active_true_section_id_A_transcriptable_course_all
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     7723 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     4222 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2012_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     4523 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2012_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_true_year_2012
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1870 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_transcriptable_course_all_quarter_winter_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494FCE_transcriptable_course_no_quarter_spring_is_active_true_year_2013_verbose_on
--rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_true_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      990 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_transcriptable_course_all_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_quarter_winter_facility_code_KNE_year_2013
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_autumn_include_secondaries__year_2012_future_terms_4_transcriptable_course_all_delete_flag_active
--rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries__year_2013_future_terms_2_transcriptable_course_all_delete_flag_active
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_all_delete_flag_active
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.451562 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_sinter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2008_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2012_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2012_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2012_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2014_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2014_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2015_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2016_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1848 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_autumn.json
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2021_spring.json
--rw-r--r--   0 runner    (1001) docker     (122)     1922 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2021_summer.json
--rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2021_winter.json
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/current.json
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/next.json
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/previous.json
--rw-r--r--   0 runner    (1001) docker     (122)    22431 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/section.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/section_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/term.py
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:25.455561 UW-RestClients-SWS-2.4.1/uw_sws/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5556 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/compatible.py
--rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_adviser.py
--rw-r--r--   0 runner    (1001) docker     (122)      494 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_campus.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_college.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_course.py
--rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_curriculum.py
--rw-r--r--   0 runner    (1001) docker     (122)      565 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_degree.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_department.py
--rw-r--r--   0 runner    (1001) docker     (122)    12190 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (122)      811 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_financial.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_independent_study.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_instructor_no_regid.py
--rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_notice.py
--rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_person.py
--rw-r--r--   0 runner    (1001) docker     (122)    15233 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_registrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4728 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_schedule_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31016 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_section.py
--rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_section_status.py
--rw-r--r--   0 runner    (1001) docker     (122)    28764 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/tests/test_term.py
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/thread.py
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-03-20 20:39:15.000000 UW-RestClients-SWS-2.4.1/uw_sws/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.879031 UW-RestClients-SWS-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 20:30:28.879031 UW-RestClients-SWS-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.787030 UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 20:30:28.000000 UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    77597 2023-04-19 20:30:28.000000 UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 20:30:28.000000 UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-19 20:30:28.000000 UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-19 20:30:28.000000 UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 20:30:28.879031 UW-RestClients-SWS-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1271 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.791030 UW-RestClients-SWS-2.4.2/uw_sws/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-19 20:30:28.000000 UW-RestClients-SWS-2.4.2/uw_sws/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/adviser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      868 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/campus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/college.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6685 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/course.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2031 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4595 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/degree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/department.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5245 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/financial.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62111 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/notice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3374 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/person.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12563 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.767030 UW-RestClients-SWS-2.4.2/uw_sws/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.767030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.767030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.791030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/just_test.xhtml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/campus.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/college.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.775030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W/
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W/status.json
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3748 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_555/
+-rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_555/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/
+-rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/AD.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_M%20SCI_201/
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_M%20SCI_201/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/
+-rw-r--r--   0 runner    (1001) docker     (122)     4347 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/CA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_O%20S_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_O%20S_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALB_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALB_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_545/
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_545/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PEDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PEDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.795030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PROS_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PROS_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_510/
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_510/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_574/
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_574/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_581/
+-rw-r--r--   0 runner    (1001) docker     (122)     3663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_581/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_585/
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_585/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_591/
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_591/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     9077 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_650/
+-rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_650/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9490 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.799030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2809 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_548/
+-rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_548/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_555/
+-rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_555/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_EDC_I_461/
+-rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_EDC_I_461/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/
+-rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/AD.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/CA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_O%20S_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_O%20S_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALB_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3666 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALB_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3577 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_545/
+-rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_545/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PEDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PEDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3585 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.803030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9463 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PROS_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PROS_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/
+-rw-r--r--   0 runner    (1001) docker     (122)     4458 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/
+-rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_650/
+-rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_650/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_T%20BUS_310/
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_T%20BUS_310/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TEST_098/
+-rw-r--r--   0 runner    (1001) docker     (122)     5133 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TEST_098/T.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_CSS_161/
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_CSS_161/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_EDC_I_461/
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_EDC_I_461/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ELCBUS_451/
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ELCBUS_451/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_102/
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_102/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_495/
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_495/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.807030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9462 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_T%20BUS_310/
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_T%20BUS_310/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEDADM_572/
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEDADM_572/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEST_098/
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEST_098/T.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TMATH_110/
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TMATH_110/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_102/
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_102/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_103/
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_103/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_104/
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_104/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_EDC_I_461/
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_EDC_I_461/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.811030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_ELCBUS_451/
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_ELCBUS_451/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_495/
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_495/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_600/
+-rw-r--r--   0 runner    (1001) docker     (122)     2841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_600/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEDADM_572/
+-rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEDADM_572/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEST_098/
+-rw-r--r--   0 runner    (1001) docker     (122)     5131 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEST_098/T.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TMATH_110/
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TMATH_110/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_102/
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_102/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_103/
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_103/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_104/
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_104/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ASIAN_203/
+-rw-r--r--   0 runner    (1001) docker     (122)     3595 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ASIAN_203/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_C%20LIT_396/
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_C%20LIT_396/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.815030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DENT_552/
+-rw-r--r--   0 runner    (1001) docker     (122)     3955 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DENT_552/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_503/
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_503/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_533/
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_533/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_590/
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_590/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_535/
+-rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_535/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3701 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_530/
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_530/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ORALM_532/
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ORALM_532/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PEDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PEDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_531/
+-rw-r--r--   0 runner    (1001) docker     (122)     4059 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_531/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_631/
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_631/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PROS_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PROS_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_531/
+-rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_531/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_630/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/curriculum.json_department_abbreviation_EDUC_future_terms_0
+-rw-r--r--   0 runner    (1001) docker     (122)    88163 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/curriculum.json_quarter_winter_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/department.json_college_abbreviation_MED
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.819030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/enrollment/
+-rw-r--r--   0 runner    (1001) docker     (122)     7034 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.827030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_A_course_number_100_year_2013_quarter_winter
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_B_course_number_100_year_2013_quarter_winter
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active_on_section_id_A_course_number_100_year_2013_quarter_winter
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active_on_section_id_B_course_number_100_year_2013_quarter_winter
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     4222 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1947 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1949 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1365 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_on_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.827030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2012_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2012_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2012_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2014_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2014_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/current.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/next.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/previous.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/campus.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6111 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/college.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W/
+-rw-r--r--   0 runner    (1001) docker     (122)      563 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W/status.json
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3748 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_199/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4080 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_199/W.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4793 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_555/
+-rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_555/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     5255 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/
+-rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/AD.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_M%20SCI_201/
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_M%20SCI_201/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/
+-rw-r--r--   0 runner    (1001) docker     (122)     4347 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/CA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.835030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_O%20S_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4967 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_O%20S_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALB_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALB_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_545/
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_545/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PEDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PEDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3584 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PROS_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PROS_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_510/
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_510/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_574/
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_574/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_581/
+-rw-r--r--   0 runner    (1001) docker     (122)     3663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_581/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_585/
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_585/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_591/
+-rw-r--r--   0 runner    (1001) docker     (122)     3835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_591/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     9077 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_650/
+-rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_650/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.839030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9490 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_101/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013,spring,ATMO%20S,142.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1608 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013,spring,CSE,142.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3713 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2809 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2979 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_548/
+-rw-r--r--   0 runner    (1001) docker     (122)     4104 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_548/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_555/
+-rw-r--r--   0 runner    (1001) docker     (122)     3958 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_555/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_EDC_I_461/
+-rw-r--r--   0 runner    (1001) docker     (122)     2902 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_EDC_I_461/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/
+-rw-r--r--   0 runner    (1001) docker     (122)     4226 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3142 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4459 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/AD.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/
+-rw-r--r--   0 runner    (1001) docker     (122)     3576 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3170 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4348 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/CA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4001 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/ZZ.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_O%20S_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4965 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_O%20S_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALB_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3666 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALB_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3577 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_545/
+-rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_545/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     4858 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PEDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     4029 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PEDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3585 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.843030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     6461 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9463 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PROS_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     9079 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PROS_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/
+-rw-r--r--   0 runner    (1001) docker     (122)     4458 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4746 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/
+-rw-r--r--   0 runner    (1001) docker     (122)     4062 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4324 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/
+-rw-r--r--   0 runner    (1001) docker     (122)     3446 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/
+-rw-r--r--   0 runner    (1001) docker     (122)     3510 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/
+-rw-r--r--   0 runner    (1001) docker     (122)     3603 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/C.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_540/
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_540/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_640/
+-rw-r--r--   0 runner    (1001) docker     (122)     8344 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_640/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_650/
+-rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_650/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_T%20BUS_310/
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_T%20BUS_310/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TEST_098/
+-rw-r--r--   0 runner    (1001) docker     (122)     5133 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TEST_098/T.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3217 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     2765 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3618 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_BIGDATA_230/
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_BIGDATA_230/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.847030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSHP_230/
+-rw-r--r--   0 runner    (1001) docker     (122)     5386 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSHP_230/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSS_161/
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSS_161/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_EDC_I_461/
+-rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_EDC_I_461/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_EFS_FAILT_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_EFS_FAILT_101/AQ.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ELCBUS_451/
+-rw-r--r--   0 runner    (1001) docker     (122)     3086 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ELCBUS_451/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ESS_107/
+-rw-r--r--   0 runner    (1001) docker     (122)     5441 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ESS_107/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_102/
+-rw-r--r--   0 runner    (1001) docker     (122)     3109 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_102/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/GA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3417 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/H.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_495/
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_495/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2991 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9156 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2978 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2887 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_T%20BUS_310/
+-rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_T%20BUS_310/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEDADM_572/
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEDADM_572/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEST_098/
+-rw-r--r--   0 runner    (1001) docker     (122)     5132 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEST_098/T.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.851030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TMATH_110/
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TMATH_110/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3216 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     3082 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_102/
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_102/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_103/
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_103/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_104/
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_104/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2789 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/AA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A/
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3090 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_EDC_I_461/
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_EDC_I_461/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_ELCBUS_451/
+-rw-r--r--   0 runner    (1001) docker     (122)     3052 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_ELCBUS_451/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G/
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G/status.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3629 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/GA.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHIL_495/
+-rw-r--r--   0 runner    (1001) docker     (122)     2810 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHIL_495/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/
+-rw-r--r--   0 runner    (1001) docker     (122)     9502 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AB.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2989 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AC.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AF.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AG.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AH.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AI.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AJ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AK.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AM.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AN.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AO.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AP.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AQ.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AR.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AS.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AT.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AU.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2896 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AV.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.855030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEDADM_572/
+-rw-r--r--   0 runner    (1001) docker     (122)     2861 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEDADM_572/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEST_098/
+-rw-r--r--   0 runner    (1001) docker     (122)     5131 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEST_098/T.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TMATH_110/
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TMATH_110/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3220 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AA.json
+-rw-r--r--   0 runner    (1001) docker     (122)     2542 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AB.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_101/
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_101/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_102/
+-rw-r--r--   0 runner    (1001) docker     (122)     2631 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_102/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_103/
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_103/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_104/
+-rw-r--r--   0 runner    (1001) docker     (122)     2633 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_104/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ASIAN_203/
+-rw-r--r--   0 runner    (1001) docker     (122)     3595 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ASIAN_203/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_BIGDATA_220/
+-rw-r--r--   0 runner    (1001) docker     (122)     5328 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_BIGDATA_220/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_C%20LIT_396/
+-rw-r--r--   0 runner    (1001) docker     (122)     2993 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_C%20LIT_396/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_COM_201/
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_COM_201/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DENT_552/
+-rw-r--r--   0 runner    (1001) docker     (122)     3955 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DENT_552/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_503/
+-rw-r--r--   0 runner    (1001) docker     (122)     2976 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_503/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_533/
+-rw-r--r--   0 runner    (1001) docker     (122)     2996 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_533/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_590/
+-rw-r--r--   0 runner    (1001) docker     (122)     2793 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_590/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_535/
+-rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_535/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3701 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_JAVA_125/
+-rw-r--r--   0 runner    (1001) docker     (122)     8279 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_JAVA_125/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_530/
+-rw-r--r--   0 runner    (1001) docker     (122)     4160 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_530/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     5912 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ORALM_532/
+-rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ORALM_532/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PEDO_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3722 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PEDO_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_531/
+-rw-r--r--   0 runner    (1001) docker     (122)     4059 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_531/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_631/
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_631/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PROS_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3609 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PROS_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_531/
+-rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_531/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_630/
+-rw-r--r--   0 runner    (1001) docker     (122)     3039 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_630/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2017_autumn_EDC%26I_552/
+-rw-r--r--   0 runner    (1001) docker     (122)     7809 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2017_autumn_EDC%26I_552/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/
+-rw-r--r--   0 runner    (1001) docker     (122)     8280 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7307 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_autumn_E%20E_233/
+-rw-r--r--   0 runner    (1001) docker     (122)     9125 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_autumn_E%20E_233/A.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.859030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_summer_EDIT_120/
+-rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_summer_EDIT_120/B.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_summer_PHIL_600/
+-rw-r--r--   0 runner    (1001) docker     (122)     6666 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_summer_PHIL_600/A.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/curriculum.json_department_abbreviation_EDUC_future_terms_0_view_unpublished_false
+-rw-r--r--   0 runner    (1001) docker     (122)    88163 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_false
+-rw-r--r--   0 runner    (1001) docker     (122)    88163 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_true
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/department.json_college_abbreviation_MED
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_00000000000000000000000000000001.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7034 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10069 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_FE36CCB8F66711D5BE060004AC494FCD.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4774 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_winter_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_00000000000000000000000000000001_verbose_true_transcriptable_course_all_changed_since_date_
+-rw-r--r--   0 runner    (1001) docker     (122)    54400 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_verbose_true_transcriptable_course_all_changed_since_date_
+-rw-r--r--   0 runner    (1001) docker     (122)    13401 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_verbose_true_transcriptable_course_all_changed_since_date_
+-rw-r--r--   0 runner    (1001) docker     (122)    13436 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_verbose_true_transcriptable_course_all_changed_since_date_
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/00000000000000000000000000000001.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494F31.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10779 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)    11996 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494F31.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494FCD.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001/
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001/advisers.json.http-headers
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001/financial.json
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/advisers.json
+-rw-r--r--   0 runner    (1001) docker     (122)      534 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/degree.json_deg_status_all
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/financial.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/24A20F50AE3511D68CBC0004AC494FFE.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31/financial.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/advisers.json
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/degree.json_deg_status_all
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/financial.json
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/registrationblock.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1381 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494F31/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494F31/financial.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.863031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494FCD/
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/FE36CCB8F66711D5BE060004AC494FCD/financial.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.871030 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      838 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      842 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_ESS_107_A_FE36CCB8F66711D5BE060004AC494FCE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      699 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_BIGDATA_220_A_FE36CCB8F66711D5BE060004AC494F31_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      690 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)      689 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json
+-rw-r--r--   0 runner    (1001) docker     (122)     3787 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_A
+-rw-r--r--   0 runner    (1001) docker     (122)     5368 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B
+-rw-r--r--   0 runner    (1001) docker     (122)     8553 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B_transcriptable_course_all
+-rw-r--r--   0 runner    (1001) docker     (122)      649 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_A
+-rw-r--r--   0 runner    (1001) docker     (122)     2224 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_B
+-rw-r--r--   0 runner    (1001) docker     (122)     4006 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_EDC_I_instructor_reg_id__course_number_552_verbose_true_year_2017_quarter_autumn_is_active_true_section_id_A_transcriptable_course_all
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1421 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     7723 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     4971 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     4222 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     2053 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2012_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     2069 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     4523 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     3762 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2012_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     1088 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1804 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1415 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_true_year_2012
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1870 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_transcriptable_course_all_quarter_winter_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     1573 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494FCE_transcriptable_course_no_quarter_spring_is_active_true_year_2013_verbose_on
+-rw-r--r--   0 runner    (1001) docker     (122)     5760 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     5761 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_true_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_transcriptable_course_all_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_quarter_winter_facility_code_KNE_year_2013
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_autumn_include_secondaries__year_2012_future_terms_4_transcriptable_course_all_delete_flag_active
+-rw-r--r--   0 runner    (1001) docker     (122)     1665 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries__year_2013_future_terms_2_transcriptable_course_all_delete_flag_active
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_all_delete_flag_active
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.875031 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_sinter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1356 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1844 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2008_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2012_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2012_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2012_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1124 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2014_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1118 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2014_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2015_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2016_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1362 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1442 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1848 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_autumn.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1841 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2021_spring.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1922 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2021_summer.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1840 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2021_winter.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/current.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/next.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/previous.json
+-rw-r--r--   0 runner    (1001) docker     (122)    22431 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/section.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/section_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3878 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/term.py
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:28.879031 UW-RestClients-SWS-2.4.2/uw_sws/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5556 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/compatible.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_adviser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      494 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_campus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_college.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_course.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_degree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12513 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      811 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_financial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_independent_study.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_instructor_no_regid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6201 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_notice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6229 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15233 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_registrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4728 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_schedule_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31016 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1373 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_section_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28764 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/tests/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/thread.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-04-19 20:30:19.000000 UW-RestClients-SWS-2.4.2/uw_sws/util.py
```

### Comparing `UW-RestClients-SWS-2.4.1/LICENSE` & `UW-RestClients-SWS-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/PKG-INFO` & `UW-RestClients-SWS-2.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-SWS
-Version: 2.4.1
+Version: 2.4.2
 Summary: A library for connecting to the SWS at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-sws
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-SWS-2.4.1/README.md` & `UW-RestClients-SWS-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/PKG-INFO` & `UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-SWS
-Version: 2.4.1
+Version: 2.4.2
 Summary: A library for connecting to the SWS at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-sws
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-SWS-2.4.1/UW_RestClients_SWS.egg-info/SOURCES.txt` & `UW-RestClients-SWS-2.4.2/UW_RestClients_SWS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/setup.py` & `UW-RestClients-SWS-2.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/__init__.py` & `UW-RestClients-SWS-2.4.2/uw_sws/__init__.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/adviser.py` & `UW-RestClients-SWS-2.4.2/uw_sws/adviser.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/campus.py` & `UW-RestClients-SWS-2.4.2/uw_sws/campus.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/college.py` & `UW-RestClients-SWS-2.4.2/uw_sws/college.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/compat.py` & `UW-RestClients-SWS-2.4.2/uw_sws/compat.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/course.py` & `UW-RestClients-SWS-2.4.2/uw_sws/course.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/curriculum.py` & `UW-RestClients-SWS-2.4.2/uw_sws/curriculum.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/dao.py` & `UW-RestClients-SWS-2.4.2/uw_sws/dao.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/degree.py` & `UW-RestClients-SWS-2.4.2/uw_sws/degree.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/department.py` & `UW-RestClients-SWS-2.4.2/uw_sws/department.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/exceptions.py` & `UW-RestClients-SWS-2.4.2/uw_sws/exceptions.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/financial.py` & `UW-RestClients-SWS-2.4.2/uw_sws/financial.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/models.py` & `UW-RestClients-SWS-2.4.2/uw_sws/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1396,16 +1396,15 @@
         self.qtr_non_grd_earned = json_data.get('QtrNonGrdEarned')
         self.is_honors = json_data.get('HonorsProgram', False)
         self.has_pending_major_change = json_data.get(
             'PendingMajorChange', False)
         self.is_enroll_src_pce = self._is_src_location_pce(
             json_data.get('Metadata', ''), ENROLLMENT_SOURCE_PCE)
 
-        self.term = Term(year=int(json_data["Term"]["Year"]),
-                         quarter=json_data["Term"]["Quarter"])
+        self.term = kwargs.get("term")
 
         registrations = json_data.get('Registrations', [])
         self.is_registered = len(registrations) > 0
         for json_reg in registrations:
             registration = Registration(data=json_reg)
             registration.section = SectionReference(
                 term=self.term,
```

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/notice.py` & `UW-RestClients-SWS-2.4.2/uw_sws/notice.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/person.py` & `UW-RestClients-SWS-2.4.2/uw_sws/person.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/registration.py` & `UW-RestClients-SWS-2.4.2/uw_sws/registration.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/index.html` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/index.html`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/campus.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/campus.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/college.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/college.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_CSE_100/W.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_548/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_555/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_DENT_555/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ENGL_207/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_M%20SCI_201/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_M%20SCI_201/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/CA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_MATH_120/CA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_O%20S_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_O%20S_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALB_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALB_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_545/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_545/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_ORALM_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PEDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PEDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PERIO_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PROS_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_PROS_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_510/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_510/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_574/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_574/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_581/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_581/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_585/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_585/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_591/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_REHAB_591/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_650/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_autumn_RES%20D_650/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2012_summer_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_548/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_548/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_555/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_DENT_555/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_EDC_I_461/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_EDC_I_461/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ENGL_207/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_M%20SCI_201/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/CA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_120/CA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_O%20S_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_O%20S_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALB_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALB_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_545/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_545/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_ORALM_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PEDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PEDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PERIO_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PROS_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_PROS_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_510/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_574/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_581/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_585/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_REHAB_591/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_650/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_RES%20D_650/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_T%20BUS_310/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_T%20BUS_310/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TEST_098/T.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TEST_098/T.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_autumn_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_CSS_161/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_CSS_161/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_EDC_I_461/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_EDC_I_461/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ELCBUS_451/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ELCBUS_451/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_102/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_ErrFX_102/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_495/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_495/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHIL_600/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_T%20BUS_310/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_T%20BUS_310/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEDADM_572/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEDADM_572/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEST_098/T.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TEST_098/T.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TMATH_110/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TMATH_110/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_102/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_102/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_103/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_103/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_104/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_spring_TRAIN_104/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSE_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_CSS_161/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_EDC_I_461/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_EDC_I_461/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_ELCBUS_451/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_ELCBUS_451/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_495/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_495/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_600/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHIL_600/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEDADM_572/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEDADM_572/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEST_098/T.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TEST_098/T.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TMATH_110/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TMATH_110/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_102/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_102/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_103/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_103/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_104/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_summer_TRAIN_104/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ASIAN_203/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ASIAN_203/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_C%20LIT_396/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_C%20LIT_396/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DENT_552/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DENT_552/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_DROP_T_100/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_503/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_503/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_533/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_533/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_590/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_EMBA_590/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_535/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_535/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ENDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_530/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_530/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_O%20S_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_ORALM_532/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_ORALM_532/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PEDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PEDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_531/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_531/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_631/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PERIO_631/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_PROS_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_PROS_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_531/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_531/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/course/2013_winter_RES%20D_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/curriculum.json_department_abbreviation_EDUC_future_terms_0` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/curriculum.json_department_abbreviation_EDUC_future_terms_0`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/curriculum.json_quarter_winter_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/curriculum.json_quarter_winter_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/department.json_college_abbreviation_MED` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/department.json_college_abbreviation_MED`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_A_course_number_100_year_2013_quarter_winter` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_A_course_number_100_year_2013_quarter_winter`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_B_course_number_100_year_2013_quarter_winter` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active__section_id_B_course_number_100_year_2013_quarter_winter`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active_on_section_id_B_course_number_100_year_2013_quarter_winter` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_instructor_reg_id__curriculum_abbreviation_DROP_T_is_active_on_section_id_B_course_number_100_year_2013_quarter_winter`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_on_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_on_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2012_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2012_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2012_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2012_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2012_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2012_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2013_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2013_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2014_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2014_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/2014_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/2014_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/current.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/current.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/next.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/next.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v4/term/previous.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v4/term/previous.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/campus.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/campus.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/college.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/college.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_100/W.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_199/W.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_CSE_199/W.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_548/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_555/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_DENT_555/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ENGL_207/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_M%20SCI_201/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_M%20SCI_201/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/CA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_MATH_120/CA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_O%20S_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_O%20S_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALB_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALB_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_545/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_545/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_ORALM_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PEDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PEDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PERIO_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PROS_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_PROS_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_510/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_510/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_574/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_574/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_581/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_581/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_585/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_585/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_591/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_REHAB_591/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_650/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_autumn_RES%20D_650/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2012_summer_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013,spring,ATMO%20S,142.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013,spring,ATMO%20S,142.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013,spring,CSE,142.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013,spring,CSE,142.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/2012_autumn_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_548/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_548/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_555/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_DENT_555/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_EDC_I_461/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_EDC_I_461/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/2012_autumn_ENGL_207/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ENGL_207/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/2012_autumn_M%20SCI_201/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_M%20SCI_201/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/2012_autumn_MATH_120/CA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/CA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/CA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/ZZ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_120/ZZ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_O%20S_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_O%20S_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALB_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALB_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_545/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_545/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_ORALM_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PEDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PEDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PERIO_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PROS_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_PROS_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/2012_autumn_REHAB_510/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_510/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/2012_autumn_REHAB_574/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_574/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/2012_autumn_REHAB_581/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_581/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/2012_autumn_REHAB_585/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_585/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/2012_autumn_REHAB_591/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/C.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_REHAB_591/C.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_540/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_540/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_640/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_640/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_650/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_RES%20D_650/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_T%20BUS_310/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_T%20BUS_310/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TEST_098/T.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TEST_098/T.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_autumn_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_BIGDATA_230/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_BIGDATA_230/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSHP_230/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSHP_230/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSS_161/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_CSS_161/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_EDC_I_461/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_EDC_I_461/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_EFS_FAILT_101/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_EFS_FAILT_101/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ELCBUS_451/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ELCBUS_451/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ESS_107/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ESS_107/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_102/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_ErrFX_102/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/H.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_MATH_125/H.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_495/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_495/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHIL_600/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_T%20BUS_310/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_T%20BUS_310/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEDADM_572/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEDADM_572/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEST_098/T.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TEST_098/T.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TMATH_110/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TMATH_110/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_102/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_102/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_103/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_103/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_104/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_spring_TRAIN_104/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_B%20BIO_180/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSE_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_CSS_161/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_EDC_I_461/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_EDC_I_461/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_ELCBUS_451/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_ELCBUS_451/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G/status.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G/status.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/G.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/GA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_MATH_125/GA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHIL_495/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHIL_495/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AF.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AF.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AG.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AG.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AH.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AH.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AI.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AI.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AJ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AJ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AK.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AK.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AM.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AM.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AN.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AN.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AO.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AO.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AP.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AP.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AQ.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AQ.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AR.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AR.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AS.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AS.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AT.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AT.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AU.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AU.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AV.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_PHYS_121/AV.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEDADM_572/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEDADM_572/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEST_098/T.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TEST_098/T.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TMATH_110/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TMATH_110/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AA.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AA.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AB.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_100/AB.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_101/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_101/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_102/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_102/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_103/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_103/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_104/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_summer_TRAIN_104/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ASIAN_203/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ASIAN_203/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_BIGDATA_220/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_BIGDATA_220/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_C%20LIT_396/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_C%20LIT_396/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_COM_201/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_COM_201/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DENT_552/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DENT_552/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_DROP_T_100/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_503/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_503/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_533/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_533/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_590/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_EMBA_590/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_535/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_535/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ENDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_JAVA_125/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_JAVA_125/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_530/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_530/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_O%20S_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_ORALM_532/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_ORALM_532/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PEDO_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PEDO_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_531/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_531/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_631/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PERIO_631/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_PROS_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_PROS_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_531/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_531/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_630/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2013_winter_RES%20D_630/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2017_autumn_EDC%26I_552/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2017_autumn_EDC%26I_552/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2018_winter_INFX_543/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_autumn_E%20E_233/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_autumn_E%20E_233/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_summer_EDIT_120/B.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_summer_EDIT_120/B.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/course/2020_summer_PHIL_600/A.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/course/2020_summer_PHIL_600/A.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/curriculum.json_department_abbreviation_EDUC_future_terms_0_view_unpublished_false` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/curriculum.json_department_abbreviation_EDUC_future_terms_0_view_unpublished_false`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_false` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_false`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_true` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/curriculum.json_quarter_winter_year_2013_view_unpublished_true`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/department.json_college_abbreviation_MED` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/department.json_college_abbreviation_MED`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_FE36CCB8F66711D5BE060004AC494FCD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_spring_FE36CCB8F66711D5BE060004AC494FCD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_summer_9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment/2013_winter_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment/2013_winter_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_verbose_true_transcriptable_course_all_changed_since_date_` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_verbose_true_transcriptable_course_all_changed_since_date_`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_verbose_true_transcriptable_course_all_changed_since_date_` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_verbose_true_transcriptable_course_all_changed_since_date_`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8622186016333616%*

 * *Differences: {"'Current'": "{'Href': "*

 * *              "'/student/v5/enrollment.json?reg_id=FE36CCB8F66711D5BE060004AC494F31&verbose=true&changed_since_date=&transcriptable_course=all', "*

 * *              "'RegID': 'FE36CCB8F66711D5BE060004AC494F31'}",*

 * * "'Enrollments'": "{0: {'ClassLevel': 'BLANK', 'EnrollmentStatus': None, 'EnrollmentStatusDate': "*

 * *                  "'', 'FullName': 'Jessie New Student', 'Majors': [], 'Metadata': "*

 * *                  "'EnrollmentSourceLocation=EOS;', 'Person': {'Href': "*

 * *                  "' […]*

```diff
@@ -1,317 +1,318 @@
 {
     "Current": {
-        "Href": "/student/v5/enrollment.json?reg_id=AABBCCDDEEFFAABBCCDDEEFFAABBCCDC&verbose=true&changed_since_date=&transcriptable_course=all",
-        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC",
+        "Href": "/student/v5/enrollment.json?reg_id=FE36CCB8F66711D5BE060004AC494F31&verbose=true&changed_since_date=&transcriptable_course=all",
+        "RegID": "FE36CCB8F66711D5BE060004AC494F31",
         "Verbose": true
     },
     "Enrollments": [
         {
-            "ClassLevel": "NON_MATRIC",
+            "ClassLevel": "BLANK",
             "CurrentRegisteredCredits": null,
-            "EnrollmentStatus": "Registered",
-            "EnrollmentStatusDate": "2013-01-25",
-            "FullName": "Late Pce",
+            "EnrollmentStatus": null,
+            "EnrollmentStatusDate": "",
+            "FullName": "Jessie New Student",
             "HonorsProgram": false,
             "LeaveEndQuarter": 0,
             "LeaveEndYear": 0,
-            "Majors": [
-                {
-                    "Abbreviation": "N MATR",
-                    "Campus": "Seattle",
-                    "CollegeAbbreviation": "INDUG",
-                    "CollegeFullName": "INTERDISCIPLINARY UNDERGRADUATE PROGRAMS",
-                    "DegreeLevel": 0,
-                    "DegreeName": null,
-                    "DegreeType": 0,
-                    "FullName": "Non Matriculated",
-                    "MajorName": "NON MATRICULATED",
-                    "Pathway": 0,
-                    "ShortName": "N MATR"
-                }
-            ],
-            "Metadata": "EnrollmentSourceLocation=SDB_EOS;",
+            "Majors": [],
+            "Metadata": "EnrollmentSourceLocation=EOS;",
             "Minors": [],
             "PendingClassChange": false,
             "PendingHonorsChange": false,
             "PendingMajorChange": false,
             "PendingResidentChange": false,
             "PendingSpecialProgramChange": false,
             "Person": {
-                "Href": "/student/v5/person/27844DAE1712511A4FA00C83BAF90A8F.json",
-                "Name": "Late Pce",
-                "RegID": "27844DAE1712511A4FA00C83BAF90A8F"
+                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                "Name": "Jessie New Student",
+                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
             },
-            "QtrGradePoints": 0.0,
-            "QtrGradedAttmp": 0.0,
-            "QtrNonGrdEarned": 0.0,
-            "RegID": "27844DAE1712511A4FA00C83BAF90A8F",
+            "QtrGradePoints": null,
+            "QtrGradedAttmp": null,
+            "QtrNonGrdEarned": null,
+            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
             "Registrations": [
                 {
-                    "AccessDateRangeEnd": "07/25/2013",
-                    "AccessDateRangeStart": "12/19/2012",
-                    "Auditor": false,
-                    "Credits": "5.0",
-                    "DuplicateCode": "0",
-                    "EducationUnitType": null,
-                    "EndDate": "04/29/2013",
-                    "FeeBaseType": "",
-                    "Grade": "X",
-                    "GradeDate": "",
-                    "GradeDocumentID": "",
-                    "GradingSystem": null,
-                    "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,winter,COM,201,A,27844DAE1712511A4FA00C83BAF90A8F,0.json",
-                    "Instructor": null,
-                    "IsActive": true,
-                    "IsCredit": true,
-                    "IsIndependentStart": true,
-                    "Metadata": "RegistrationSourceLocation=SDB_EOS;",
-                    "Person": {
-                        "Href": "/student/v5/person/27844DAE1712511A4FA00C83BAF90A8F.json",
-                        "Name": "Late Pce",
-                        "RegID": "27844DAE1712511A4FA00C83BAF90A8F"
-                    },
-                    "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:16:41 PM",
-                    "RequestDate": "",
-                    "RequestStatus": "",
-                    "Section": {
-                        "CourseNumber": "201",
-                        "CurriculumAbbreviation": "COM",
-                        "Href": "/student/v5/course/2013,winter,COM,201/A.json",
-                        "Quarter": "winter",
-                        "SectionID": "A",
-                        "Year": 2013
-                    },
-                    "StartDate": "01/30/2013",
-                    "VariableCredit": false,
-                    "WritingCourse": false
-                },
-                {
-                    "AccessDateRangeEnd": "07/25/2013",
-                    "AccessDateRangeStart": "12/19/2012",
+                    "AccessDateRangeEnd": "03/10/2014",
+                    "AccessDateRangeStart": "12/28/2012",
                     "Auditor": false,
-                    "Credits": "4.0",
-                    "DuplicateCode": "0",
-                    "EducationUnitType": null,
-                    "EndDate": "04/30/2013",
+                    "Credits": "0.0",
+                    "DuplicateCode": "",
+                    "EducationUnitType": "CEU",
+                    "EndDate": "03/20/2013",
                     "FeeBaseType": "",
-                    "Grade": "X",
-                    "GradeDate": "",
+                    "Grade": "SC",
+                    "GradeDate": "3/22/2013 3:44:00 PM",
                     "GradeDocumentID": "",
-                    "GradingSystem": null,
+                    "GradingSystem": "SCUSC",
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,winter,PSYCH,203,A,27844DAE1712511A4FA00C83BAF90A8F,0.json",
+                    "Href": "/student/v5/registration/2013,winter,BIGDATA,220,A,FE36CCB8F66711D5BE060004AC494F31,.json",
                     "Instructor": null,
                     "IsActive": true,
-                    "IsCredit": true,
+                    "IsCredit": false,
                     "IsIndependentStart": false,
-                    "Metadata": "RegistrationSourceLocation=SDB;",
+                    "Metadata": "RegistrationSourceLocation=EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/27844DAE1712511A4FA00C83BAF90A8F.json",
-                        "Name": "Late Pce",
-                        "RegID": "27844DAE1712511A4FA00C83BAF90A8F"
+                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                        "Name": "Jessie New Student",
+                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:17:37 PM",
-                    "RequestDate": "",
-                    "RequestStatus": "",
+                    "RepositoryTimeStamp": "3/28/2013 1:16:05 PM",
+                    "RequestDate": "2012-12-16",
+                    "RequestStatus": "Added to class",
                     "Section": {
-                        "CourseNumber": "203",
-                        "CurriculumAbbreviation": "PSYCH",
-                        "Href": "/student/v5/course/2013,winter,PSYCH,203/A.json",
+                        "CourseNumber": "220",
+                        "CurriculumAbbreviation": "BIGDATA",
+                        "Href": "/student/v5/course/2013,winter,BIGDATA,220/A.json",
                         "Quarter": "winter",
                         "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "01/29/2013",
+                    "StartDate": "01/16/2013",
                     "VariableCredit": false,
                     "WritingCourse": false
                 }
             ],
-            "RepositoryTimeStamp": "3/28/2013 2:22:05 PM",
+            "RepositoryTimeStamp": "3/28/2013 2:21:36 PM",
             "Term": {
                 "Href": "/student/v5/term/2013,winter.json",
                 "Quarter": "winter",
                 "Year": 2013
             }
         },
         {
-            "ClassLevel": "NON_MATRIC",
+            "ClassLevel": "BLANK",
             "CurrentRegisteredCredits": null,
             "EnrollmentStatus": null,
             "EnrollmentStatusDate": "",
-            "FullName": "Late Pce",
+            "FullName": "Jessie New Student",
             "HonorsProgram": false,
             "LeaveEndQuarter": 0,
             "LeaveEndYear": 0,
-            "Majors": [
-                {
-                    "Abbreviation": "N MATR",
-                    "Campus": "Seattle",
-                    "CollegeAbbreviation": "INDUG",
-                    "CollegeFullName": "INTERDISCIPLINARY UNDERGRADUATE PROGRAMS",
-                    "DegreeLevel": 0,
-                    "DegreeName": null,
-                    "DegreeType": 0,
-                    "FullName": "Non Matriculated",
-                    "MajorName": "NON MATRICULATED",
-                    "Pathway": 0,
-                    "ShortName": "N MATR"
-                }
-            ],
+            "Majors": [],
             "Metadata": "EnrollmentSourceLocation=EOS;",
             "Minors": [],
             "PendingClassChange": false,
             "PendingHonorsChange": false,
             "PendingMajorChange": false,
             "PendingResidentChange": false,
             "PendingSpecialProgramChange": false,
             "Person": {
-                "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
-                "Name": "Late Pce",
-                "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
+                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                "Name": "Jessie New Student",
+                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
             },
             "QtrGradePoints": null,
             "QtrGradedAttmp": null,
             "QtrNonGrdEarned": null,
-            "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC",
+            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
             "Registrations": [
                 {
                     "AccessDateRangeEnd": "06/02/2014",
-                    "AccessDateRangeStart": "04/17/2013",
+                    "AccessDateRangeStart": "03/22/2013",
                     "Auditor": false,
                     "Credits": "0.0",
                     "DuplicateCode": "",
                     "EducationUnitType": "CEU",
-                    "EndDate": "06/28/2013",
+                    "EndDate": "06/12/2013",
                     "FeeBaseType": "",
                     "Grade": "",
                     "GradeDate": "",
                     "GradeDocumentID": "",
                     "GradingSystem": "SCUSC",
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,spring,CPROGRM,712,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
+                    "Href": "/student/v5/registration/2013,spring,BIGDATA,230,A,FE36CCB8F66711D5BE060004AC494F31,.json",
                     "Instructor": null,
                     "IsActive": true,
                     "IsCredit": false,
                     "IsIndependentStart": false,
                     "Metadata": "RegistrationSourceLocation=EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
-                        "Name": "Late Pce",
-                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
+                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                        "Name": "Jessie New Student",
+                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:13:18 PM",
-                    "RequestDate": "2013-03-07",
+                    "RepositoryTimeStamp": "3/28/2013 1:13:17 PM",
+                    "RequestDate": "2013-03-10",
                     "RequestStatus": "Added to class",
                     "Section": {
-                        "CourseNumber": "712",
-                        "CurriculumAbbreviation": "CPROGRM",
-                        "Href": "/student/v5/course/2013,spring,CPROGRM,712/A.json",
+                        "CourseNumber": "230",
+                        "CurriculumAbbreviation": "BIGDATA",
+                        "Href": "/student/v5/course/2013,spring,BIGDATA,230/A.json",
                         "Quarter": "spring",
                         "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "04/29/2013",
+                    "StartDate": "04/03/2013",
                     "VariableCredit": false,
                     "WritingCourse": false
-                },
+                }
+            ],
+            "RepositoryTimeStamp": "3/28/2013 2:20:52 PM",
+            "Term": {
+                "Href": "/student/v5/term/2013,spring.json",
+                "Quarter": "spring",
+                "Year": 2013
+            }
+        },
+        {
+            "ClassLevel": "BLANK",
+            "CurrentRegisteredCredits": null,
+            "EnrollmentStatus": null,
+            "EnrollmentStatusDate": "",
+            "FullName": "Jessie New Student",
+            "HonorsProgram": false,
+            "LeaveEndQuarter": 0,
+            "LeaveEndYear": 0,
+            "Majors": [],
+            "Metadata": "EnrollmentSourceLocation=EOS;",
+            "Minors": [],
+            "PendingClassChange": false,
+            "PendingHonorsChange": false,
+            "PendingMajorChange": false,
+            "PendingResidentChange": false,
+            "PendingSpecialProgramChange": false,
+            "Person": {
+                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                "Name": "Jessie New Student",
+                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+            },
+            "QtrGradePoints": null,
+            "QtrGradedAttmp": null,
+            "QtrNonGrdEarned": null,
+            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
+            "Registrations": [
                 {
-                    "AccessDateRangeEnd": "06/02/2014",
-                    "AccessDateRangeStart": "03/13/2013",
+                    "AccessDateRangeEnd": "08/18/2014",
+                    "AccessDateRangeStart": "07/03/2013",
                     "Auditor": false,
-                    "Credits": "6.0",
+                    "Credits": "3",
                     "DuplicateCode": "",
                     "EducationUnitType": null,
-                    "EndDate": "06/19/2013",
-                    "FeeBaseType": "Fee based course",
-                    "Grade": "X",
+                    "EndDate": "07/19/2013",
+                    "FeeBaseType": "",
+                    "Grade": "",
                     "GradeDate": "",
                     "GradeDocumentID": "",
                     "GradingSystem": null,
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,spring,ACCTG,508,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
+                    "Href": "/student/v5/registration/2013,summer,LIS,498,C,FE36CCB8F66711D5BE060004AC494F31,.json",
                     "Instructor": null,
                     "IsActive": true,
                     "IsCredit": true,
                     "IsIndependentStart": false,
-                    "Metadata": "RegistrationSourceLocation=SDB_EOS;",
+                    "Metadata": "RegistrationSourceLocation=EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
-                        "Name": "Late Pce",
-                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
+                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                        "Name": "Jessie New Student",
+                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:13:22 PM",
-                    "RequestDate": "2013-03-16",
-                    "RequestStatus": "ADDED TO CLASS",
+                    "RepositoryTimeStamp": "5/18/2013 12:11:53 PM",
+                    "RequestDate": "2013-05-18",
+                    "RequestStatus": "Added to standby",
                     "Section": {
-                        "CourseNumber": "508",
-                        "CurriculumAbbreviation": "ACCTG",
-                        "Href": "/student/v5/course/2013,spring,ACCTG,508/A.json",
-                        "Quarter": "spring",
-                        "SectionID": "A",
+                        "CourseNumber": "498",
+                        "CurriculumAbbreviation": "LIS",
+                        "Href": "/student/v5/course/2013,summer,LIS,498/C.json",
+                        "Quarter": "summer",
+                        "SectionID": "C",
                         "Year": 2013
                     },
-                    "StartDate": "04/01/2013",
+                    "StartDate": "07/15/2013",
                     "VariableCredit": false,
                     "WritingCourse": false
-                },
+                }
+            ],
+            "RepositoryTimeStamp": "5/18/2013 12:11:27 PM",
+            "Term": {
+                "Href": "/student/v5/term/2013,summer.json",
+                "Quarter": "summer",
+                "Year": 2013
+            }
+        },
+        {
+            "ClassLevel": "BLANK",
+            "CurrentRegisteredCredits": null,
+            "EnrollmentStatus": null,
+            "EnrollmentStatusDate": "",
+            "FullName": "Jessie New Student",
+            "HonorsProgram": false,
+            "LeaveEndQuarter": 0,
+            "LeaveEndYear": 0,
+            "Majors": [],
+            "Metadata": "EnrollmentSourceLocation=EOS;",
+            "Minors": [],
+            "PendingClassChange": false,
+            "PendingHonorsChange": false,
+            "PendingMajorChange": false,
+            "PendingResidentChange": false,
+            "PendingSpecialProgramChange": false,
+            "Person": {
+                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                "Name": "Jessie New Student",
+                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+            },
+            "QtrGradePoints": null,
+            "QtrGradedAttmp": null,
+            "QtrNonGrdEarned": null,
+            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
+            "Registrations": [
                 {
-                    "AccessDateRangeEnd": "06/02/2014",
-                    "AccessDateRangeStart": "03/15/2013",
+                    "AccessDateRangeEnd": "12/08/2014",
+                    "AccessDateRangeStart": "09/13/2013",
                     "Auditor": false,
-                    "Credits": "0.0",
+                    "Credits": "3",
                     "DuplicateCode": "",
-                    "EducationUnitType": "CEUNUM",
-                    "EndDate": "06/07/2013",
+                    "EducationUnitType": null,
+                    "EndDate": "12/13/2013",
                     "FeeBaseType": "",
                     "Grade": "",
                     "GradeDate": "",
                     "GradeDocumentID": "",
-                    "GradingSystem": "standard",
+                    "GradingSystem": null,
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,spring,AAES,150,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
+                    "Href": "/student/v5/registration/2013,autumn,MUSEUM,700,A,FE36CCB8F66711D5BE060004AC494F31,.json",
                     "Instructor": null,
                     "IsActive": true,
-                    "IsCredit": false,
+                    "IsCredit": true,
                     "IsIndependentStart": false,
                     "Metadata": "RegistrationSourceLocation=EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
-                        "Name": "Late Pce",
-                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
+                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
+                        "Name": "Jessie New Student",
+                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:13:17 PM",
-                    "RequestDate": "2013-03-03",
-                    "RequestStatus": "Added to class",
+                    "RepositoryTimeStamp": "5/17/2013 3:48:32 PM",
+                    "RequestDate": "2013-05-16",
+                    "RequestStatus": "Pending Added to class",
                     "Section": {
-                        "CourseNumber": "150",
-                        "CurriculumAbbreviation": "AAES",
-                        "Href": "/student/v5/course/2013,spring,AAES,150/A.json",
-                        "Quarter": "spring",
+                        "CourseNumber": "700",
+                        "CurriculumAbbreviation": "MUSEUM",
+                        "Href": "/student/v5/course/2013,autumn,MUSEUM,700/A.json",
+                        "Quarter": "autumn",
                         "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "04/03/2013",
-                    "VariableCredit": false,
+                    "StartDate": "09/25/2013",
+                    "VariableCredit": true,
                     "WritingCourse": false
                 }
             ],
-            "RepositoryTimeStamp": "3/28/2013 2:20:53 PM",
+            "RepositoryTimeStamp": "5/18/2013 5:03:45 AM",
             "Term": {
-                "Href": "/student/v5/term/2013,spring.json",
-                "Quarter": "spring",
+                "Href": "/student/v5/term/2013,autumn.json",
+                "Quarter": "autumn",
                 "Year": 2013
             }
         }
     ],
     "Next": null,
     "PageSize": "10",
     "PageStart": "1",
     "Previous": null,
-    "TotalCount": 2
+    "TotalCount": 4
 }
```

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_verbose_true_transcriptable_course_all_changed_since_date_` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/enrollment.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_verbose_true_transcriptable_course_all_changed_since_date_`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8629593276112528%*

 * *Differences: {"'Current'": "{'Href': "*

 * *              "'/student/v5/enrollment.json?reg_id=AABBCCDDEEFFAABBCCDDEEFFAABBCCDC&verbose=true&changed_since_date=&transcriptable_course=all', "*

 * *              "'RegID': 'AABBCCDDEEFFAABBCCDDEEFFAABBCCDC'}",*

 * * "'Enrollments'": "{0: {'ClassLevel': 'NON_MATRIC', 'CurrentRegisteredCredits': 9.0, "*

 * *                  "'EnrollmentStatus': 'Registered', 'EnrollmentStatusDate': '2013-01-27', "*

 * *                  "'FullName': 'Late Average Student', 'Majors': [OrderedDict([('Abbreviation', ' […]*

```diff
@@ -1,318 +1,317 @@
 {
     "Current": {
-        "Href": "/student/v5/enrollment.json?reg_id=FE36CCB8F66711D5BE060004AC494F31&verbose=true&changed_since_date=&transcriptable_course=all",
-        "RegID": "FE36CCB8F66711D5BE060004AC494F31",
+        "Href": "/student/v5/enrollment.json?reg_id=AABBCCDDEEFFAABBCCDDEEFFAABBCCDC&verbose=true&changed_since_date=&transcriptable_course=all",
+        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC",
         "Verbose": true
     },
     "Enrollments": [
         {
-            "ClassLevel": "BLANK",
-            "CurrentRegisteredCredits": null,
-            "EnrollmentStatus": null,
-            "EnrollmentStatusDate": "",
-            "FullName": "Jessie New Student",
+            "ClassLevel": "NON_MATRIC",
+            "CurrentRegisteredCredits": 9.0,
+            "EnrollmentStatus": "Registered",
+            "EnrollmentStatusDate": "2013-01-27",
+            "FullName": "Late Average Student",
             "HonorsProgram": false,
             "LeaveEndQuarter": 0,
             "LeaveEndYear": 0,
-            "Majors": [],
-            "Metadata": "EnrollmentSourceLocation=EOS;",
+            "Majors": [
+                {
+                    "Abbreviation": "N MATR",
+                    "Campus": "Seattle",
+                    "CollegeAbbreviation": "INDUG",
+                    "CollegeFullName": "INTERDISCIPLINARY UNDERGRADUATE PROGRAMS",
+                    "DegreeLevel": 0,
+                    "DegreeName": null,
+                    "DegreeType": 0,
+                    "FullName": "Non Matriculated",
+                    "MajorName": "NON MATRICULATED",
+                    "Pathway": 0,
+                    "ShortName": "N MATR"
+                }
+            ],
+            "Metadata": "EnrollmentSourceLocation=SDB_EOS;",
             "Minors": [],
             "PendingClassChange": false,
             "PendingHonorsChange": false,
             "PendingMajorChange": false,
             "PendingResidentChange": false,
             "PendingSpecialProgramChange": false,
             "Person": {
-                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                "Name": "Jessie New Student",
-                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+                "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                "Name": "Late Average Student",
+                "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
             },
             "QtrGradePoints": null,
             "QtrGradedAttmp": null,
             "QtrNonGrdEarned": null,
-            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
+            "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC",
             "Registrations": [
                 {
-                    "AccessDateRangeEnd": "03/10/2014",
-                    "AccessDateRangeStart": "12/28/2012",
+                    "AccessDateRangeEnd": "07/25/2013",
+                    "AccessDateRangeStart": "12/19/2012",
                     "Auditor": false,
-                    "Credits": "0.0",
+                    "Credits": "5.0",
                     "DuplicateCode": "",
-                    "EducationUnitType": "CEU",
-                    "EndDate": "03/20/2013",
-                    "FeeBaseType": "",
-                    "Grade": "SC",
-                    "GradeDate": "3/22/2013 3:44:00 PM",
+                    "EducationUnitType": null,
+                    "EndDate": "04/29/2013",
+                    "FeeBaseType": "Fee based course",
+                    "Grade": "X",
+                    "GradeDate": "",
                     "GradeDocumentID": "",
-                    "GradingSystem": "SCUSC",
+                    "GradingSystem": null,
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,winter,BIGDATA,220,A,FE36CCB8F66711D5BE060004AC494F31,.json",
+                    "Href": "/student/v5/registration/2013,winter,COM,201,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
                     "Instructor": null,
                     "IsActive": true,
-                    "IsCredit": false,
-                    "IsIndependentStart": false,
-                    "Metadata": "RegistrationSourceLocation=EOS;",
+                    "IsCredit": true,
+                    "IsIndependentStart": true,
+                    "Metadata": "RegistrationSourceLocation=SDB_EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                        "Name": "Jessie New Student",
-                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                        "Name": "Late Average Student",
+                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:16:05 PM",
-                    "RequestDate": "2012-12-16",
-                    "RequestStatus": "Added to class",
+                    "RepositoryTimeStamp": "1/28/2013 2:06:34 AM",
+                    "RequestDate": "2013-01-27",
+                    "RequestStatus": "ADDED TO CLASS",
                     "Section": {
-                        "CourseNumber": "220",
-                        "CurriculumAbbreviation": "BIGDATA",
-                        "Href": "/student/v5/course/2013,winter,BIGDATA,220/A.json",
+                        "CourseNumber": "201",
+                        "CurriculumAbbreviation": "COM",
+                        "Href": "/student/v5/course/2013,winter,COM,201/A.json",
                         "Quarter": "winter",
                         "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "01/16/2013",
+                    "StartDate": "01/28/2013",
+                    "VariableCredit": false,
+                    "WritingCourse": false
+                },
+                {
+                    "AccessDateRangeEnd": "07/25/2013",
+                    "AccessDateRangeStart": "12/19/2012",
+                    "Auditor": false,
+                    "Credits": "4.0",
+                    "DuplicateCode": "",
+                    "EducationUnitType": null,
+                    "EndDate": "06/22/2013",
+                    "FeeBaseType": "Fee based course",
+                    "Grade": "X",
+                    "GradeDate": "",
+                    "GradeDocumentID": "",
+                    "GradingSystem": null,
+                    "HonorsCourse": false,
+                    "Href": "/student/v5/registration/2013,winter,PSYCH,203,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
+                    "Instructor": null,
+                    "IsActive": true,
+                    "IsCredit": true,
+                    "IsIndependentStart": true,
+                    "Metadata": "RegistrationSourceLocation=SDB_EOS;",
+                    "Person": {
+                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                        "Name": "Late Average Student",
+                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
+                    },
+                    "RepeatCourse": false,
+                    "RepositoryTimeStamp": "1/29/2013 2:06:34 AM",
+                    "RequestDate": "2013-01-27",
+                    "RequestStatus": "ADDED TO CLASS",
+                    "Section": {
+                        "CourseNumber": "203",
+                        "CurriculumAbbreviation": "PSYCH",
+                        "Href": "/student/v5/course/2013,winter,PSYCH,203/A.json",
+                        "Quarter": "winter",
+                        "SectionID": "A",
+                        "Year": 2013
+                    },
+                    "StartDate": "01/29/2013",
                     "VariableCredit": false,
                     "WritingCourse": false
                 }
             ],
-            "RepositoryTimeStamp": "3/28/2013 2:21:36 PM",
+            "RepositoryTimeStamp": "1/29/2013 3:05:09 AM",
             "Term": {
                 "Href": "/student/v5/term/2013,winter.json",
                 "Quarter": "winter",
                 "Year": 2013
             }
         },
         {
-            "ClassLevel": "BLANK",
+            "ClassLevel": "NON_MATRIC",
             "CurrentRegisteredCredits": null,
             "EnrollmentStatus": null,
             "EnrollmentStatusDate": "",
-            "FullName": "Jessie New Student",
+            "FullName": "Late Pce",
             "HonorsProgram": false,
             "LeaveEndQuarter": 0,
             "LeaveEndYear": 0,
-            "Majors": [],
+            "Majors": [
+                {
+                    "Abbreviation": "N MATR",
+                    "Campus": "Seattle",
+                    "CollegeAbbreviation": "INDUG",
+                    "CollegeFullName": "INTERDISCIPLINARY UNDERGRADUATE PROGRAMS",
+                    "DegreeLevel": 0,
+                    "DegreeName": null,
+                    "DegreeType": 0,
+                    "FullName": "Non Matriculated",
+                    "MajorName": "NON MATRICULATED",
+                    "Pathway": 0,
+                    "ShortName": "N MATR"
+                }
+            ],
             "Metadata": "EnrollmentSourceLocation=EOS;",
             "Minors": [],
             "PendingClassChange": false,
             "PendingHonorsChange": false,
             "PendingMajorChange": false,
             "PendingResidentChange": false,
             "PendingSpecialProgramChange": false,
             "Person": {
-                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                "Name": "Jessie New Student",
-                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+                "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                "Name": "Late Pce",
+                "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
             },
             "QtrGradePoints": null,
             "QtrGradedAttmp": null,
             "QtrNonGrdEarned": null,
-            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
+            "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC",
             "Registrations": [
                 {
                     "AccessDateRangeEnd": "06/02/2014",
-                    "AccessDateRangeStart": "03/22/2013",
+                    "AccessDateRangeStart": "04/17/2013",
                     "Auditor": false,
                     "Credits": "0.0",
                     "DuplicateCode": "",
                     "EducationUnitType": "CEU",
-                    "EndDate": "06/12/2013",
+                    "EndDate": "06/28/2013",
                     "FeeBaseType": "",
                     "Grade": "",
                     "GradeDate": "",
                     "GradeDocumentID": "",
                     "GradingSystem": "SCUSC",
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,spring,BIGDATA,230,A,FE36CCB8F66711D5BE060004AC494F31,.json",
+                    "Href": "/student/v5/registration/2013,spring,CPROGRM,712,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
                     "Instructor": null,
                     "IsActive": true,
                     "IsCredit": false,
                     "IsIndependentStart": false,
                     "Metadata": "RegistrationSourceLocation=EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                        "Name": "Jessie New Student",
-                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                        "Name": "Late Pce",
+                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "3/28/2013 1:13:17 PM",
-                    "RequestDate": "2013-03-10",
+                    "RepositoryTimeStamp": "3/28/2013 1:13:18 PM",
+                    "RequestDate": "2013-03-07",
                     "RequestStatus": "Added to class",
                     "Section": {
-                        "CourseNumber": "230",
-                        "CurriculumAbbreviation": "BIGDATA",
-                        "Href": "/student/v5/course/2013,spring,BIGDATA,230/A.json",
+                        "CourseNumber": "712",
+                        "CurriculumAbbreviation": "CPROGRM",
+                        "Href": "/student/v5/course/2013,spring,CPROGRM,712/A.json",
                         "Quarter": "spring",
                         "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "04/03/2013",
+                    "StartDate": "04/29/2013",
                     "VariableCredit": false,
                     "WritingCourse": false
-                }
-            ],
-            "RepositoryTimeStamp": "3/28/2013 2:20:52 PM",
-            "Term": {
-                "Href": "/student/v5/term/2013,spring.json",
-                "Quarter": "spring",
-                "Year": 2013
-            }
-        },
-        {
-            "ClassLevel": "BLANK",
-            "CurrentRegisteredCredits": null,
-            "EnrollmentStatus": null,
-            "EnrollmentStatusDate": "",
-            "FullName": "Jessie New Student",
-            "HonorsProgram": false,
-            "LeaveEndQuarter": 0,
-            "LeaveEndYear": 0,
-            "Majors": [],
-            "Metadata": "EnrollmentSourceLocation=EOS;",
-            "Minors": [],
-            "PendingClassChange": false,
-            "PendingHonorsChange": false,
-            "PendingMajorChange": false,
-            "PendingResidentChange": false,
-            "PendingSpecialProgramChange": false,
-            "Person": {
-                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                "Name": "Jessie New Student",
-                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
-            },
-            "QtrGradePoints": null,
-            "QtrGradedAttmp": null,
-            "QtrNonGrdEarned": null,
-            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
-            "Registrations": [
+                },
                 {
-                    "AccessDateRangeEnd": "08/18/2014",
-                    "AccessDateRangeStart": "07/03/2013",
+                    "AccessDateRangeEnd": "06/02/2014",
+                    "AccessDateRangeStart": "03/13/2013",
                     "Auditor": false,
-                    "Credits": "3",
+                    "Credits": "6.0",
                     "DuplicateCode": "",
                     "EducationUnitType": null,
-                    "EndDate": "07/19/2013",
-                    "FeeBaseType": "",
-                    "Grade": "",
+                    "EndDate": "06/19/2013",
+                    "FeeBaseType": "Fee based course",
+                    "Grade": "X",
                     "GradeDate": "",
                     "GradeDocumentID": "",
                     "GradingSystem": null,
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,summer,LIS,498,C,FE36CCB8F66711D5BE060004AC494F31,.json",
+                    "Href": "/student/v5/registration/2013,spring,ACCTG,508,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
                     "Instructor": null,
                     "IsActive": true,
                     "IsCredit": true,
                     "IsIndependentStart": false,
-                    "Metadata": "RegistrationSourceLocation=EOS;",
+                    "Metadata": "RegistrationSourceLocation=SDB_EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                        "Name": "Jessie New Student",
-                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                        "Name": "Late Pce",
+                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "5/18/2013 12:11:53 PM",
-                    "RequestDate": "2013-05-18",
-                    "RequestStatus": "Added to standby",
+                    "RepositoryTimeStamp": "3/28/2013 1:13:22 PM",
+                    "RequestDate": "2013-03-16",
+                    "RequestStatus": "ADDED TO CLASS",
                     "Section": {
-                        "CourseNumber": "498",
-                        "CurriculumAbbreviation": "LIS",
-                        "Href": "/student/v5/course/2013,summer,LIS,498/C.json",
-                        "Quarter": "summer",
-                        "SectionID": "C",
+                        "CourseNumber": "508",
+                        "CurriculumAbbreviation": "ACCTG",
+                        "Href": "/student/v5/course/2013,spring,ACCTG,508/A.json",
+                        "Quarter": "spring",
+                        "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "07/15/2013",
+                    "StartDate": "04/01/2013",
                     "VariableCredit": false,
                     "WritingCourse": false
-                }
-            ],
-            "RepositoryTimeStamp": "5/18/2013 12:11:27 PM",
-            "Term": {
-                "Href": "/student/v5/term/2013,summer.json",
-                "Quarter": "summer",
-                "Year": 2013
-            }
-        },
-        {
-            "ClassLevel": "BLANK",
-            "CurrentRegisteredCredits": null,
-            "EnrollmentStatus": null,
-            "EnrollmentStatusDate": "",
-            "FullName": "Jessie New Student",
-            "HonorsProgram": false,
-            "LeaveEndQuarter": 0,
-            "LeaveEndYear": 0,
-            "Majors": [],
-            "Metadata": "EnrollmentSourceLocation=EOS;",
-            "Minors": [],
-            "PendingClassChange": false,
-            "PendingHonorsChange": false,
-            "PendingMajorChange": false,
-            "PendingResidentChange": false,
-            "PendingSpecialProgramChange": false,
-            "Person": {
-                "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                "Name": "Jessie New Student",
-                "RegID": "FE36CCB8F66711D5BE060004AC494F31"
-            },
-            "QtrGradePoints": null,
-            "QtrGradedAttmp": null,
-            "QtrNonGrdEarned": null,
-            "RegID": "FE36CCB8F66711D5BE060004AC494F31",
-            "Registrations": [
+                },
                 {
-                    "AccessDateRangeEnd": "12/08/2014",
-                    "AccessDateRangeStart": "09/13/2013",
+                    "AccessDateRangeEnd": "06/02/2014",
+                    "AccessDateRangeStart": "03/15/2013",
                     "Auditor": false,
-                    "Credits": "3",
+                    "Credits": "0.0",
                     "DuplicateCode": "",
-                    "EducationUnitType": null,
-                    "EndDate": "12/13/2013",
+                    "EducationUnitType": "CEUNUM",
+                    "EndDate": "06/07/2013",
                     "FeeBaseType": "",
                     "Grade": "",
                     "GradeDate": "",
                     "GradeDocumentID": "",
-                    "GradingSystem": null,
+                    "GradingSystem": "standard",
                     "HonorsCourse": false,
-                    "Href": "/student/v5/registration/2013,autumn,MUSEUM,700,A,FE36CCB8F66711D5BE060004AC494F31,.json",
+                    "Href": "/student/v5/registration/2013,spring,AAES,150,A,AABBCCDDEEFFAABBCCDDEEFFAABBCCDC,.json",
                     "Instructor": null,
                     "IsActive": true,
-                    "IsCredit": true,
+                    "IsCredit": false,
                     "IsIndependentStart": false,
                     "Metadata": "RegistrationSourceLocation=EOS;",
                     "Person": {
-                        "Href": "/student/v5/person/FE36CCB8F66711D5BE060004AC494F31.json",
-                        "Name": "Jessie New Student",
-                        "RegID": "FE36CCB8F66711D5BE060004AC494F31"
+                        "Href": "/student/v5/person/AABBCCDDEEFFAABBCCDDEEFFAABBCCDC.json",
+                        "Name": "Late Pce",
+                        "RegID": "AABBCCDDEEFFAABBCCDDEEFFAABBCCDC"
                     },
                     "RepeatCourse": false,
-                    "RepositoryTimeStamp": "5/17/2013 3:48:32 PM",
-                    "RequestDate": "2013-05-16",
-                    "RequestStatus": "Pending Added to class",
+                    "RepositoryTimeStamp": "3/28/2013 1:13:17 PM",
+                    "RequestDate": "2013-03-03",
+                    "RequestStatus": "Added to class",
                     "Section": {
-                        "CourseNumber": "700",
-                        "CurriculumAbbreviation": "MUSEUM",
-                        "Href": "/student/v5/course/2013,autumn,MUSEUM,700/A.json",
-                        "Quarter": "autumn",
+                        "CourseNumber": "150",
+                        "CurriculumAbbreviation": "AAES",
+                        "Href": "/student/v5/course/2013,spring,AAES,150/A.json",
+                        "Quarter": "spring",
                         "SectionID": "A",
                         "Year": 2013
                     },
-                    "StartDate": "09/25/2013",
-                    "VariableCredit": true,
+                    "StartDate": "04/03/2013",
+                    "VariableCredit": false,
                     "WritingCourse": false
                 }
             ],
-            "RepositoryTimeStamp": "5/18/2013 5:03:45 AM",
+            "RepositoryTimeStamp": "3/28/2013 2:20:53 PM",
             "Term": {
-                "Href": "/student/v5/term/2013,autumn.json",
-                "Quarter": "autumn",
+                "Href": "/student/v5/term/2013,spring.json",
+                "Quarter": "spring",
                 "Year": 2013
             }
         }
     ],
     "Next": null,
     "PageSize": "10",
     "PageStart": "1",
     "Previous": null,
-    "TotalCount": 4
+    "TotalCount": 2
 }
```

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494F31.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494F31.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494F31.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494F31.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494FCD.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/notice/FE36CCB8F66711D5BE060004AC494FCD.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/00000000000000000000000000000001.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/advisers.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/advisers.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/degree.json_deg_status_all` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012/degree.json_deg_status_all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/12345678901234567890123456789012.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/24A20F50AE3511D68CBC0004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/24A20F50AE3511D68CBC0004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494F31.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/advisers.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/advisers.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/degree.json_deg_status_all` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE/degree.json_deg_status_all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/person/9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_AA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_B%20BIO_180_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_CSS_161_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_EDC_I_461_A_00000000000000000000000000000004_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_ELCBUS_451_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_3.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_GA_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_MATH_125_G_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_00000000000000000000000000000003_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_T%20BUS_310_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEDADM_572_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TEST_098_T_00000000000000000000000000000004_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TMATH_110_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_101_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_102_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_103_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2012_summer_TRAIN_104_A_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_AA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_B%20BIO_180_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_EDC_I_461_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_GA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_MATH_125_G_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AC_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_AQ_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_510_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_574_A_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_581_A_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_585_A_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_REHAB_591_C_2817F385001347AD80D653A8E352FDC9_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_T%20BUS_310_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TEST_098_T_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_autumn_TRAIN_100_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_AA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_B%20BIO_180_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_EDC_I_461_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_ESS_107_A_FE36CCB8F66711D5BE060004AC494FCE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_ESS_107_A_FE36CCB8F66711D5BE060004AC494FCE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_GA_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_MATH_125_G_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_495_A_BB000000000000000000000000009994_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHIL_600_A_BB000000000000000000000000000004_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_T%20BUS_310_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TEST_098_T_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_100_A_AA36CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_12345678901234567890123456789012_1.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_spring_TRAIN_101_A_AA36CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AC_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_AQ_9136CCB8F66711D5BE060004AC494FFE_2.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_PHYS_121_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_100_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_summer_TRAIN_101_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_BIGDATA_220_A_FE36CCB8F66711D5BE060004AC494F31_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_BIGDATA_220_A_FE36CCB8F66711D5BE060004AC494F31_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_503_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_533_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration/2013_winter_EMBA_590_A_9136CCB8F66711D5BE060004AC494FFE_.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_A` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_A`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B_transcriptable_course_all` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active__section_id_B_transcriptable_course_all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_A` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_A`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_B` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_DROP_T_instructor_reg_id__course_number_100_verbose_true_year_2013_quarter_winter_is_active_true_section_id_B`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_EDC_I_instructor_reg_id__course_number_552_verbose_true_year_2017_quarter_autumn_is_active_true_section_id_A_transcriptable_course_all` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_curriculum_abbreviation_EDC_I_instructor_reg_id__course_number_552_verbose_true_year_2017_quarter_autumn_is_active_true_section_id_A_transcriptable_course_all`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_autumn_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_spring_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_summer_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_quarter_winter_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000001_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000003_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_00000000000000000000000000000004_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_autumn_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_spring_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_summer_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_quarter_winter_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_12345678901234567890123456789012_transcriptable_course_all_quarter_summer_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_autumn_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2012_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2012_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2012_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2012_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_9136CCB8F66711D5BE060004AC494FFE_quarter_winter_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_spring_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AA36CCB8F66711D5BE060004AC494FFE_quarter_summer_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDA_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDB_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDC_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDD_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_true_year_2012` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_AABBCCDDEEFFAABBCCDDEEFFAABBCCDE_quarter_summer_is_active_true_year_2012`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_spring_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000000004_quarter_summer_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_spring_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_BB000000000000000000000000009994_quarter_summer_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_quarter_autumn_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_transcriptable_course_all_quarter_winter_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494F31_transcriptable_course_all_quarter_winter_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494FCE_transcriptable_course_no_quarter_spring_is_active_true_year_2013_verbose_on` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FE36CCB8F66711D5BE060004AC494FCE_transcriptable_course_no_quarter_spring_is_active_true_year_2013_verbose_on`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF1_quarter_spring_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_true_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/registration.json_reg_id_FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF2_quarter_spring_is_active_true_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_quarter_winter_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_transcriptable_course_all_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_curriculum_abbreviation_ENDO_transcriptable_course_all_changed_since_date_2013-12-12_quarter_winter_page_size_1000_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_quarter_winter_facility_code_KNE_year_2013` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_quarter_winter_facility_code_KNE_year_2013`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_autumn_include_secondaries__year_2012_future_terms_4_transcriptable_course_all_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_autumn_include_secondaries__year_2012_future_terms_4_transcriptable_course_all_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries__year_2013_future_terms_2_transcriptable_course_all_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries__year_2013_future_terms_2_transcriptable_course_all_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_all_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_260A0DEC95CB11D78BAA000629C31437_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_all_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_GradeSubmissionDelegate_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_spring_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active_suspended`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/section.json_reg_id_FBB38FE46A7C11D5A4AE0004AC494FFE_search_by_Instructor_quarter_summer_include_secondaries_on_year_2013_future_terms_0_transcriptable_course_yes_delete_flag_active`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1996_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1996_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1997_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1997_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/1998_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/1998_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2008_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2008_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2012_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2012_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2012_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2012_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2012_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2012_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2013_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2013_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2014_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2014_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2014_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2014_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2015_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2015_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2016_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2016_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2017_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2017_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2018_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2018_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_autumn.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_autumn.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2020_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2020_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2021_spring.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2021_spring.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2021_summer.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2021_summer.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/2021_winter.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/2021_winter.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/current.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/current.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/next.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/next.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/resources/sws/file/student/v5/term/previous.json` & `UW-RestClients-SWS-2.4.2/uw_sws/resources/sws/file/student/v5/term/previous.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/section.py` & `UW-RestClients-SWS-2.4.2/uw_sws/section.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/section_status.py` & `UW-RestClients-SWS-2.4.2/uw_sws/section_status.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/term.py` & `UW-RestClients-SWS-2.4.2/uw_sws/term.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/compatible.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/compatible.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_adviser.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_adviser.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_course.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_course.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_curriculum.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_curriculum.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_dao.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_dao.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_degree.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_degree.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_department.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_department.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_enrollment.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_enrollment.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 # SPDX-License-Identifier: Apache-2.0
 
 from unittest import TestCase
 from uw_sws.util import fdao_sws_override
 from uw_pws.util import fdao_pws_override
 from uw_sws.models import Enrollment, Term, ENROLLMENT_SOURCE_PCE
 from uw_sws.term import (
-    get_current_term, get_next_term, get_term_by_year_and_quarter,
-    get_term_after, get_term_before)
+    get_current_term, get_term_by_year_and_quarter, get_term_before)
 from uw_sws.enrollment import (
     get_grades_by_regid_and_term, get_enrollment_by_regid_and_term,
-    enrollment_search_by_regid, get_enrollment_history_by_regid)
+    enrollment_search_by_regid, get_enrollment_history_by_regid, _get_term)
 from restclients_core.exceptions import DataFailureException
 
 
 @fdao_pws_override
 @fdao_sws_override
 class SWSTestEnrollments(TestCase):
     def test_javerage_grades(self):
@@ -156,15 +155,15 @@
         self.assertFalse(section1.is_standby_status())
         self.assertFalse(section1.is_dropped_status())
 
         term0 = get_term_before(term)
         self.assertTrue(term0 in result_dict)
         enrollment0 = result_dict.get(term0)
         self.assertEquals(enrollment.majors[0], enrollment0.majors[0])
-        self.assertEqual(len(enrollment0.unf_pce_courses), 1)
+        self.assertEqual(len(enrollment0.unf_pce_courses), 2)
 
         # regular course
         result_dict = enrollment_search_by_regid(
             '9136CCB8F66711D5BE060004AC494FFE')
         self.assertEqual(len(result_dict), 7)
         term = get_current_term()
         self.assertTrue(term in result_dict)
@@ -262,7 +261,18 @@
         self.assertEqual(result_list[0].term.quarter, "autumn")
         self.assertEqual(result_list[0].majors[0].major_name,
                          "PRE MAJOR (A&S)")
 
         self.assertEqual(result_list[-2].term.year, 2013)
         self.assertEqual(result_list[-2].term.quarter, "summer")
         self.assertEqual(result_list[-2].majors[0].major_name, "ENGLISH")
+
+    def test_get_term(self):
+        t = _get_term(
+            {"Term": {
+                "Year": 2013,
+                "Quarter": "spring"
+            }})
+        self.assertEqual(t.year, 2013)
+        self.assertEqual(t.quarter, "spring")
+        self.assertIsNotNone(t.last_final_exam_date)
+        self.assertIsNone(_get_term({"Term": {}}))
```

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_financial.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_financial.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_independent_study.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_independent_study.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_instructor_no_regid.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_instructor_no_regid.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_notice.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_notice.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_person.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_registrations.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_registrations.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_schedule_data.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_schedule_data.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_section.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_section.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_section_status.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_section_status.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/tests/test_term.py` & `UW-RestClients-SWS-2.4.2/uw_sws/tests/test_term.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/thread.py` & `UW-RestClients-SWS-2.4.2/uw_sws/thread.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-SWS-2.4.1/uw_sws/util.py` & `UW-RestClients-SWS-2.4.2/uw_sws/util.py`

 * *Files identical despite different names*

