# Comparing `tmp/sentry_cli-2.17.2.tar.gz` & `tmp/sentry_cli-2.17.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.17.2.tar", last modified: Wed Apr 12 12:00:19 2023, max compression
+gzip compressed data, was "sentry_cli-2.17.3.tar", last modified: Wed Apr 19 10:09:30 2023, max compression
```

## Comparing `sentry_cli-2.17.2.tar` & `sentry_cli-2.17.3.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/
--rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.238543 sentry_cli-2.17.2/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.238543 sentry_cli-2.17.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:29.996271 sentry_cli-2.17.3/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:09:29.000000 sentry_cli-2.17.3/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:29.996271 sentry_cli-2.17.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/bundle_jvm.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.000271 sentry_cli-2.17.3/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.004271 sentry_cli-2.17.3/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.008271 sentry_cli-2.17.3/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.008271 sentry_cli-2.17.3/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.008271 sentry_cli-2.17.3/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.012271 sentry_cli-2.17.3/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16926 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:09:30.016271 sentry_cli-2.17.3/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-19 10:09:08.000000 sentry_cli-2.17.3/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.17.2/Cargo.lock` & `sentry_cli-2.17.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2191,15 +2191,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.17.2"
+version = "2.17.3"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
```

### Comparing `sentry_cli-2.17.2/Cargo.toml` & `sentry_cli-2.17.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.17.2"
+version = "2.17.3"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
```

### Comparing `sentry_cli-2.17.2/LICENSE` & `sentry_cli-2.17.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/PKG-INFO` & `sentry_cli-2.17.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.17.2
+Version: 2.17.3
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.2 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.3 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.2/README.md` & `sentry_cli-2.17.3/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/build.rs` & `sentry_cli-2.17.3/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.17.3/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.17.2
+Version: 2.17.3
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.2 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.3 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.2/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.17.3/sentry_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 src/commands/send_envelope.rs
 src/commands/send_event.rs
 src/commands/uninstall.rs
 src/commands/update.rs
 src/commands/upload_dif.rs
 src/commands/upload_dsym.rs
 src/commands/upload_proguard.rs
+src/commands/debug_files/bundle_jvm.rs
 src/commands/debug_files/bundle_sources.rs
 src/commands/debug_files/check.rs
 src/commands/debug_files/find.rs
 src/commands/debug_files/mod.rs
 src/commands/debug_files/print_sources.rs
 src/commands/debug_files/upload.rs
 src/commands/deploys/list.rs
```

### Comparing `sentry_cli-2.17.2/setup.cfg` & `sentry_cli-2.17.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/setup.py` & `sentry_cli-2.17.3/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/api.rs` & `sentry_cli-2.17.3/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/bashsupport.sh` & `sentry_cli-2.17.3/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/bash_hook.rs` & `sentry_cli-2.17.3/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.17.3/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/debug_files/check.rs` & `sentry_cli-2.17.3/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/debug_files/find.rs` & `sentry_cli-2.17.3/src/commands/debug_files/find.rs`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
                 DifType::Elf => find_ids_for_elf(&dirent, &remaining),
                 DifType::Pe => find_ids_for_pe(&dirent, &remaining),
                 DifType::Pdb => find_ids_for_pdb(&dirent, &remaining),
                 DifType::PortablePdb => find_ids_for_portablepdb(&dirent, &remaining),
                 DifType::SourceBundle => find_ids_for_sourcebundle(&dirent, &remaining),
                 DifType::Breakpad => find_ids_for_breakpad(&dirent, &remaining),
                 DifType::Proguard => find_ids_for_proguard(&dirent, &proguard_uuids),
+                DifType::Jvm => find_ids_for_sourcebundle(&dirent, &remaining),
                 DifType::Wasm => None,
             })
             .flatten()
             .collect();
 
         for (id, ty) in found {
             let path = dirent.path().to_path_buf();
```

### Comparing `sentry_cli-2.17.2/src/commands/debug_files/mod.rs` & `sentry_cli-2.17.3/src/commands/debug_files/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 use anyhow::Result;
 use clap::{ArgMatches, Command};
 
+pub mod bundle_jvm;
 pub mod bundle_sources;
 pub mod check;
 pub mod find;
 pub mod print_sources;
 pub mod upload;
 
 macro_rules! each_subcommand {
     ($mac:ident) => {
         $mac!(bundle_sources);
         $mac!(check);
+        $mac!(bundle_jvm);
         $mac!(find);
         $mac!(print_sources);
         $mac!(upload);
     };
 }
 
 pub fn make_command(mut command: Command) -> Command {
```

### Comparing `sentry_cli-2.17.2/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.17.3/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/debug_files/upload.rs` & `sentry_cli-2.17.3/src/commands/debug_files/upload.rs`

 * *Files 1% similar despite different names*

```diff
@@ -230,14 +230,15 @@
             "dsym" => upload.filter_format(DifFormat::Object(FileFormat::MachO)),
             "elf" => upload.filter_format(DifFormat::Object(FileFormat::Elf)),
             "breakpad" => upload.filter_format(DifFormat::Object(FileFormat::Breakpad)),
             "pdb" => upload.filter_format(DifFormat::Object(FileFormat::Pdb)),
             "pe" => upload.filter_format(DifFormat::Object(FileFormat::Pe)),
             "sourcebundle" => upload.filter_format(DifFormat::Object(FileFormat::SourceBundle)),
             "portablepdb" => upload.filter_format(DifFormat::Object(FileFormat::PortablePdb)),
+            "jvm" => upload.filter_format(DifFormat::Object(FileFormat::SourceBundle)),
             "bcsymbolmap" => {
                 upload.filter_format(DifFormat::BcSymbolMap);
                 upload.filter_format(DifFormat::PList)
             }
             other => bail!("Unsupported type: {}", other),
         };
     }
```

### Comparing `sentry_cli-2.17.2/src/commands/deploys/list.rs` & `sentry_cli-2.17.3/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/deploys/mod.rs` & `sentry_cli-2.17.3/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/deploys/new.rs` & `sentry_cli-2.17.3/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/events/list.rs` & `sentry_cli-2.17.3/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/events/mod.rs` & `sentry_cli-2.17.3/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/files/delete.rs` & `sentry_cli-2.17.3/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/files/list.rs` & `sentry_cli-2.17.3/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/files/mod.rs` & `sentry_cli-2.17.3/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/files/upload.rs` & `sentry_cli-2.17.3/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/info.rs` & `sentry_cli-2.17.3/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/issues/mod.rs` & `sentry_cli-2.17.3/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/issues/mute.rs` & `sentry_cli-2.17.3/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/issues/resolve.rs` & `sentry_cli-2.17.3/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/issues/unresolve.rs` & `sentry_cli-2.17.3/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/login.rs` & `sentry_cli-2.17.3/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/mod.rs` & `sentry_cli-2.17.3/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/monitors/list.rs` & `sentry_cli-2.17.3/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/monitors/mod.rs` & `sentry_cli-2.17.3/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/monitors/run.rs` & `sentry_cli-2.17.3/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/organizations/list.rs` & `sentry_cli-2.17.3/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/organizations/mod.rs` & `sentry_cli-2.17.3/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/projects/list.rs` & `sentry_cli-2.17.3/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/projects/mod.rs` & `sentry_cli-2.17.3/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/react_native/appcenter.rs` & `sentry_cli-2.17.3/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/react_native/gradle.rs` & `sentry_cli-2.17.3/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/react_native/mod.rs` & `sentry_cli-2.17.3/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/react_native/xcode.rs` & `sentry_cli-2.17.3/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/archive.rs` & `sentry_cli-2.17.3/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/delete.rs` & `sentry_cli-2.17.3/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/finalize.rs` & `sentry_cli-2.17.3/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/info.rs` & `sentry_cli-2.17.3/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/list.rs` & `sentry_cli-2.17.3/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/mod.rs` & `sentry_cli-2.17.3/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/new.rs` & `sentry_cli-2.17.3/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/restore.rs` & `sentry_cli-2.17.3/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/releases/set_commits.rs` & `sentry_cli-2.17.3/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/repos/list.rs` & `sentry_cli-2.17.3/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/repos/mod.rs` & `sentry_cli-2.17.3/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/send_envelope.rs` & `sentry_cli-2.17.3/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/send_event.rs` & `sentry_cli-2.17.3/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.17.3/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/sourcemaps/inject.rs` & `sentry_cli-2.17.3/src/commands/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.17.3/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.17.3/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.17.3/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/uninstall.rs` & `sentry_cli-2.17.3/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/update.rs` & `sentry_cli-2.17.3/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/commands/upload_proguard.rs` & `sentry_cli-2.17.3/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/config.rs` & `sentry_cli-2.17.3/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/constants.rs` & `sentry_cli-2.17.3/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/android.rs` & `sentry_cli-2.17.3/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/appcenter.rs` & `sentry_cli-2.17.3/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/args.rs` & `sentry_cli-2.17.3/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/chunks.rs` & `sentry_cli-2.17.3/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/codepush.rs` & `sentry_cli-2.17.3/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/cordova.rs` & `sentry_cli-2.17.3/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/dif.rs` & `sentry_cli-2.17.3/src/utils/dif.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,56 +17,60 @@
     Breakpad,
     Proguard,
     SourceBundle,
     Pe,
     Pdb,
     PortablePdb,
     Wasm,
+    Jvm,
 }
 
 impl DifType {
     pub fn name(self) -> &'static str {
         match self {
             DifType::Dsym => "dsym",
             DifType::Elf => "elf",
             DifType::Pe => "pe",
             DifType::Pdb => "pdb",
             DifType::PortablePdb => "portablepdb",
             DifType::SourceBundle => "sourcebundle",
             DifType::Breakpad => "breakpad",
             DifType::Proguard => "proguard",
             DifType::Wasm => "wasm",
+            DifType::Jvm => "jvm",
         }
     }
 
     pub fn all() -> &'static [DifType] {
         &[
             DifType::Dsym,
             DifType::Elf,
             DifType::Pe,
             DifType::Pdb,
             DifType::PortablePdb,
             DifType::SourceBundle,
             DifType::Breakpad,
             DifType::Proguard,
             DifType::Wasm,
+            DifType::Jvm,
         ]
     }
 
     pub fn all_names() -> &'static [&'static str] {
         &[
             "dsym",
             "elf",
             "pe",
             "pdb",
             "portablepdb",
             "sourcebundle",
             "breakpad",
             "proguard",
             "wasm",
+            "jvm",
         ]
     }
 }
 
 impl fmt::Display for DifType {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         write!(f, "{}", self.name())
@@ -83,14 +87,15 @@
             "pe" => Ok(DifType::Pe),
             "pdb" => Ok(DifType::Pdb),
             "portablepdb" => Ok(DifType::PortablePdb),
             "sourcebundle" => Ok(DifType::SourceBundle),
             "breakpad" => Ok(DifType::Breakpad),
             "proguard" => Ok(DifType::Proguard),
             "wasm" => Ok(DifType::Wasm),
+            "jvm" => Ok(DifType::Jvm),
             _ => bail!("Invalid debug info file type"),
         }
     }
 }
 
 /// Declares which features an object may have to be uploaded.
 #[derive(Clone, Copy, Debug)]
@@ -247,14 +252,15 @@
             Some(DifType::Pe) => DifFile::open_object(path, FileFormat::Pe),
             Some(DifType::Pdb) => DifFile::open_object(path, FileFormat::Pdb),
             Some(DifType::PortablePdb) => DifFile::open_object(path, FileFormat::PortablePdb),
             Some(DifType::SourceBundle) => DifFile::open_object(path, FileFormat::SourceBundle),
             Some(DifType::Wasm) => DifFile::open_object(path, FileFormat::Wasm),
             Some(DifType::Breakpad) => DifFile::open_object(path, FileFormat::Breakpad),
             Some(DifType::Proguard) => DifFile::open_proguard(path),
+            Some(DifType::Jvm) => DifFile::open_object(path, FileFormat::SourceBundle),
             None => DifFile::try_open(path),
         }
     }
 }
 
 #[derive(Serialize)]
 pub struct DifVariant {
```

### Comparing `sentry_cli-2.17.2/src/utils/dif_upload.rs` & `sentry_cli-2.17.3/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/enc.rs` & `sentry_cli-2.17.3/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/event.rs` & `sentry_cli-2.17.3/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/file_search.rs` & `sentry_cli-2.17.3/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/file_upload.rs` & `sentry_cli-2.17.3/src/utils/file_upload.rs`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,18 @@
 
         let concurrency = self
             .context
             .chunk_upload_options
             .map_or(DEFAULT_CONCURRENCY, |o| usize::from(o.concurrency));
         upload_files_parallel(self.context, &self.files, concurrency)
     }
+
+    pub fn build_jvm_bundle(&self, debug_id: Option<DebugId>) -> Result<TempFile> {
+        build_artifact_bundle(self.context, &self.files, debug_id)
+    }
 }
 
 fn upload_files_parallel(
     context: &UploadContext,
     files: &SourceFiles,
     num_threads: usize,
 ) -> Result<()> {
@@ -270,15 +274,15 @@
 }
 
 fn upload_files_chunked(
     context: &UploadContext,
     files: &SourceFiles,
     options: &ChunkUploadOptions,
 ) -> Result<()> {
-    let archive = build_artifact_bundle(context, files)?;
+    let archive = build_artifact_bundle(context, files, None)?;
 
     let progress_style =
         ProgressStyle::default_spinner().template("{spinner} Optimizing bundle for upload...");
 
     let pb = ProgressBar::new_spinner();
     pb.enable_steady_tick(100);
     pb.set_style(progress_style);
@@ -392,29 +396,35 @@
     }
 
     let mut sha1_bytes = [0u8; 16];
     sha1_bytes.copy_from_slice(&hash.digest().bytes()[..16]);
     DebugId::from_uuid(uuid::Builder::from_sha1_bytes(sha1_bytes).into_uuid())
 }
 
-fn build_artifact_bundle(context: &UploadContext, files: &SourceFiles) -> Result<TempFile> {
+fn build_artifact_bundle(
+    context: &UploadContext,
+    files: &SourceFiles,
+    debug_id: Option<DebugId>,
+) -> Result<TempFile> {
     let progress_style = ProgressStyle::default_bar().template(
         "{prefix:.dim} Bundling files for upload... {msg:.dim}\
        \n{wide_bar}  {pos}/{len}",
     );
 
     let pb = ProgressBar::new(files.len());
     pb.set_style(progress_style);
     pb.set_prefix(">");
 
     let archive = TempFile::create()?;
     let mut bundle = SourceBundleWriter::start(BufWriter::new(archive.open()?))?;
 
     // artifact bundles get a random UUID as debug id
-    bundle.set_attribute("debug_id", build_debug_id(files).to_string());
+    let debug_id = debug_id.unwrap_or_else(|| build_debug_id(files));
+    bundle.set_attribute("debug_id", debug_id.to_string());
+
     if let Some(note) = context.note {
         bundle.set_attribute("note", note.to_owned());
     }
 
     bundle.set_attribute("org".to_owned(), context.org.to_owned());
     if let Some(project) = context.project {
         bundle.set_attribute("project".to_owned(), project.to_owned());
```

### Comparing `sentry_cli-2.17.2/src/utils/formatting.rs` & `sentry_cli-2.17.3/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/fs.rs` & `sentry_cli-2.17.3/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/http.rs` & `sentry_cli-2.17.3/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/logging.rs` & `sentry_cli-2.17.3/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/progress.rs` & `sentry_cli-2.17.3/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/releases.rs` & `sentry_cli-2.17.3/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/retry.rs` & `sentry_cli-2.17.3/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.17.3/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.17.3/src/utils/sourcemaps/inject.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/sourcemaps.rs` & `sentry_cli-2.17.3/src/utils/sourcemaps.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/system.rs` & `sentry_cli-2.17.3/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/ui.rs` & `sentry_cli-2.17.3/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/update.rs` & `sentry_cli-2.17.3/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/vcs.rs` & `sentry_cli-2.17.3/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.2/src/utils/xcode.rs` & `sentry_cli-2.17.3/src/utils/xcode.rs`

 * *Files identical despite different names*

