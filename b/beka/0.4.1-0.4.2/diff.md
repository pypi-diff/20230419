# Comparing `tmp/beka-0.4.1.tar.gz` & `tmp/beka-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beka-0.4.1.tar", last modified: Tue Feb  1 20:57:29 2022, max compression
+gzip compressed data, was "beka-0.4.2.tar", last modified: Tue Apr 18 22:12:07 2023, max compression
```

## Comparing `beka-0.4.1.tar` & `beka-0.4.2.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.964844 beka-0.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.952844 beka-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.956844 beka-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-02-01 20:57:27.000000 beka-0.4.1/.github/workflows/release-debian.yml
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-02-01 20:57:27.000000 beka-0.4.1/.github/workflows/release-python.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-02-01 20:57:27.000000 beka-0.4.1/.github/workflows/tests-codecheck.yml
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-02-01 20:57:27.000000 beka-0.4.1/.github/workflows/tests-unit.yml
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-01 20:57:27.000000 beka-0.4.1/.github/workflows/tests-yaml-lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-02-01 20:57:27.000000 beka-0.4.1/.renovaterc.json
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-02-01 20:57:27.000000 beka-0.4.1/.stickler.yml
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-02-01 20:57:29.000000 beka-0.4.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-02-01 20:57:29.000000 beka-0.4.1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)    10758 2022-02-01 20:57:27.000000 beka-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-02-01 20:57:29.964844 beka-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-02-01 20:57:27.000000 beka-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.960844 beka-0.4.1/beka/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:27.000000 beka-0.4.1/beka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-02-01 20:57:27.000000 beka-0.4.1/beka/beka.py
--rw-r--r--   0 runner    (1001) docker     (121)    20682 2022-02-01 20:57:27.000000 beka-0.4.1/beka/bgp_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2022-02-01 20:57:27.000000 beka-0.4.1/beka/chopper.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-02-01 20:57:27.000000 beka-0.4.1/beka/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-01 20:57:27.000000 beka-0.4.1/beka/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-02-01 20:57:27.000000 beka-0.4.1/beka/ip.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-02-01 20:57:27.000000 beka-0.4.1/beka/packing_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     3690 2022-02-01 20:57:27.000000 beka-0.4.1/beka/peering.py
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-02-01 20:57:27.000000 beka-0.4.1/beka/route.py
--rw-r--r--   0 runner    (1001) docker     (121)    11203 2022-02-01 20:57:27.000000 beka-0.4.1/beka/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-02-01 20:57:27.000000 beka-0.4.1/beka/stream_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-02-01 20:57:27.000000 beka-0.4.1/beka/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.960844 beka-0.4.1/beka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-02-01 20:57:29.000000 beka-0.4.1/beka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-02-01 20:57:29.000000 beka-0.4.1/beka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 20:57:29.000000 beka-0.4.1/beka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-01 20:57:29.000000 beka-0.4.1/beka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-01 20:57:29.000000 beka-0.4.1/beka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-01 20:57:29.000000 beka-0.4.1/beka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-02-01 20:57:27.000000 beka-0.4.1/beka.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-02-01 20:57:27.000000 beka-0.4.1/bird.conf
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-01 20:57:27.000000 beka-0.4.1/bird6.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)       41 2022-02-01 20:57:27.000000 beka-0.4.1/birdc.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)       44 2022-02-01 20:57:27.000000 beka-0.4.1/birdc6.sh
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-02-01 20:57:27.000000 beka-0.4.1/codecheck-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-02-01 20:57:27.000000 beka-0.4.1/daemon.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.960844 beka-0.4.1/debian/
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-02-01 20:57:27.000000 beka-0.4.1/debian/README.source
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-02-01 20:57:27.000000 beka-0.4.1/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-02-01 20:57:27.000000 beka-0.4.1/debian/compat
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-02-01 20:57:27.000000 beka-0.4.1/debian/control
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-02-01 20:57:27.000000 beka-0.4.1/debian/copyright
--rwxr-xr-x   0 runner    (1001) docker     (121)       95 2022-02-01 20:57:27.000000 beka-0.4.1/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.960844 beka-0.4.1/debian/source/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-01 20:57:27.000000 beka-0.4.1/debian/source/format
--rwxr-xr-x   0 runner    (1001) docker     (121)      630 2022-02-01 20:57:27.000000 beka-0.4.1/deploy_bird.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      173 2022-02-01 20:57:27.000000 beka-0.4.1/deploy_test.sh
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-02-01 20:57:27.000000 beka-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-02-01 20:57:27.000000 beka-0.4.1/run.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1069 2022-02-01 20:57:27.000000 beka-0.4.1/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-02-01 20:57:29.964844 beka-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      486 2022-02-01 20:57:27.000000 beka-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.956844 beka-0.4.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.964844 beka-0.4.1/test/codecheck/
--rwxr-xr-x   0 runner    (1001) docker     (121)      378 2022-02-01 20:57:27.000000 beka-0.4.1/test/codecheck/min_pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      234 2022-02-01 20:57:27.000000 beka-0.4.1/test/codecheck/pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (121)      668 2022-02-01 20:57:27.000000 beka-0.4.1/test/codecheck/src_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-01 20:57:29.964844 beka-0.4.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_beka.py
--rw-r--r--   0 runner    (1001) docker     (121)    14199 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_bgp_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_chopper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_peering.py
--rw-r--r--   0 runner    (1001) docker     (121)    22393 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-02-01 20:57:27.000000 beka-0.4.1/test/unit/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-02-01 20:57:27.000000 beka-0.4.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.559074 beka-0.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-18 22:12:01.000000 beka-0.4.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.559074 beka-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 22:12:01.000000 beka-0.4.2/.github/workflows/release-debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 22:12:01.000000 beka-0.4.2/.github/workflows/release-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-18 22:12:01.000000 beka-0.4.2/.github/workflows/tests-codecheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 22:12:01.000000 beka-0.4.2/.github/workflows/tests-unit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-18 22:12:01.000000 beka-0.4.2/.github/workflows/tests-yaml-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 22:12:01.000000 beka-0.4.2/.stickler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 22:12:07.000000 beka-0.4.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 22:12:07.000000 beka-0.4.2/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-18 22:12:01.000000 beka-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-18 22:12:07.563074 beka-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-18 22:12:01.000000 beka-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/beka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:01.000000 beka-0.4.2/beka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-18 22:12:01.000000 beka-0.4.2/beka/beka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-18 22:12:01.000000 beka-0.4.2/beka/bgp_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-18 22:12:01.000000 beka-0.4.2/beka/chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 22:12:01.000000 beka-0.4.2/beka/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-18 22:12:01.000000 beka-0.4.2/beka/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-18 22:12:01.000000 beka-0.4.2/beka/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-18 22:12:01.000000 beka-0.4.2/beka/packing_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-18 22:12:01.000000 beka-0.4.2/beka/peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-18 22:12:01.000000 beka-0.4.2/beka/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-18 22:12:01.000000 beka-0.4.2/beka/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-18 22:12:01.000000 beka-0.4.2/beka/stream_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 22:12:01.000000 beka-0.4.2/beka/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/beka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 22:12:07.000000 beka-0.4.2/beka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-18 22:12:01.000000 beka-0.4.2/beka.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-18 22:12:01.000000 beka-0.4.2/bird.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-18 22:12:01.000000 beka-0.4.2/bird6.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-04-18 22:12:01.000000 beka-0.4.2/birdc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-04-18 22:12:01.000000 beka-0.4.2/birdc6.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 22:12:01.000000 beka-0.4.2/codecheck-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 22:12:01.000000 beka-0.4.2/daemon.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 22:12:01.000000 beka-0.4.2/debian/README.source
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 22:12:01.000000 beka-0.4.2/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-18 22:12:01.000000 beka-0.4.2/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-18 22:12:01.000000 beka-0.4.2/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 22:12:01.000000 beka-0.4.2/debian/copyright
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-04-18 22:12:01.000000 beka-0.4.2/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 22:12:01.000000 beka-0.4.2/debian/source/format
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-18 22:12:01.000000 beka-0.4.2/deploy_bird.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-04-18 22:12:01.000000 beka-0.4.2/deploy_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:12:01.000000 beka-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-18 22:12:01.000000 beka-0.4.2/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-04-18 22:12:01.000000 beka-0.4.2/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-18 22:12:07.563074 beka-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-04-18 22:12:01.000000 beka-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.555074 beka-0.4.2/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/test/codecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-04-18 22:12:01.000000 beka-0.4.2/test/codecheck/min_pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-18 22:12:01.000000 beka-0.4.2/test/codecheck/pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-18 22:12:01.000000 beka-0.4.2/test/codecheck/src_files.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:12:07.563074 beka-0.4.2/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_beka.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_bgp_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_chopper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22393 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-18 22:12:01.000000 beka-0.4.2/test/unit/test_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 22:12:01.000000 beka-0.4.2/test-requirements.txt
```

### Comparing `beka-0.4.1/.github/workflows/release-debian.yml` & `beka-0.4.2/.github/workflows/release-debian.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,23 +11,23 @@
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
           debchange --newversion "${GITHUB_REF_NAME}" -b "New upstream release"
       - name: Build package
         run: |
```

### Comparing `beka-0.4.1/.github/workflows/release-python.yml` & `beka-0.4.2/.github/workflows/release-python.yml`

 * *Files 2% similar despite different names*

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
-        uses: pypa/gh-action-pypi-publish@v1.5.0
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `beka-0.4.1/.github/workflows/tests-codecheck.yml` & `beka-0.4.2/.github/workflows/tests-codecheck.yml`

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
-        python-version: [3.7, 3.8, 3.9]
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

### Comparing `beka-0.4.1/.github/workflows/tests-unit.yml` & `beka-0.4.2/.github/workflows/tests-unit.yml`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 jobs:
   unit-tests:
     name: Unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.7, 3.8, 3.9]
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

### Comparing `beka-0.4.1/LICENSE` & `beka-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/PKG-INFO` & `beka-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: beka
-Version: 0.4.1
+Version: 0.4.2
 Summary: A bare-bones BGP speaker
 Home-page: https://github.com/faucetsdn/beka
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache-2
 Description: 
         Beka is a fairly basic BGP speaker. It can send
@@ -18,8 +18,8 @@
         More information at https://github.com/faucetsdn/beka
 Keywords: bgp,beka,routing,sdn,networking
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `beka-0.4.1/README.md` & `beka-0.4.2/README.md`

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

### Comparing `beka-0.4.1/beka/beka.py` & `beka-0.4.2/beka/beka.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/bgp_message.py` & `beka-0.4.2/beka/bgp_message.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/chopper.py` & `beka-0.4.2/beka/chopper.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/event.py` & `beka-0.4.2/beka/event.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/ip.py` & `beka-0.4.2/beka/ip.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/peering.py` & `beka-0.4.2/beka/peering.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/route.py` & `beka-0.4.2/beka/route.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/state_machine.py` & `beka-0.4.2/beka/state_machine.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka/stream_server.py` & `beka-0.4.2/beka/stream_server.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/beka.egg-info/PKG-INFO` & `beka-0.4.2/beka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: beka
-Version: 0.4.1
+Version: 0.4.2
 Summary: A bare-bones BGP speaker
 Home-page: https://github.com/faucetsdn/beka
 Author: Sam Russell
 Author-email: sam.h.russell@gmail.com
 License: Apache-2
 Description: 
         Beka is a fairly basic BGP speaker. It can send
@@ -18,8 +18,8 @@
         More information at https://github.com/faucetsdn/beka
 Keywords: bgp,beka,routing,sdn,networking
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.8
```

### Comparing `beka-0.4.1/beka.egg-info/SOURCES.txt` & `beka-0.4.2/beka.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

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
@@ -15,14 +14,15 @@
 deploy_test.sh
 requirements.txt
 run.py
 run_tests.sh
 setup.cfg
 setup.py
 test-requirements.txt
+.github/dependabot.yml
 .github/workflows/release-debian.yml
 .github/workflows/release-python.yml
 .github/workflows/tests-codecheck.yml
 .github/workflows/tests-unit.yml
 .github/workflows/tests-yaml-lint.yml
 beka/__init__.py
 beka/beka.py
@@ -37,14 +37,15 @@
 beka/state_machine.py
 beka/stream_server.py
 beka/timer.py
 beka.egg-info/PKG-INFO
 beka.egg-info/SOURCES.txt
 beka.egg-info/dependency_links.txt
 beka.egg-info/not-zip-safe
+beka.egg-info/pbr.json
 beka.egg-info/requires.txt
 beka.egg-info/top_level.txt
 debian/README.source
 debian/changelog
 debian/compat
 debian/control
 debian/copyright
```

### Comparing `beka-0.4.1/bird.conf` & `beka-0.4.2/bird.conf`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/bird6.conf` & `beka-0.4.2/bird6.conf`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/debian/control` & `beka-0.4.2/debian/control`

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
-X-Python3-Version: >= 3.7
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

### Comparing `beka-0.4.1/debian/copyright` & `beka-0.4.2/debian/copyright`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/deploy_bird.sh` & `beka-0.4.2/deploy_bird.sh`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/run.py` & `beka-0.4.2/run.py`

 * *Files 14% similar despite different names*

```diff
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

### Comparing `beka-0.4.1/run_tests.sh` & `beka-0.4.2/run_tests.sh`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/setup.cfg` & `beka-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/codecheck/src_files.sh` & `beka-0.4.2/test/codecheck/src_files.sh`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/unit/test_beka.py` & `beka-0.4.2/test/unit/test_beka.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/unit/test_bgp_message.py` & `beka-0.4.2/test/unit/test_bgp_message.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/unit/test_chopper.py` & `beka-0.4.2/test/unit/test_chopper.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/unit/test_ip.py` & `beka-0.4.2/test/unit/test_ip.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/unit/test_peering.py` & `beka-0.4.2/test/unit/test_peering.py`

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

### Comparing `beka-0.4.1/test/unit/test_state_machine.py` & `beka-0.4.2/test/unit/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `beka-0.4.1/test/unit/test_timer.py` & `beka-0.4.2/test/unit/test_timer.py`

 * *Files identical despite different names*

