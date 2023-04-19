# Comparing `tmp/docker_composer_v2-0.8.5.tar.gz` & `tmp/docker_composer_v2-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_composer_v2-0.8.5.tar", max compression
+gzip compressed data, was "docker_composer_v2-0.8.6.tar", max compression
```

## Comparing `docker_composer_v2-0.8.5.tar` & `docker_composer_v2-0.8.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rwxr-xr-x   0        0        0    11358 2023-04-19 17:21:29.639833 docker_composer_v2-0.8.5/LICENSE.txt
--rwxr-xr-x   0        0        0     2347 2023-04-19 17:21:29.639833 docker_composer_v2-0.8.5/README.md
--rwxr-xr-x   0        0        0     1434 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/pyproject.toml
--rwxr-xr-x   0        0        0       60 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/__init__.py
--rwxr-xr-x   0        0        0        0 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/__init__.py
--rw-r--r--   0        0        0      184 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     7902 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/argument.cpython-311.pyc
--rw-r--r--   0        0        0    14761 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/generate_class.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    14876 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/generate_class.cpython-311.pyc
--rwxr-xr-x   0        0        0     4482 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/argument.py
--rwxr-xr-x   0        0        0     7724 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/_utils/generate_class.py
--rwxr-xr-x   0        0        0     3997 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/base.py
--rwxr-xr-x   0        0        0        0 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/py.typed
--rw-r--r--   0        0        0    36637 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/__pycache__/root.cpython-311.pyc
--rw-r--r--   0        0        0     1123 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/build.cpython-311.pyc
--rw-r--r--   0        0        0     1226 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     1243 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/cp.cpython-311.pyc
--rw-r--r--   0        0        0     1064 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/create.cpython-311.pyc
--rw-r--r--   0        0        0     1194 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/down.cpython-311.pyc
--rw-r--r--   0        0        0     1067 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/events.cpython-311.pyc
--rw-r--r--   0        0        0     1339 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/exec.cpython-311.pyc
--rw-r--r--   0        0        0     1135 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/images.cpython-311.pyc
--rw-r--r--   0        0        0     1124 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/kill.cpython-311.pyc
--rw-r--r--   0        0        0     1192 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/logs.cpython-311.pyc
--rw-r--r--   0        0        0     1097 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/ls.cpython-311.pyc
--rw-r--r--   0        0        0      936 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/pause.cpython-311.pyc
--rw-r--r--   0        0        0     1054 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/port.cpython-311.pyc
--rw-r--r--   0        0        0     1100 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/ps.cpython-311.pyc
--rw-r--r--   0        0        0     1123 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/pull.cpython-311.pyc
--rw-r--r--   0        0        0     1126 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/push.cpython-311.pyc
--rw-r--r--   0        0        0     1129 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/restart.cpython-311.pyc
--rw-r--r--   0        0        0     1413 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/rm.cpython-311.pyc
--rw-r--r--   0        0        0     1691 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/run.cpython-311.pyc
--rw-r--r--   0        0        0      936 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/start.cpython-311.pyc
--rw-r--r--   0        0        0     1016 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/stop.cpython-311.pyc
--rw-r--r--   0        0        0      944 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/top.cpython-311.pyc
--rw-r--r--   0        0        0      946 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/unpause.cpython-311.pyc
--rw-r--r--   0        0        0     1315 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/up.cpython-311.pyc
--rw-r--r--   0        0        0     1044 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0     1150 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/build.py
--rw-r--r--   0        0        0     1506 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/config.py
--rw-r--r--   0        0        0      923 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/cp.py
--rw-r--r--   0        0        0     1226 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/create.py
--rw-r--r--   0        0        0     1048 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/down.py
--rw-r--r--   0        0        0      606 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/events.py
--rw-r--r--   0        0        0     1236 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/exec.py
--rw-r--r--   0        0        0      695 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/images.py
--rw-r--r--   0        0        0      734 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/kill.py
--rw-r--r--   0        0        0     1157 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/logs.py
--rw-r--r--   0        0        0      799 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/ls.py
--rw-r--r--   0        0        0      461 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/pause.py
--rw-r--r--   0        0        0      674 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/port.py
--rw-r--r--   0        0        0     1069 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/ps.py
--rw-r--r--   0        0        0      869 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/pull.py
--rw-r--r--   0        0        0      826 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/push.py
--rw-r--r--   0        0        0      687 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/restart.py
--rw-r--r--   0        0        0     1012 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/rm.py
--rw-r--r--   0        0        0     2111 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/run.py
--rw-r--r--   0        0        0      461 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/start.py
--rw-r--r--   0        0        0      562 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/stop.py
--rw-r--r--   0        0        0      471 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/top.py
--rw-r--r--   0        0        0      469 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/unpause.py
--rw-r--r--   0        0        0     2979 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/up.py
--rw-r--r--   0        0        0      667 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/version.py
--rw-r--r--   0        0        0    25842 2023-04-19 17:21:29.643833 docker_composer_v2-0.8.5/src/docker_composer/runner/root.py
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 docker_composer_v2-0.8.5/PKG-INFO
+-rwxr-xr-x   0        0        0    11358 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/LICENSE.txt
+-rwxr-xr-x   0        0        0     2347 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/README.md
+-rwxr-xr-x   0        0        0     1489 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/pyproject.toml
+-rwxr-xr-x   0        0        0       60 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__init__.py
+-rw-r--r--   0        0        0      184 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7902 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/argument.cpython-311.pyc
+-rw-r--r--   0        0        0    14761 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/generate_class.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    14876 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/generate_class.cpython-311.pyc
+-rwxr-xr-x   0        0        0     4482 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/argument.py
+-rwxr-xr-x   0        0        0     7724 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/_utils/generate_class.py
+-rwxr-xr-x   0        0        0     3997 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/base.py
+-rwxr-xr-x   0        0        0        0 2023-04-19 17:34:21.784500 docker_composer_v2-0.8.6/src/docker_composer/py.typed
+-rw-r--r--   0        0        0    36637 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/__pycache__/root.cpython-311.pyc
+-rw-r--r--   0        0        0     1123 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/build.cpython-311.pyc
+-rw-r--r--   0        0        0     1226 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     1243 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/cp.cpython-311.pyc
+-rw-r--r--   0        0        0     1064 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/create.cpython-311.pyc
+-rw-r--r--   0        0        0     1194 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/down.cpython-311.pyc
+-rw-r--r--   0        0        0     1067 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/events.cpython-311.pyc
+-rw-r--r--   0        0        0     1339 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/exec.cpython-311.pyc
+-rw-r--r--   0        0        0     1135 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/images.cpython-311.pyc
+-rw-r--r--   0        0        0     1124 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/kill.cpython-311.pyc
+-rw-r--r--   0        0        0     1192 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/logs.cpython-311.pyc
+-rw-r--r--   0        0        0     1097 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/ls.cpython-311.pyc
+-rw-r--r--   0        0        0      936 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/pause.cpython-311.pyc
+-rw-r--r--   0        0        0     1054 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/port.cpython-311.pyc
+-rw-r--r--   0        0        0     1100 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/ps.cpython-311.pyc
+-rw-r--r--   0        0        0     1123 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/pull.cpython-311.pyc
+-rw-r--r--   0        0        0     1126 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/push.cpython-311.pyc
+-rw-r--r--   0        0        0     1129 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/restart.cpython-311.pyc
+-rw-r--r--   0        0        0     1413 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/rm.cpython-311.pyc
+-rw-r--r--   0        0        0     1691 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/run.cpython-311.pyc
+-rw-r--r--   0        0        0      936 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/start.cpython-311.pyc
+-rw-r--r--   0        0        0     1016 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/stop.cpython-311.pyc
+-rw-r--r--   0        0        0      944 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/top.cpython-311.pyc
+-rw-r--r--   0        0        0      946 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/unpause.cpython-311.pyc
+-rw-r--r--   0        0        0     1315 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/up.cpython-311.pyc
+-rw-r--r--   0        0        0     1044 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0        0        0     1150 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/build.py
+-rw-r--r--   0        0        0     1506 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/config.py
+-rw-r--r--   0        0        0      923 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1226 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/create.py
+-rw-r--r--   0        0        0     1048 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/down.py
+-rw-r--r--   0        0        0      606 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/events.py
+-rw-r--r--   0        0        0     1236 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/exec.py
+-rw-r--r--   0        0        0      695 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/images.py
+-rw-r--r--   0        0        0      734 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1157 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/logs.py
+-rw-r--r--   0        0        0      799 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ls.py
+-rw-r--r--   0        0        0      461 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/pause.py
+-rw-r--r--   0        0        0      674 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/port.py
+-rw-r--r--   0        0        0     1069 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ps.py
+-rw-r--r--   0        0        0      869 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/pull.py
+-rw-r--r--   0        0        0      826 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/push.py
+-rw-r--r--   0        0        0      687 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1012 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2111 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/run.py
+-rw-r--r--   0        0        0      461 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/start.py
+-rw-r--r--   0        0        0      562 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/stop.py
+-rw-r--r--   0        0        0      471 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/top.py
+-rw-r--r--   0        0        0      469 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     2979 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/up.py
+-rw-r--r--   0        0        0      667 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/version.py
+-rw-r--r--   0        0        0    25842 2023-04-19 17:34:21.788499 docker_composer_v2-0.8.6/src/docker_composer/runner/root.py
+-rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 docker_composer_v2-0.8.6/PKG-INFO
```

### Comparing `docker_composer_v2-0.8.5/LICENSE.txt` & `docker_composer_v2-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/README.md` & `docker_composer_v2-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/pyproject.toml` & `docker_composer_v2-0.8.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "docker-composer-v2"
-version = "0.8.5"
+version = "0.8.6"
 description = "Use `docker compose` from within Python. This is a branch forked from https://github.com/schollm/docker-composer to support Docker Compose V2."
-authors = ["Micha <schollm-git@gmx.com>"]
+authors = ["Micha <schollm-git@gmx.com>", "Jensen <jensen@kairosaerospace.com>"]
 readme = "README.md"
-homepage = "https://github.com/schollm/docker-composer"
-repository = "https://github.com/schollm/docker-composer"
+homepage = "https://github.com/jensenkairos/docker-composer-v2"
+repository = "https://github.com/jensenkairos/docker-composer-v2"
 license = "Apache-2.0"
 packages = [
     { include = "docker_composer", from = "src" },
 ]
 classifiers = [
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
```

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/argument.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/argument.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/generate_class.cpython-311-pytest-7.3.1.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/generate_class.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/_utils/__pycache__/generate_class.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/_utils/__pycache__/generate_class.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/_utils/argument.py` & `docker_composer_v2-0.8.6/src/docker_composer/_utils/argument.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/_utils/generate_class.py` & `docker_composer_v2-0.8.6/src/docker_composer/_utils/generate_class.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/base.py` & `docker_composer_v2-0.8.6/src/docker_composer/base.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/__pycache__/root.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/__pycache__/root.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/build.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/build.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/config.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/cp.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/cp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/create.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/create.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/down.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/down.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/events.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/events.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/exec.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/exec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/images.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/images.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/kill.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/kill.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/logs.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/logs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/ls.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/ls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/pause.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/pause.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/port.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/port.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/ps.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/ps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/pull.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/pull.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/push.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/push.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/restart.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/restart.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/rm.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/rm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/run.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/run.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/start.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/start.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/stop.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/stop.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/top.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/top.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/unpause.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/unpause.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/up.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/up.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/__pycache__/version.cpython-311.pyc` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/__pycache__/version.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/build.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/build.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/config.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/config.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/cp.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/cp.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/create.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/create.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/down.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/down.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/events.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/events.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/exec.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/exec.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/images.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/images.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/kill.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/kill.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/logs.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/logs.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/ls.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ls.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/port.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/port.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/ps.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/ps.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/pull.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/pull.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/push.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/push.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/restart.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/restart.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/rm.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/rm.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/run.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/run.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/stop.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/stop.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/up.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/up.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/cmd/version.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/cmd/version.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/src/docker_composer/runner/root.py` & `docker_composer_v2-0.8.6/src/docker_composer/runner/root.py`

 * *Files identical despite different names*

### Comparing `docker_composer_v2-0.8.5/PKG-INFO` & `docker_composer_v2-0.8.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: docker-composer-v2
-Version: 0.8.5
+Version: 0.8.6
 Summary: Use `docker compose` from within Python. This is a branch forked from https://github.com/schollm/docker-composer to support Docker Compose V2.
-Home-page: https://github.com/schollm/docker-composer
+Home-page: https://github.com/jensenkairos/docker-composer-v2
 License: Apache-2.0
 Author: Micha
 Author-email: schollm-git@gmx.com
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Dist: attrs (>=20.3.0,<21.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
-Project-URL: Repository, https://github.com/schollm/docker-composer
+Project-URL: Repository, https://github.com/jensenkairos/docker-composer-v2
 Description-Content-Type: text/markdown
 
 # Docker Composer
 
 A library to interact with `docker compose` (Compose V2) from a python Program.
 All commands and parameters are exposed as python classes and attributes
 to allow for full auto-completion of its parameters with IDEs
```

