# Comparing `tmp/kraken_std-0.8.4.tar.gz` & `tmp/kraken_std-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_std-0.8.4.tar", max compression
+gzip compressed data, was "kraken_std-0.8.5.tar", max compression
```

## Comparing `kraken_std-0.8.4.tar` & `kraken_std-0.8.5.tar`

### file list

```diff
@@ -1,79 +1,81 @@
--rw-r--r--   0        0        0      988 2023-04-12 13:02:29.929332 kraken_std-0.8.4/LICENSE
--rw-r--r--   0        0        0     1745 2023-04-12 13:03:14.573957 kraken_std-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     1498 2023-04-12 13:02:29.933332 kraken_std-0.8.4/readme.md
--rw-r--r--   0        0        0       22 2023-04-12 13:03:14.573957 kraken_std-0.8.4/src/kraken/std/__init__.py
--rw-r--r--   0        0        0    13390 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/__init__.py
--rw-r--r--   0        0        0     2403 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/config.py
--rw-r--r--   0        0        0     1753 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/data/certs/cert.pem
--rw-r--r--   0        0        0     3243 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/data/certs/key.pem
--rw-r--r--   0        0        0     7912 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/manifest.py
--rw-r--r--   0        0        0     2294 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/mitm.py
--rw-r--r--   0        0        0     1737 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/mitm_impl.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/__init__.py
--rw-r--r--   0        0        0     5640 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
--rw-r--r--   0        0        0     5959 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_build_task.py
--rw-r--r--   0        0        0     3163 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
--rw-r--r--   0        0        0     2177 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
--rw-r--r--   0        0        0      907 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_clippy_task.py
--rw-r--r--   0        0        0      732 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_deny_task.py
--rw-r--r--   0        0        0      730 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_fmt_task.py
--rw-r--r--   0        0        0     2074 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_publish_task.py
--rw-r--r--   0        0        0     2088 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
--rw-r--r--   0        0        0      493 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_test_task.py
--rw-r--r--   0        0        0      391 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_update_task.py
--rw-r--r--   0        0        0      720 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/version.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/descriptors/__init__.py
--rw-r--r--   0        0        0      874 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/descriptors/resource.py
--rw-r--r--   0        0        0    10002 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/dist.py
--rw-r--r--   0        0        0     3911 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/__init__.py
--rw-r--r--   0        0        0     3254 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/buildx.py
--rw-r--r--   0        0        0     1426 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/dockerapi.py
--rw-r--r--   0        0        0     7438 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/kaniko.py
--rw-r--r--   0        0        0     1938 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/manifest_tool.py
--rw-r--r--   0        0        0     3650 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/native.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/py.typed
--rw-r--r--   0        0        0     1214 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/util.py
--rw-r--r--   0        0        0     1761 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/__init__.py
--rw-r--r--   0        0        0     1107 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/config.py
--rw-r--r--   0        0        0     9451 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/gitignore.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/__init__.py
--rw-r--r--   0        0        0      448 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/const.py
--rw-r--r--   0        0        0     2919 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_check_task.py
--rw-r--r--   0        0        0     2754 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_sync_task.py
--rw-r--r--   0        0        0     2973 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/version.py
--rw-r--r--   0        0        0     6368 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/helm/__init__.py
--rw-r--r--   0        0        0     2132 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/helm/helmapi.py
--rw-r--r--   0        0        0     2310 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/http/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/py.typed
--rw-r--r--   0        0        0     1598 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/__init__.py
--rw-r--r--   0        0        0     3586 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/helpers.py
--rw-r--r--   0        0        0     3120 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/maturin.py
--rw-r--r--   0        0        0     7926 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/poetry.py
--rw-r--r--   0        0        0     4415 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/slap.py
--rw-r--r--   0        0        0     4892 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/pyproject.py
--rw-r--r--   0        0        0     6401 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/settings.py
--rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/__init__.py
--rw-r--r--   0        0        0     3249 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/base_task.py
--rw-r--r--   0        0        0     2076 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/black_task.py
--rw-r--r--   0        0        0     1922 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/build_task.py
--rw-r--r--   0        0        0     1046 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/flake8_task.py
--rw-r--r--   0        0        0     2834 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/install_task.py
--rw-r--r--   0        0        0     1844 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/isort_task.py
--rw-r--r--   0        0        0      946 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/login_task.py
--rw-r--r--   0        0        0     1463 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_subtest_task.py
--rw-r--r--   0        0        0     2352 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_task.py
--rw-r--r--   0        0        0     2598 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/publish_task.py
--rw-r--r--   0        0        0     2043 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pycln_task.py
--rw-r--r--   0        0        0     1034 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pylint_task.py
--rw-r--r--   0        0        0     2398 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pytest_task.py
--rw-r--r--   0        0        0     4531 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pyupgrade_task.py
--rw-r--r--   0        0        0     1778 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/update_lockfile_task.py
--rw-r--r--   0        0        0     1656 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/update_pyproject_task.py
--rw-r--r--   0        0        0     1127 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/version.py
--rw-r--r--   0        0        0     4042 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/sccache.py
--rw-r--r--   0        0        0      390 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/__init__.py
--rw-r--r--   0        0        0     1906 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/check_file_exists_and_is_committed_task.py
--rw-r--r--   0        0        0     6010 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/check_valid_readme_exists_task.py
--rw-r--r--   0        0        0     2645 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/copyright_task.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-01-22 14:38:01.549959 kraken_std-0.8.5/LICENSE
+-rw-r--r--   0        0        0     1745 2023-04-19 15:41:46.082711 kraken_std-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     1498 2023-02-08 16:53:28.240291 kraken_std-0.8.5/readme.md
+-rw-r--r--   0        0        0       22 2023-04-19 15:41:46.086711 kraken_std-0.8.5/src/kraken/std/__init__.py
+-rw-r--r--   0        0        0    13390 2023-04-06 12:43:19.047013 kraken_std-0.8.5/src/kraken/std/cargo/__init__.py
+-rw-r--r--   0        0        0     2403 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/config.py
+-rw-r--r--   0        0        0     1753 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/data/certs/cert.pem
+-rw-r--r--   0        0        0     3243 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/data/certs/key.pem
+-rw-r--r--   0        0        0     7912 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/cargo/manifest.py
+-rw-r--r--   0        0        0     2294 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/mitm.py
+-rw-r--r--   0        0        0     1737 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/mitm_impl.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/cargo/tasks/__init__.py
+-rw-r--r--   0        0        0     5640 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
+-rw-r--r--   0        0        0     5959 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_build_task.py
+-rw-r--r--   0        0        0     3163 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
+-rw-r--r--   0        0        0     2177 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
+-rw-r--r--   0        0        0      907 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py
+-rw-r--r--   0        0        0      732 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_deny_task.py
+-rw-r--r--   0        0        0      730 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py
+-rw-r--r--   0        0        0     2074 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_publish_task.py
+-rw-r--r--   0        0        0     2088 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
+-rw-r--r--   0        0        0      493 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_test_task.py
+-rw-r--r--   0        0        0      391 2023-02-14 17:29:44.373684 kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_update_task.py
+-rw-r--r--   0        0        0      720 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/cargo/version.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/descriptors/__init__.py
+-rw-r--r--   0        0        0      874 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/descriptors/resource.py
+-rw-r--r--   0        0        0    10002 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/dist.py
+-rw-r--r--   0        0        0     3911 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/__init__.py
+-rw-r--r--   0        0        0     3254 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/buildx.py
+-rw-r--r--   0        0        0     1426 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/dockerapi.py
+-rw-r--r--   0        0        0     8949 2023-04-19 15:39:43.860433 kraken_std-0.8.5/src/kraken/std/docker/kaniko.py
+-rw-r--r--   0        0        0     1938 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/manifest_tool.py
+-rw-r--r--   0        0        0     3650 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/native.py
+-rw-r--r--   0        0        0        0 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/docker/py.typed
+-rw-r--r--   0        0        0     2264 2023-04-19 15:40:38.993462 kraken_std-0.8.5/src/kraken/std/docker/util.py
+-rw-r--r--   0        0        0     1761 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/__init__.py
+-rw-r--r--   0        0        0     1107 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/git/config.py
+-rw-r--r--   0        0        0     9451 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/git/gitignore.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/git/tasks/__init__.py
+-rw-r--r--   0        0        0      448 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/tasks/const.py
+-rw-r--r--   0        0        0     2919 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_check_task.py
+-rw-r--r--   0        0        0     2754 2023-04-05 21:42:55.754805 kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_sync_task.py
+-rw-r--r--   0        0        0     2973 2023-03-06 13:53:50.490907 kraken_std-0.8.5/src/kraken/std/git/version.py
+-rw-r--r--   0        0        0     6368 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/helm/__init__.py
+-rw-r--r--   0        0        0     2132 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/helm/helmapi.py
+-rw-r--r--   0        0        0     2310 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/http/__init__.py
+-rw-r--r--   0        0        0     3431 2023-04-19 15:08:11.413164 kraken_std-0.8.5/src/kraken/std/http/lint_ban_bare_requests.py
+-rw-r--r--   0        0        0        0 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/py.typed
+-rw-r--r--   0        0        0     1670 2023-04-19 15:39:43.860433 kraken_std-0.8.5/src/kraken/std/python/__init__.py
+-rw-r--r--   0        0        0     3586 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1332 2023-04-05 22:25:55.652556 kraken_std-0.8.5/src/kraken/std/python/buildsystem/helpers.py
+-rw-r--r--   0        0        0     3120 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/buildsystem/maturin.py
+-rw-r--r--   0        0        0     7926 2023-04-05 22:23:34.040338 kraken_std-0.8.5/src/kraken/std/python/buildsystem/poetry.py
+-rw-r--r--   0        0        0     4415 2023-04-05 22:03:27.278276 kraken_std-0.8.5/src/kraken/std/python/buildsystem/slap.py
+-rw-r--r--   0        0        0     4892 2023-04-05 22:23:34.040338 kraken_std-0.8.5/src/kraken/std/python/pyproject.py
+-rw-r--r--   0        0        0     6401 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/settings.py
+-rw-r--r--   0        0        0        0 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/tasks/__init__.py
+-rw-r--r--   0        0        0     3249 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/base_task.py
+-rw-r--r--   0        0        0     2076 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/black_task.py
+-rw-r--r--   0        0        0     1922 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/build_task.py
+-rw-r--r--   0        0        0     1046 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/flake8_task.py
+-rw-r--r--   0        0        0     2377 2023-04-19 15:39:43.860433 kraken_std-0.8.5/src/kraken/std/python/tasks/info_task.py
+-rw-r--r--   0        0        0     2834 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/install_task.py
+-rw-r--r--   0        0        0     1844 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/isort_task.py
+-rw-r--r--   0        0        0      946 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/login_task.py
+-rw-r--r--   0        0        0     1463 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_subtest_task.py
+-rw-r--r--   0        0        0     2352 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_task.py
+-rw-r--r--   0        0        0     2598 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/publish_task.py
+-rw-r--r--   0        0        0     2043 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/pycln_task.py
+-rw-r--r--   0        0        0     1034 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/pylint_task.py
+-rw-r--r--   0        0        0     2398 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/tasks/pytest_task.py
+-rw-r--r--   0        0        0     4531 2023-03-06 13:53:50.494907 kraken_std-0.8.5/src/kraken/std/python/tasks/pyupgrade_task.py
+-rw-r--r--   0        0        0     1778 2023-02-08 16:53:28.240291 kraken_std-0.8.5/src/kraken/std/python/tasks/update_lockfile_task.py
+-rw-r--r--   0        0        0     1656 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/python/tasks/update_pyproject_task.py
+-rw-r--r--   0        0        0     1127 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/python/version.py
+-rw-r--r--   0        0        0     4042 2023-01-22 14:38:01.549959 kraken_std-0.8.5/src/kraken/std/sccache.py
+-rw-r--r--   0        0        0      390 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/check_file_exists_and_is_committed_task.py
+-rw-r--r--   0        0        0     6010 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/check_valid_readme_exists_task.py
+-rw-r--r--   0        0        0     2645 2023-03-20 14:35:25.194513 kraken_std-0.8.5/src/kraken/std/util/copyright_task.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.5/PKG-INFO
```

### Comparing `kraken_std-0.8.4/LICENSE` & `kraken_std-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/pyproject.toml` & `kraken_std-0.8.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-std"
-version = "0.8.4"
+version = "0.8.5"
 description = "The Kraken standard library."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "kraken/std", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_std-0.8.4/readme.md` & `kraken_std-0.8.5/readme.md`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/__init__.py` & `kraken_std-0.8.5/src/kraken/std/cargo/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/config.py` & `kraken_std-0.8.5/src/kraken/std/cargo/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/data/certs/cert.pem` & `kraken_std-0.8.5/src/kraken/std/cargo/data/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/data/certs/key.pem` & `kraken_std-0.8.5/src/kraken/std/cargo/data/certs/key.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/manifest.py` & `kraken_std-0.8.5/src/kraken/std/cargo/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/mitm.py` & `kraken_std-0.8.5/src/kraken/std/cargo/mitm.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/mitm_impl.py` & `kraken_std-0.8.5/src/kraken/std/cargo/mitm_impl.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_build_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_bump_version_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_bump_version_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_clippy_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_clippy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_deny_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_deny_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_fmt_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_fmt_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_publish_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_sync_config_task.py` & `kraken_std-0.8.5/src/kraken/std/cargo/tasks/cargo_sync_config_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/cargo/version.py` & `kraken_std-0.8.5/src/kraken/std/cargo/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/descriptors/resource.py` & `kraken_std-0.8.5/src/kraken/std/descriptors/resource.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/dist.py` & `kraken_std-0.8.5/src/kraken/std/dist.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/docker/__init__.py` & `kraken_std-0.8.5/src/kraken/std/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/docker/buildx.py` & `kraken_std-0.8.5/src/kraken/std/docker/buildx.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/docker/dockerapi.py` & `kraken_std-0.8.5/src/kraken/std/docker/dockerapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/docker/kaniko.py` & `kraken_std-0.8.5/src/kraken/std/docker/kaniko.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,32 @@
 
 from . import DockerBuildTask
 from .dockerapi import docker_load, docker_run
 from .util import render_docker_auth, update_run_commands
 
 
 class KanikoBuildTask(DockerBuildTask):
-    """An implementation for building Docker images with Kaniko."""
+    """
+    An implementation for building Docker images with Kaniko.
+
+    In order to make secrets available in the Dockerfile under `/run/secrets`, and `RUN` command that is executed
+    by the root user will be surrounded by additional shell commands to link `/kaniko/secrets` to `/run/secrets`.
+    This is to ensure a degree of compatibility with BuildKit, which mounts secrets to `/run/secrets` when using
+    the `--secret` flag.
+
+    However, this compatibility is limited because we can only actually create a at `/run/secrets` if the `RUN`
+    command runs as root. Any command that is executed as a non-root user will not be able to access the secrets.
+    We use a heuristic to detect this, but it is not perfect. If you need to use secrets in a `RUN` command that
+    is executed as a non-root user, you will need to read from `/kaniko/secrets` instead.
+
+    If you start from a base image that doesn't start as the root user, you will need to explicitly add a `USER`
+    command to your Dockerfile to either inform the `KanikoBuildTask` that the subsequent commands are not run as
+    root, or use it to switch to the root user. Otherwise, the `KanikoBuildTask` will assume that the subsequent
+    commands are run as root and it can not know in advance if they are or not.
+    """
 
     kaniko_image: Property[str] = Property.default("gcr.io/kaniko-project/executor:v1.9.0-debug")
     kaniko_context: Property[str] = Property.default("/workspace")
     kaniko_cache_copy_layers: Property[bool] = Property.default(True)
     kaniko_snapshot_mode: Property[str] = Property.default("redo")
     kaniko_secrets_mount_dir: Property[str] = Property.default("/kaniko/secrets")
     kaniko_secrets_from_env: Property[Sequence[str]] = Property.default(())
@@ -147,14 +164,18 @@
     # DockerBuildTask
 
     def _preprocess_dockerfile(self, dockerfile: Path) -> str:
         return update_run_commands(
             dockerfile.read_text(),
             prefix="ln -sf /kaniko/secrets /run/secrets && ( ",
             suffix=" ); __ret=$?; unlink /run/secrets; exit $__ret",
+            # We can only link to /run/secrets if the user running the command is the root user. In any other
+            # case, we cannot link to /run/secrets and reading the secrets from /run/secrets in the Dockerfile
+            # will fail.
+            only_for_root_user=True,
         )
 
     # Task
 
     def finalize(self) -> None:
         if self.cache.get() and not self.push.get() and not self.cache_repo.get():
             self.logger.warning(
```

### Comparing `kraken_std-0.8.4/src/kraken/std/docker/manifest_tool.py` & `kraken_std-0.8.5/src/kraken/std/docker/manifest_tool.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/docker/native.py` & `kraken_std-0.8.5/src/kraken/std/docker/native.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/git/__init__.py` & `kraken_std-0.8.5/src/kraken/std/git/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/git/config.py` & `kraken_std-0.8.5/src/kraken/std/git/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/git/gitignore.py` & `kraken_std-0.8.5/src/kraken/std/git/gitignore.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_check_task.py` & `kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_check_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_sync_task.py` & `kraken_std-0.8.5/src/kraken/std/git/tasks/gitignore_sync_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/git/version.py` & `kraken_std-0.8.5/src/kraken/std/git/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/helm/__init__.py` & `kraken_std-0.8.5/src/kraken/std/helm/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/helm/helmapi.py` & `kraken_std-0.8.5/src/kraken/std/helm/helmapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/http/__init__.py` & `kraken_std-0.8.5/src/kraken/std/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/__init__.py` & `kraken_std-0.8.5/src/kraken/std/python/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .settings import PythonSettings, python_settings
 from .tasks.black_task import BlackTask, black
 from .tasks.build_task import BuildTask, build
 from .tasks.flake8_task import Flake8Task, flake8
+from .tasks.info_task import InfoTask, info
 from .tasks.install_task import InstallTask, install
 from .tasks.isort_task import IsortTask, isort
 from .tasks.login_task import login
 from .tasks.mypy_subtest_task import MypyStubtestTask, mypy_subtest
 from .tasks.mypy_task import MypyTask, mypy
 from .tasks.publish_task import PublishTask, publish
 from .tasks.pycln_task import PyclnTask, pycln
@@ -25,14 +26,16 @@
     "BuildTask",
     "flake8",
     "Flake8Task",
     "git_version_to_python_version",
     "git_version_to_python",
     "install",
     "InstallTask",
+    "InfoTask",
+    "info",
     "isort",
     "IsortTask",
     "login",
     "mypy",
     "MypyTask",
     "mypy_subtest",
     "MypyStubtestTask",
```

### Comparing `kraken_std-0.8.4/src/kraken/std/python/buildsystem/__init__.py` & `kraken_std-0.8.5/src/kraken/std/python/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/buildsystem/helpers.py` & `kraken_std-0.8.5/src/kraken/std/python/buildsystem/helpers.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/buildsystem/maturin.py` & `kraken_std-0.8.5/src/kraken/std/python/buildsystem/maturin.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/buildsystem/poetry.py` & `kraken_std-0.8.5/src/kraken/std/python/buildsystem/poetry.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/buildsystem/slap.py` & `kraken_std-0.8.5/src/kraken/std/python/buildsystem/slap.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/pyproject.py` & `kraken_std-0.8.5/src/kraken/std/python/pyproject.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/settings.py` & `kraken_std-0.8.5/src/kraken/std/python/settings.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/base_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/black_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/black_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/build_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/flake8_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/flake8_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/install_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/install_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/isort_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/isort_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/login_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/login_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_subtest_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_subtest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/mypy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/publish_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/pycln_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/pycln_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/pylint_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/pylint_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/pytest_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/pytest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/pyupgrade_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/pyupgrade_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/update_lockfile_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/update_lockfile_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/tasks/update_pyproject_task.py` & `kraken_std-0.8.5/src/kraken/std/python/tasks/update_pyproject_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/python/version.py` & `kraken_std-0.8.5/src/kraken/std/python/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/sccache.py` & `kraken_std-0.8.5/src/kraken/std/sccache.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/util/check_file_exists_and_is_committed_task.py` & `kraken_std-0.8.5/src/kraken/std/util/check_file_exists_and_is_committed_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/util/check_valid_readme_exists_task.py` & `kraken_std-0.8.5/src/kraken/std/util/check_valid_readme_exists_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/src/kraken/std/util/copyright_task.py` & `kraken_std-0.8.5/src/kraken/std/util/copyright_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.4/PKG-INFO` & `kraken_std-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-std
-Version: 0.8.4
+Version: 0.8.5
 Summary: The Kraken standard library.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

