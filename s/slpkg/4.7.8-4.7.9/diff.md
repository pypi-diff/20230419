# Comparing `tmp/slpkg-4.7.8.tar.gz` & `tmp/slpkg-4.7.9.tar.gz`

## Comparing `slpkg-4.7.8.tar` & `slpkg-4.7.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:55:04.000000 slpkg-4.7.8/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-14 09:46:56.000000 slpkg-4.7.8/filelists/README
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:50:47.000000 slpkg-4.7.8/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4281 2023-04-14 09:46:56.000000 slpkg-4.7.8/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-14 09:46:56.000000 slpkg-4.7.8/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     8312 2023-04-14 09:53:51.000000 slpkg-4.7.8/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-14 09:46:56.000000 slpkg-4.7.8/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8603 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     3267 2023-04-14 09:46:56.000000 slpkg-4.7.8/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2394 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1894 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1590 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-14 09:46:56.000000 slpkg-4.7.8/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-14 09:46:56.000000 slpkg-4.7.8/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-14 09:46:56.000000 slpkg-4.7.8/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    44892 2023-04-14 09:46:56.000000 slpkg-4.7.8/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-14 09:46:56.000000 slpkg-4.7.8/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-14 09:46:56.000000 slpkg-4.7.8/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-14 09:46:56.000000 slpkg-4.7.8/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-14 09:46:56.000000 slpkg-4.7.8/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1954 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9717 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    62222 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    24043 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2488 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    14874 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1042 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/form_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)    32658 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2246 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     7067 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6319 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5523 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/ascii.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4043 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     9794 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3055 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1344 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5311 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/clean_logs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6613 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3970 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11019 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1521 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2617 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3136 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    30270 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1470 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3061 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2872 2023-04-14 09:46:56.000000 slpkg-4.7.8/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1363 2023-04-14 09:46:56.000000 slpkg-4.7.8/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1106 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     9576 2023-04-14 09:55:01.000000 slpkg-4.7.8/slpkg.egg-info/PKG-INFO
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-14 09:46:56.000000 slpkg-4.7.8/tools/gen_sbo_txt.sh
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-14 09:46:56.000000 slpkg-4.7.8/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-14 09:46:56.000000 slpkg-4.7.8/bin/slpkg_new-configs
--rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-14 09:46:56.000000 slpkg-4.7.8/bin/slpkg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:43:01.000000 slpkg-4.7.9/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-19 14:36:36.000000 slpkg-4.7.9/filelists/README
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4280 2023-04-19 14:36:36.000000 slpkg-4.7.9/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-19 14:36:36.000000 slpkg-4.7.9/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-19 14:36:36.000000 slpkg-4.7.9/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9164 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     3634 2023-04-19 14:36:36.000000 slpkg-4.7.9/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2340 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      588 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-19 14:36:36.000000 slpkg-4.7.9/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-19 14:36:36.000000 slpkg-4.7.9/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1773 2023-04-19 14:36:36.000000 slpkg-4.7.9/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    45099 2023-04-19 14:36:36.000000 slpkg-4.7.9/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8987 2023-04-19 14:36:36.000000 slpkg-4.7.9/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9918 2023-04-19 14:36:36.000000 slpkg-4.7.9/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-19 14:36:36.000000 slpkg-4.7.9/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-19 14:36:36.000000 slpkg-4.7.9/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1947 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9605 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    63573 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    27456 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2463 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    14873 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1042 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3983 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/form_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    34184 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1791 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2391 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     7070 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6319 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5523 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/ascii.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4043 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9821 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3029 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1344 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5193 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/clean_logs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7000 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3970 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11207 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1521 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2603 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3136 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      245 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    30063 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1470 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3212 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2872 2023-04-19 14:36:36.000000 slpkg-4.7.9/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1363 2023-04-19 14:36:36.000000 slpkg-4.7.9/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1105 2023-04-19 14:42:56.000000 slpkg-4.7.9/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1271 2023-04-19 14:42:55.000000 slpkg-4.7.9/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8341 2023-04-19 14:36:36.000000 slpkg-4.7.9/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-19 14:36:36.000000 slpkg-4.7.9/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-19 14:36:36.000000 slpkg-4.7.9/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)    11470 2023-04-19 14:36:36.000000 slpkg-4.7.9/bin/slpkg_new-configs
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      184 2023-04-19 14:36:36.000000 slpkg-4.7.9/bin/slpkg
```

### Comparing `slpkg-4.7.8/filelists/multilib/README.ERIC` & `slpkg-4.7.9/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/filelists/multilib/README` & `slpkg-4.7.9/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/filelists/multilib/compat32.pkgs` & `slpkg-4.7.9/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slackbuild/slack-desc` & `slpkg-4.7.9/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slackbuild/slpkg.SlackBuild` & `slpkg-4.7.9/slackbuild/slpkg.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 cp man/slpkg.1 $PKG/usr/man/man1
 cp man/slpkg-fr.1 $PKG/usr/man/fr/man1/slpkg.1
 
 find $PKG/usr/man -type f -exec gzip -9 {} \;
 for i in $( find $PKG/usr/man -type l ) ; do ln -s $( readlink $i ).gz $i.gz; rm $i ; done
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
-cp -a README.rst ChangeLog.txt LICENSE requirements.txt $PKG/usr/doc/$PRGNAM-$VERSION
+cp -a README.md ChangeLog.txt LICENSE requirements.txt $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
 
 mkdir -p $PKG/install
 cat $CWD/slack-desc > $PKG/install/slack-desc
 cat $CWD/doinst.sh > $PKG/install/doinst.sh
 
 cd $PKG
```

### Comparing `slpkg-4.7.8/configs/repositories.toml` & `slpkg-4.7.9/configs/repositories.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,204 +4,211 @@
 # and many binaries for all versions.                                  #
 # Set 'true' to 'PONCE_REPO' to switch with the ponce repository.      #
 # Set 'true' to the binaries repositories you want to enable.          #
 # Default is the 'sbo' Slackbuilds.org repository.                     #
 ########################################################################
 
 ########################################################################
+# If you are going to use a local repository, set the mirror:          #
+# Example: ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]   #
+#                                                                      #
+# A binary local repository will must contain the files:               #
+# ChangeLog.txt, PACKAGES.TXT and CHECKSUMS.md5                        #
+# A SlackBuilds repository will must contain the files:                #
+# SLACKBUILDS.TXT and ChangeLog.txt                                    #
+# Note: ponce repository needs the 'gen_sbo_txt.sh' tool from          #
+# the 'slpkg/tools/' folder, if the SLACKBUILDS.TXT missing.           #
+#                                                                      #
+# After the mirror changed, you should update the database:            #
+# slpkg update or apply the option --bin-repo=<repo_name> for          #
+# binaries repositories.                                               #
+########################################################################
+
+########################################################################
 # Note: Before using a repository, make sure you have read about it.   #
 #       Some repositories are for -current only. Change the mirror if  #
 #       it is necessary. The mirror should end with a slash '/'.       #
 ########################################################################
 
 [REPOSITORIES]
 
 # SBo Repository for Slackware 15.0 stable.
 SBO_REPO_NAME = "sbo"
-SBO_REPO_MIRROR = "https://slackbuilds.org/slackbuilds/15.0/"
+SBO_REPO_MIRROR = ["https://slackbuilds.org/slackbuilds/15.0/"]
 SBO_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
 SBO_REPO_CHANGELOG = "ChangeLog.txt"
 SBO_REPO_TAR_SUFFIX = ".tar.gz"
 SBO_REPO_TAG = "_SBo"  # Default repo TAG.
 SBO_REPO_PATCH_TAG = ""  # Patch the TAG.
 
 # Ponce Repository for Slackware -current.
 PONCE_REPO = false
 PONCE_REPO_NAME = "ponce"
-PONCE_REPO_MIRROR = "https://cgit.ponce.cc/slackbuilds/plain/"
+PONCE_REPO_MIRROR = ["https://cgit.ponce.cc/slackbuilds/plain/"]
 PONCE_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
 PONCE_REPO_CHANGELOG = "ChangeLog.txt"
 PONCE_REPO_TAG = "_SBo"  # Default repo TAG.
 PONCE_REPO_PATCH_TAG = ""  # Patch the TAG.
 
 # Official repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://slackware.uk/slackware/slackware64-current/
+# ["https://slackware.uk/slackware/slackware64-current/"]
 SLACK_REPO = false
 SLACK_REPO_NAME = "slack"
-SLACK_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
+SLACK_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/"]
 SLACK_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_REPO_TAG = ""
 
 # Official repository for Slackware patches x86_64 15.0 stable.
 # For Slackware patches x86_64 -current:
-# https://slackware.uk/slackware/slackware64-current/extra/
+# ["https://slackware.uk/slackware/slackware64-current/", "extra/"]
 SLACK_EXTRA_REPO = false
 SLACK_EXTRA_REPO_NAME = "slack_extra"
-SLACK_EXTRA_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
-SLACK_EXTRA_REPO_PACKAGES_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/extra/"
+SLACK_EXTRA_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "extra/"]
 SLACK_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_EXTRA_REPO_TAG = ""
 
 # Official repository for Slackware patches x86_64 15.0 stable.
 # For Slackware patches x86_64 -current:
-# https://slackware.uk/slackware/slackware64-current/patches/
+# ["https://slackware.uk/slackware/slackware64-current/", "patches/"]
 SLACK_PATCHES_REPO = false
 SLACK_PATCHES_REPO_NAME = "slack_patches"
-SLACK_PATCHES_REPO_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/"
-SLACK_PATCHES_REPO_PACKAGES_MIRROR = "https://slackware.uk/slackware/slackware64-15.0/patches/"
+SLACK_PATCHES_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "patches/"]
 SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_PATCHES_REPO_TAG = ""
 
 # AlienBob Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# http://slackware.uk/people/alien/sbrepos/current/x86_64/
+# ["http://slackware.uk/people/alien/sbrepos/", "current/", "x86_64/"]
 ALIEN_REPO = false
 ALIEN_REPO_NAME = "alien"
-ALIEN_REPO_MIRROR = "https://slackware.nl/people/alien/sbrepos/"
-ALIEN_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/sbrepos/15.0/x86_64/"
+ALIEN_REPO_MIRROR = ["https://slackware.nl/people/alien/sbrepos/", "15.0/", "x86_64/"]
 ALIEN_REPO_PACKAGES = "PACKAGES.TXT"
 ALIEN_REPO_CHECKSUMS = "CHECKSUMS.md5"
 ALIEN_REPO_CHANGELOG = "ChangeLog.txt"
 ALIEN_REPO_TAG = "alien"
 
 # Multilib Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://slackware.nl/people/alien/multilib/current/
+# ["https://slackware.nl/people/alien/multilib/", current/"]
 MULTILIB_REPO = false
 MULTILIB_REPO_NAME = "multilib"
-MULTILIB_REPO_MIRROR = "https://slackware.nl/people/alien/multilib/"
-MULTILIB_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/multilib/15.0/"
+MULTILIB_REPO_MIRROR = ["https://slackware.nl/people/alien/multilib/", "15.0/"]
 MULTILIB_REPO_PACKAGES = "PACKAGES.TXT"
 MULTILIB_REPO_CHECKSUMS = "CHECKSUMS.md5"
 MULTILIB_REPO_CHANGELOG = "ChangeLog.txt"
 MULTILIB_REPO_TAG = "alien"
 
 # Restricted Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://slackware.nl/people/alien/restricted_sbrepos/current/x86_64/
+# ["https://slackware.nl/people/alien/restricted_sbrepos/", "current/", "x86_64/"]
 RESTRICTED_REPO = false
 RESTRICTED_REPO_NAME = "restricted"
-RESTRICTED_REPO_MIRROR = "https://slackware.nl/people/alien/restricted_sbrepos/"
-RESTRICTED_REPO_PACKAGES_MIRROR = "https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/"
+RESTRICTED_REPO_MIRROR = ["https://slackware.nl/people/alien/restricted_sbrepos/", "15.0/", "x86_64/"]
 RESTRICTED_REPO_PACKAGES = "PACKAGES.TXT"
 RESTRICTED_REPO_CHECKSUMS = "CHECKSUMS.md5"
 RESTRICTED_REPO_CHANGELOG = "ChangeLog.txt"
 RESTRICTED_REPO_TAG = "alien"
 
 # Gnome Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/
+# ["https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/"]
 GNOME_REPO = false
 GNOME_REPO_NAME = "gnome"
-GNOME_REPO_MIRROR = "https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/"
+GNOME_REPO_MIRROR = ["https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/"]
 GNOME_REPO_PACKAGES = "PACKAGES.TXT"
 GNOME_REPO_CHECKSUMS = "CHECKSUMS.md5"
 GNOME_REPO_CHANGELOG = "ChangeLog.txt"
 GNOME_REPO_TAG = "gfs"
 
 # MATE Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://slackware.uk/msb/current/1.26/x86_64/
+# ["https://slackware.uk/msb/current/", "1.26/", "x86_64/"]
 MSB_REPO = false
 MSB_REPO_NAME = "msb"
-MSB_REPO_MIRROR = "https://slackware.uk/msb/"
-MSB_REPO_PACKAGES_MIRROR = 'https://slackware.uk/msb/15.0/1.26/x86_64/'
+MSB_REPO_MIRROR = ["https://slackware.uk/msb/", "15.0/", "1.26/", "x86_64/"]
 MSB_REPO_PACKAGES = "PACKAGES.TXT"
 MSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
 MSB_REPO_CHANGELOG = "ChangeLog.txt"
 MSB_REPO_TAG = "msb"
 
 # Cinnamon Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://slackware.uk/csb/current/x86_64/
+# ["https://slackware.uk/csb/", "current/", "x86_64/"]
 CSB_REPO = false
 CSB_REPO_NAME = "csb"
-CSB_REPO_MIRROR = "https://slackware.uk/csb/"
-CSB_REPO_PACKAGES_MIRROR = 'https://slackware.uk/csb/15.0/x86_64/'
+CSB_REPO_MIRROR = ["https://slackware.uk/csb/", "15.0/", "x86_64/"]
 CSB_REPO_PACKAGES = "PACKAGES.TXT"
 CSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
 CSB_REPO_CHANGELOG = "ChangeLog.txt"
 CSB_REPO_TAG = "csb"
 
 # Conraid Repository for Slackware x86_64 -current.
 CONRAID_REPO = false
 CONRAID_REPO_NAME = "conraid"
-CONRAID_REPO_MIRROR = "https://slack.conraid.net/repository/slackware64-current/"
+CONRAID_REPO_MIRROR = ["https://slack.conraid.net/repository/slackware64-current/"]
 CONRAID_REPO_PACKAGES = "PACKAGES.TXT"
 CONRAID_REPO_CHECKSUMS = "CHECKSUMS.md5"
 CONRAID_REPO_CHANGELOG = "ChangeLog.txt"
 CONRAID_REPO_TAG = "cf"
 
 # Slackonly Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
-# https://packages.slackonly.com/pub/packages/current-x86_64/
+# ["https://packages.slackonly.com/pub/packages/current-x86_64/"]
 SLACKONLY_REPO = false
 SLACKONLY_REPO_NAME = "slackonly"
-SLACKONLY_REPO_MIRROR = "https://packages.slackonly.com/pub/packages/15.0-x86_64/"
+SLACKONLY_REPO_MIRROR = ["https://packages.slackonly.com/pub/packages/15.0-x86_64/"]
 SLACKONLY_REPO_PACKAGES = "PACKAGES.TXT"
 SLACKONLY_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACKONLY_REPO_CHANGELOG = "ChangeLog.txt"
 SLACKONLY_REPO_TAG = "slonly"
 
 # Repository for Salix OS x86_64 15.0 stable.
 SALIXOS_REPO = false
 SALIXOS_REPO_NAME = "salixos"
-SALIXOS_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
+SALIXOS_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/"]
 SALIXOS_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_REPO_CHANGELOG = "ChangeLog.txt"
 SALIXOS_REPO_TAG = ""
 
 # Repository for Salix OS x86_64 15.0 stable.
 SALIXOS_EXTRA_REPO = false
 SALIXOS_EXTRA_REPO_NAME = "salixos_extra"
-SALIXOS_EXTRA_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
-SALIXOS_EXTRA_REPO_PACKAGES_MIRROR = 'https://download.salixos.org/x86_64/slackware-15.0/extra/'
+SALIXOS_EXTRA_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/", "extra/"]
 SALIXOS_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
 SALIXOS_EXTRA_REPO_TAG = ""
 
 # Repository for Salix OS x86_64 15.0 stable.
 SALIXOS_PATCHES_REPO = false
 SALIXOS_PATCHES_REPO_NAME = "salixos_patches"
-SALIXOS_PATCHES_REPO_MIRROR = "https://download.salixos.org/x86_64/slackware-15.0/"
-SALIXOS_PATCHES_REPO_PACKAGES_MIRROR = 'https://download.salixos.org/x86_64/slackware-15.0/patches/'
+SALIXOS_PATCHES_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/", "patches/"]
 SALIXOS_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
 SALIXOS_PATCHES_REPO_TAG = "_slack15.0"
 
 # Repository for Slackel OS x86_64 -current.
 SLACKEL_REPO = false
 SLACKEL_REPO_NAME = "slackel"
-SLACKEL_REPO_MIRROR = "http://www.slackel.gr/repo/x86_64/current/"
+SLACKEL_REPO_MIRROR = ["http://www.slackel.gr/repo/x86_64/current/"]
 SLACKEL_REPO_PACKAGES = "PACKAGES.TXT"
 SLACKEL_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACKEL_REPO_CHANGELOG = "ChangeLog.txt"
 SLACKEL_REPO_TAG = "dj"
 
 # Slint Repository for Slackware x86_64 15.0 stable.
 SLINT_REPO = false
 SLINT_REPO_NAME = "slint"
-SLINT_REPO_MIRROR = "https://slackware.uk/slint/x86_64/slint-15.0/"
+SLINT_REPO_MIRROR = ["https://slackware.uk/slint/x86_64/slint-15.0/"]
 SLINT_REPO_PACKAGES = "PACKAGES.TXT"
 SLINT_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLINT_REPO_CHANGELOG = "ChangeLog.txt"
 SLINT_REPO_TAG = "slint"
```

### Comparing `slpkg-4.7.8/configs/slpkg.toml` & `slpkg-4.7.9/configs/slpkg.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,98 @@
 [CONFIGS]
 
 # OS architecture by default.
 OS_ARCH = "x86_64"
+
 # Where the packages download.
 # This path working only with the command download.
 DOWNLOAD_ONLY_PATH = "/tmp/slpkg/"
+
 # File suffix for list packages.
 # Change here if you are going to use '.sqf' files.
 FILE_LIST_SUFFIX = ".pkgs"
+
 # Configs for displaying colorful menu. Default is true. [true/false]
 COLORS = true
+
 # Dialog is a program that will let you present a variety of questions or
 # display messages using dialog boxes from a shell script.
 # Default is true. [true/false]
 DIALOG = true
+
 # If silent mode is true, it does not print the commands as they are executed.
 # Default is true. [true/false]
 SILENT_MODE = true
+
 # Choose ascii printable characters.
 # If true, it uses the extended characters, otherwise the basic ones.
 # Default is true. [true/false].
 ASCII_CHARACTERS = true
+
 # Set false to all the questions. If set false, option --yes will not work.
 # Default is true. [true/false].
 ASK_QUESTION = true
+
 # Download sources in parallel. Default is false. [true/false]
+# Alternatively, you can use the option '--parallel'.
 PARALLEL_DOWNLOADS = false
+
 # Pass your file pattern here, if you want to work only with 'sbo' packages
 # add '*_SBo' pattern. Default is the '*'.
 FILE_PATTERN = "*"
+
 # There are 5 predefined spinners for the progress bar.
 # Default is pixel. [spinner/pie/moon/line/pixel]
 PROGRESS_SPINNER = "pixel"
+
 # Choose color for the progress bar spinner.
 # Default is green. [green/violet/yellow/blue/cyan/grey/red]
 SPINNER_COLOR = "green"
 
 # Slackware command for install packages, instead, you can use 'installpkg'.
 # Normally upgradepkg only upgrades packages that are already installed
 # on the system, and will skip any packages that do not already have a
 # version installed. If --install- new is specified, the behavior is
 # modified to install new packages in addition to upgrading existing ones.
+# See: $ man upgradepkg.
 INSTALLPKG = "upgradepkg --install-new"
+
 # Slackware command to reinstall packages.
 # Upgradepkg usually skips packages if the exact same package (matching name,
 # version, arch, and build number) is already installed on the system. Use
 # the --reinstall option if you want to upgrade all packages even if the same
-# version is already installed.
+# version is already installed. See: $ man upgradepkg.
 REINSTALL = "upgradepkg --install-new --reinstall"
+
 # Slackware command to remove packages.
+#removepkg removes a previously installed Slackware package, while writing
+# a progress report to the standard output.  A package may be specified either
+# by the full package name (as you'd see listed in /var/lib/pkgtools/packages/),
+# or by the base package name. See: $ man removepkg.
 REMOVEPKG = "removepkg"
 
 # You can choose a downloader among wget, curl and lftp.
 # Default is wget. [wget/wget2/curl/lftp]
 DOWNLOADER = "wget"
+
 # Wget downloader options.
 # -c, --continue: resume getting a partially-downloaded file.
 # -q, Turn off Wget's output.
 # --show-progress, Force wget to display the progress bar in any verbosity.
 WGET_OPTIONS = "-c -q --progress=bar:force:noscroll --show-progress"
+
 # Curl downloader options.
 CURL_OPTIONS = ""
+
 # Lftp donwloader options.
 LFTP_GET_OPTIONS = "-c get -e"
+
 # Lftp mirror options are used to synchronize with the repositories.
 LFTP_MIRROR_OPTIONS = "-c mirror --parallel=100 --only-newer"
 
 # If you are going to use a proxy server, try to fill in these variables.
-# Choose between http or socks proxy type, not both.
+# Choose between http or socks proxy type.
 # For a socks proxy, you need to install the PySocks package.
 # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
-HTTP_PROXY_ADDRESS = ""
-SOCKS_PROXY_ADDRESS = ""
+PROXY_ADDRESS = ""
 PROXY_USERNAME = ""
 PROXY_PASSWORD = ""
```

### Comparing `slpkg-4.7.8/tests/test_configs.py` & `slpkg-4.7.9/tests/test_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         self.assertEqual(Path('/etc', 'slpkg'), self.configs.etc_path)
         self.assertEqual(Path('/var/lib/', 'slpkg', 'database'), self.configs.db_path)
         self.assertEqual(Path('/var', 'log', 'packages'), self.configs.log_packages)
 
         self.assertEqual('database.slpkg', self.configs.database_name)
         self.assertEqual('.pkgs', self.configs.file_list_suffix)
         self.assertEqual('upgradepkg --install-new', self.configs.installpkg)
-        self.assertEqual('upgradepkg --reinstall', self.configs.reinstall)
+        self.assertEqual('upgradepkg --install-new --reinstall', self.configs.reinstall)
         self.assertEqual('removepkg', self.configs.removepkg)
         self.assertEqual(True, self.configs.colors)
         self.assertEqual(True, self.configs.dialog)
         self.assertEqual('wget', self.configs.downloader)
         self.assertEqual('-c -q --progress=bar:force:noscroll --show-progress', self.configs.wget_options)
         self.assertEqual('', self.configs.curl_options)
         self.assertEqual('-c get -e', self.configs.lftp_get_options)
@@ -34,15 +34,14 @@
         self.assertEqual(True, self.configs.silent_mode)
         self.assertEqual(True, self.configs.ascii_characters)
         self.assertEqual(True, self.configs.ask_question)
         self.assertEqual(False, self.configs.parallel_downloads)
         self.assertEqual('*', self.configs.file_pattern)
         self.assertEqual('pixel', self.configs.progress_spinner)
         self.assertEqual('green', self.configs.spinner_color)
-        self.assertEqual('', self.configs.http_proxy_address)
-        self.assertEqual('', self.configs.socks_proxy_address)
+        self.assertEqual('', self.configs.proxy_address)
         self.assertEqual('', self.configs.proxy_username)
         self.assertEqual('', self.configs.proxy_password)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.7.8/tests/test_checks.py` & `slpkg-4.7.9/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/tests/test_utilities.py` & `slpkg-4.7.9/tests/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.assertEqual('1', self.utils.read_sbo_build_tag('slpkg', 'system'))
 
     def test_is_option(self):
         self.assertTrue(True, self.utils.is_option(['-P', '--parallel'],
                                                    ['-k', '-p', '-P', '--parallel', '--bin-repo']))
 
     def test_get_file_size(self):
-        self.assertEqual('2154 KB', self.utils.get_file_size(Path('/var/log/packages/', self.package)))
+        self.assertEqual('2 MB', self.utils.get_file_size(Path('/var/log/packages/', self.package)))
 
     def test_apply_package_pattern(self):
         self.assertGreater(len(self.utils.apply_package_pattern(self.data, ['*'])), 1)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.7.8/tests/test_sbo_queries.py` & `slpkg-4.7.9/tests/test_sbo_queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,27 +13,27 @@
         self.assertTrue(True, self.data[self.name])
 
     def test_location(self):
         self.assertEqual('system', self.data[self.name][0])
 
     def test_sources_x86(self):
         self.assertEqual(['https://gitlab.com/dslackw/slpkg/-/archive'
-                         '/4.7.6/slpkg-4.7.6.tar.gz'], self.data[self.name][3].split())
+                         '/4.7.8/slpkg-4.7.8.tar.gz'], self.data[self.name][3].split())
 
     def test_sources_x86_64(self):
         self.assertEqual([], self.data[self.name][4].split())
 
     def test_requires(self):
         self.assertEqual(['SQLAlchemy', 'python3-pythondialog', 'python3-progress'], self.data[self.name][7].split())
 
     def test_version(self):
-        self.assertEqual('4.7.6', self.data[self.name][2])
+        self.assertEqual('4.7.8', self.data[self.name][2])
 
     def test_checksum_x86(self):
-        self.assertListEqual(['26577e39fa7f58d9fa24fa24d91d1012'], self.data[self.name][5].split())
+        self.assertListEqual(['d0ba1c826dc691ceec1ad12603e51330'], self.data[self.name][5].split())
 
     def test_checksum_x86_64(self):
         self.assertListEqual([], self.data[self.name][6].split())
 
     def test_files(self):
         self.assertEqual(5, len(self.data[self.name][1].split()))
```

### Comparing `slpkg-4.7.8/tests/test_colors.py` & `slpkg-4.7.9/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/tests/test_upgrade.py` & `slpkg-4.7.9/tests/test_upgrade.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,37 +10,36 @@
 
     def setUp(self):
         self.utils = Utilities()
         self.sbo_queries = SBoQueries()
         self.data: dict = self.sbo_queries.repository_data()
 
     def test_installed_is_upgradable_for_sbo_repository(self):
-        repo: str = ''
         flags: list = []
         packages: list = ['sbo-create', 'ptpython', 'pycharm', 'powerline-status']
 
         for pkg in packages:
-            self.assertFalse(False, Upgrade(flags, self.data, repo).is_package_upgradeable(pkg))
+            self.assertFalse(False, Upgrade(flags, self.data).is_package_upgradeable(pkg))
 
     def test_installed_is_upgradable_for_slack_patches_repository(self):
         repo: str = 'slack_patches'
         bin_queries = BinQueries(repo)
         data: dict = bin_queries.repository_data()
         flags: list = ['-B', '--bin-repo=']
-        packages: list = ['vim', 'gvim', 'httpd','seamonkey', 'sudo']
+        packages: list = ['vim', 'httpd', 'seamonkey', 'sudo', 'python3', 'qt5', 'php']
 
         for pkg in packages:
-            self.assertFalse(False, Upgrade(flags, data, repo).is_package_upgradeable(pkg))
+            self.assertFalse(False, Upgrade(flags, data).is_package_upgradeable(pkg))
 
     def test_installed_is_upgradable_for_alien_repository(self):
         repo: str = 'alien'
         bin_queries = BinQueries(repo)
         data: dict = bin_queries.repository_data()
         flags: list = ['-B', '--bin-repo=']
         packages: list = ['audacity', 'vlc', 'dnspython']
 
         for pkg in packages:
-            self.assertFalse(False, Upgrade(flags, data, repo).is_package_upgradeable(pkg))
+            self.assertFalse(False, Upgrade(flags, data).is_package_upgradeable(pkg))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.7.8/tests/test_bin_queries.py` & `slpkg-4.7.9/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/LICENSE` & `slpkg-4.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/install.sh` & `slpkg-4.7.9/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/ChangeLog.txt` & `slpkg-4.7.9/ChangeLog.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+4.7.9 - 15/04/203
+Updated:
+- For proxies configuration
+- For convert file sizes
+- For packages upgrade
+Fixed:
+- Clear screen when dialog is disabled
+Added:
+- Support to local repositories (Thanks to marav)
+
 4.7.8 - 12/04/203
 Added:
-- Module to support for Unix shell-style wildcards for blacklist (Thanks yo marav)
+- Module to support for Unix shell-style wildcards for blacklist (Thanks to marav)
 - Supports proxies (Thanks to tpiszcze) #160
 Updated:
 - Config file for --reinstall option (Thanks to rizitis)
 - Improve speed
 
 4.7.7 - 07/04/2023
 Updated:
```

### Comparing `slpkg-4.7.8/man/slpkg.1` & `slpkg-4.7.9/man/slpkg.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/man/slpkg-fr.1` & `slpkg-4.7.9/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/completion/slpkg` & `slpkg-4.7.9/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/binaries/required.py` & `slpkg-4.7.9/slpkg/binaries/required.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 from slpkg.repositories import Repositories
 
 
 class Required:
     """ Creates a list of dependencies with
     the right order to install. """
 
-    def __init__(self, data: dict, name: str, repo: str):
-        __slots__ = 'data', 'name,' 'repo'
+    def __init__(self, data: dict, name: str):
+        __slots__ = 'data', 'name,'
         self.data: dict = data
         self.name: str = name
-        self.repo: str = repo
         self.repos = Repositories()
         self.utils = Utilities()
 
         self.special_repos: list = [
             self.repos.salixos_repo_name,
             self.repos.salixos_extra_repo_name,
             self.repos.slackel_repo_name,
             self.repos.slint_repo_name
         ]
 
+        self.repo = self.data[name][11]
+
     def resolve(self) -> list:
         """ Resolve the dependencies. """
         required: list[str] = self.data[self.name][6].split()
 
         # Resolve dependencies for some special repos.
         if self.repo in self.special_repos:
             requires: list = []
```

### Comparing `slpkg-4.7.8/slpkg/binaries/queries.py` & `slpkg-4.7.9/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/binaries/install.py` & `slpkg-4.7.9/slpkg/binaries/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 from slpkg.binaries.required import Required
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class Packages(Configs):
 
-    def __init__(self, data: dict, packages: list, flags: list, repo: str, mode: str):
-        __slots__ = 'data', 'packages', 'flags', 'repo', 'mode'
+    def __init__(self, data: dict, packages: list, flags: list, mode: str):
+        __slots__ = 'data', 'packages', 'flags', 'mode'
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
-        self.repo: str = repo
         self.mode: str = mode
 
         self.progress = ProgressBar()
         self.color = self.colour()
         self.utils = Utilities()
         self.repos = Repositories()
         self.dialogbox = DialogBox()
-        self.upgrade = Upgrade(self.flags, self.data, self.repo)
-        self.view_message = ViewMessage(self.flags, self.data, self.repo)
+        self.upgrade = Upgrade(self.flags, self.data)
+        self.view_message = ViewMessage(self.flags, self.data)
         self.session = Session
 
         self.output: int = 0
         self.stderr = None
         self.stdout = None
         self.process_message: str = ''
         self.bold: str = self.color['bold']
@@ -91,15 +90,15 @@
 
             for pkg in self.packages:
 
                 # Skip installed package when the option --skip-installed is applied.
                 if self.option_for_skip_installed and self.utils.is_package_installed(pkg):
                     continue
 
-                self.packages_requires += Required(self.data, pkg, self.repo).resolve()
+                self.packages_requires += Required(self.data, pkg).resolve()
 
             # Clean dependencies from the dependencies list if already added with main packages.
             requires = list(OrderedDict.fromkeys(self.packages_requires))
 
             if requires:
                 self.packages_requires = self.choose_dependencies(requires)
 
@@ -113,14 +112,15 @@
 
             if self.continue_install(pkg):
                 package: str = self.data[pkg][1]
                 mirror: str = self.data[pkg][2]
                 location: str = self.data[pkg][3]
 
                 pkg_urls.append(f'{mirror}{location}/{package}')
+
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
             else:
                 version: str = self.data[pkg][0]
                 self.view_message.view_skipping_packages(pkg, version)
 
         if pkg_urls:
@@ -170,19 +170,19 @@
             self.multi_process(command, package, message)
 
             if not self.option_for_resolve_off:
                 name: str = self.utils.split_binary_pkg(package[:-4])[0]
                 self.logging_installed_dependencies(name)
 
     def logging_installed_dependencies(self, name: str) -> None:
-        """ Logging installed dependencies and used for remove. """
+        """ Logging installed dependencies. """
         exist = self.session.query(LogsDependencies.name).filter(
             LogsDependencies.name == name).first()
 
-        requires: list = Required(self.data, name, self.repo).resolve()
+        requires: list = Required(self.data, name).resolve()
 
         # Update the dependencies if exist else create it.
         if exist:
             self.session.query(
                 LogsDependencies).filter(
                     LogsDependencies.name == name).update(
                         {LogsDependencies.requires: ' '.join(requires)})
```

### Comparing `slpkg-4.7.8/slpkg/install_data.py` & `slpkg-4.7.9/slpkg/install_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         self.session = Session
         self.utils = Utilities()
         self.repos = Repositories()
         self.color = self.colour()
 
         self.bold: str = self.color['bold']
         self.yellow: str = self.color['yellow']
+        self.cyan: str = self.color['cyan']
         self.byellow: str = f'{self.bold}{self.yellow}'
         self.endc: str = self.color['endc']
 
     def last_updated(self, repo_file: Path) -> str:
         """ Reads the first date of the changelog file."""
         lines: list = self.utils.read_file(repo_file)
         days = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
@@ -45,28 +46,28 @@
             'SLACKBUILD MD5SUM:',
             'SLACKBUILD MD5SUM_x86_64:',
             'SLACKBUILD REQUIRES:',
             'SLACKBUILD SHORT DESCRIPTION:'
         ]
         sbo_table = SBoTable
         sbo_name: str = self.repos.sbo_repo_name
-        path: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
+        path_slackbuilds: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
         path_changelog: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
 
         if self.repos.ponce_repo:
             sbo_table = PonceTable
             sbo_name: str = self.repos.ponce_repo_name
-            path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
+            path_slackbuilds = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
             path_changelog: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
 
-        slackbuilds_txt: list = self.utils.read_file(path)
+        slackbuilds_txt: list = self.utils.read_file(path_slackbuilds)
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
+        print(f"Updating the database for '{self.cyan}{sbo_name}{self.endc}'... ", end='', flush=True)
 
         for i, line in enumerate(slackbuilds_txt, 1):
 
             for tag in sbo_tags:
                 if line.startswith(tag):
                     line = line.replace(tag, '').strip()
                     cache.append(line)
@@ -87,14 +88,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_slack_data(self) -> None:
         """ Install the data for slackware repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.slack_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE MIRROR:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
@@ -111,25 +115,23 @@
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.slack_repo_mirror)
+                cache.append(self.repos.slack_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
@@ -174,14 +176,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_slack_extra_data(self) -> None:
         """ Install the data for slackware extra repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.slack_extra_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE MIRROR:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
@@ -198,25 +203,23 @@
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.slack_extra_repo_mirror)
+                cache.append(self.repos.slack_extra_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
@@ -261,14 +264,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_slack_patches_data(self) -> None:
         """ Install the data for slackware patches repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.slack_patches_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE MIRROR:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
@@ -285,25 +291,23 @@
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.slack_patches_repo_mirror)
+                cache.append(self.repos.slack_patches_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
@@ -348,14 +352,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_alien_data(self) -> None:
         """ Install the data for alien repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.alien_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -373,25 +380,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.alien_repo_packages_mirror)
+                cache.append("".join(self.repos.alien_repo_mirror))
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -441,14 +446,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_multilib_data(self) -> None:
         """ Install the data for multilib repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.multilib_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
@@ -465,25 +473,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.multilib_repo_packages_mirror)
+                cache.append("".join(self.repos.multilib_repo_mirror))
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -528,14 +534,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_restricted_data(self) -> None:
         """ Install the data for multilib repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.restricted_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
@@ -552,25 +561,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.restricted_repo_packages_mirror)
+                cache.append("".join(self.repos.restricted_repo_mirror))
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -615,14 +622,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_gnome_data(self) -> None:
         """ Install the data for gnome repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.gnome_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE MIRROR:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
@@ -640,25 +650,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.gnome_repo_mirror)
+                cache.append(self.repos.gnome_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
@@ -703,14 +711,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_msb_data(self) -> None:
         """ Install the data for msb repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.msb_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
@@ -727,25 +738,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.msb_repo_packages_mirror)
+                cache.append("".join(self.repos.msb_repo_mirror))
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -790,14 +799,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_csb_data(self) -> None:
         """ Install the data for csb repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.csb_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
@@ -814,25 +826,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.csb_repo_packages_mirror)
+                cache.append("".join(self.repos.csb_repo_mirror))
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -877,14 +887,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_conraid_data(self) -> None:
         """ Install the data for conraid repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.conraid_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE MIRROR:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
@@ -903,25 +916,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name: str = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.conraid_repo_mirror)
+                cache.append(self.repos.conraid_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location: str = line.replace(pkg_tag[2], '').strip()
@@ -966,14 +977,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_slackonly_data(self) -> None:
         """ Install the data for slackonly repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.slackonly_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -991,25 +1005,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.slackonly_repo_mirror)
+                cache.append(self.repos.slackonly_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -1059,14 +1071,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_salixos_data(self) -> None:
         """ Install the data for salixos repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.salixos_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -1084,25 +1099,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.salixos_repo_mirror)
+                cache.append(self.repos.salixos_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -1160,14 +1173,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_salixos_extra_data(self) -> None:
         """ Install the data for salixos_extra repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.salixos_extra_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -1186,25 +1202,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.salixos_extra_repo_mirror)
+                cache.append(self.repos.salixos_extra_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -1262,14 +1276,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_salixos_patches_data(self) -> None:
         """ Install the data for salixos_patches repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.salixos_patches_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -1288,25 +1305,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.salixos_patches_repo_mirror)
+                cache.append(self.repos.salixos_patches_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -1364,14 +1379,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_slackel_data(self) -> None:
         """ Install the data for slackel repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.slackel_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -1389,25 +1407,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.slackel_repo_mirror)
+                cache.append(self.repos.slackel_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
@@ -1465,14 +1481,17 @@
 
         print(f'{self.byellow}Done{self.endc}')
 
         self.session.commit()
 
     def install_slint_data(self) -> None:
         """ Install the data for slint repository. """
+        print(f"Updating the database for '{self.cyan}{self.repos.slint_repo_name}{self.endc}'... ",
+              end='', flush=True)
+
         checksums_dict: dict = {}
         pkg_tag = [
             'PACKAGE NAME:',
             'PACKAGE LOCATION:',
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
@@ -1490,25 +1509,23 @@
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
-        print('Creating the database... ', end='', flush=True)
-
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
                 package_name = line.replace(pkg_tag[0], '').strip()
                 split_package: list = self.utils.split_binary_pkg(package_name)
                 cache.append(split_package[0])  # package name
                 cache.append(split_package[1])  # package version
                 cache.append(package_name)
-                cache.append(self.repos.slint_repo_mirror)
+                cache.append(self.repos.slint_repo_mirror[0])
                 try:
                     cache.append(checksums_dict[package_name])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
```

### Comparing `slpkg-4.7.8/slpkg/repositories.py` & `slpkg-4.7.9/slpkg/repositories.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,458 +15,531 @@
     color = configs.colour()
     bold: str = color['bold']
     red: str = color['red']
     cyan: str = color['cyan']
     endc: str = color['endc']
     bred: str = f'{bold}{red}'
 
-    repositories_file_toml: Path = Path(configs.etc_path, 'repositories.toml')
+    repositories_toml_file: Path = Path(configs.etc_path, 'repositories.toml')
     repositories_path: Path = Path(configs.lib_path, 'repositories')
 
     repos_config = {}
     repositories = {}
     bin_repos_name = []
     bin_enabled_repos = []
-    sbo_enabled_repo: bool = True
 
+    sbo_repo: bool = True
     sbo_repo_name: str = 'sbo'
     sbo_repo_path: Path = Path(repositories_path, sbo_repo_name)
-    sbo_repo_mirror: str = 'https://slackbuilds.org/slackbuilds/15.0/'
+    sbo_repo_mirror = ['https://slackbuilds.org/slackbuilds/15.0/']
     sbo_repo_slackbuilds: str = 'SLACKBUILDS.TXT'
     sbo_repo_changelog: str = 'ChangeLog.txt'
     sbo_repo_tar_suffix: str = '.tar.gz'
     sbo_repo_tag: str = '_SBo'
     sbo_repo_patch_tag: str = ''
 
     ponce_repo: bool = False
     ponce_repo_name: str = 'ponce'
     ponce_repo_path: Path = Path(repositories_path, ponce_repo_name)
-    ponce_repo_mirror: str = 'https://cgit.ponce.cc/slackbuilds/plain/'
+    ponce_repo_mirror = ['https://cgit.ponce.cc/slackbuilds/plain/']
     ponce_repo_slackbuilds: str = 'SLACKBUILDS.TXT'
     ponce_repo_changelog: str = 'ChangeLog.txt'
     ponce_repo_tag: str = '_SBo'
     ponce_repo_patch_tag: str = ''
 
     slack_repo: bool = False
     slack_repo_name: str = 'slack'
     slack_repo_path: Path = Path(repositories_path, slack_repo_name)
-    slack_repo_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/'
+    slack_repo_mirror = ['https://slackware.uk/slackware/slackware64-15.0/']
     slack_repo_packages: str = 'PACKAGES.TXT'
     slack_repo_checksums: str = 'CHECKSUMS.md5'
     slack_repo_changelog: str = 'ChangeLog.txt'
     slack_repo_tag: str = ''
 
     slack_extra_repo: bool = False
     slack_extra_repo_name: str = 'slack_extra'
     slack_extra_repo_path: Path = Path(repositories_path, slack_extra_repo_name)
-    slack_extra_repo_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/'
-    slack_extra_packages_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/extra/'
+    slack_extra_repo_mirror = ['https://slackware.uk/slackware/slackware64-15.0/', "extra/"]
     slack_extra_repo_packages: str = 'PACKAGES.TXT'
     slack_extra_repo_checksums: str = 'CHECKSUMS.md5'
     slack_extra_repo_changelog: str = 'ChangeLog.txt'
     slack_extra_repo_tag: str = ''
 
     slack_patches_repo: bool = False
     slack_patches_repo_name: str = 'slack_patches'
     slack_patches_repo_path: Path = Path(repositories_path, slack_patches_repo_name)
-    slack_patches_repo_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/'
-    slack_patches_packages_mirror: str = 'https://slackware.uk/slackware/slackware64-15.0/patches/'
+    slack_patches_repo_mirror = ['https://slackware.uk/slackware/slackware64-15.0/', 'patches/']
     slack_patches_repo_packages: str = 'PACKAGES.TXT'
     slack_patches_repo_checksums: str = 'CHECKSUMS.md5'
     slack_patches_repo_changelog: str = 'ChangeLog.txt'
     slack_patches_repo_tag: str = '_slack15.0'
 
     alien_repo: bool = False
     alien_repo_name: str = 'alien'
     alien_repo_path: Path = Path(repositories_path, alien_repo_name)
-    alien_repo_mirror: str = 'https://slackware.nl/people/alien/sbrepos/'
-    alien_repo_packages_mirror: str = 'https://slackware.nl/people/alien/sbrepos/15.0/x86_64/'
+    alien_repo_mirror = ['https://slackware.nl/people/alien/sbrepos/', '15.0/', 'x86_64/']
     alien_repo_packages: str = 'PACKAGES.TXT'
     alien_repo_checksums: str = 'CHECKSUMS.md5'
     alien_repo_changelog: str = 'ChangeLog.txt'
     alien_repo_tag: str = 'alien'
 
     multilib_repo: bool = False
     multilib_repo_name: str = 'multilib'
     multilib_repo_path: Path = Path(repositories_path, multilib_repo_name)
-    multilib_repo_mirror: str = 'https://slackware.nl/people/alien/multilib/'
-    multilib_repo_packages_mirror: str = 'https://slackware.nl/people/alien/multilib/15.0/'
+    multilib_repo_mirror = ['https://slackware.nl/people/alien/multilib/', '15.0/']
     multilib_repo_packages: str = 'PACKAGES.TXT'
     multilib_repo_checksums: str = 'CHECKSUMS.md5'
     multilib_repo_changelog: str = 'ChangeLog.txt'
     multilib_repo_tag: str = 'alien'
 
     restricted_repo: bool = False
     restricted_repo_name: str = 'restricted'
     restricted_repo_path: Path = Path(repositories_path, restricted_repo_name)
-    restricted_repo_mirror: str = 'https://slackware.nl/people/alien/restricted_sbrepos/'
-    restricted_repo_packages_mirror: str = 'https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/'
+    restricted_repo_mirror = ['https://slackware.nl/people/alien/restricted_sbrepos/', '15.0/', 'x86_64/']
     restricted_repo_packages: str = 'PACKAGES.TXT'
     restricted_repo_checksums: str = 'CHECKSUMS.md5'
     restricted_repo_changelog: str = 'ChangeLog.txt'
     restricted_repo_tag: str = 'alien'
 
     gnome_repo: bool = False
     gnome_repo_name: str = 'gnome'
     gnome_repo_path: Path = Path(repositories_path, gnome_repo_name)
-    gnome_repo_mirror: str = 'https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/'
+    gnome_repo_mirror = ['https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/']
     gnome_repo_packages: str = 'PACKAGES.TXT'
     gnome_repo_checksums: str = 'CHECKSUMS.md5'
     gnome_repo_changelog: str = 'ChangeLog.txt'
     gnome_repo_tag: str = 'gfs'
 
     msb_repo: bool = False
     msb_repo_name: str = 'msb'
     msb_repo_path: Path = Path(repositories_path, msb_repo_name)
-    msb_repo_mirror: str = 'https://slackware.uk/msb/'
-    msb_repo_packages_mirror: str = 'https://slackware.uk/msb/15.0/1.26/x86_64/'
+    msb_repo_mirror = ['https://slackware.uk/msb/', '15.0/', '1.26/', 'x86_64/']
     msb_repo_packages: str = 'PACKAGES.TXT'
     msb_repo_checksums: str = 'CHECKSUMS.md5'
     msb_repo_changelog: str = 'ChangeLog.txt'
     msb_repo_tag: str = 'msb'
 
     csb_repo: bool = False
     csb_repo_name: str = 'csb'
     csb_repo_path: Path = Path(repositories_path, csb_repo_name)
-    csb_repo_mirror: str = 'https://slackware.uk/csb/'
-    csb_repo_packages_mirror: str = 'https://slackware.uk/csb/15.0/x86_64/'
+    csb_repo_mirror = ['https://slackware.uk/csb/', '15.0/', 'x86_64/']
     csb_repo_packages: str = 'PACKAGES.TXT'
     csb_repo_checksums: str = 'CHECKSUMS.md5'
     csb_repo_changelog: str = 'ChangeLog.txt'
     csb_repo_tag: str = 'csb'
 
     conraid_repo: bool = False
     conraid_repo_name: str = 'conraid'
     conraid_repo_path: Path = Path(repositories_path, conraid_repo_name)
-    conraid_repo_mirror: str = 'https://slack.conraid.net/repository/slackware64-current/'
+    conraid_repo_mirror = ['https://slack.conraid.net/repository/slackware64-current/']
     conraid_repo_packages: str = 'PACKAGES.TXT'
     conraid_repo_checksums: str = 'CHECKSUMS.md5'
     conraid_repo_changelog: str = 'ChangeLog.txt'
     conraid_repo_tag: str = 'cf'
 
     slackonly_repo: bool = False
     slackonly_repo_name: str = 'slackonly'
     slackonly_repo_path: Path = Path(repositories_path, slackonly_repo_name)
-    slackonly_repo_mirror: str = 'https://packages.slackonly.com/pub/packages/15.0-x86_64/'
+    slackonly_repo_mirror = ['https://packages.slackonly.com/pub/packages/15.0-x86_64/']
     slackonly_repo_packages: str = 'PACKAGES.TXT'
     slackonly_repo_checksums: str = 'CHECKSUMS.md5'
     slackonly_repo_changelog: str = 'ChangeLog.txt'
     slackonly_repo_tag: str = 'slonly'
 
     salixos_repo: bool = False
     salixos_repo_name: str = 'salixos'
     salixos_repo_path: Path = Path(repositories_path, salixos_repo_name)
-    salixos_repo_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/'
+    salixos_repo_mirror = ['https://download.salixos.org/x86_64/slackware-15.0/']
     salixos_repo_packages: str = 'PACKAGES.TXT'
     salixos_repo_checksums: str = 'CHECKSUMS.md5'
     salixos_repo_changelog: str = 'ChangeLog.txt'
     salixos_repo_tag: str = ''
 
     salixos_extra_repo: bool = False
     salixos_extra_repo_name: str = 'salixos_extra'
     salixos_extra_repo_path: Path = Path(repositories_path, salixos_extra_repo_name)
-    salixos_extra_repo_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/'
-    salixos_extra_repo_packages_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/extra/'
+    salixos_extra_repo_mirror = ['https://download.salixos.org/x86_64/slackware-15.0/', 'extra/']
     salixos_extra_repo_packages: str = 'PACKAGES.TXT'
     salixos_extra_repo_checksums: str = 'CHECKSUMS.md5'
     salixos_extra_repo_changelog: str = 'ChangeLog.txt'
     salixos_extra_repo_tag: str = ''
 
     salixos_patches_repo: bool = False
     salixos_patches_repo_name: str = 'salixos_patches'
     salixos_patches_repo_path: Path = Path(repositories_path, salixos_patches_repo_name)
-    salixos_patches_repo_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/'
-    salixos_patches_repo_packages_mirror: str = 'https://download.salixos.org/x86_64/slackware-15.0/patches/'
+    salixos_patches_repo_mirror = ['https://download.salixos.org/x86_64/slackware-15.0/', 'patches/']
     salixos_patches_repo_packages: str = 'PACKAGES.TXT'
     salixos_patches_repo_checksums: str = 'CHECKSUMS.md5'
     salixos_patches_repo_changelog: str = 'ChangeLog.txt'
     salixos_patches_repo_tag: str = '_slack15.0'
 
     slackel_repo: bool = False
     slackel_repo_name: str = 'slackel'
     slackel_repo_path: Path = Path(repositories_path, slackel_repo_name)
-    slackel_repo_mirror: str = 'http://www.slackel.gr/repo/x86_64/current/'
+    slackel_repo_mirror = ['http://www.slackel.gr/repo/x86_64/current/']
     slackel_repo_packages: str = 'PACKAGES.TXT'
     slackel_repo_checksums: str = 'CHECKSUMS.md5'
     slackel_repo_changelog: str = 'ChangeLog.txt'
     slackel_repo_tag: str = 'dj'
 
     slint_repo: bool = False
     slint_repo_name: str = 'slint'
     slint_repo_path: Path = Path(repositories_path, slint_repo_name)
-    slint_repo_mirror: str = 'https://slackware.uk/slint/x86_64/slint-15.0/'
+    slint_repo_mirror = ['https://slackware.uk/slint/x86_64/slint-15.0/']
     slint_repo_packages: str = 'PACKAGES.TXT'
     slint_repo_checksums: str = 'CHECKSUMS.md5'
     slint_repo_changelog: str = 'ChangeLog.txt'
     slint_repo_tag: str = 'slint'
 
     try:
-        if repositories_file_toml.is_file():
-            with open(repositories_file_toml, 'rb') as repo:
+        if repositories_toml_file.is_file():
+            with open(repositories_toml_file, 'rb') as repo:
                 repos_config = tomli.load(repo)['REPOSITORIES']
 
             sbo_repo_name: str = repos_config['SBO_REPO_NAME']
-            sbo_repo_mirror: str = repos_config['SBO_REPO_MIRROR']
+            sbo_repo_mirror = repos_config['SBO_REPO_MIRROR']
             sbo_repo_slackbuilds: str = repos_config['SBO_REPO_SLACKBUILDS']
             sbo_repo_changelog: str = repos_config['SBO_REPO_CHANGELOG']
             sbo_repo_tar_suffix: str = repos_config['SBO_REPO_TAR_SUFFIX']
             sbo_repo_tag: str = repos_config['SBO_REPO_TAG']
             sbo_repo_patch_tag: str = repos_config['SBO_REPO_PATCH_TAG']
+            if sbo_repo_mirror[0].startswith('file'):
+                sbo_repo_path: str = sbo_repo_mirror[0][7:]
 
             ponce_repo: bool = repos_config['PONCE_REPO']
             ponce_repo_name: str = repos_config['PONCE_REPO_NAME']
-            ponce_repo_mirror: str = repos_config['PONCE_REPO_MIRROR']
+            ponce_repo_mirror = repos_config['PONCE_REPO_MIRROR']
             ponce_repo_slackbuilds: str = repos_config['PONCE_REPO_SLACKBUILDS']
             ponce_repo_changelog: str = repos_config['PONCE_REPO_CHANGELOG']
             ponce_repo_tag: str = repos_config['PONCE_REPO_TAG']
             ponce_repo_patch_tag: str = repos_config['PONCE_REPO_PATCH_TAG']
+            if ponce_repo_mirror[0].startswith('file'):
+                ponce_repo_path: str = ponce_repo_mirror[0][7:]
 
             slack_repo: bool = repos_config['SLACK_REPO']
             slack_repo_name: str = repos_config['SLACK_REPO_NAME']
-            slack_repo_mirror: str = repos_config['SLACK_REPO_MIRROR']
+            slack_repo_mirror = repos_config['SLACK_REPO_MIRROR']
             slack_repo_packages: str = repos_config['SLACK_REPO_PACKAGES']
             slack_repo_checksums: str = repos_config['SLACK_REPO_CHECKSUMS']
             slack_repo_changelog: str = repos_config['SLACK_REPO_CHANGELOG']
             slack_repo_tag: str = repos_config['SLACK_REPO_TAG']
+            if slack_repo_mirror[0].startswith('file'):
+                slack_repo_path: str = slack_repo_mirror[0][7:]
 
             slack_extra_repo: bool = repos_config['SLACK_EXTRA_REPO']
             slack_extra_repo_name: str = repos_config['SLACK_EXTRA_REPO_NAME']
-            slack_extra_repo_mirror: str = repos_config['SLACK_EXTRA_REPO_MIRROR']
-            slack_extra_repo_packages_mirror: str = repos_config['SLACK_EXTRA_REPO_PACKAGES_MIRROR']
+            slack_extra_repo_mirror = repos_config['SLACK_EXTRA_REPO_MIRROR']
             slack_extra_repo_packages: str = repos_config['SLACK_EXTRA_REPO_PACKAGES']
             slack_extra_repo_checksums: str = repos_config['SLACK_EXTRA_REPO_CHECKSUMS']
             slack_extra_repo_changelog: str = repos_config['SLACK_EXTRA_REPO_CHANGELOG']
             slack_extra_repo_tag: str = repos_config['SLACK_EXTRA_REPO_TAG']
+            if slack_extra_repo_mirror[0].startswith('file'):
+                slack_extra_repo_path: str = ''.join(slack_extra_repo_mirror)[7:]
 
             slack_patches_repo: bool = repos_config['SLACK_PATCHES_REPO']
             slack_patches_repo_name: str = repos_config['SLACK_PATCHES_REPO_NAME']
-            slack_patches_repo_mirror: str = repos_config['SLACK_PATCHES_REPO_MIRROR']
-            slack_patches_repo_packages_mirror: str = repos_config['SLACK_PATCHES_REPO_PACKAGES_MIRROR']
+            slack_patches_repo_mirror = repos_config['SLACK_PATCHES_REPO_MIRROR']
             slack_patches_repo_packages: str = repos_config['SLACK_PATCHES_REPO_PACKAGES']
             slack_patches_repo_checksums: str = repos_config['SLACK_PATCHES_REPO_CHECKSUMS']
             slack_patches_repo_changelog: str = repos_config['SLACK_PATCHES_REPO_CHANGELOG']
             slack_patches_repo_tag: str = repos_config['SLACK_PATCHES_REPO_TAG']
+            if slack_patches_repo_mirror[0].startswith('file'):
+                slack_patches_repo_path: str = ''.join(slack_patches_repo_mirror)[7:]
 
             alien_repo: bool = repos_config['ALIEN_REPO']
             alien_repo_name: str = repos_config['ALIEN_REPO_NAME']
-            alien_repo_mirror: str = repos_config['ALIEN_REPO_MIRROR']
-            alien_repo_packages_mirror: str = repos_config['ALIEN_REPO_PACKAGES_MIRROR']
+            alien_repo_mirror = repos_config['ALIEN_REPO_MIRROR']
             alien_repo_packages: str = repos_config['ALIEN_REPO_PACKAGES']
             alien_repo_checksums: str = repos_config['ALIEN_REPO_CHECKSUMS']
             alien_repo_changelog: str = repos_config['ALIEN_REPO_CHANGELOG']
             alien_repo_tag: str = repos_config['ALIEN_REPO_TAG']
+            if alien_repo_mirror[0].startswith('file'):
+                alien_repo_path: str = ''.join(alien_repo_mirror)[7:]
 
             multilib_repo: bool = repos_config['MULTILIB_REPO']
             multilib_repo_name: str = repos_config['MULTILIB_REPO_NAME']
-            multilib_repo_mirror: str = repos_config['MULTILIB_REPO_MIRROR']
-            multilib_repo_packages_mirror: str = repos_config['MULTILIB_REPO_PACKAGES_MIRROR']
+            multilib_repo_mirror = repos_config['MULTILIB_REPO_MIRROR']
             multilib_repo_packages: str = repos_config['MULTILIB_REPO_PACKAGES']
             multilib_repo_checksums: str = repos_config['MULTILIB_REPO_CHECKSUMS']
             multilib_repo_changelog: str = repos_config['MULTILIB_REPO_CHANGELOG']
             multilib_repo_tag: str = repos_config['MULTILIB_REPO_TAG']
+            if multilib_repo_mirror[0].startswith('file'):
+                multilib_repo_path: str = ''.join(multilib_repo_mirror)[7:]
 
             restricted_repo: bool = repos_config['RESTRICTED_REPO']
             restricted_repo_name: str = repos_config['RESTRICTED_REPO_NAME']
-            restricted_repo_mirror: str = repos_config['RESTRICTED_REPO_MIRROR']
-            restricted_repo_packages_mirror: str = repos_config['RESTRICTED_REPO_PACKAGES_MIRROR']
+            restricted_repo_mirror = repos_config['RESTRICTED_REPO_MIRROR']
             restricted_repo_packages: str = repos_config['RESTRICTED_REPO_PACKAGES']
             restricted_repo_checksums: str = repos_config['RESTRICTED_REPO_CHECKSUMS']
             restricted_repo_changelog: str = repos_config['RESTRICTED_REPO_CHANGELOG']
             restricted_repo_tag: str = repos_config['RESTRICTED_REPO_TAG']
+            if restricted_repo_mirror[0].startswith('file'):
+                restricted_repo_path: str = ''.join(restricted_repo_mirror)[7:]
 
             gnome_repo: bool = repos_config['GNOME_REPO']
             gnome_repo_name: str = repos_config['GNOME_REPO_NAME']
-            gnome_repo_mirror: str = repos_config['GNOME_REPO_MIRROR']
+            gnome_repo_mirror = repos_config['GNOME_REPO_MIRROR']
             gnome_repo_packages: str = repos_config['GNOME_REPO_PACKAGES']
             gnome_repo_checksums: str = repos_config['GNOME_REPO_CHECKSUMS']
             gnome_repo_changelog: str = repos_config['GNOME_REPO_CHANGELOG']
             gnome_repo_tag: str = repos_config['GNOME_REPO_TAG']
+            if gnome_repo_mirror[0].startswith('file'):
+                gnome_repo_path: str = gnome_repo_mirror[0][7:]
 
             msb_repo: bool = repos_config['MSB_REPO']
             msb_repo_name: str = repos_config['MSB_REPO_NAME']
-            msb_repo_mirror: str = repos_config['MSB_REPO_MIRROR']
-            msb_repo_packages_mirror: str = repos_config['MSB_REPO_PACKAGES_MIRROR']
+            msb_repo_mirror = repos_config['MSB_REPO_MIRROR']
             msb_repo_packages: str = repos_config['MSB_REPO_PACKAGES']
             msb_repo_checksums: str = repos_config['MSB_REPO_CHECKSUMS']
             msb_repo_changelog: str = repos_config['MSB_REPO_CHANGELOG']
             msb_repo_tag: str = repos_config['MSB_REPO_TAG']
+            if msb_repo_mirror[0].startswith('file'):
+                msb_repo_path: str = ''.join(msb_repo_mirror)[7:]
 
             csb_repo: bool = repos_config['CSB_REPO']
             csb_repo_name: str = repos_config['CSB_REPO_NAME']
-            csb_repo_mirror: str = repos_config['CSB_REPO_MIRROR']
-            csb_repo_packages_mirror: str = repos_config['CSB_REPO_PACKAGES_MIRROR']
+            csb_repo_mirror = repos_config['CSB_REPO_MIRROR']
             csb_repo_packages: str = repos_config['CSB_REPO_PACKAGES']
             csb_repo_checksums: str = repos_config['CSB_REPO_CHECKSUMS']
             csb_repo_changelog: str = repos_config['CSB_REPO_CHANGELOG']
             csb_repo_tag: str = repos_config['CSB_REPO_TAG']
+            if csb_repo_mirror[0].startswith('file'):
+                csb_repo_path: str = ''.join(csb_repo_mirror)[7:]
 
             conraid_repo: bool = repos_config['CONRAID_REPO']
             conraid_repo_name: str = repos_config['CONRAID_REPO_NAME']
-            conraid_repo_mirror: str = repos_config['CONRAID_REPO_MIRROR']
+            conraid_repo_mirror = repos_config['CONRAID_REPO_MIRROR']
             conraid_repo_packages: str = repos_config['CONRAID_REPO_PACKAGES']
             conraid_repo_checksums: str = repos_config['CONRAID_REPO_CHECKSUMS']
             conraid_repo_changelog: str = repos_config['CONRAID_REPO_CHANGELOG']
             conraid_repo_tag: str = repos_config['CONRAID_REPO_TAG']
+            if conraid_repo_mirror[0].startswith('file'):
+                conraid_repo_path: str = conraid_repo_mirror[0][7:]
 
             slackonly_repo: bool = repos_config['SLACKONLY_REPO']
             slackonly_repo_name: str = repos_config['SLACKONLY_REPO_NAME']
-            slackonly_repo_mirror: str = repos_config['SLACKONLY_REPO_MIRROR']
+            slackonly_repo_mirror = repos_config['SLACKONLY_REPO_MIRROR']
             slackonly_repo_packages: str = repos_config['SLACKONLY_REPO_PACKAGES']
             slackonly_repo_checksums: str = repos_config['SLACKONLY_REPO_CHECKSUMS']
             slackonly_repo_changelog: str = repos_config['SLACKONLY_REPO_CHANGELOG']
             slackonly_repo_tag: str = repos_config['SLACKONLY_REPO_TAG']
+            if slackonly_repo_mirror[0].startswith('file'):
+                slackonly_repo_path: str = slackonly_repo_mirror[0][7:]
 
             salixos_repo: bool = repos_config['SALIXOS_REPO']
             salixos_repo_name: str = repos_config['SALIXOS_REPO_NAME']
-            salixos_repo_mirror: str = repos_config['SALIXOS_REPO_MIRROR']
+            salixos_repo_mirror = repos_config['SALIXOS_REPO_MIRROR']
             salixos_repo_packages: str = repos_config['SALIXOS_REPO_PACKAGES']
             salixos_repo_checksums: str = repos_config['SALIXOS_REPO_CHECKSUMS']
             salixos_repo_changelog: str = repos_config['SALIXOS_REPO_CHANGELOG']
             salixos_repo_tag: str = repos_config['SALIXOS_REPO_TAG']
+            if salixos_repo_mirror[0].startswith('file'):
+                salixos_repo_path: str = salixos_repo_mirror[0][7:]
 
             salixos_extra_repo: bool = repos_config['SALIXOS_EXTRA_REPO']
             salixos_extra_repo_name: str = repos_config['SALIXOS_EXTRA_REPO_NAME']
-            salixos_extra_repo_mirror: str = repos_config['SALIXOS_EXTRA_REPO_MIRROR']
-            salixos_extra_repo_packages_mirror: str = repos_config['SALIXOS_EXTRA_REPO_PACKAGES_MIRROR']
+            salixos_extra_repo_mirror = repos_config['SALIXOS_EXTRA_REPO_MIRROR']
             salixos_extra_repo_packages: str = repos_config['SALIXOS_EXTRA_REPO_PACKAGES']
             salixos_extra_repo_checksums: str = repos_config['SALIXOS_EXTRA_REPO_CHECKSUMS']
             salixos_extra_repo_changelog: str = repos_config['SALIXOS_EXTRA_REPO_CHANGELOG']
             salixos_extra_repo_tag: str = repos_config['SALIXOS_EXTRA_REPO_TAG']
+            if salixos_extra_repo_mirror[0].startswith('file'):
+                salixos_extra_repo_path: str = ''.join(salixos_extra_repo_mirror)[7:]
 
             salixos_patches_repo: bool = repos_config['SALIXOS_PATCHES_REPO']
             salixos_patches_repo_name: str = repos_config['SALIXOS_PATCHES_REPO_NAME']
-            salixos_patches_repo_mirror: str = repos_config['SALIXOS_PATCHES_REPO_MIRROR']
-            salixos_patches_repo_packages_mirror: str = repos_config['SALIXOS_PATCHES_REPO_PACKAGES_MIRROR']
+            salixos_patches_repo_mirror = repos_config['SALIXOS_PATCHES_REPO_MIRROR']
             salixos_patches_repo_packages: str = repos_config['SALIXOS_PATCHES_REPO_PACKAGES']
             salixos_patches_repo_checksums: str = repos_config['SALIXOS_PATCHES_REPO_CHECKSUMS']
             salixos_patches_repo_changelog: str = repos_config['SALIXOS_PATCHES_REPO_CHANGELOG']
             salixos_patches_repo_tag: str = repos_config['SALIXOS_PATCHES_REPO_TAG']
+            if salixos_patches_repo_mirror[0].startswith('file'):
+                salixos_patches_repo_path: str = ''.join(salixos_patches_repo_mirror)[7:]
 
             slackel_repo: bool = repos_config['SLACKEL_REPO']
             slackel_repo_name: str = repos_config['SLACKEL_REPO_NAME']
-            slackel_repo_mirror: str = repos_config['SLACKEL_REPO_MIRROR']
+            slackel_repo_mirror = repos_config['SLACKEL_REPO_MIRROR']
             slackel_repo_packages: str = repos_config['SLACKEL_REPO_PACKAGES']
             slackel_repo_checksums: str = repos_config['SLACKEL_REPO_CHECKSUMS']
             slackel_repo_changelog: str = repos_config['SLACKEL_REPO_CHANGELOG']
             slackel_repo_tag: str = repos_config['SLACKEL_REPO_TAG']
+            if slackel_repo_mirror[0].startswith('file'):
+                slackel_repo_path: str = slackel_repo_mirror[0][7:]
 
             slint_repo: bool = repos_config['SLINT_REPO']
             slint_repo_name: str = repos_config['SLINT_REPO_NAME']
-            slint_repo_mirror: str = repos_config['SLINT_REPO_MIRROR']
+            slint_repo_mirror = repos_config['SLINT_REPO_MIRROR']
             slint_repo_packages: str = repos_config['SLINT_REPO_PACKAGES']
             slint_repo_checksums: str = repos_config['SLINT_REPO_CHECKSUMS']
             slint_repo_changelog: str = repos_config['SLINT_REPO_CHANGELOG']
             slint_repo_tag: str = repos_config['SLINT_REPO_TAG']
+            if slint_repo_mirror[0].startswith('file'):
+                slint_repo_path: str = slint_repo_mirror[0][7:]
 
     except (tomli.TOMLDecodeError, KeyError) as error:
         raise SystemExit(f'\n{configs.prog_name} {bred}Error{endc}: {error}: in the configuration file '
-                         f"'{repositories_file_toml}'.\n"
+                         f"'{repositories_toml_file}'.\n"
                          f"\nIf you have upgraded the '{configs.prog_name}' probably you need to run:\n"
-                         f"'mv {repositories_file_toml}.new {repositories_file_toml}'.\n"
+                         f"'mv {repositories_toml_file}.new {repositories_toml_file}'.\n"
                          f"or '{cyan}slpkg_new-configs{endc}' command.\n")
 
     # Default sbo repository configs.
     repo_tag: str = sbo_repo_tag
     patch_repo_tag: str = sbo_repo_patch_tag
-    sbo_enabled_repository: str = sbo_repo_name
+    sbo_enabled_repo_name: str = sbo_repo_name
     if ponce_repo:
-        sbo_enabled_repository: str = ponce_repo_name
+        sbo_enabled_repo_name: str = ponce_repo_name
         repo_tag: str = ponce_repo_tag
         patch_repo_tag: str = ponce_repo_patch_tag
-        sbo_enabled_repo: bool = False
+        sbo_repo: bool = False
 
     # List of repositories.
     repositories = {
-        sbo_repo_name: [sbo_enabled_repo,
+        sbo_repo_name: [sbo_repo,
                         sbo_repo_path,
+                        sbo_repo_mirror,
+                        sbo_repo_slackbuilds,
                         sbo_repo_changelog,
-                        sbo_repo_tag],
+                        sbo_repo_tar_suffix,
+                        sbo_repo_tag,
+                        sbo_repo_patch_tag],
 
         ponce_repo_name: [ponce_repo,
                           ponce_repo_path,
+                          ponce_repo_mirror,
+                          ponce_repo_slackbuilds,
                           ponce_repo_changelog,
-                          ponce_repo_tag],
+                          ponce_repo_tag,
+                          ponce_repo_patch_tag],
 
         slack_repo_name: [slack_repo,
                           slack_repo_path,
+                          slack_repo_mirror,
+                          slack_repo_packages,
+                          slack_repo_checksums,
                           slack_repo_changelog,
                           slack_repo_tag],
 
         slack_extra_repo_name: [slack_extra_repo,
                                 slack_extra_repo_path,
+                                slack_extra_repo_mirror,
+                                slack_extra_repo_packages,
+                                slack_extra_repo_checksums,
                                 slack_extra_repo_changelog,
                                 slack_extra_repo_tag],
 
         slack_patches_repo_name: [slack_patches_repo,
                                   slack_patches_repo_path,
+                                  slack_patches_repo_mirror,
+                                  slack_patches_repo_packages,
+                                  slack_patches_repo_checksums,
                                   slack_patches_repo_changelog,
                                   slack_patches_repo_tag],
 
         alien_repo_name: [alien_repo,
                           alien_repo_path,
+                          alien_repo_mirror,
+                          alien_repo_packages,
+                          alien_repo_checksums,
                           alien_repo_changelog,
                           alien_repo_tag],
 
         multilib_repo_name: [multilib_repo,
                              multilib_repo_path,
+                             multilib_repo_mirror,
+                             multilib_repo_packages,
+                             multilib_repo_checksums,
                              multilib_repo_changelog,
                              multilib_repo_tag],
 
         restricted_repo_name: [restricted_repo,
                                restricted_repo_path,
+                               restricted_repo_mirror,
+                               restricted_repo_packages,
+                               restricted_repo_checksums,
                                restricted_repo_changelog,
                                restricted_repo_tag],
 
         gnome_repo_name: [gnome_repo,
                           gnome_repo_path,
+                          gnome_repo_mirror,
+                          gnome_repo_packages,
+                          gnome_repo_checksums,
                           gnome_repo_changelog,
                           gnome_repo_tag],
 
         msb_repo_name: [msb_repo,
                         msb_repo_path,
+                        msb_repo_mirror,
+                        msb_repo_packages,
+                        msb_repo_checksums,
                         msb_repo_changelog,
                         msb_repo_tag],
 
         csb_repo_name: [csb_repo,
                         csb_repo_path,
+                        csb_repo_mirror,
+                        csb_repo_packages,
+                        csb_repo_checksums,
                         csb_repo_changelog,
                         csb_repo_tag],
 
         conraid_repo_name: [conraid_repo,
                             conraid_repo_path,
+                            conraid_repo_mirror,
+                            conraid_repo_packages,
+                            conraid_repo_checksums,
                             conraid_repo_changelog,
                             conraid_repo_tag],
 
         slackonly_repo_name: [slackonly_repo,
                               slackonly_repo_path,
+                              slackonly_repo_mirror,
+                              slackonly_repo_packages,
+                              slackonly_repo_checksums,
                               slackonly_repo_changelog,
                               slackonly_repo_tag],
 
         salixos_repo_name: [salixos_repo,
                             salixos_repo_path,
+                            salixos_repo_mirror,
+                            salixos_repo_packages,
+                            salixos_repo_checksums,
                             salixos_repo_changelog,
                             salixos_repo_tag],
 
         salixos_extra_repo_name: [salixos_extra_repo,
                                   salixos_extra_repo_path,
+                                  salixos_extra_repo_mirror,
+                                  salixos_extra_repo_packages,
+                                  salixos_extra_repo_checksums,
                                   salixos_extra_repo_changelog,
                                   slack_extra_repo_tag],
 
         salixos_patches_repo_name: [salixos_patches_repo,
                                     salixos_patches_repo_path,
+                                    salixos_patches_repo_mirror,
+                                    salixos_patches_repo_packages,
+                                    salixos_patches_repo_checksums,
                                     salixos_patches_repo_changelog,
                                     salixos_patches_repo_tag],
 
         slackel_repo_name: [slackel_repo,
                             slackel_repo_path,
+                            slackel_repo_mirror,
+                            slackel_repo_packages,
+                            slackel_repo_checksums,
                             slackel_repo_changelog,
                             slackel_repo_tag],
 
         slint_repo_name: [slint_repo,
                           slint_repo_path,
+                          slint_repo_mirror,
+                          slint_repo_packages,
+                          slint_repo_checksums,
                           slint_repo_changelog,
                           slint_repo_tag]
     }
 
     # All the binary repositories names.
     bin_repos_names = list(repositories.keys())[2:]
```

### Comparing `slpkg-4.7.8/slpkg/repo_info.py` & `slpkg-4.7.9/slpkg/repo_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,27 +41,26 @@
         print('=' * self.columns)
 
         for repo, value in self.repos.repositories.items():
             count: int = 0
             status: str = 'Disabled'
             color: str = self.red
 
-            if value[0]:
-                enabled += 1
-                status: str = 'Enabled'
-                color: str = self.green
-
             last: str = self.session.query(
                 LastRepoUpdated.date).where(
                 LastRepoUpdated.repo == repo).first()
 
             if last is None:
                 last: tuple = ('',)
 
             if value[0]:
+                enabled += 1
+                status: str = 'Enabled'
+                color: str = self.green
+
                 if repo in [self.repos.sbo_repo_name, self.repos.ponce_repo_name]:
                     count = self.session.query(SBoTable.id).count()
                 else:
                     count = self.session.query(BinariesTable).where(BinariesTable.repo == repo).count()
 
             total_packages += count
```

### Comparing `slpkg-4.7.8/slpkg/sbos/queries.py` & `slpkg-4.7.9/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/sbos/slackbuild.py` & `slpkg-4.7.9/slpkg/sbos/slackbuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,14 +401,13 @@
 
             choices += [(package, repo_ver, status, help_text)]
 
         text: str = f'There are {len(choices)} dependencies:'
 
         code, tags = self.dialogbox.checklist(text, dependencies, title, height,
                                               width, list_height, choices)
-
         if not code:
             return dependencies
 
         os.system('clear')
 
         return tags
```

### Comparing `slpkg-4.7.8/slpkg/sbos/dependencies.py` & `slpkg-4.7.9/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/form_configs.py` & `slpkg-4.7.9/slpkg/form_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/update_repository.py` & `slpkg-4.7.9/slpkg/update_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.color = self.colour()
         self.data = InstallData()
         self.check_updates = CheckUpdates(
             self.flags, self.repo
         )
 
         if not self.repo:
-            self.repo = self.repos.sbo_enabled_repository
+            self.repo = self.repos.sbo_enabled_repo_name
 
         self.repos_for_update: dict = {}
         self.bold: str = self.color['bold']
         self.green: str = self.color['green']
         self.red: str = self.color['red']
         self.yellow: str = self.color['yellow']
         self.bgreen: str = f'{self.bold}{self.green}'
@@ -93,507 +93,525 @@
                     bin_repositories[repo]()
         else:
             self.slackbuild_repositories()
         print()
 
     def slack_repository(self):
         if self.repos.slack_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.slack_repo_name}{self.endc}"
-                  f"' repository, please wait...\n")
-            self.make_dirs(self.repos.slack_repo_name)
 
-            urls.append(f'{self.repos.slack_repo_mirror}{self.repos.slack_repo_packages}')
-            urls.append(f'{self.repos.slack_repo_mirror}{self.repos.slack_repo_changelog}')
-            urls.append(f'{self.repos.slack_repo_mirror}{self.repos.slack_repo_checksums}')
+            if not self.repos.slack_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.slack_repo_name}{self.endc}"
+                      f"' repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.slack_repo_name)
+
+                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
+                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
+                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
+
+                down = Downloader(self.repos.slack_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
-
-            down = Downloader(self.repos.slack_repo_path, urls, self.flags)
-            down.download()
-            print()
-
-            self.delete_binaries_data(self.repos.slack_repo_name)
+            self.delete_bin_database_data(self.repos.slack_repo_name)
             self.delete_last_updated(self.repos.slack_repo_name)
             self.data.install_slack_data()
             print()
         else:
             self.not_enabled_message(self.repos.slack_repo_name)
 
     def slack_extra_repository(self):
         if self.repos.slack_extra_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.slack_extra_repo_name}{self.endc}"
-                  f"' repository, please wait...\n")
-            self.make_dirs(self.repos.slack_extra_repo_name)
-
-            urls.append(f'{self.repos.slack_extra_repo_packages_mirror}{self.repos.slack_extra_repo_packages}')
-            urls.append(f'{self.repos.slack_extra_repo_mirror}{self.repos.slack_extra_repo_changelog}')
-            urls.append(f'{self.repos.slack_extra_repo_mirror}{self.repos.slack_extra_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                             self.repos.slack_extra_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                             self.repos.slack_extra_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                             self.repos.slack_extra_repo_checksums)
 
-            down = Downloader(self.repos.slack_extra_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.slack_extra_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.slack_extra_repo_name}{self.endc}"
+                      f"' repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.slack_extra_repo_name)
+
+                urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
+                urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}')
+                urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
+                                                 self.repos.slack_extra_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
+                                                 self.repos.slack_extra_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
+                                                 self.repos.slack_extra_repo_checksums)
+
+                down = Downloader(self.repos.slack_extra_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.slack_extra_repo_name)
+            self.delete_bin_database_data(self.repos.slack_extra_repo_name)
             self.delete_last_updated(self.repos.slack_extra_repo_name)
             self.data.install_slack_extra_data()
             print()
         else:
             self.not_enabled_message(self.repos.slack_extra_repo_name)
 
     def slack_patches_repository(self):
         if self.repos.slack_patches_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.slack_patches_repo_name}{self.endc}"
-                  f"' repository, please wait...\n")
-            self.make_dirs(self.repos.slack_patches_repo_name)
-
-            urls.append(f'{self.repos.slack_patches_repo_packages_mirror}{self.repos.slack_patches_repo_packages}')
-            urls.append(f'{self.repos.slack_patches_repo_mirror}{self.repos.slack_patches_repo_changelog}')
-            urls.append(f'{self.repos.slack_patches_repo_mirror}{self.repos.slack_patches_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                             self.repos.slack_patches_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                             self.repos.slack_patches_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                             self.repos.slack_patches_repo_checksums)
 
-            down = Downloader(self.repos.slack_patches_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.slack_patches_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.slack_patches_repo_name}{self.endc}"
+                      f"' repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.slack_patches_repo_name)
+
+                urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
+                urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
+                urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                                 self.repos.slack_patches_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                                 self.repos.slack_patches_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                                 self.repos.slack_patches_repo_checksums)
+
+                down = Downloader(self.repos.slack_patches_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.slack_patches_repo_name)
+            self.delete_bin_database_data(self.repos.slack_patches_repo_name)
             self.delete_last_updated(self.repos.slack_patches_repo_name)
             self.data.install_slack_patches_data()
             print()
         else:
             self.not_enabled_message(self.repos.slack_patches_repo_name)
 
     def alien_repository(self):
         if self.repos.alien_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.alien_repo_name}{self.endc}' repository, please wait...\n")
-            self.make_dirs(self.repos.alien_repo_name)
-
-            urls.append(f'{self.repos.alien_repo_packages_mirror}{self.repos.alien_repo_packages}')
-            urls.append(f'{self.repos.alien_repo_mirror}{self.repos.alien_repo_changelog}')
-            urls.append(f'{self.repos.alien_repo_packages_mirror}{self.repos.alien_repo_checksums}')
 
-            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
+            if not self.repos.alien_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.alien_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.alien_repo_name)
+
+                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
+                urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
+                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
+
+                down = Downloader(self.repos.alien_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            down = Downloader(self.repos.alien_repo_path, urls, self.flags)
-            down.download()
-            print()
-
-            self.delete_binaries_data(self.repos.alien_repo_name)
+            self.delete_bin_database_data(self.repos.alien_repo_name)
             self.delete_last_updated(self.repos.alien_repo_name)
             self.data.install_alien_data()
             print()
         else:
             self.not_enabled_message(self.repos.alien_repo_name)
 
     def multilib_repository(self) -> None:
         if self.repos.multilib_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.multilib_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.multilib_repo_name)
-
-            urls.append(f'{self.repos.multilib_repo_packages_mirror}{self.repos.multilib_repo_packages}')
-            urls.append(f'{self.repos.multilib_repo_mirror}{self.repos.multilib_repo_changelog}')
-            urls.append(f'{self.repos.multilib_repo_mirror}{self.repos.multilib_repo_checksums}')
 
-            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
-
-            down = Downloader(self.repos.multilib_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.multilib_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.multilib_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.multilib_repo_name)
+
+                urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
+                urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
+                urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
+
+                down = Downloader(self.repos.multilib_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.multilib_repo_name)
+            self.delete_bin_database_data(self.repos.multilib_repo_name)
             self.delete_last_updated(self.repos.multilib_repo_name)
             self.data.install_multilib_data()
             print()
         else:
             self.not_enabled_message(self.repos.multilib_repo_name)
 
     def restricted_repository(self) -> None:
         if self.repos.restricted_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.restricted_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.restricted_repo_name)
 
-            urls.append(f'{self.repos.restricted_repo_packages_mirror}{self.repos.restricted_repo_packages}')
-            urls.append(f'{self.repos.restricted_repo_mirror}{self.repos.restricted_repo_changelog}')
-            urls.append(f'{self.repos.restricted_repo_packages_mirror}{self.repos.restricted_repo_checksums}')
+            if not self.repos.restricted_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.restricted_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.restricted_repo_name)
+
+                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
+                urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
+                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
+
+                down = Downloader(self.repos.restricted_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
-
-            down = Downloader(self.repos.restricted_repo_path, urls, self.flags)
-            down.download()
-            print()
-
-            self.delete_binaries_data(self.repos.restricted_repo_name)
+            self.delete_bin_database_data(self.repos.restricted_repo_name)
             self.delete_last_updated(self.repos.restricted_repo_name)
             self.data.install_restricted_data()
             print()
         else:
             self.not_enabled_message(self.repos.restricted_repo_name)
 
     def gnome_repository(self) -> None:
         if self.repos.gnome_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.gnome_repo_name}{self.endc}' repository, please wait...\n")
-            self.make_dirs(self.repos.gnome_repo_name)
-
-            urls.append(f'{self.repos.gnome_repo_mirror}{self.repos.gnome_repo_packages}')
-            urls.append(f'{self.repos.gnome_repo_mirror}{self.repos.gnome_repo_changelog}')
-            urls.append(f'{self.repos.gnome_repo_mirror}{self.repos.gnome_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
 
-            down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.gnome_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.gnome_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.gnome_repo_name)
+
+                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
+                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
+                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
+
+                down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.gnome_repo_name)
+            self.delete_bin_database_data(self.repos.gnome_repo_name)
             self.delete_last_updated(self.repos.gnome_repo_name)
             self.data.install_gnome_data()
             print()
         else:
             self.not_enabled_message(self.repos.gnome_repo_name)
 
     def msb_repository(self) -> None:
         if self.repos.msb_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.msb_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.msb_repo_name)
-
-            urls.append(f'{self.repos.msb_repo_packages_mirror}{self.repos.msb_repo_packages}')
-            urls.append(f'{self.repos.msb_repo_mirror}{self.repos.msb_repo_changelog}')
-            urls.append(f'{self.repos.msb_repo_mirror}{self.repos.msb_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                             self.repos.msb_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                             self.repos.msb_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                             self.repos.msb_repo_checksums)
 
-            down = Downloader(self.repos.msb_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.msb_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.msb_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.msb_repo_name)
+
+                urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
+                urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}')
+                urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.msb_repo_path,
+                                                 self.repos.msb_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.msb_repo_path,
+                                                 self.repos.msb_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.msb_repo_path,
+                                                 self.repos.msb_repo_checksums)
+
+                down = Downloader(self.repos.msb_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.msb_repo_name)
+            self.delete_bin_database_data(self.repos.msb_repo_name)
             self.delete_last_updated(self.repos.msb_repo_name)
             self.data.install_msb_data()
             print()
         else:
             self.not_enabled_message(self.repos.msb_repo_name)
 
     def csb_repository(self) -> None:
         if self.repos.csb_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.csb_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.csb_repo_name)
-
-            urls.append(f'{self.repos.csb_repo_packages_mirror}{self.repos.csb_repo_packages}')
-            urls.append(f'{self.repos.csb_repo_mirror}{self.repos.csb_repo_changelog}')
-            urls.append(f'{self.repos.csb_repo_mirror}{self.repos.csb_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                             self.repos.csb_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                             self.repos.csb_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                             self.repos.csb_repo_checksums)
 
-            down = Downloader(self.repos.csb_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.csb_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.csb_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.csb_repo_name)
+
+                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
+                urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_changelog}')
+                urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.csb_repo_path,
+                                                 self.repos.csb_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.csb_repo_path,
+                                                 self.repos.csb_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.csb_repo_path,
+                                                 self.repos.csb_repo_checksums)
+
+                down = Downloader(self.repos.csb_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.csb_repo_name)
+            self.delete_bin_database_data(self.repos.csb_repo_name)
             self.delete_last_updated(self.repos.csb_repo_name)
             self.data.install_csb_data()
             print()
         else:
             self.not_enabled_message(self.repos.csb_repo_name)
 
     def conraid_repository(self) -> None:
         if self.repos.conraid_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.conraid_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.conraid_repo_name)
-
-            urls.append(f'{self.repos.conraid_repo_mirror}{self.repos.conraid_repo_packages}')
-            urls.append(f'{self.repos.conraid_repo_mirror}{self.repos.conraid_repo_changelog}')
-            urls.append(f'{self.repos.conraid_repo_mirror}{self.repos.conraid_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
 
-            down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.conraid_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.conraid_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.conraid_repo_name)
+
+                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
+                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
+                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
+
+                down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.conraid_repo_name)
+            self.delete_bin_database_data(self.repos.conraid_repo_name)
             self.delete_last_updated(self.repos.conraid_repo_name)
             self.data.install_conraid_data()
             print()
         else:
             self.not_enabled_message(self.repos.conraid_repo_name)
 
     def slackonly_repository(self) -> None:
         if self.repos.slackonly_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.slackonly_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.slackonly_repo_name)
-
-            urls.append(f'{self.repos.slackonly_repo_mirror}{self.repos.slackonly_repo_packages}')
-            urls.append(f'{self.repos.slackonly_repo_mirror}{self.repos.slackonly_repo_changelog}')
-            urls.append(f'{self.repos.slackonly_repo_mirror}{self.repos.slackonly_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
 
-            down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.slackonly_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.slackonly_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.slackonly_repo_name)
+
+                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
+                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
+                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
+
+                down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.slackonly_repo_name)
+            self.delete_bin_database_data(self.repos.slackonly_repo_name)
             self.delete_last_updated(self.repos.slackonly_repo_name)
             self.data.install_slackonly_data()
             print()
         else:
             self.not_enabled_message(self.repos.slackonly_repo_name)
 
     def salixos_repository(self) -> None:
         if self.repos.salixos_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.salixos_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.salixos_repo_name)
-
-            urls.append(f'{self.repos.salixos_repo_mirror}{self.repos.salixos_repo_packages}')
-            urls.append(f'{self.repos.salixos_repo_mirror}{self.repos.salixos_repo_changelog}')
-            urls.append(f'{self.repos.salixos_repo_mirror}{self.repos.salixos_repo_checksums}')
 
-            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
+            if not self.repos.salixos_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.salixos_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.salixos_repo_name)
+
+                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
+                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
+                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
+
+                down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
-            down.download()
-            print()
-
-            self.delete_binaries_data(self.repos.salixos_repo_name)
+            self.delete_bin_database_data(self.repos.salixos_repo_name)
             self.delete_last_updated(self.repos.salixos_repo_name)
             self.data.install_salixos_data()
             print()
         else:
             self.not_enabled_message(self.repos.salixos_repo_name)
 
     def salixos_extra_repository(self) -> None:
         if self.repos.salixos_extra_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.salixos_extra_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.salixos_extra_repo_name)
-
-            urls.append(f'{self.repos.salixos_extra_repo_packages_mirror}{self.repos.salixos_extra_repo_packages}')
-            urls.append(f'{self.repos.salixos_extra_repo_mirror}{self.repos.salixos_extra_repo_changelog}')
-            urls.append(f'{self.repos.salixos_extra_repo_mirror}{self.repos.salixos_extra_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                             self.repos.salixos_extra_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                             self.repos.salixos_extra_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                             self.repos.salixos_extra_repo_checksums)
 
-            down = Downloader(self.repos.salixos_extra_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.salixos_extra_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.salixos_extra_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.salixos_extra_repo_name)
+
+                urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
+                urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
+                urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                                 self.repos.salixos_extra_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                                 self.repos.salixos_extra_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                                 self.repos.salixos_extra_repo_checksums)
+
+                down = Downloader(self.repos.salixos_extra_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.salixos_extra_repo_name)
+            self.delete_bin_database_data(self.repos.salixos_extra_repo_name)
             self.delete_last_updated(self.repos.salixos_extra_repo_name)
             self.data.install_salixos_extra_data()
             print()
         else:
             self.not_enabled_message(self.repos.salixos_extra_repo_name)
 
     def salixos_patches_repository(self) -> None:
         if self.repos.salixos_patches_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.salixos_patches_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.salixos_patches_repo_name)
-
-            urls.append(f'{self.repos.salixos_patches_repo_packages_mirror}{self.repos.salixos_patches_repo_packages}')
-            urls.append(f'{self.repos.salixos_patches_repo_mirror}{self.repos.salixos_patches_repo_changelog}')
-            urls.append(f'{self.repos.salixos_patches_repo_mirror}{self.repos.salixos_patches_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                             self.repos.salixos_patches_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                             self.repos.salixos_patches_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                             self.repos.salixos_patches_repo_checksums)
 
-            down = Downloader(self.repos.salixos_patches_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if not self.repos.salixos_patches_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.salixos_patches_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.salixos_patches_repo_name)
+
+                urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
+                            f'{self.repos.salixos_patches_repo_packages}')
+                urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
+                urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                                 self.repos.salixos_patches_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                                 self.repos.salixos_patches_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                                 self.repos.salixos_patches_repo_checksums)
+
+                down = Downloader(self.repos.salixos_patches_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.delete_binaries_data(self.repos.salixos_patches_repo_name)
+            self.delete_bin_database_data(self.repos.salixos_patches_repo_name)
             self.delete_last_updated(self.repos.salixos_patches_repo_name)
             self.data.install_salixos_patches_data()
             print()
         else:
             self.not_enabled_message(self.repos.salixos_patches_repo_name)
 
     def slackel_repository(self) -> None:
         if self.repos.slackel_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.slackel_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.slackel_repo_name)
 
-            urls.append(f'{self.repos.slackel_repo_mirror}{self.repos.slackel_repo_packages}')
-            urls.append(f'{self.repos.slackel_repo_mirror}{self.repos.slackel_repo_changelog}')
-            urls.append(f'{self.repos.slackel_repo_mirror}{self.repos.slackel_repo_checksums}')
+            if not self.repos.slackel_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.slackel_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.slackel_repo_name)
+
+                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
+                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
+                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
+
+                down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
-
-            down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
-            down.download()
-            print()
-
-            self.delete_binaries_data(self.repos.slackel_repo_name)
+            self.delete_bin_database_data(self.repos.slackel_repo_name)
             self.delete_last_updated(self.repos.slackel_repo_name)
             self.data.install_slackel_data()
             print()
         else:
             self.not_enabled_message(self.repos.slackel_repo_name)
 
     def slint_repository(self) -> None:
         if self.repos.slint_repo:
-            urls: list = []
-            print('Updating the packages list...\n')
-            print(f"Downloading the '{self.green}{self.repos.slint_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
-            self.make_dirs(self.repos.slint_repo_name)
-
-            urls.append(f'{self.repos.slint_repo_mirror}{self.repos.slint_repo_packages}')
-            urls.append(f'{self.repos.slint_repo_mirror}{self.repos.slint_repo_changelog}')
-            urls.append(f'{self.repos.slint_repo_mirror}{self.repos.slint_repo_checksums}')
 
-            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
+            if not self.repos.slint_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.slint_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                urls: list = []
+                self.make_dirs(self.repos.slint_repo_name)
+
+                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
+                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
+                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
+
+                self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
+                self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
+                self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
+
+                down = Downloader(self.repos.slint_repo_path, urls, self.flags)
+                down.download()
+                print()
 
-            down = Downloader(self.repos.slint_repo_path, urls, self.flags)
-            down.download()
-            print()
-
-            self.delete_binaries_data(self.repos.slint_repo_name)
+            self.delete_bin_database_data(self.repos.slint_repo_name)
             self.delete_last_updated(self.repos.slint_repo_name)
             self.data.install_slint_data()
             print()
         else:
             self.not_enabled_message(self.repos.slint_repo_name)
 
     def slackbuild_repositories(self) -> None:
         """ Update the slackbuild repositories. """
         if self.repos.ponce_repo:
-            self.make_dirs(self.repos.gnome_repo_name)
-            if not self.utils.is_option(self.flag_generate, self.flags):
-                print('Updating the packages list...\n')
+
+            if (not self.utils.is_option(self.flag_generate, self.flags) or
+                    not self.repos.ponce_repo_mirror[0].startswith('file')):
                 print(f"Downloading the '{self.green}{self.repos.ponce_repo_name}"
                       f"{self.endc}' repository, please wait...\n")
+                self.make_dirs(self.repos.gnome_repo_name)
                 self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
-                lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.ponce_repo_mirror} '
+                lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.ponce_repo_mirror[0]} '
                                      f'{self.repos.ponce_repo_path}')
                 self.utils.process(lftp_command)
 
-            # Remove the SLACKBUILDS.TXT file before generating the new one.
-            sbo_file_txt = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
-            if sbo_file_txt.is_file():
-                sbo_file_txt.unlink()
-
-            # Generating the ponce SLACKBUILDS.TXT file.
-            print(f'Generating the {self.repos.ponce_repo_slackbuilds} file... ', end='', flush=True)
-            os.chdir(self.repos.ponce_repo_path)
-            gen_command: str = f'./gen_sbo_txt.sh > {self.repos.ponce_repo_slackbuilds}'
-            self.utils.process(gen_command)
-            self.delete_last_updated(self.repos.ponce_repo_name)
-            print('\n')
-
-        else:
-            self.make_dirs(self.repos.sbo_repo_name)
-            print('Updating the packages list...\n')
-
-            self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
-            self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
-
-            print(f"Downloading the '{self.green}{self.repos.sbo_repo_name}{self.endc}' repository, please wait...\n")
-            lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.sbo_repo_mirror} '
-                                 f'{self.repos.sbo_repo_path}')
-            self.utils.process(lftp_command)
+            gen_script: Path = Path(self.repos.ponce_repo_path, 'gen_sbo_txt.sh')
+            if gen_script.is_file():
+                # Generating the ponce SLACKBUILDS.TXT file.
+                print(f'Generating the {self.repos.ponce_repo_slackbuilds} file... ', end='', flush=True)
+                os.chdir(self.repos.ponce_repo_path)
+                gen_command: str = f'./gen_sbo_txt.sh > {self.repos.ponce_repo_slackbuilds}'
+                self.utils.process(gen_command)
+                self.delete_last_updated(self.repos.ponce_repo_name)
+                print('\n')
+
+        else:
+
+            if not self.repos.sbo_repo_mirror[0].startswith('file'):
+                print(f"Downloading the '{self.green}{self.repos.sbo_repo_name}{self.endc}' "
+                      f"repository, please wait...\n")
+                self.make_dirs(self.repos.sbo_repo_name)
+                self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
+                self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
+                lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.sbo_repo_mirror[0]} '
+                                     f'{self.repos.sbo_repo_path}')
+                self.utils.process(lftp_command)
+
             self.delete_last_updated(self.repos.sbo_repo_name)
 
-        self.delete_sbo_data()
+        self.delete_sbo_database_data()
         self.data.install_sbos_data()
 
     def not_enabled_message(self, repo: str) -> None:
         print(f"{self.prog_name}: Repository '{self.green}{repo}{self.endc}' is not enabled.")
 
     def make_dirs(self, repo) -> None:
-        path = Path(self.lib_path, 'repositories', repo)
+        path = Path(self.repos.repositories_path, repo)
         if not os.path.isdir(path):
             os.makedirs(path)
 
     def check(self, queue) -> None:
         compare = self.check_updates.check()
         is_update: dict = {}
 
@@ -633,23 +651,23 @@
 
         # Restore the terminal cursor
         print('\x1b[?25h', self.endc, end='')
 
         self.repos_for_update = queue.get()
         self.update_the_repositories()
 
-    def delete_sbo_data(self) -> None:
+    def delete_sbo_database_data(self) -> None:
         """ Delete all the data from a table of the database. """
         if self.repos.ponce_repo:
             self.session.query(PonceTable).delete()
         else:
             self.session.query(SBoTable).delete()
         self.session.commit()
 
-    def delete_binaries_data(self, repo) -> None:
+    def delete_bin_database_data(self, repo) -> None:
         """ Delete the repository data from a table of the database. """
         self.session.query(BinariesTable).where(BinariesTable.repo == repo).delete()
         self.session.commit()
 
     def delete_last_updated(self, repo) -> None:
         """ Deletes the last updated date. """
         self.session.query(LastRepoUpdated).where(LastRepoUpdated.repo == repo).delete()
```

### Comparing `slpkg-4.7.8/slpkg/progress_bar.py` & `slpkg-4.7.9/slpkg/progress_bar.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/downloader.py` & `slpkg-4.7.9/slpkg/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+import shutil
 from typing import Union
 from pathlib import Path
 from urllib.parse import unquote
 from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
@@ -41,25 +42,28 @@
                 self.tools(url)
 
     def tools(self, url: str) -> None:
         """ Downloader tools wget, curl and lftp. """
         command: str = ''
         filename: str = url.split('/')[-1]
 
-        if self.downloader in ['wget', 'wget2']:
-            command: str = f'{self.downloader} {self.wget_options} --directory-prefix={self.path} "{url}"'
+        if url.startswith('file'):
+            shutil.copy2(url[7:], self.tmp_slpkg)
+        else:
+            if self.downloader in ['wget', 'wget2']:
+                command: str = f'{self.downloader} {self.wget_options} --directory-prefix={self.path} "{url}"'
 
-        elif self.downloader == 'curl':
-            command: str = f'{self.downloader} {self.curl_options} "{url}" --output {self.path}/{filename}'
+            elif self.downloader == 'curl':
+                command: str = f'{self.downloader} {self.curl_options} "{url}" --output {self.path}/{filename}'
 
-        elif self.downloader == 'lftp':
-            command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
+            elif self.downloader == 'lftp':
+                command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
 
-        else:
-            self.utils.raise_error_message(f"Downloader '{self.downloader}' not supported")
+            else:
+                self.utils.raise_error_message(f"Downloader '{self.downloader}' not supported")
 
         self.utils.process(command)
         self.check_if_downloaded(url)
 
     def check_if_downloaded(self, url: str) -> None:
         """ Checks if the file downloaded. """
         url: str = unquote(url)
```

### Comparing `slpkg-4.7.8/slpkg/models/models.py` & `slpkg-4.7.9/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/views/view_package.py` & `slpkg-4.7.9/slpkg/views/view_package.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.cyan: str = self.color['cyan']
         self.red: str = self.color['red']
         self.violet: str = self.color['violet']
         self.endc: str = self.color['endc']
 
         # Switch between sbo and ponce repository.
         self.sbo_table = SBoTable
-        self.repo_url: str = self.repos.sbo_repo_mirror
+        self.repo_url: str = self.repos.sbo_repo_mirror[0]
         self.repo_path: Path = self.repos.sbo_repo_path
         self.repo_tar_suffix: str = self.repos.sbo_repo_tar_suffix
         if self.repos.ponce_repo:
             self.sbo_table = PonceTable
             self.repo_url: str = self.repos.ponce_repo_mirror
             self.repo_path: Path = self.repos.ponce_repo_path
             self.repo_tar_suffix: str = ''
```

### Comparing `slpkg-4.7.8/slpkg/views/version.py` & `slpkg-4.7.9/slpkg/views/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 7, 8)
+        self.version_info: tuple = (4, 7, 9)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.7.8/slpkg/views/cli_menu.py` & `slpkg-4.7.9/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/views/ascii.py` & `slpkg-4.7.9/slpkg/views/ascii.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/views/help_commands.py` & `slpkg-4.7.9/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/views/views.py` & `slpkg-4.7.9/slpkg/views/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
+import re
 from typing import Any
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
@@ -13,26 +14,25 @@
 from slpkg.repositories import Repositories
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class ViewMessage(Configs):
 
-    def __init__(self, flags: list, data=None, repo=None):
-        __slots__ = 'flags', 'data', 'repo'
+    def __init__(self, flags: list, data=None):
+        __slots__ = 'flags', 'data'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.data: dict = data
-        self.repo: str = repo
 
         self.session = Session
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.ascii = Ascii()
-        self.upgrade = Upgrade(self.flags, self.data, self.repo)
+        self.upgrade = Upgrade(self.flags, self.data)
         self.color = self.colour()
         self.repos = Repositories()
 
         self.yellow: str = self.color['yellow']
         self.cyan: str = self.color['cyan']
         self.red: str = self.color['red']
         self.grey: str = self.color['grey']
@@ -49,26 +49,28 @@
 
         self.option_for_yes: bool = self.utils.is_option(
             ['-y', '--yes'], self.flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
 
+        self.repo: str = self.utils.repository_name(self.data)
+
     def view_packages(self, package: str, mode: str) -> None:
         """ Printing the main packages. """
         size: str = ''
         color: str = self.red
 
         if self.option_for_binaries:
             version: str = self.data[package][0]
-            size: str = self.data[package][4]
-            repo: str = self.repo
+            size: str = self.utils.convert_file_sizes(
+                int(''.join(re.findall(r'\d+', self.data[package][4])))
+            )
         else:
             version: str = self.data[package][2]
-            repo: str = self.repos.sbo_enabled_repository
 
         if mode in ['install', 'download']:
             color: str = self.cyan
         if mode == 'build':
             color: str = self.yellow
         if mode == 'upgrade':
             color: str = self.violet
@@ -80,15 +82,15 @@
         if self.upgrade.is_package_upgradeable(package) and mode == 'install':
             color: str = self.violet
 
         if (package in self.utils.installed_packages.keys() and mode == 'install'
                 and self.option_for_reinstall):
             color: str = self.violet
 
-        self.ascii.draw_view_package(package, version, size, color, repo)
+        self.ascii.draw_view_package(package, version, size, color, self.repo)
 
     def view_skipping_packages(self, package: str, version: str) -> None:
         """ Print the skipping packages. """
         print(f'[{self.yellow}Skipping{self.endc}] {package}-{version} {self.red}(already installed){self.endc}')
 
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
         """ View packages for build only. """
@@ -183,15 +185,15 @@
         """ View and creates list with packages for remove. """
         installed = self.utils.is_package_installed(name)
 
         if installed:
             pkg: list = self.utils.split_binary_pkg(installed)
             self.installed_packages.append(installed)
             size: str = self.utils.get_file_size(Path(self.log_packages, installed))
-            self.ascii.draw_view_package(pkg[0], pkg[1], size, self.red, '')
+            self.ascii.draw_view_package(pkg[0], pkg[1], size, self.red, repo='')
 
     def choose_dependencies_for_remove(self, dependencies: list) -> list:
         """ Choose packages for remove using the dialog box. """
         height: int = 10
         width: int = 70
         list_height: int = 0
         choices: list = []
```

### Comparing `slpkg-4.7.8/slpkg/checks.py` & `slpkg-4.7.9/slpkg/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from slpkg.models.models import SBoTable, PonceTable, BinariesTable
 
 
 class Check(Configs):
     """ Some checks before proceed. """
 
     def __init__(self, flags: list, data: dict):
-        __slots__ = 'flags', 'sbo_repo_dict', 'bin_repo_dict'
+        __slots__ = 'flags', 'data'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.data: dict = data
 
         self.utils = Utilities()
         self.repos = Repositories()
```

### Comparing `slpkg-4.7.8/slpkg/checksum.py` & `slpkg-4.7.9/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/dialog_box.py` & `slpkg-4.7.9/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/configs.py` & `slpkg-4.7.9/slpkg/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,16 +73,15 @@
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     file_pattern: str = '*'
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
 
-    http_proxy_address: str = ''
-    socks_proxy_address: str = ''
+    proxy_address: str = ''
     proxy_username: str = ''
     proxy_password: str = ''
 
     load = Load()
     configs = load.config_file(etc_path, prog_name)
 
     if configs:
@@ -105,16 +104,15 @@
             silent_mode: bool = config['SILENT_MODE']
             ascii_characters: bool = config['ASCII_CHARACTERS']
             file_list_suffix: str = config['FILE_LIST_SUFFIX']
             parallel_downloads: bool = config['PARALLEL_DOWNLOADS']
             file_pattern_conf: str = config['FILE_PATTERN']
             progress_spinner: str = config['PROGRESS_SPINNER']
             spinner_color: str = config['SPINNER_COLOR']
-            http_proxy_address: str = config['HTTP_PROXY_ADDRESS']
-            socks_proxy_address: str = config['SOCKS_PROXY_ADDRESS']
+            proxy_address: str = config['PROXY_ADDRESS']
             proxy_username: str = config['PROXY_USERNAME']
             proxy_password: str = config['PROXY_PASSWORD']
 
         except KeyError as error:
             raise SystemExit(f"\n{prog_name}: {color['bold']}{color['red']}Error{color['endc']}: "
                              f"{error}: in the configuration file '/etc/slpkg/slpkg.toml'.\n"
                              f"\nIf you have upgraded the '{prog_name}' probably you need to run:\n"
```

### Comparing `slpkg-4.7.8/slpkg/clean_logs.py` & `slpkg-4.7.9/slpkg/clean_logs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/utilities.py` & `slpkg-4.7.9/slpkg/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,31 +158,28 @@
         if output != 0:
             raise SystemExit(output)
 
     def raise_error_message(self, message: str) -> None:
         """ A general method to raise an error message and exit. """
         raise SystemExit(f"\n{self.configs.prog_name}: {self.bred}Error{self.endc}: {message}.\n")
 
-    @staticmethod
-    def get_file_size(file: Path) -> str:
-        """ Get the file size and converted to units. """
-        unit: str = 'KB'
-        file_size = Path(file).stat().st_size
-        mb = file_size / 1024 ** 2
-        gb = file_size / 1024 ** 3
-
-        if mb >= 0.1:
-            file_size = mb
-            unit: str = 'MB'
-
-        if gb >= 0.1:
-            file_size = mb
-            unit: str = 'GB'
+    def get_file_size(self, file: Path) -> str:
+        """ Get the local file size and converted to units. """
+        size = Path(file).stat().st_size
+        return self.convert_file_sizes(size)
 
-        return f'{str(round(file_size, 2))} {unit}'
+    @staticmethod
+    def convert_file_sizes(size: int) -> str:
+        """ Convert file sizes. """
+        units: list = ['KB', 'MB', 'GB']
+
+        for unit in units:
+            if size < 1000:
+                return f'{size:.0f} {unit}'
+            size /= 1000
 
     @staticmethod
     def apply_package_pattern(data: dict, packages: list) -> list:
         """ Apply the pattern. """
         for pkg in packages:
 
             if pkg == '*':
@@ -191,7 +188,18 @@
 
         return packages
 
     def blacklist_pattern(self, name):
         """ This module provides support for Unix shell-style wildcards. """
         if [black for black in self.black.packages() if fnmatch.fnmatch(name, black)]:
             return True
+
+    def repository_name(self, data):
+        """ Get the binary repository name from the repository data. """
+        try:
+            # Binary repository name
+            repo: list = list(data.values())[0][11]
+        except (IndexError, AttributeError):
+            # Slackbuilds repository name 'sbo | ponce'
+            repo: str = self.repos.sbo_enabled_repo_name
+
+        return repo
```

### Comparing `slpkg-4.7.8/slpkg/dependees.py` & `slpkg-4.7.9/slpkg/dependees.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/check_updates.py` & `slpkg-4.7.9/slpkg/check_updates.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository
         }
 
         if self.option_for_binaries:
 
             for repo in bin_repositories.keys():
+
                 if repo in self.repos.bin_enabled_repos and repo == self.repo:
                     bin_repositories[repo]()
                     break
 
                 if repo in self.repos.bin_enabled_repos and self.repo == '*':
                     bin_repositories[repo]()
         else:
@@ -73,119 +74,124 @@
             else:
                 self.sbo_repository()
 
         return self.compare
 
     def slack_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.slack_repo_mirror}{self.repos.slack_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}'
         self.compare[self.repos.slack_repo_name] = self.compare_dates()
 
     def slack_extra_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.slack_extra_repo_mirror}{self.repos.slack_extra_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}'
         self.compare[self.repos.slack_extra_repo_name] = self.compare_dates()
 
     def slack_patches_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.slack_patches_repo_path, self.repos.slack_patches_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.slack_patches_repo_mirror}{self.repos.slack_patches_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}'
         self.compare[self.repos.slack_patches_repo_name] = self.compare_dates()
 
     def alien_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.alien_repo_mirror}{self.repos.alien_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}'
         self.compare[self.repos.alien_repo_name] = self.compare_dates()
 
     def multilib_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.multilib_repo_mirror}{self.repos.multilib_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}'
         self.compare[self.repos.multilib_repo_name] = self.compare_dates()
 
     def restricted_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.restricted_repo_mirror}{self.repos.restricted_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}'
         self.compare[self.repos.restricted_repo_name] = self.compare_dates()
 
     def gnome_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.gnome_repo_mirror}{self.repos.gnome_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}'
         self.compare[self.repos.gnome_repo_name] = self.compare_dates()
 
     def msb_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.msb_repo_path, self.repos.msb_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.msb_repo_mirror}{self.repos.msb_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}'
         self.compare[self.repos.msb_repo_name] = self.compare_dates()
 
     def csb_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.csb_repo_path, self.repos.csb_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.csb_repo_mirror}{self.repos.csb_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_changelog}'
         self.compare[self.repos.csb_repo_name] = self.compare_dates()
 
     def conraid_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.conraid_repo_mirror}{self.repos.conraid_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}'
         self.compare[self.repos.conraid_repo_name] = self.compare_dates()
 
     def slackonly_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.slackonly_repo_mirror}{self.repos.slackonly_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}'
         self.compare[self.repos.slackonly_repo_name] = self.compare_dates()
 
     def salixos_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.salixos_repo_mirror}{self.repos.salixos_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}'
         self.compare[self.repos.salixos_repo_name] = self.compare_dates()
 
     def salixos_extra_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.salixos_extra_repo_path, self.repos.salixos_extra_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.salixos_extra_repo_mirror}{self.repos.salixos_extra_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}'
         self.compare[self.repos.salixos_extra_repo_name] = self.compare_dates()
 
     def salixos_patches_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.salixos_patches_repo_path, self.repos.salixos_patches_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.salixos_patches_repo_mirror}{self.repos.salixos_patches_repo_changelog}'
+        self.repo_chg_txt: str = (f'{self.repos.salixos_patches_repo_mirror[0]}'
+                                  f'{self.repos.salixos_patches_repo_changelog}')
         self.compare[self.repos.salixos_patches_repo_name] = self.compare_dates()
 
     def slackel_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.slackel_repo_mirror}{self.repos.slackel_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}'
         self.compare[self.repos.slackel_repo_name] = self.compare_dates()
 
     def slint_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.slint_repo_mirror}{self.repos.slint_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}'
         self.compare[self.repos.slint_repo_name] = self.compare_dates()
 
     def sbo_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.sbo_repo_mirror}{self.repos.sbo_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.sbo_repo_mirror[0]}{self.repos.sbo_repo_changelog}'
         self.compare[self.repos.sbo_repo_name] = self.compare_dates()
 
     def ponce_repository(self) -> None:
         self.local_chg_txt: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
-        self.repo_chg_txt: str = f'{self.repos.ponce_repo_mirror}{self.repos.ponce_repo_changelog}'
+        self.repo_chg_txt: str = f'{self.repos.ponce_repo_mirror[0]}{self.repos.ponce_repo_changelog}'
         self.compare[self.repos.ponce_repo_name] = self.compare_dates()
 
     def compare_dates(self) -> bool:
         local_date: int = 0
+
+        if self.repo_chg_txt.startswith('file'):
+            return False
+
         try:
             http = PoolManager()
             proxy_default_headers = make_headers(proxy_basic_auth=f'{self.proxy_username}:{self.proxy_password}')
 
-            if self.http_proxy_address:
-                http = ProxyManager(f'{self.http_proxy_address}', headers=proxy_default_headers)
+            if self.proxy_address.startswith('http'):
+                http = ProxyManager(f'{self.proxy_address}', headers=proxy_default_headers)
 
-            elif self.socks_proxy_address:
+            elif self.proxy_address.startswith('socks'):
                 # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
                 try:  # Try to import PySocks if it's installed.
                     from urllib3.contrib.socks import SOCKSProxyManager
                 except (ModuleNotFoundError, ImportError):
                     raise SystemExit()
 
-                http = SOCKSProxyManager(f'{self.socks_proxy_address}', headers=proxy_default_headers)
+                http = SOCKSProxyManager(f'{self.proxy_address}', headers=proxy_default_headers)
 
             repo = http.request('GET', self.repo_chg_txt)
         except KeyboardInterrupt:
             raise SystemExit(1)
 
         if self.local_chg_txt.is_file():
             local_date = int(os.stat(self.local_chg_txt).st_size)
```

### Comparing `slpkg-4.7.8/slpkg/remove_packages.py` & `slpkg-4.7.9/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/blacklist.py` & `slpkg-4.7.9/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/download_only.py` & `slpkg-4.7.9/slpkg/download_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 
         self.option_for_directory: bool = self.utils.is_option(
             ['-z', '--directory='], self.flags)
 
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
 
-    def packages(self, data: dict, packages: list, repo=None) -> None:
+    def packages(self, data: dict, packages: list) -> None:
         """ Download the package only. """
         packages: list = self.utils.apply_package_pattern(data, packages)
 
-        view = ViewMessage(self.flags, data, repo)
+        view = ViewMessage(self.flags, data)
         view.download_packages(packages, self.directory)
         view.question()
 
         download_path: Path = self.download_only_path
         if self.option_for_directory:
             download_path: Path = self.directory
 
@@ -63,14 +63,14 @@
                 urls += sources
 
                 if self.repos.ponce_repo:
                     ponce_repo_path_package = Path(self.repos.ponce_repo_path, location, pkg)
                     shutil.copytree(ponce_repo_path_package, Path(download_path, pkg))
                 else:
                     file: str = f'{pkg}{self.repos.sbo_repo_tar_suffix}'
-                    urls += [f'{self.repos.sbo_repo_mirror}{location}/{file}']
+                    urls += [f'{self.repos.sbo_repo_mirror[0]}{location}/{file}']
 
         down = Downloader(download_path, urls, self.flags)
         down.download()
 
         elapsed_time: float = time.time() - start
         self.utils.finished_time(elapsed_time)
```

### Comparing `slpkg-4.7.8/slpkg/tracking.py` & `slpkg-4.7.9/slpkg/tracking.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/main.py` & `slpkg-4.7.9/slpkg/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,32 +477,33 @@
                             try:
                                 repo_ver: str = self.data[pkg][0]
                             except KeyError:
                                 repo_ver: str = ''
                             repo: str = self.binary_repo
                         else:
                             repo_ver: str = self.data[package][2]
-                            repo: str = self.repos.sbo_enabled_repository
+                            repo: str = self.repos.sbo_enabled_repo_name
                         choices += [(package, repo_ver, False, f'Package: {package}-{repo_ver} '
                                                                f'> {repo}')]
 
         if not choices:
             return packages
 
         text: str = f'There are {len(choices)} packages:'
         code, tags = self.dialogbox.checklist(text, packages, title, height,
                                               width, list_height, choices)
-        os.system('clear')
-
         if code == 'cancel':
+            os.system('clear')
             raise SystemExit()
 
-        if not tags:
+        if not tags or not code:
             return packages
 
+        os.system('clear')
+
         return list(set(tags))
 
     def help(self) -> None:
         if len(self.args) == 1:
             self.usage.help(0)
         self.usage.help_short(1)
 
@@ -522,25 +523,25 @@
 
     def upgrade(self) -> None:
         command = Argparse.upgrade.__name__
 
         if len(self.args) == 1:
             self.check.is_empty_database()
 
-            upgrade = Upgrade(self.flags, self.data, self.binary_repo)
+            upgrade = Upgrade(self.flags, self.data)
             packages: list = list(upgrade.packages())
 
             packages: list = self.choose_packages(packages, command)
 
             if not packages:
                 print('\nEverything is up-to-date!\n')
                 raise SystemExit()
 
             if self.utils.is_option(self.flag_binaries, self.flags):
-                install = Packages(self.data, packages, self.flags, self.binary_repo, mode=command)
+                install = Packages(self.data, packages, self.flags, mode=command)
                 install.execute()
             else:
                 install = Slackbuilds(self.data, packages, self.flags, mode=command)
                 install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
@@ -626,15 +627,15 @@
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             if self.utils.is_option(self.flag_binaries, self.flags):
                 self.check.exists_in_the_database(packages)
 
-                install = Packages(self.data, packages, self.flags, self.binary_repo, mode=command)
+                install = Packages(self.data, packages, self.flags, mode=command)
                 install.execute()
             else:
                 self.check.exists_in_the_database(packages)
                 self.check.is_package_unsupported(packages)
 
                 install = Slackbuilds(self.data, packages, self.flags, mode=command)
                 install.execute()
@@ -650,15 +651,15 @@
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
             self.check.exists_in_the_database(packages)
             download = Download(self.directory, self.flags)
-            download.packages(self.data, packages, self.binary_repo)
+            download.packages(self.data, packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def remove(self) -> None:
         command = Argparse.remove.__name__
 
         if len(self.args) >= 2:
@@ -822,23 +823,17 @@
         '-s': argparse.search,
         'dependees': argparse.dependees,
         '-e': argparse.dependees,
         'tracking': argparse.tracking,
         '-t': argparse.tracking
     }
 
-    # try:
-    #     arguments[args[0]]()
-    # except (KeyError, IndexError) as err:
-    #     logger = logging.getLogger(__name__)
-    #     logger.info('%s: %s', main.__name__, err)
-    #     usage.help_short(1)
-
-    # For development mode.
-    arguments[args[0]]()
-    logger = logging.getLogger(__name__)
-    logger.info('%s: %s', main.__name__, err)
-    usage.help_short(1)
+    try:
+        arguments[args[0]]()
+    except (KeyError, IndexError) as err:
+        logger = logging.getLogger(__name__)
+        logger.info('%s: %s', main.__name__, err)
+        usage.help_short(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `slpkg-4.7.8/slpkg/find_installed.py` & `slpkg-4.7.9/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/slpkg/upgrade.py` & `slpkg-4.7.9/slpkg/upgrade.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
 
 
 class Upgrade(Configs):
     """ Upgrade the installed packages. """
 
-    def __init__(self, flags: list, data: dict, repo=None):
-        __slots__ = 'flags', 'data', 'repo'
+    def __init__(self, flags: list, data: dict):
+        __slots__ = 'flags', 'data'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.data: dict = data
-        self.repo: str = repo
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.option_for_binaries: bool = self.utils.is_option(
             ['-B', '--bin-repo='], self.flags)
 
         logging.basicConfig(filename=str(LoggingConfig.log_file),
@@ -45,15 +44,15 @@
         """ Compares version of packages and returns the maximum. """
         repo_version = repo_build = '0'
         inst_version = inst_build = '0'
         inst_package: str = self.utils.is_package_installed(name)
 
         repo_tag: str = self.repos.repo_tag
         if self.option_for_binaries:
-            repo_tag: str = self.repos.repositories[self.repo][3]
+            repo_tag: str = self.repos.repositories[self.data[name][11]][6]
 
         if inst_package and inst_package.endswith(repo_tag):
             inst_version: str = self.utils.split_binary_pkg(inst_package)[1]
             inst_build: str = self.utils.split_binary_pkg(inst_package)[3]
 
             if self.option_for_binaries and self.data.get(name):
                 repo_version: str = self.data[name][0]
@@ -61,22 +60,32 @@
                 repo_build: str = self.utils.split_binary_pkg(repo_package)[3]
 
             else:
                 repo_version: str = self.data[name][2]
                 repo_location: str = self.data[name][0]
                 repo_build: str = self.utils.read_sbo_build_tag(name, repo_location)
 
+        repo_pkg: str = f'{name}-{repo_version}'
+        inst_pkg: str = f'{name}-{inst_version}'
+
         try:
-            if parse(repo_version) > parse(inst_version):
+            if parse(repo_pkg) > parse(inst_pkg):
                 return True
 
-            if parse(repo_version) == parse(inst_version) and parse(repo_build) > parse(inst_build):
+            if (parse(repo_pkg) == parse(inst_pkg)
+                    and parse(repo_build) > parse(inst_build)):
                 return True
+
         except InvalidVersion as err:
             logger = logging.getLogger(__name__)
             logger.info('%s: %s: %s: %s', self.__class__.__name__,
                         Upgrade.is_package_upgradeable.__name__,
                         name,
                         err)
-            return repo_version > inst_version and repo_build > inst_build
+
+            if repo_pkg > inst_pkg:
+                return True
+
+            if repo_pkg == inst_pkg and repo_build > inst_build:
+                return True
 
         return False
```

### Comparing `slpkg-4.7.8/slpkg/search.py` & `slpkg-4.7.9/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/setup.cfg` & `slpkg-4.7.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.7.8
+version = 4.7.9
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = d.zlatanidis@gmail.com
 description = Packaging tool that interacts with the SBo repository
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.7.8/slpkg.egg-info/SOURCES.txt` & `slpkg-4.7.9/slpkg.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 setup.cfg
 setup.py
 slpkg/__init__.py
 slpkg/blacklist.py
 slpkg/check_updates.py
 slpkg/checks.py
 slpkg/checksum.py
```

### Comparing `slpkg-4.7.8/slpkg.egg-info/PKG-INFO` & `slpkg-4.7.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,270 +1,247 @@
-Metadata-Version: 2.1
-Name: slpkg
-Version: 4.7.8
-Summary: Packaging tool that interacts with the SBo repository
-Home-page: https://dslackw.gitlab.io/slpkg/
-Author: Dimitris Zlatanidis
-Author-email: d.zlatanidis@gmail.com
-License: UNKNOWN
-Project-URL: Source, https://dslackw.gitlab.io/slpkg/
-Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Unix Shell
-Classifier: Topic :: Utilities
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: System :: Archiving :: Packaging
-Classifier: Topic :: System :: Software Distribution
-Classifier: Topic :: System :: Installation/Setup
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: System :: Software Distribution
-Requires-Python: >=3.9
-Provides-Extra: socks
-License-File: LICENSE
+### Table of contents 
 
-.. contents:: Table of Contents:
+1. [About](#About)
+2. [Screenshots](#Screenshots)
+3. [Installation](#Installation)
+4. [Requirements](#Requirements)
+5. [Recommended](#Recommended)
+6. [Testing](#Testing)
+7. [Command Line Tool Usage](#Command-Line-Tool-Usage)
+8. [How to start](#How-to-start)
+9. [Configuration files](#Configuration-files)
+10. [Repositories](#Repositories)
+11. [Multilib Packages](#Multilib-Packages)
+12. [Issues](#Issues)
+13. [Donate](#Donate)
+14. [Support](#Support)
+15. [Copyright](#Copyright)
 
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_packages.png" width="400" height="200">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/poweredbyslack.gif" width="200" height="50">
 
-About
------
 
-Slpkg is a software package manager that installs, updates and removes packages on `Slackware <http://www.slackware.com/>`_-based systems.
-It automatically calculates dependencies and figures out what things need to happen to install packages. 
-Slpkg makes it easier to manage groups of machines without the need for manual updates.
+### About
 
-Slpkg works in accordance with the standards of the `SlackBuilds.org <https://www.slackbuilds.org>`__ organization to build packages. 
+Slpkg is a software package manager that installs, updates and removes packages on [Slackware](https://www.slackware.com)-based systems.
+It automatically calculates dependencies and figures out what things need to happen to install packages.
+Slpkg makes it easier to manage groups of machines without the need for manual updates.
+Slpkg works in accordance with the standards of the [slackbuilds.org](https://www.slackbuilds.org) organization to build packages.
 It also uses the Slackware Linux instructions for installing, upgrading or removing packages.
 
-.. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_package.png
-    :target: https://gitlab.com/dslackw/slpkg
-
-
-Requirements
-------------
-
-.. code-block:: bash
-
-    SQLAlchemy >= 1.4.46
-    pythondialog >= 3.5.3
-    progress >= 1.6
-
-Install
--------
-
-Install it from the official third-party `SlackBuilds.org <https://slackbuilds.org/repository/15.0/system/slpkg/>`__ repository or directly from source:
-
-.. code-block:: bash
-
-    $ tar xvf slpkg-4.7.8.tar.gz
-    $ cd slpkg-4.7.8
-    $ ./install.sh
-
-Screenshots
------------
-
-.. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png
-    :target: https://gitlab.com/dslackw/slpkg
-
-.. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove.png
-    :target: https://gitlab.com/dslackw/slpkg
-
-.. image:: https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_dependees.png
-    :target: https://gitlab.com/dslackw/slpkg
-
-
-Usage
------
-
-.. code-block:: bash
-
-    $ slpkg --help
-      USAGE: slpkg [OPTIONS] [COMMAND] [FILELIST|PACKAGES...]
-
-      DESCRIPTION:
-        Package manager utility for Slackware.
+### Screenshots
 
-      COMMANDS:
-        -u, update                    Update the package lists.
-        -U, upgrade                   Upgrade all the packages.
-        -c, check-updates             Check for news on ChangeLog.txt.
-        -I, repo-info                 Prints the repositories information.
-        -g, configs                   Edit the configuration file.
-        -L, clean-logs                Clean dependencies log tracking.
-        -T, clean-data                Clean all the repositories data
-        -D, clean-tmp                 Deletes all the downloaded sources.
-        -b, build [packages...]       Build only the packages.
-        -i, install [packages...]     Build and install the packages.
-        -d, download [packages...]    Download only the scripts and sources.
-        -R, remove [packages...]      Remove installed packages.
-        -f, find [packages...]        Find installed packages.
-        -w, view [packages...]        View packages from the repository.
-        -s, search [packages...]      Search packages from the repository.
-        -e, dependees [packages...]   Show which packages depend.
-        -t, tracking [packages...]    Tracking the packages dependencies.
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_repo_info.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_done.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_remove_done.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_dependees.png" width="700">
+<img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="700">
+
+### Installation
+
+```
+$ tar xvf slpkg-4.7.9.tar.gz
+$ cd slpkg-4.7.9
+$ ./install.sh
+```
+
+### Requirements
+
+```
+SQLAlchemy >= 1.4.46
+pythondialog >= 3.5.3
+progress >= 1.6
+```
+
+### Recommended
+
+Stay always updated, see my other project SUN [(Slackware Update Notifier)](https://gitlab.com/dslackw/sun)
+
+
+### Testing
+
+The majority of trials have been made in Slackware x86_64 'stable' environment.
+
+
+### Command Line Tool Usage
+
+```
+USAGE: slpkg [OPTIONS] [COMMAND] [FILELIST|PACKAGES...]
+
+DESCRIPTION: Package manager utility for Slackware.
+
+COMMANDS:
+  -u, update                    Update the package lists.
+  -U, upgrade                   Upgrade all the packages.
+  -c, check-updates             Check for news on ChangeLog.txt.
+  -I, repo-info                 Prints the repositories information.
+  -g, configs                   Edit the configuration file.
+  -L, clean-logs                Clean dependencies log tracking.
+  -T, clean-data                Clean all the repositories data.
+  -D, clean-tmp                 Delete all the downloaded sources.
+  -b, build [packages...]       Build only the packages.
+  -i, install [packages...]     Build and install the packages.
+  -d, download [packages...]    Download only the scripts and sources.
+  -R, remove [packages...]      Remove installed packages.
+  -f, find [packages...]        Find installed packages.
+  -w, view [packages...]        View packages from the repository.
+  -s, search [packages...]      Search packages from the repository.
+  -e, dependees [packages...]   Show which packages depend.
+  -t, tracking [packages...]    Tracking the packages dependencies.
+
+OPTIONS:
+  -y, --yes                     Answer Yes to all questions.
+  -j, --jobs                    Set it for multicore systems.
+  -o, --resolve-off             Turns off dependency resolving.
+  -r, --reinstall               Upgrade packages of the same version.
+  -k, --skip-installed          Skip installed packages.
+  -E, --full-reverse            Full reverse dependency.
+  -S, --search                  Search packages from the repository.
+  -n, --no-silent               Disable silent mode.
+  -p, --pkg-version             Print the repository package version.
+  -G, --generate-only           Generates only the SLACKBUILDS.TXT file.
+  -B, --bin-repo=[REPO]         Set a binary repository.
+  -z, --directory=[PATH]        Download files to a specific path.
+
+  -h, --help                    Show this message and exit.
+  -v, --version                 Print version and exit.
+```
 
-      OPTIONS:
-        -y, --yes                     Answer Yes to all questions.
-        -j, --jobs                    Set it for multicore systems.
-        -o, --resolve-off             Turns off dependency resolving.
-        -r, --reinstall               Upgrade packages of the same version.
-        -k, --skip-installed          Skip installed packages.
-        -E, --full-reverse            Full reverse dependency.
-        -S, --search                  Search packages from the repository.
-        -n, --no-silent               Disable silent mode.
-        -p, --pkg-version             Print the repository package version.
-        -G, --generate-only           Generates only the SLACKBUILDS.TXT file.
-        -P, --parallel                Download files in parallel.
-        -B, --bin-repo=[REPO]         Set a binary repository.
-        -z, --directory=[PATH]        Download files to a specific path.
 
-        -h, --help                    Show this message and exit.
-        -v, --version                 Print version and exit.
+### How to start
 
-   If you need more information try to use slpkg manpage.
-   Extra help for the commands, use: 'slpkg help [command]'.
-   Edit the config file in the /etc/slpkg/slpkg.toml or 'slpkg configs'.
-
-
-How to start
-------------
-
-If you are going to use only the `SlackBuilds.org <https://slackbuilds.org/>`__ repository, you don't need to edit the
-:code:`/etc/slpkg/repositories.toml` file, otherwise edit the file and set :code:`true` the repositories you want.
+If you are going to use only the [SlackBuilds.org](https://slackbuilds.org) repository, you don't need to edit
+the `/etc/slpkg/repositories.toml` file, otherwise edit the file and set `true` the repositories you want.
 
 The second step is to update the package lists and install the data to the database, just run:
 
-.. code-block:: bash
 
+```
     $ slpkg update
+```
 
 or for binary repositories:
 
-.. code-block:: bash
-
+```
     $ slpkg update --bin-repo='*'
-
+```
 Now you are ready to start!
 
-To install a package from the `SlackBuilds.org <https://slackbuilds.org/>`__ or `Ponce <https://cgit.ponce.cc/slackbuilds/>`_ repository, run:
-
-.. code-block:: bash
+To install a package from the [SlackBuilds.org](https://slackbuilds.org) or [Ponce](https://cgit.ponce.cc/slackbuilds) repository, run:
 
+```
     $ slpkg install <package_name>
+```
 
 or from a binary repository:
 
-.. code-block:: bash
-
+```
     $ slpkg install <package_name> --bin-repo=<repo_name>
+```
 
 You can install a whole repository with the command:
 
-.. code-block:: bash
-
+```
     $ slpkg install '*' --bin-repo=<repository_name> --resolve-off
+```
 
 Note: Apply the option '--resolve-off' to speed up the process, if the repository has no references to the dependencies.
 
 To remove a package with the dependencies:
 
-.. code-block:: bash
-
+```
     $ slpkg remove <package_name>
+```
 
-If you wan to search a package from all binaries repositories, run:
-
-.. code-block:: bash
+If you want to search a package from all binaries repositories, run:
 
+```
     $ slpkg search <package_name> --bin-repo='*'
+```
 
-Edit the configuration :code:`/etc/slpkg/slpkg.toml` file:
-
-.. code-block:: bash
+Edit the configuration `/etc/slpkg/slpkg.toml` file:
 
+```
     $ slpkg configs
-
+```
 
 For further information, please read the manpage:
 
-.. code-block:: bash
-
+```
     $ man slpkg
+```
 
 
-Configuration files
--------------------
+### Configuration files
 
-.. code-block:: bash
+```
+/etc/slpkg/slpkg.toml
+    General configuration of slpkg
+    
+/etc/slpkg/repositories.toml
+    Repositories configuration
+
+/etc/slpkg/blacklist.toml
+    Blacklist of packages
+```
+
+### Repositories
+
+This is the list of the supported repositories:
+
+* [Slackbuilds](https://slackbuilds.org/)
+* [Ponce](https://cgit.ponce.cc/slackbuilds/)
+* [Slackware](https://slackware.uk/slackware/slackware64-15.0/)
+* [Slackware Extra](https://slackware.uk/slackware/slackware64-15.0/extra/)
+* [Slackware Patches](https://slackware.uk/slackware/slackware64-15.0/patches/)
+* [Alien](http://slackware.uk/people/alien/sbrepos/15.0/x86_64/)
+* [Multilib](https://slackware.nl/people/alien/multilib/15.0/)
+* [Restricted](https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/)
+* [Gnome](https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/)
+* [Msb](https://slackware.uk/msb/15.0/1.26/x86_64/)
+* [Csb](https://slackware.uk/csb/15.0/x86_64/)
+* [Conraid](https://slack.conraid.net/repository/slackware64-current/)
+* [Slackonly](https://packages.slackonly.com/pub/packages/15.0-x86_64/)
+* [SalixOS](https://download.salixos.org/x86_64/slackware-15.0/)
+* [SalixOS Extra](https://download.salixos.org/x86_64/slackware-15.0/extra/)
+* [SalixOS Patches](https://download.salixos.org/x86_64/slackware-15.0/patches/)
+* [Slackel](http://www.slackel.gr/repo/x86_64/current/)
+* [Slint](https://slackware.uk/slint/x86_64/slint-15.0/)
 
-    /etc/slpkg/slpkg.toml
-        General configuration of slpkg
 
-    /etc/slpkg/repositories.toml
-        Repositories configurations
-
-    /etc/slpkg/blacklist.toml
-        Blacklist of packages
-
-
-Repositories
-------------
-
-The supported repositories, please read the repositories configuration file.
-
-- `Slackbuilds <https://slackbuilds.org/>`_ repository.
-- `Ponce <https://cgit.ponce.cc/slackbuilds/>`_ repository.
-- `Slackware <https://slackware.uk/slackware/slackware64-15.0/>`__ repository.
-- `Slackware extra <https://slackware.uk/slackware/slackware64-15.0/extra/>`__ repository.
-- `Slackware patches <https://slackware.uk/slackware/slackware64-15.0/patches/>`__ repository.
-- `Alien <http://slackware.uk/people/alien/sbrepos/15.0/x86_64/>`_ repository.
-- `Multilib <https://slackware.nl/people/alien/multilib/15.0/>`_ repository.
-- `Restricted <https://slackware.nl/people/alien/restricted_sbrepos/15.0/x86_64/>`_ repository.
-- `Gnome <https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/>`_ repository.
-- `Msb <https://slackware.uk/msb/15.0/1.26/x86_64/>`_ repository.
-- `Csb <https://slackware.uk/csb/15.0/x86_64/>`_ repository.
-- `Conraid <https://slack.conraid.net/repository/slackware64-current/>`_ repository.
-- `Slackonly <https://packages.slackonly.com/pub/packages/15.0-x86_64/>`_ repository.
-- `Salix OS <https://download.salixos.org/x86_64/slackware-15.0/>`_ repository.
-- `Salix OS extra <https://download.salixos.org/x86_64/slackware-15.0/extra/>`_ repository.
-- `Salix OS patches <https://download.salixos.org/x86_64/slackware-15.0/patches/>`_ repository.
-- `Slackel OS <http://www.slackel.gr/repo/x86_64/current/>`_ repository.
-- `Slint OS <https://slackware.uk/slint/x86_64/slint-15.0/>`_ repository.
+### Multilib Packages
 
+Slackware for x86_64 - multilib packages & install instructions:
 
-Multilib packages
------------------
+Please read the file [README](https://gitlab.com/dslackw/slpkg/-/raw/master/filelists/multilib/README) you will find in the folder [multlib](https://gitlab.com/dslackw/slpkg/-/tree/master/filelists/multilib)
+
+
+### Issues
+
+Please report any bugs in [ISSUES](https://gitlab.com/dslackw/slpkg/issues)
 
-Slackware for x86_64 - multilib packages & install instructions:
 
-- Please read the file `README <https://gitlab.com/dslackw/slpkg/-/raw/master/filelists/multilib/README>`_ you will find in the folder `multlib <https://gitlab.com/dslackw/slpkg/-/tree/master/filelists/multilib>`_.
+### Donate
 
-Donate
-------
+If you feel satisfied with this project and want to thank me, treat me to a coffee ☕ !
 
-If you feel satisfied with this project and want to thanks me make a donation.
+[<img src="https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png">](https://www.paypal.me/dslackw)
 
-.. image:: https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png
-   :target: https://www.paypal.me/dslackw
 
-Report bugs
------------
+### Support
 
-Please report any issue here: `Issues <https://gitlab.com/dslackw/slpkg/-/issues>`_
+Please support:
 
+* [Slackware](https://www.patreon.com/slackwarelinux) project.
+* [SlackBuilds](https://slackbuilds.org/contributors/) repository.
+* [AlienBob](https://alien.slackbook.org/blog/) Eric Hameleers.
 
-Copyright
----------
+Thank you all for your support!
 
-- Copyright 2014-2023 © Dimitris Zlatanidis.
-- Slackware® is a Registered Trademark of Patrick Volkerding. 
-- Linux is a Registered Trademark of Linus Torvalds.
 
+### Copyright
 
+Copyright 2014-2023 © Dimitris Zlatanidis.
+Slackware® is a Registered Trademark of Patrick Volkerding.
+Linux is a Registered Trademark of Linus Torvalds.
```

### Comparing `slpkg-4.7.8/tools/gen_sbo_txt.sh` & `slpkg-4.7.9/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.7.8/bin/slpkg_new-configs` & `slpkg-4.7.9/bin/slpkg_new-configs`

 * *Files identical despite different names*

