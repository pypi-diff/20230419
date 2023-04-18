# Comparing `tmp/c65beka-1.0.0.tar.gz` & `tmp/c65beka-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c65beka-1.0.0.tar", last modified: Tue Sep 14 22:09:22 2021, max compression
+gzip compressed data, was "c65beka-1.0.1.tar", last modified: Tue Apr 18 22:42:34 2023, max compression
```

## Comparing `c65beka-1.0.0.tar` & `c65beka-1.0.1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.270991 c65beka-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.262991 c65beka-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.266991 c65beka-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-09-14 22:09:20.000000 c65beka-1.0.0/.github/workflows/release-debian.yml
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-09-14 22:09:20.000000 c65beka-1.0.0/.github/workflows/release-python.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-09-14 22:09:20.000000 c65beka-1.0.0/.github/workflows/tests-codecheck.yml
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-09-14 22:09:20.000000 c65beka-1.0.0/.github/workflows/tests-unit.yml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2021-09-14 22:09:20.000000 c65beka-1.0.0/.github/workflows/tests-yaml-lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      289 2021-09-14 22:09:20.000000 c65beka-1.0.0/.renovaterc.json
--rw-r--r--   0 runner    (1001) docker     (121)      137 2021-09-14 22:09:20.000000 c65beka-1.0.0/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-09-14 22:09:22.000000 c65beka-1.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-09-14 22:09:22.000000 c65beka-1.0.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)    10758 2021-09-14 22:09:20.000000 c65beka-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-09-14 22:09:22.270991 c65beka-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-09-14 22:09:20.000000 c65beka-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.266991 c65beka-1.0.0/beka/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/beka.py
--rw-r--r--   0 runner    (1001) docker     (121)    20682 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/bgp_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/chopper.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/packing_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/peering.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/route.py
--rw-r--r--   0 runner    (1001) docker     (121)    11203 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/stream_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-09-14 22:09:20.000000 c65beka-1.0.0/beka.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-09-14 22:09:20.000000 c65beka-1.0.0/bird.conf
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-09-14 22:09:20.000000 c65beka-1.0.0/bird6.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)       41 2021-09-14 22:09:20.000000 c65beka-1.0.0/birdc.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       44 2021-09-14 22:09:20.000000 c65beka-1.0.0/birdc6.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.270991 c65beka-1.0.0/c65beka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-09-14 22:09:22.000000 c65beka-1.0.0/c65beka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-09-14 22:09:20.000000 c65beka-1.0.0/codecheck-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-09-14 22:09:20.000000 c65beka-1.0.0/daemon.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.270991 c65beka-1.0.0/debian/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/README.source
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (121)        2 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/compat
--rw-r--r--   0 runner    (1001) docker     (121)      832 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/control
--rw-r--r--   0 runner    (1001) docker     (121)      965 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (121)       95 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.270991 c65beka-1.0.0/debian/source/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-14 22:09:20.000000 c65beka-1.0.0/debian/source/format
--rwxr-xr-x   0 runner    (1001) docker     (121)      630 2021-09-14 22:09:20.000000 c65beka-1.0.0/deploy_bird.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      173 2021-09-14 22:09:20.000000 c65beka-1.0.0/deploy_test.sh
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-09-14 22:09:20.000000 c65beka-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2021-09-14 22:09:20.000000 c65beka-1.0.0/run.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1069 2021-09-14 22:09:20.000000 c65beka-1.0.0/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-09-14 22:09:22.270991 c65beka-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      486 2021-09-14 22:09:20.000000 c65beka-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.262991 c65beka-1.0.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.270991 c65beka-1.0.0/test/codecheck/
--rwxr-xr-x   0 runner    (1001) docker     (121)      354 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/codecheck/min_pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/codecheck/pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      668 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/codecheck/src_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 22:09:22.270991 c65beka-1.0.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_beka.py
--rw-r--r--   0 runner    (1001) docker     (121)    14199 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_bgp_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_chopper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_peering.py
--rw-r--r--   0 runner    (1001) docker     (121)    22393 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-09-14 22:09:20.000000 c65beka-1.0.0/test/unit/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2021-09-14 22:09:20.000000 c65beka-1.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.247617 c65beka-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.235617 c65beka-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 22:42:31.000000 c65beka-1.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.239617 c65beka-1.0.1/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.239617 c65beka-1.0.1/.github/workflows/disabled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 22:42:31.000000 c65beka-1.0.1/.github/workflows/disabled/release-debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 22:42:31.000000 c65beka-1.0.1/.github/workflows/release-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-18 22:42:31.000000 c65beka-1.0.1/.github/workflows/tests-codecheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 22:42:31.000000 c65beka-1.0.1/.github/workflows/tests-unit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-18 22:42:31.000000 c65beka-1.0.1/.github/workflows/tests-yaml-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 22:42:31.000000 c65beka-1.0.1/.stickler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-18 22:42:33.000000 c65beka-1.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:42:33.000000 c65beka-1.0.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-18 22:42:31.000000 c65beka-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 22:42:34.247617 c65beka-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-18 22:42:31.000000 c65beka-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.243617 c65beka-1.0.1/beka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/beka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/bgp_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/packing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/stream_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-18 22:42:31.000000 c65beka-1.0.1/beka.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 22:42:31.000000 c65beka-1.0.1/bird.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-18 22:42:31.000000 c65beka-1.0.1/bird6.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-18 22:42:31.000000 c65beka-1.0.1/birdc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-18 22:42:31.000000 c65beka-1.0.1/birdc6.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.243617 c65beka-1.0.1/c65beka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 22:42:33.000000 c65beka-1.0.1/c65beka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-18 22:42:34.000000 c65beka-1.0.1/c65beka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:42:33.000000 c65beka-1.0.1/c65beka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:42:33.000000 c65beka-1.0.1/c65beka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 22:42:33.000000 c65beka-1.0.1/c65beka.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:42:33.000000 c65beka-1.0.1/c65beka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 22:42:33.000000 c65beka-1.0.1/c65beka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 22:42:31.000000 c65beka-1.0.1/codecheck-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 22:42:31.000000 c65beka-1.0.1/daemon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.247617 c65beka-1.0.1/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/README.source
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.247617 c65beka-1.0.1/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 22:42:31.000000 c65beka-1.0.1/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-18 22:42:31.000000 c65beka-1.0.1/deploy_bird.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-18 22:42:31.000000 c65beka-1.0.1/deploy_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:42:31.000000 c65beka-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-18 22:42:31.000000 c65beka-1.0.1/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-04-18 22:42:31.000000 c65beka-1.0.1/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-18 22:42:34.251617 c65beka-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-04-18 22:42:31.000000 c65beka-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.231617 c65beka-1.0.1/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.247617 c65beka-1.0.1/test/codecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/codecheck/min_pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/codecheck/pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/codecheck/src_files.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:42:34.247617 c65beka-1.0.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_beka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_bgp_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-18 22:42:31.000000 c65beka-1.0.1/test/unit/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:42:31.000000 c65beka-1.0.1/test-requirements.txt
```

### Comparing `c65beka-1.0.0/.github/workflows/release-debian.yml` & `c65beka-1.0.1/.github/workflows/disabled/release-debian.yml`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 jobs:
   debian-package:
     name: "Build debian packages"
     runs-on: ubuntu-latest
     environment:
       name: "release"
     container:
-      image: "ubuntu:bionic"
+      image: "debian:latest"
     steps:
       - name: Install dependencies
         run: |
           apt-get update
           apt-get -y upgrade
           apt-get -y install devscripts dpkg-dev debhelper equivs
       - name: Checkout repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Bump version
         run: |
           export DEBEMAIL='maintainers@faucet.nz'
           export DEBFULLNAME='Faucet Maintainers'
-          debchange --newversion ${{ github.event.release.tag_name }} -b "New upstream release"
+          debchange --newversion "${GITHUB_REF_NAME}" -b "New upstream release"
       - name: Build package
         run: |
           mk-build-deps -i -r -t 'apt-get -f -y --force-yes'
           dpkg-buildpackage -b -us -uc -rfakeroot
       - name: Store package
         run: |
           mkdir -p packages/all
```

### Comparing `c65beka-1.0.0/.github/workflows/release-python.yml` & `c65beka-1.0.1/.github/workflows/release-python.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
   python-package:
     name: "Build and publish python packages"
     runs-on: ubuntu-latest
     environment:
       name: "release"
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Set up python-${{ env.RELEASE_PY_VER }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ env.RELEASE_PY_VER }}
       - name: Build python package
         run: python3 setup.py sdist
       - name: Publish python package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.4.2
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `c65beka-1.0.0/.github/workflows/tests-codecheck.yml` & `c65beka-1.0.1/.github/workflows/tests-codecheck.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 
 jobs:
   pylint:
     name: Pylint
     runs-on: ubuntu-latest
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Set up python-${{ env.CODECHECK_PY_VER }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ env.CODECHECK_PY_VER }}
       - name: Install dependencies
         run: |
           pip3 install --upgrade -r "codecheck-requirements.txt"
       - name: Run pylint
         run: |
           ./test/codecheck/pylint.sh
 
   pytype:
     name: Pytype
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9]
+        python-version: [3.8, 3.9, '3.10']
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Set up python-${{ env.CODECHECK_PY_VER }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ env.CODECHECK_PY_VER }}
       - name: Install dependencies
         run: |
           pip3 install --upgrade -r "codecheck-requirements.txt"
       - name: Run pytype
         run: |
```

### Comparing `c65beka-1.0.0/.github/workflows/tests-unit.yml` & `c65beka-1.0.1/.github/workflows/tests-unit.yml`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 jobs:
   unit-tests:
     name: Unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.5, 3.6, 3.7, 3.8, 3.9]
+        python-version: [3.8, 3.9, '3.10', 3.11]
     steps:
       - name: Checkout repo
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Set up python-${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Run unit tests
         run: |
           BEKA_TESTS=-uz ./run_tests.sh
       - if: ${{ matrix.python-version == env.CODECOV_PY_VER }}
         name: Upload codecov
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
```

### Comparing `c65beka-1.0.0/LICENSE` & `c65beka-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/PKG-INFO` & `c65beka-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: c65beka
-Version: 1.0.0
+Version: 1.0.1
 Summary: A bare-bones BGP speaker
-Home-page: https://github.com/faucetsdn/beka
+Home-page: https://github.com/c65sdn/beka
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache-2
 Description: 
         Beka is a fairly basic BGP speaker. It can send
         and receive unicast route updates in IPv4 and IPv6,
         but not too much else. It is designed to be simple to use
         and to extend, without too much overhead.
         
         It uses eventlet for concurrency, but is easy enough to port to
         gevent if that takes your fancy.
         
-        More information at https://github.com/c65beka/beka
+        More information at https://github.com/c65sdn/beka
 Keywords: bgp,beka,routing,sdn,networking
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.8
```

### Comparing `c65beka-1.0.0/README.md` & `c65beka-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Beka
 
-[![Build Status](https://github.com/faucetsdn/beka/workflows/Unit%20tests/badge.svg?branch=master)](https://github.com/faucetsdn/beka/actions?query=workflow%3A%22Unit+tests%22)
-[![Test Coverage](https://codecov.io/gh/faucetsdn/beka/branch/master/graph/badge.svg)](https://codecov.io/gh/faucetsdn/beka)
+[![Build Status](https://github.com/faucetsdn/beka/workflows/Unit%20tests/badge.svg?branch=main)](https://github.com/faucetsdn/beka/actions?query=workflow%3A%22Unit+tests%22)
+[![Test Coverage](https://codecov.io/gh/faucetsdn/beka/branch/main/graph/badge.svg)](https://codecov.io/gh/faucetsdn/beka)
 
 Beka is a fairly basic BGP speaker. It can send
 and receive unicast route updates in IPv4 and IPv6,
 but not too much else. It is designed to be simple to use
 and to extend, without too much overhead.
 
 It uses eventlet for concurrency, but is easy enough to port to
```

### Comparing `c65beka-1.0.0/beka/beka.py` & `c65beka-1.0.1/beka/beka.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/bgp_message.py` & `c65beka-1.0.1/beka/bgp_message.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/chopper.py` & `c65beka-1.0.1/beka/chopper.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/event.py` & `c65beka-1.0.1/beka/event.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/ip.py` & `c65beka-1.0.1/beka/ip.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/peering.py` & `c65beka-1.0.1/beka/peering.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/route.py` & `c65beka-1.0.1/beka/route.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/state_machine.py` & `c65beka-1.0.1/beka/state_machine.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/beka/stream_server.py` & `c65beka-1.0.1/beka/stream_server.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/bird.conf` & `c65beka-1.0.1/bird.conf`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/bird6.conf` & `c65beka-1.0.1/bird6.conf`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/c65beka.egg-info/PKG-INFO` & `c65beka-1.0.1/c65beka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: c65beka
-Version: 1.0.0
+Version: 1.0.1
 Summary: A bare-bones BGP speaker
-Home-page: https://github.com/faucetsdn/beka
+Home-page: https://github.com/c65sdn/beka
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache-2
 Description: 
         Beka is a fairly basic BGP speaker. It can send
         and receive unicast route updates in IPv4 and IPv6,
         but not too much else. It is designed to be simple to use
         and to extend, without too much overhead.
         
         It uses eventlet for concurrency, but is easy enough to port to
         gevent if that takes your fancy.
         
-        More information at https://github.com/c65beka/beka
+        More information at https://github.com/c65sdn/beka
 Keywords: bgp,beka,routing,sdn,networking
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.5
+Requires-Python: >=3.8
```

### Comparing `c65beka-1.0.0/c65beka.egg-info/SOURCES.txt` & `c65beka-1.0.1/c65beka.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.renovaterc.json
 .stickler.yml
 AUTHORS
 ChangeLog
 LICENSE
 README.md
 beka.yaml
 bird.conf
@@ -15,19 +14,20 @@
 deploy_test.sh
 requirements.txt
 run.py
 run_tests.sh
 setup.cfg
 setup.py
 test-requirements.txt
-.github/workflows/release-debian.yml
+.github/dependabot.yml
 .github/workflows/release-python.yml
 .github/workflows/tests-codecheck.yml
 .github/workflows/tests-unit.yml
 .github/workflows/tests-yaml-lint.yml
+.github/workflows/disabled/release-debian.yml
 beka/__init__.py
 beka/beka.py
 beka/bgp_message.py
 beka/chopper.py
 beka/error.py
 beka/event.py
 beka/ip.py
```

### Comparing `c65beka-1.0.0/debian/control` & `c65beka-1.0.1/debian/control`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Source: beka
 Section: python
 Priority: optional
-Maintainer: Brad Cowie <brad@faucet.nz>
-Build-Depends: debhelper (>=9),
+Maintainer: Faucet Maintainers <maintainers@faucet.nz>
+Build-Depends: debhelper (>= 11),
                dh-python,
                python3-all,
                python3-setuptools,
-               python3-pbr (>=1.9),
-               python3-eventlet
+               python3-eventlet,
+               python3-pbr (>= 1.9),
 Standards-Version: 3.9.6
-Homepage: https://pypi.org/project/beka/
-X-Python3-Version: >= 3.2
-#Vcs-Git: git://github.com/faucetsdn/beka.git
-#Vcs-Browser: https://github.com/faucetsdn/beka.git
+Homepage: https://github.com/faucetsdn/beka
+X-Python3-Version: >= 3.8
+Vcs-Git: https://github.com/faucetsdn/beka.git
+Vcs-Browser: https://github.com/faucetsdn/beka
 
 Package: python3-beka
 Architecture: all
-Depends: ${python3:Depends}, ${misc:Depends}
+Depends: ${python3:Depends},
+         python3:any (>= 3.8~),
+         ${misc:Depends}
 Description: Beka is a fairly basic BGP speaker. (Python 3)
  It can send and receive unicast route updates in IPv4 and IPv6,
  but not too much else. It is designed to be simple to use and to
  extend, without too much overhead.
  .
  This package installs the library for Python 3.
```

### Comparing `c65beka-1.0.0/debian/copyright` & `c65beka-1.0.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/deploy_bird.sh` & `c65beka-1.0.1/deploy_bird.sh`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/run.py` & `c65beka-1.0.1/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         self.greenlets = []
         self.bekas = []
 
     def run(self):
         signal.signal(signal.SIGINT, self.signal_handler)
         pool = GreenPool()
 
-        with open("beka.yaml") as file:
-            config = yaml.load(file.read())
+        with open("beka.yaml", encoding='utf-8') as file:
+            config = yaml.safe_load(file.read())
         for router in config["routers"]:
             printmsg("Starting Beka on %s" % router["local_address"])
             beka = Beka(
                 router["local_address"],
                 router["bgp_port"],
                 router["local_as"],
                 router["router_id"],
@@ -58,24 +58,24 @@
         self.shutdown()
 
     def shutdown(self):
         for beka in self.bekas:
             printmsg("Shutting down Beka %s" % beka)
             beka.shutdown()
 
-    def peer_up_handler(self, peer_ip, peer_as):  # pylint: disable=no-self-use
+    def peer_up_handler(self, peer_ip, peer_as):
         printmsg("[Peer up] %s %d" % (peer_ip, peer_as))
 
-    def peer_down_handler(self, peer_ip, peer_as):  # pylint: disable=no-self-use
+    def peer_down_handler(self, peer_ip, peer_as):
         printmsg("[Peer down] %s %s" % (peer_ip, peer_as))
 
-    def error_handler(self, msg):  # pylint: disable=no-self-use
+    def error_handler(self, msg):
         printmsg("[Error] %s" % msg)
 
-    def route_handler(self, route_update):  # pylint: disable=no-self-use
+    def route_handler(self, route_update):
         if route_update.is_withdraw:
             printmsg("[Route handler] Route removed: %s" % route_update)
         else:
             printmsg("[Route handler] New route received: %s" % route_update)
 
 
 if __name__ == "__main__":
```

### Comparing `c65beka-1.0.0/run_tests.sh` & `c65beka-1.0.1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/setup.cfg` & `c65beka-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 	and receive unicast route updates in IPv4 and IPv6,
 	but not too much else. It is designed to be simple to use
 	and to extend, without too much overhead.
 	
 	It uses eventlet for concurrency, but is easy enough to port to
 	gevent if that takes your fancy.
 	
-	More information at https://github.com/c65beka/beka
+	More information at https://github.com/c65sdn/beka
 license = Apache-2
 author = Sam Russell
 author-email = sam.h.russell@gmail.com
-home-page = https://github.com/faucetsdn/beka
+home-page = https://github.com/c65sdn/beka
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 keywords = 
 	bgp
```

### Comparing `c65beka-1.0.0/test/codecheck/src_files.sh` & `c65beka-1.0.1/test/codecheck/src_files.sh`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/test/unit/test_beka.py` & `c65beka-1.0.1/test/unit/test_beka.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/test/unit/test_bgp_message.py` & `c65beka-1.0.1/test/unit/test_bgp_message.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/test/unit/test_chopper.py` & `c65beka-1.0.1/test/unit/test_chopper.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/test/unit/test_ip.py` & `c65beka-1.0.1/test/unit/test_ip.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/test/unit/test_peering.py` & `c65beka-1.0.1/test/unit/test_peering.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class FakeSocket():  # pylint: disable=too-few-public-methods
     """Mocked Socket"""
 
     def __init__(self):
         pass
 
-    def makefile(self, *args, **kwargs):  # pylint: disable=unused-argument,no-self-use
+    def makefile(self, *args, **kwargs):  # pylint: disable=unused-argument
         return None
 
 
 class FakeChopper():  # pylint: disable=too-few-public-methods
     """Mocked Chopper"""
 
     def __init__(self):
```

### Comparing `c65beka-1.0.0/test/unit/test_state_machine.py` & `c65beka-1.0.1/test/unit/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `c65beka-1.0.0/test/unit/test_timer.py` & `c65beka-1.0.1/test/unit/test_timer.py`

 * *Files identical despite different names*

