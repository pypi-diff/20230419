# Comparing `tmp/pysequoia-0.1.8.tar.gz` & `tmp/pysequoia-0.1.9.tar.gz`

## Comparing `pysequoia-0.1.8.tar` & `pysequoia-0.1.9.tar`

### file list

```diff
@@ -1,789 +1,841 @@
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 pysequoia-0.1.8/Cargo.toml
--rw-r--r--   0     1000     1000       17 2023-01-19 11:23:14.000000 pysequoia-0.1.8/.dockerignore
--rw-r--r--   0     1000     1000     6128 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0     1000     1000       44 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/_distutils_hack/override.py
--rw-r--r--   0     1000     1000      151 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/distutils-precedence.pth
--rw-r--r--   0     1000     1000     5748 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin/__init__.py
--rw-r--r--   0     1000     1000      953 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin/__main__.py
--rw-r--r--   0     1000     1000     4835 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin/import_hook.py
--rw-r--r--   0     1000     1000        4 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/INSTALLER
--rw-r--r--   0     1000     1000    17737 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/METADATA
--rw-r--r--   0     1000     1000      859 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/REQUESTED
--rw-r--r--   0     1000     1000      149 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/WHEEL
--rw-r--r--   0     1000     1000      357 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/__init__.py
--rw-r--r--   0     1000     1000     1198 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/__main__.py
--rw-r--r--   0     1000     1000     1444 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/__pip-runner__.py
--rw-r--r--   0     1000     1000      573 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/__init__.py
--rw-r--r--   0     1000     1000    10234 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/build_env.py
--rw-r--r--   0     1000     1000    10734 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cache.py
--rw-r--r--   0     1000     1000      132 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0     1000     1000     6676 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0     1000     1000     7842 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0     1000     1000    29381 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0     1000     1000      774 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0     1000     1000     2472 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0     1000     1000     4338 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0     1000     1000    10817 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0     1000     1000     1968 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0     1000     1000    18172 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0     1000     1000     5118 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0     1000     1000      116 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0     1000     1000     3882 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0     1000     1000     7582 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0     1000     1000     1685 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0     1000     1000     4129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0     1000     1000     9815 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0     1000     1000     6573 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0     1000     1000     5289 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0     1000     1000     2951 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0     1000     1000     1703 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0     1000     1000     1132 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0     1000     1000     4762 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0     1000     1000     3374 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0     1000     1000    31726 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0     1000     1000    12343 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0     1000     1000     5697 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0     1000     1000     6129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0     1000     1000     3680 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0     1000     1000     7396 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0     1000     1000    13529 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/configuration.py
--rw-r--r--   0     1000     1000      858 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0     1000     1000     1221 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0     1000     1000      729 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0     1000     1000     6494 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0     1000     1000     1164 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0     1000     1000    20942 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0     1000     1000       30 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0     1000     1000    16503 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0     1000     1000    37596 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0     1000     1000     6557 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0     1000     1000    17552 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0     1000     1000     6302 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0     1000     1000     7867 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0     1000     1000     2573 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0     1000     1000      340 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/main.py
--rw-r--r--   0     1000     1000     4280 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0     1000     1000     2595 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0     1000     1000    25277 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0     1000     1000      107 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0     1000     1000     1882 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0     1000     1000     8181 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0     1000     1000     7457 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0     1000     1000     9773 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0     1000     1000       63 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0     1000     1000      990 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0     1000     1000     5877 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0     1000     1000     2520 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0     1000     1000     1030 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/index.py
--rw-r--r--   0     1000     1000     2617 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0     1000     1000    18083 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/link.py
--rw-r--r--   0     1000     1000      738 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0     1000     1000     4644 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0     1000     1000     1907 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0     1000     1000     3858 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0     1000     1000     3600 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0     1000     1000       50 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0     1000     1000    12190 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0     1000     1000     2145 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0     1000     1000     6096 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/download.py
--rw-r--r--   0     1000     1000     7638 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0     1000     1000    18443 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/session.py
--rw-r--r--   0     1000     1000     4073 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0     1000     1000     1791 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0     1000     1000     4133 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0     1000     1000     1404 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0     1000     1000     1456 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0     1000     1000     2198 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0     1000     1000     1063 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0     1000     1000     1405 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0     1000     1000     3064 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0     1000     1000     5109 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0     1000     1000     9784 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0     1000     1000       51 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0     1000     1000     1354 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0     1000     1000     4105 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0     1000     1000    27407 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0     1000     1000    25091 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0     1000     1000     7074 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0     1000     1000     2807 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0     1000     1000    16611 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0     1000     1000    17646 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0     1000     1000    35600 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0     1000     1000     2858 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0     1000     1000    24045 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0     1000     1000      583 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0     1000     1000    24129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0     1000     1000     5220 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0     1000     1000    18963 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0     1000     1000    27878 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0     1000     1000     5705 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0     1000     1000     9914 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0     1000     1000     2526 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0     1000     1000     5455 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0     1000     1000    11533 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0     1000     1000     8020 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0     1000     1000     1015 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0     1000     1000     1665 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0     1000     1000     1884 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0     1000     1000     5377 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0     1000     1000      242 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0     1000     1000     5764 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0     1000     1000     3206 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0     1000     1000     1115 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0     1000     1000     2203 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0     1000     1000     1169 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0     1000     1000     3064 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0     1000     1000     5122 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0     1000     1000      716 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0     1000     1000     3110 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0     1000     1000     4831 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0     1000     1000      795 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0     1000     1000    11632 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0     1000     1000    21617 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0     1000     1000     1193 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0     1000     1000     2108 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0     1000     1000     5662 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0     1000     1000     9197 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0     1000     1000     7702 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0     1000     1000     8821 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0     1000     1000     1759 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0     1000     1000     3459 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0     1000     1000     4549 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0     1000     1000      596 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0     1000     1000     3518 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0     1000     1000    18116 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0     1000     1000     5238 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0     1000     1000    11728 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0     1000     1000    22811 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0     1000     1000    13079 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0     1000     1000     4966 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0     1000     1000      465 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0     1000     1000     1379 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0     1000     1000     5033 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0     1000     1000     1535 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0     1000     1000      242 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0     1000     1000     5271 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0     1000     1000     1033 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0     1000     1000      778 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0     1000     1000    16416 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0     1000     1000     3946 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0     1000     1000     4154 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0     1000     1000     7105 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0     1000     1000      774 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0     1000     1000       94 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0     1000     1000      255 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0     1000     1000   286370 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0     1000     1000     4279 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0     1000     1000     3705 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0     1000     1000    31274 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0     1000     1000     1741 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0     1000     1000     9608 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0     1000     1000     3817 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0     1000     1000     4801 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0     1000     1000     2406 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0     1000     1000     3559 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0     1000     1000     1838 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0     1000     1000     1619 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0     1000     1000     3864 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0     1000     1000    12021 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0     1000     1000     3676 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0     1000     1000    13566 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0     1000     1000     1731 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0     1000     1000    36913 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0     1000     1000     1731 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0     1000     1000    20735 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0     1000     1000     1737 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0     1000     1000    13919 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0     1000     1000    25796 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0     1000     1000    42498 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0     1000     1000     1730 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0     1000     1000    26797 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0     1000     1000   104562 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0     1000     1000    98484 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0     1000     1000    98196 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0     1000     1000   101363 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0     1000     1000   128035 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0     1000     1000   102774 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0     1000     1000    95372 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0     1000     1000     5260 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0     1000     1000     3367 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0     1000     1000     2056 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0     1000     1000    30068 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0     1000     1000    13280 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0     1000     1000     6199 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0     1000     1000     4129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0     1000     1000     3749 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0     1000     1000    13288 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0     1000     1000     8289 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0     1000     1000     2709 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0     1000     1000      242 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0     1000     1000      239 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0     1000     1000     2522 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0     1000     1000    10830 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0     1000     1000     1915 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0     1000     1000     5404 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0     1000     1000     6438 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0     1000     1000      581 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0     1000     1000    41259 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0     1000     1000    51697 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0     1000     1000    20834 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0     1000     1000    51991 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0     1000     1000    14811 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0     1000     1000     5058 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0     1000     1000    39801 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0     1000     1000    10820 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0     1000     1000    18102 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0     1000     1000    97792 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t32.exe
--rw-r--r--   0     1000     1000   182784 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
--rw-r--r--   0     1000     1000   108032 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0     1000     1000    66262 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0     1000     1000    23513 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0     1000     1000    91648 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w32.exe
--rw-r--r--   0     1000     1000   168448 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
--rw-r--r--   0     1000     1000   101888 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0     1000     1000    43898 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0     1000     1000      981 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0     1000     1000       64 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0     1000     1000    48841 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0     1000     1000      849 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0     1000     1000     3374 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0     1000     1000      321 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0     1000     1000    12950 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0     1000     1000    44375 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0     1000     1000     1881 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0     1000     1000       21 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0     1000     1000   206539 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0     1000     1000     1132 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0     1000     1000     1081 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0     1000     1000     6080 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0     1000     1000    34557 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0     1000     1000      661 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0     1000     1000      497 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0     1000     1000    11488 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1000     1000     4378 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1000     1000     1431 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0     1000     1000     8487 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0     1000     1000     4676 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0     1000     1000    30110 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0     1000     1000    15699 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0     1000     1000     4200 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0     1000     1000    14665 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0     1000     1000      130 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0     1000     1000      138 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/_compat.py
--rw-r--r--   0     1000     1000     3443 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0     1000     1000     6083 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0     1000     1000     3994 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0     1000     1000      607 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0     1000     1000     6081 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0     1000     1000      872 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0     1000     1000    10801 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0     1000     1000     2520 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0     1000     1000    12721 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0     1000     1000   108287 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0     1000     1000      562 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0     1000     1000    12831 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0     1000     1000     1176 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0     1000     1000     4068 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0     1000     1000     4910 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0     1000     1000     2655 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0     1000     1000     6910 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0     1000     1000       78 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0     1000     1000     6439 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0     1000     1000     2999 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0     1000     1000      353 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0     1000     1000    23685 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0     1000     1000     1697 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0     1000     1000     1938 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0     1000     1000    40386 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0     1000     1000     2917 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0     1000     1000     4810 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0     1000     1000     4104 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0     1000     1000     3314 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0     1000     1000     5086 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0     1000     1000    35441 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0     1000     1000    21938 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0     1000     1000     5871 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0     1000     1000    19351 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0     1000     1000     5073 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0     1000     1000     2212 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0     1000     1000     5014 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0     1000     1000     7335 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0     1000     1000     4674 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0     1000     1000    11753 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0     1000     1000    32005 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0     1000     1000    11174 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0     1000     1000    70232 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0     1000     1000    53376 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0     1000     1000      986 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0     1000     1000     2591 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0     1000     1000     3072 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0     1000     1000     3092 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0     1000     1000     4630 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0     1000     1000     6257 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0     1000     1000     3419 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0     1000     1000     6184 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0     1000     1000    63187 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0     1000     1000     9110 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0     1000     1000     9171 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0     1000     1000     6426 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0     1000     1000    12936 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0     1000     1000   213344 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0     1000     1000    23685 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0     1000     1000     9023 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0     1000     1000    39129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0     1000     1000    25341 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0     1000     1000    13402 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0     1000     1000    10787 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0     1000     1000     6805 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0     1000     1000     5178 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0     1000     1000      440 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0     1000     1000     1397 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0     1000     1000    21443 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0     1000     1000     6377 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0     1000     1000    10187 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0     1000     1000      575 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0     1000     1000     1286 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0     1000     1000    18560 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0     1000     1000     3823 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0     1000     1000     3879 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0     1000     1000      733 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0     1000     1000    35287 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0     1000     1000      695 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0     1000     1000    30180 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0     1000     1000     4235 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0     1000     1000     2912 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0     1000     1000    33240 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0     1000     1000      537 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0     1000     1000      156 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0     1000     1000     5872 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0     1000     1000     1583 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0     1000     1000    17592 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0     1000     1000     4794 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0     1000     1000     5944 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0     1000     1000     8808 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0     1000     1000    10096 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0     1000     1000   140235 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0     1000     1000     1064 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0     1000     1000     2114 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0     1000     1000      265 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0     1000     1000     9695 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0     1000     1000     3225 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0     1000     1000     1236 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0     1000     1000     7063 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0     1000     1000      423 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0     1000     1000     5472 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0     1000     1000    19919 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0     1000     1000      351 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0     1000     1000      417 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0     1000     1000    22820 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0     1000     1000     1926 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0     1000     1000     2783 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0     1000     1000     1840 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0     1000     1000      890 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0     1000     1000    10368 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0     1000     1000     6820 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0     1000     1000     3264 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0     1000     1000     9864 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0     1000     1000     4503 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0     1000     1000    17957 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0     1000     1000     1054 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0     1000     1000     7131 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0     1000     1000    95885 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0     1000     1000     1288 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0     1000     1000     5497 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0     1000     1000     6630 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0     1000     1000     7954 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0     1000     1000      972 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0     1000     1000     2501 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0     1000     1000      642 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0     1000     1000     1616 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0     1000     1000     2507 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0     1000     1000     9585 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0     1000     1000     5051 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0     1000     1000     3252 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0     1000     1000    14074 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0     1000     1000    14172 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0     1000     1000     3667 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0     1000     1000    11471 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0     1000     1000     8198 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0     1000     1000     5305 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0     1000     1000     4970 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0     1000     1000      828 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0     1000     1000     3396 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0     1000     1000     8744 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0     1000     1000    36576 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0     1000     1000    59746 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0     1000     1000     8161 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0     1000     1000    11303 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0     1000     1000     1391 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0     1000     1000      166 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0     1000     1000     4449 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0     1000     1000     4773 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0     1000     1000     2842 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0     1000     1000     1591 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0     1000     1000    24224 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0     1000     1000     4374 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0     1000     1000     4425 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0     1000     1000    26240 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0     1000     1000     1258 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0     1000     1000    34697 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0     1000     1000    39515 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0     1000     1000     3370 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0     1000     1000    44666 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0     1000     1000     3627 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0     1000     1000      102 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0     1000     1000    26060 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0     1000     1000     9169 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0     1000     1000    34549 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/six.py
--rw-r--r--   0     1000     1000    18364 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0     1000     1000     3314 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0     1000     1000     1944 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0     1000     1000     1496 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0     1000     1000     1376 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0     1000     1000     1908 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0     1000     1000     1383 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0     1000     1000     7550 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0     1000     1000     2790 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0     1000     1000     2145 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0     1000     1000     8011 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0     1000     1000      396 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0     1000     1000    22633 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0     1000     1000     2943 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0     1000     1000      254 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0     1000     1000    80114 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0     1000     1000     3333 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0     1000     1000    10811 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0     1000     1000       64 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0     1000     1000    20070 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0     1000     1000    39093 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0     1000     1000      957 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0     1000     1000    17632 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0     1000     1000    13922 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0     1000     1000    11034 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0     1000     1000     4538 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0     1000     1000    17182 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0     1000     1000    34448 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0     1000     1000     7097 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0     1000     1000     8217 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0     1000     1000     8579 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0     1000     1000     2440 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0     1000     1000     1417 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0     1000     1000    34665 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0     1000     1000    19786 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0     1000     1000     5985 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0     1000     1000    30109 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0     1000     1000     1155 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0     1000     1000     4901 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0     1000     1000     1605 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0     1000     1000      498 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0     1000     1000     3997 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0     1000     1000     3510 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0     1000     1000    22001 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0     1000     1000    17177 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0     1000     1000     5758 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0     1000     1000     6895 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0     1000     1000    10003 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0     1000     1000    14287 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0     1000     1000     5403 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0     1000     1000      469 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0     1000     1000    10579 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0     1000     1000     8979 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0     1000     1000     1305 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0     1000     1000     6563 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0     1000     1000     4307 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0     1000     1000      286 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/py.typed
--rw-r--r--   0     1000     1000        4 2023-01-17 08:30:19.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1093 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt
--rw-r--r--   0     1000     1000     4072 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/METADATA
--rw-r--r--   0     1000     1000    76117 2023-01-17 08:30:19.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:19.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/REQUESTED
--rw-r--r--   0     1000     1000       92 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/WHEEL
--rw-r--r--   0     1000     1000      125 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/entry_points.txt
--rw-r--r--   0     1000     1000        4 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/top_level.txt
--rw-r--r--   0     1000     1000   108568 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0     1000     1000    24701 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0     1000     1000      506 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0     1000     1000     4504 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0     1000     1000     2741 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0     1000     1000     2706 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0     1000     1000      884 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0     1000     1000     3494 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0     1000     1000     3886 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0     1000     1000     3566 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0     1000     1000     2836 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0     1000     1000     5420 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0     1000     1000    13515 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0     1000     1000    15526 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0     1000     1000       83 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0     1000     1000   132569 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0     1000     1000    18410 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0     1000     1000      661 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0     1000     1000      497 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0     1000     1000    11488 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1000     1000     4378 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1000     1000     1431 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0     1000     1000     8496 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0     1000     1000     4706 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0     1000     1000    30110 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0     1000     1000    15699 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0     1000     1000     4200 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0     1000     1000    14665 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0     1000     1000     9159 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0     1000     1000     6426 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0     1000     1000    12936 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0     1000     1000   213310 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0     1000     1000    23668 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0     1000     1000     9023 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0     1000     1000    39129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0     1000     1000    25341 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0     1000     1000    13402 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0     1000     1000    10787 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0     1000     1000     6805 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0     1000     1000     8425 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0     1000     1000     2426 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0     1000     1000      119 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia/__init__.py
--rw-r--r--   0     1000     1000        4 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     3331 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/METADATA
--rw-r--r--   0     1000     1000      735 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/REQUESTED
--rw-r--r--   0     1000     1000      101 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/WHEEL
--rw-r--r--   0     1000     1000       98 2023-01-26 11:46:06.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/direct_url.json
--rw-r--r--   0     1000     1000     8429 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/__init__.py
--rw-r--r--   0     1000     1000      218 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0     1000     1000      537 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0     1000     1000     1330 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0     1000     1000      411 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0     1000     1000      239 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0     1000     1000    19672 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0     1000     1000     8603 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0     1000     1000    14789 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0     1000     1000    47369 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0     1000     1000    17973 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0     1000     1000      430 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0     1000     1000     1614 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0     1000     1000     5441 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0     1000     1000     4701 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0     1000     1000    22051 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0     1000     1000     5617 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0     1000     1000     7728 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0     1000     1000    31558 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0     1000     1000    16568 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0     1000     1000     5624 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0     1000     1000     4888 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0     1000     1000     2603 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0     1000     1000    13137 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0     1000     1000    30221 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0     1000     1000     2779 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0     1000     1000     2785 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0     1000     1000     1189 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0     1000     1000     8434 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0     1000     1000     1936 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0     1000     1000      672 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0     1000     1000    11765 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0     1000     1000    19241 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0     1000     1000     7477 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0     1000     1000     4920 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0     1000     1000     9451 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0     1000     1000    12537 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0     1000     1000      139 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0     1000     1000     3423 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0     1000     1000     8082 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0     1000     1000    50186 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0     1000     1000     3589 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0     1000     1000    10270 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0     1000     1000    17910 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0     1000     1000     8226 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0     1000     1000    13713 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0     1000     1000     1972 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0     1000     1000    30235 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0     1000     1000    23602 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0     1000     1000      217 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0     1000     1000      639 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0     1000     1000     3517 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0     1000     1000    18858 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0     1000     1000    12096 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0     1000     1000    15641 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0     1000     1000    18128 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0     1000     1000    12952 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0     1000     1000     5248 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0     1000     1000     1972 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_entry_points.py
--rw-r--r--   0     1000     1000     2392 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_imp.py
--rw-r--r--   0     1000     1000     1311 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_importlib.py
--rw-r--r--   0     1000     1000      675 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_itertools.py
--rw-r--r--   0     1000     1000      749 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_path.py
--rw-r--r--   0     1000     1000      501 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_reqs.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0     1000     1000    30130 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0     1000     1000     1862 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0     1000     1000      743 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0     1000     1000     1828 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0     1000     1000     2895 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0     1000     1000     2068 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0     1000     1000     1154 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0     1000     1000     2166 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0     1000     1000      506 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0     1000     1000     4504 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0     1000     1000     2741 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0     1000     1000     2706 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0     1000     1000      884 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0     1000     1000     3494 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0     1000     1000     3886 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0     1000     1000     3566 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0     1000     1000     2836 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0     1000     1000     5420 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0     1000     1000    13512 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0     1000     1000    15517 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0     1000     1000       82 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0     1000     1000   117959 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0     1000     1000    16256 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0     1000     1000    15130 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0     1000     1000      661 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0     1000     1000      497 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0     1000     1000    11488 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1000     1000     4378 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1000     1000     1431 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0     1000     1000     8493 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0     1000     1000     4700 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0     1000     1000    30110 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0     1000     1000    15699 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0     1000     1000     4200 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0     1000     1000    14665 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0     1000     1000     9159 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0     1000     1000     6426 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0     1000     1000    12936 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0     1000     1000   213310 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0     1000     1000    23668 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0     1000     1000     9023 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0     1000     1000    39129 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0     1000     1000    25341 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0     1000     1000    13402 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0     1000     1000    10787 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0     1000     1000     6805 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0     1000     1000      396 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0     1000     1000    22633 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0     1000     1000     2943 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0     1000     1000      254 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0     1000     1000    87149 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0     1000     1000     8425 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0     1000     1000     7346 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/archive_util.py
--rw-r--r--   0     1000     1000    19539 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/build_meta.py
--rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli-32.exe
--rw-r--r--   0     1000     1000    74752 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli-64.exe
--rw-r--r--   0     1000     1000   137216 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli.exe
--rw-r--r--   0     1000     1000      396 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/__init__.py
--rw-r--r--   0     1000     1000     2381 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/alias.py
--rw-r--r--   0     1000     1000    16623 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0     1000     1000     1182 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0     1000     1000     6595 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build.py
--rw-r--r--   0     1000     1000     4415 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0     1000     1000    15821 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0     1000     1000    14115 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build_py.py
--rw-r--r--   0     1000     1000     7012 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/develop.py
--rw-r--r--   0     1000     1000     4800 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0     1000     1000    85662 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0     1000     1000    31188 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0     1000     1000    26795 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0     1000     1000     5163 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install.py
--rw-r--r--   0     1000     1000     2226 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0     1000     1000     3875 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0     1000     1000     2612 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0     1000     1000      628 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0     1000     1000     4946 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0     1000     1000      468 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/register.py
--rw-r--r--   0     1000     1000     2128 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/rotate.py
--rw-r--r--   0     1000     1000      658 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0     1000     1000     7071 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/sdist.py
--rw-r--r--   0     1000     1000     5086 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/setopt.py
--rw-r--r--   0     1000     1000     8102 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/test.py
--rw-r--r--   0     1000     1000      462 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/upload.py
--rw-r--r--   0     1000     1000     7494 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0     1000     1000     1121 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/__init__.py
--rw-r--r--   0     1000     1000    13398 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0     1000     1000     1038 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0     1000     1000    11266 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0     1000     1000     1153 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0     1000     1000     1612 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0     1000     1000   269900 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0     1000     1000     8736 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0     1000     1000    16319 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/expand.py
--rw-r--r--   0     1000     1000    19304 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0     1000     1000    25198 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0     1000     1000      949 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/dep_util.py
--rw-r--r--   0     1000     1000     5499 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/depends.py
--rw-r--r--   0     1000     1000    20799 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/discovery.py
--rw-r--r--   0     1000     1000    45578 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/dist.py
--rw-r--r--   0     1000     1000     2464 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/errors.py
--rw-r--r--   0     1000     1000     5591 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/extension.py
--rw-r--r--   0     1000     1000     2512 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0     1000     1000     4873 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/glob.py
--rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui-32.exe
--rw-r--r--   0     1000     1000    75264 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui-64.exe
--rw-r--r--   0     1000     1000   137728 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui.exe
--rw-r--r--   0     1000     1000     3824 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/installer.py
--rw-r--r--   0     1000     1000      812 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/launch.py
--rw-r--r--   0     1000     1000     1210 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/logging.py
--rw-r--r--   0     1000     1000     4857 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/monkey.py
--rw-r--r--   0     1000     1000    47724 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/msvc.py
--rw-r--r--   0     1000     1000     3093 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/namespaces.py
--rw-r--r--   0     1000     1000    40020 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/package_index.py
--rw-r--r--   0     1000     1000      245 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/py34compat.py
--rw-r--r--   0     1000     1000    14348 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/sandbox.py
--rw-r--r--   0     1000     1000      218 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0     1000     1000      138 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/script.tmpl
--rw-r--r--   0     1000     1000      941 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0     1000     1000      144 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/version.py
--rw-r--r--   0     1000     1000     8376 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/wheel.py
--rw-r--r--   0     1000     1000      718 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/windows_support.py
--rw-r--r--   0     1000     1000        4 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1050 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/LICENSE
--rw-r--r--   0     1000     1000     6301 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/METADATA
--rw-r--r--   0     1000     1000    37694 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/REQUESTED
--rw-r--r--   0     1000     1000       92 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/WHEEL
--rw-r--r--   0     1000     1000     2740 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
--rw-r--r--   0     1000     1000       41 2023-01-17 08:30:18.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/top_level.txt
--rw-r--r--   0     1000     1000      396 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/__init__.py
--rw-r--r--   0     1000     1000    22633 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/_parser.py
--rw-r--r--   0     1000     1000     2943 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/_re.py
--rw-r--r--   0     1000     1000      254 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/_types.py
--rw-r--r--   0     1000     1000       26 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/py.typed
--rw-r--r--   0     1000     1000        4 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1072 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0     1000     1000     8875 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA
--rw-r--r--   0     1000     1000      913 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD
--rw-r--r--   0     1000     1000       81 2023-01-25 10:59:02.000000 pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/WHEEL
--rw-r--r--   0     1000     1000       70 2023-01-25 11:53:47.000000 pysequoia-0.1.8/.env/pyvenv.cfg
--rw-r--r--   0     1000     1000      710 2023-01-19 11:23:14.000000 pysequoia-0.1.8/.gitignore
--rw-r--r--   0     1000     1000      469 2023-01-19 11:23:14.000000 pysequoia-0.1.8/.gitlab-ci.yml
--rw-r--r--   0     1000     1000     1257 2023-01-19 13:30:28.000000 pysequoia-0.1.8/.woodpecker.yml
--rw-r--r--   0     1000     1000     3003 2023-01-26 10:50:51.000000 pysequoia-0.1.8/README.md
--rw-r--r--   0     1000     1000      394 2023-01-19 11:23:14.000000 pysequoia-0.1.8/ci/build.dockerfile
--rw-r--r--   0     1000     1000      361 2023-01-19 11:23:14.000000 pysequoia-0.1.8/ci/docs.dockerfile
--rw-r--r--   0     1000     1000      511 2023-01-25 10:40:26.000000 pysequoia-0.1.8/ci/e2e.dockerfile
--rw-r--r--   0     1000     1000     8334 2023-01-19 11:23:14.000000 pysequoia-0.1.8/doc/tufte.min.css
--rw-r--r--   0     1000     1000      317 2023-01-25 10:57:15.000000 pysequoia-0.1.8/pyproject.toml
--rw-r--r--   0     1000     1000      428 2023-01-19 11:23:14.000000 pysequoia-0.1.8/signing-key.asc
--rw-r--r--   0     1000     1000     9435 2023-01-27 12:17:01.000000 pysequoia-0.1.8/src/lib.rs
--rw-r--r--   0     1000     1000    32600 2023-01-19 11:23:14.000000 pysequoia-0.1.8/wiktor-fresh.asc
--rw-r--r--   0     1000     1000   199223 2023-01-19 11:23:14.000000 pysequoia-0.1.8/wiktor.asc
--rw-r--r--   0     1000     1000    69479 2023-01-27 12:21:37.000000 pysequoia-0.1.8/Cargo.lock
--rw-r--r--   0        0        0     3331 1970-01-01 00:00:00.000000 pysequoia-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/Cargo.toml
+-rw-r--r--   0     1000     1000     1162 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/README.md
+-rw-r--r--   0     1000     1000    10364 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/algorithm.rs
+-rw-r--r--   0     1000     1000     3899 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/apdu/command.rs
+-rw-r--r--   0     1000     1000     7503 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/apdu/commands.rs
+-rw-r--r--   0     1000     1000     3629 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/apdu/response.rs
+-rw-r--r--   0     1000     1000     6890 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/apdu.rs
+-rw-r--r--   0     1000     1000     4435 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/algo_attrs.rs
+-rw-r--r--   0     1000     1000    16172 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/algo_info.rs
+-rw-r--r--   0     1000     1000     3778 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/application_id.rs
+-rw-r--r--   0     1000     1000     2454 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/cardholder.rs
+-rw-r--r--   0     1000     1000     5478 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/extended_cap.rs
+-rw-r--r--   0     1000     1000     1569 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/extended_length_info.rs
+-rw-r--r--   0     1000     1000     4055 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/fingerprint.rs
+-rw-r--r--   0     1000     1000    11261 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/historical.rs
+-rw-r--r--   0     1000     1000     2759 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/key_generation_times.rs
+-rw-r--r--   0     1000     1000     2855 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do/pw_status.rs
+-rw-r--r--   0     1000     1000    28498 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/card_do.rs
+-rw-r--r--   0     1000     1000     4850 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/crypto_data.rs
+-rw-r--r--   0     1000     1000     6084 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/errors.rs
+-rw-r--r--   0     1000     1000    19345 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/keys.rs
+-rw-r--r--   0     1000     1000    20371 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/lib.rs
+-rw-r--r--   0     1000     1000     1299 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/oid.rs
+-rw-r--r--   0     1000     1000    38995 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/openpgp.rs
+-rw-r--r--   0     1000     1000     1098 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/tlv/length.rs
+-rw-r--r--   0     1000     1000     3486 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/tlv/tag.rs
+-rw-r--r--   0     1000     1000     1412 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/tlv/value.rs
+-rw-r--r--   0     1000     1000     9637 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card/src/tlv.rs
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/Cargo.toml
+-rw-r--r--   0     1000     1000     1020 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/README.md
+-rw-r--r--   0     1000     1000      294 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/encrypted_to_25519.asc
+-rw-r--r--   0     1000     1000      428 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/encrypted_to_nist521.asc
+-rw-r--r--   0     1000     1000      529 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/encrypted_to_rsa2k.asc
+-rw-r--r--   0     1000     1000      879 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/encrypted_to_rsa4k.asc
+-rw-r--r--   0     1000     1000     1154 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/nist256.sec
+-rw-r--r--   0     1000     1000     1820 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/nist521.sec
+-rw-r--r--   0     1000     1000     1032 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/test25519.sec
+-rw-r--r--   0     1000     1000     5176 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/test2k.sec
+-rw-r--r--   0     1000     1000     7516 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/test3k.sec
+-rw-r--r--   0     1000     1000     9856 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/example/test4k.sec
+-rw-r--r--   0     1000     1000     7648 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/examples/test.rs
+-rw-r--r--   0     1000     1000     5632 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/decryptor.rs
+-rw-r--r--   0     1000     1000    29239 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/lib.rs
+-rw-r--r--   0     1000     1000     6289 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/privkey.rs
+-rw-r--r--   0     1000     1000     5811 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/signer.rs
+-rw-r--r--   0     1000     1000     5550 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/sq_util.rs
+-rw-r--r--   0     1000     1000     2547 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/state.rs
+-rw-r--r--   0     1000     1000      446 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/types.rs
+-rw-r--r--   0     1000     1000    13008 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-sequoia/src/util.rs
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-pcsc/Cargo.toml
+-rw-r--r--   0     1000     1000     1102 2022-05-27 10:41:28.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-pcsc/README.md
+-rw-r--r--   0     1000     1000    23446 2023-02-01 09:16:59.000000 pysequoia-0.1.9/local_dependencies/openpgp-card-pcsc/src/lib.rs
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 pysequoia-0.1.9/Cargo.toml
+-rw-r--r--   0     1000     1000       17 2023-01-19 11:23:14.000000 pysequoia-0.1.9/.dockerignore
+-rw-r--r--   0     1000     1000     6128 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0     1000     1000       44 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/_distutils_hack/override.py
+-rw-r--r--   0     1000     1000      151 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/distutils-precedence.pth
+-rw-r--r--   0     1000     1000     5748 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin/__init__.py
+-rw-r--r--   0     1000     1000      953 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin/__main__.py
+-rw-r--r--   0     1000     1000     4835 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin/import_hook.py
+-rw-r--r--   0     1000     1000        4 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/INSTALLER
+-rw-r--r--   0     1000     1000    17737 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/METADATA
+-rw-r--r--   0     1000     1000      859 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/RECORD
+-rw-r--r--   0     1000     1000        0 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/REQUESTED
+-rw-r--r--   0     1000     1000      149 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/WHEEL
+-rw-r--r--   0     1000     1000      357 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/__init__.py
+-rw-r--r--   0     1000     1000     1198 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/__main__.py
+-rw-r--r--   0     1000     1000     1444 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0     1000     1000      573 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0     1000     1000    10234 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0     1000     1000    10734 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cache.py
+-rw-r--r--   0     1000     1000      132 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0     1000     1000     6676 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0     1000     1000     7842 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0     1000     1000    29381 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0     1000     1000      774 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0     1000     1000     2472 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0     1000     1000     4338 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0     1000     1000    10817 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0     1000     1000     1968 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0     1000     1000    18172 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0     1000     1000     5118 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0     1000     1000      116 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0     1000     1000     3882 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0     1000     1000     7582 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0     1000     1000     1685 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0     1000     1000     4129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0     1000     1000     9815 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0     1000     1000     6573 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0     1000     1000     5289 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0     1000     1000     2951 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0     1000     1000     1703 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0     1000     1000     1132 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0     1000     1000     4762 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0     1000     1000     3374 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0     1000     1000    31726 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0     1000     1000    12343 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0     1000     1000     5697 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0     1000     1000     6129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0     1000     1000     3680 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0     1000     1000     7396 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0     1000     1000    13529 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0     1000     1000      858 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0     1000     1000     1221 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0     1000     1000      729 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0     1000     1000     6494 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0     1000     1000     1164 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0     1000     1000    20942 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0     1000     1000       30 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0     1000     1000    16503 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0     1000     1000    37596 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0     1000     1000     6557 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0     1000     1000    17552 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0     1000     1000     6302 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0     1000     1000     7867 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0     1000     1000     2573 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0     1000     1000      340 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/main.py
+-rw-r--r--   0     1000     1000     4280 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0     1000     1000     2595 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0     1000     1000    25277 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0     1000     1000      107 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0     1000     1000     1882 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0     1000     1000     8181 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0     1000     1000     7457 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0     1000     1000     9773 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0     1000     1000       63 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0     1000     1000      990 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0     1000     1000     5877 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0     1000     1000     2520 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0     1000     1000     1030 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0     1000     1000     2617 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0     1000     1000    18083 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0     1000     1000      738 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0     1000     1000     4644 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0     1000     1000     1907 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0     1000     1000     3858 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0     1000     1000     3600 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0     1000     1000       50 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0     1000     1000    12190 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0     1000     1000     2145 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0     1000     1000     6096 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0     1000     1000     7638 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0     1000     1000    18443 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0     1000     1000     4073 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0     1000     1000     1791 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0     1000     1000     4133 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0     1000     1000     1404 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0     1000     1000     1456 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0     1000     1000     2198 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0     1000     1000     1063 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0     1000     1000     1405 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0     1000     1000     3064 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0     1000     1000     5109 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0     1000     1000     9784 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0     1000     1000       51 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0     1000     1000     1354 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0     1000     1000     4105 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0     1000     1000    27407 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0     1000     1000    25091 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0     1000     1000     7074 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0     1000     1000     2807 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0     1000     1000    16611 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0     1000     1000    17646 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0     1000     1000    35600 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0     1000     1000     2858 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0     1000     1000    24045 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0     1000     1000      583 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0     1000     1000    24129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0     1000     1000     5220 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0     1000     1000    18963 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0     1000     1000    27878 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0     1000     1000     5705 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0     1000     1000     9914 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0     1000     1000     2526 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0     1000     1000     5455 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0     1000     1000    11533 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0     1000     1000     8020 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0     1000     1000     1015 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0     1000     1000     1665 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0     1000     1000     1884 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0     1000     1000     5377 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0     1000     1000      242 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0     1000     1000     5764 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0     1000     1000     3206 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0     1000     1000     1115 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0     1000     1000     2203 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0     1000     1000     1169 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0     1000     1000     3064 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0     1000     1000     5122 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0     1000     1000      716 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0     1000     1000     3110 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0     1000     1000     4831 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0     1000     1000      795 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0     1000     1000    11632 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0     1000     1000    21617 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0     1000     1000     1193 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0     1000     1000     2108 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0     1000     1000     5662 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0     1000     1000     9197 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0     1000     1000     7702 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0     1000     1000     8821 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0     1000     1000     1759 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0     1000     1000     3459 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0     1000     1000     4549 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0     1000     1000      596 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0     1000     1000     3518 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0     1000     1000    18116 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0     1000     1000     5238 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0     1000     1000    11728 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0     1000     1000    22811 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0     1000     1000    13079 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0     1000     1000     4966 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0     1000     1000      465 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0     1000     1000     1379 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0     1000     1000     5033 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0     1000     1000     1535 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0     1000     1000      242 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0     1000     1000     5271 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0     1000     1000     1033 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0     1000     1000      778 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0     1000     1000    16416 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0     1000     1000     3946 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0     1000     1000     4154 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0     1000     1000     7105 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0     1000     1000      774 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0     1000     1000       94 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0     1000     1000      255 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0     1000     1000   286370 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0     1000     1000     4279 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0     1000     1000     3705 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0     1000     1000    31274 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0     1000     1000     1741 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0     1000     1000     9608 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0     1000     1000     3817 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0     1000     1000     4801 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0     1000     1000     2406 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0     1000     1000     3559 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0     1000     1000     1838 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0     1000     1000     1619 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0     1000     1000     3864 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0     1000     1000    12021 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0     1000     1000     3676 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0     1000     1000    13566 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0     1000     1000     1731 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0     1000     1000    36913 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0     1000     1000     1731 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0     1000     1000    20735 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0     1000     1000     1737 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0     1000     1000    13919 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0     1000     1000    25796 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0     1000     1000    42498 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0     1000     1000     1730 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0     1000     1000    26797 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0     1000     1000   104562 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0     1000     1000    98484 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0     1000     1000    98196 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0     1000     1000   101363 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0     1000     1000   128035 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0     1000     1000   102774 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0     1000     1000    95372 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0     1000     1000     5260 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0     1000     1000     3367 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0     1000     1000     2056 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0     1000     1000    30068 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0     1000     1000    13280 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0     1000     1000     6199 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0     1000     1000     4129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0     1000     1000     3749 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0     1000     1000    13288 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0     1000     1000     8289 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0     1000     1000     2709 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0     1000     1000      242 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0     1000     1000      239 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0     1000     1000     2522 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0     1000     1000    10830 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0     1000     1000     1915 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0     1000     1000     5404 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0     1000     1000     6438 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0     1000     1000      581 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0     1000     1000    41259 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0     1000     1000    51697 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0     1000     1000    20834 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0     1000     1000    51991 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0     1000     1000    14811 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0     1000     1000     5058 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0     1000     1000    39801 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0     1000     1000    10820 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0     1000     1000    18102 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0     1000     1000    97792 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t32.exe
+-rw-r--r--   0     1000     1000   182784 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rw-r--r--   0     1000     1000   108032 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0     1000     1000    66262 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0     1000     1000    23513 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0     1000     1000    91648 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w32.exe
+-rw-r--r--   0     1000     1000   168448 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rw-r--r--   0     1000     1000   101888 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0     1000     1000    43898 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0     1000     1000      981 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0     1000     1000       64 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0     1000     1000    48841 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0     1000     1000      849 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0     1000     1000     3374 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0     1000     1000      321 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0     1000     1000    12950 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0     1000     1000    44375 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0     1000     1000     1881 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0     1000     1000       21 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0     1000     1000   206539 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0     1000     1000     1132 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0     1000     1000     1081 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0     1000     1000     6080 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0     1000     1000    34557 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0     1000     1000      661 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0     1000     1000      497 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0     1000     1000    11488 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0     1000     1000     4378 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0     1000     1000     1431 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0     1000     1000     8487 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0     1000     1000     4676 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0     1000     1000    30110 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0     1000     1000    15699 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0     1000     1000     4200 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0     1000     1000    14665 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0     1000     1000      130 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0     1000     1000      138 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/_compat.py
+-rw-r--r--   0     1000     1000     3443 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0     1000     1000     6083 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0     1000     1000     3994 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0     1000     1000      607 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0     1000     1000     6081 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
+-rw-r--r--   0     1000     1000      872 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-r--r--   0     1000     1000    10801 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-r--r--   0     1000     1000     2520 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0     1000     1000    12721 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
+-rw-r--r--   0     1000     1000   108287 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0     1000     1000      562 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0     1000     1000    12831 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0     1000     1000     1176 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0     1000     1000     4068 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0     1000     1000     4910 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0     1000     1000     2655 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0     1000     1000     6910 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0     1000     1000       78 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0     1000     1000     6439 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0     1000     1000     2999 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0     1000     1000      353 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0     1000     1000    23685 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0     1000     1000     1697 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0     1000     1000     1938 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0     1000     1000    40386 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0     1000     1000     2917 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0     1000     1000     4810 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0     1000     1000     4104 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0     1000     1000     3314 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0     1000     1000     5086 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0     1000     1000    35441 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0     1000     1000    21938 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0     1000     1000     5871 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0     1000     1000    19351 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0     1000     1000     5073 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0     1000     1000     2212 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0     1000     1000     5014 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0     1000     1000     7335 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0     1000     1000     4674 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0     1000     1000    11753 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0     1000     1000    32005 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0     1000     1000    11174 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0     1000     1000    70232 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0     1000     1000    53376 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0     1000     1000      986 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0     1000     1000     2591 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0     1000     1000     3072 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0     1000     1000     3092 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0     1000     1000     4630 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0     1000     1000     6257 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0     1000     1000     3419 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0     1000     1000     6184 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0     1000     1000    63187 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0     1000     1000     9110 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0     1000     1000     9171 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0     1000     1000     6426 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0     1000     1000    12936 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0     1000     1000   213344 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0     1000     1000    23685 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0     1000     1000     9023 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0     1000     1000    39129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0     1000     1000    25341 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0     1000     1000    13402 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0     1000     1000    10787 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0     1000     1000     6805 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0     1000     1000     5178 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0     1000     1000      440 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0     1000     1000     1397 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0     1000     1000    21443 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0     1000     1000     6377 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0     1000     1000    10187 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0     1000     1000      575 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0     1000     1000     1286 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0     1000     1000    18560 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0     1000     1000     3823 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0     1000     1000     3879 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0     1000     1000      733 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0     1000     1000    35287 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0     1000     1000      695 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0     1000     1000    30180 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0     1000     1000     4235 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0     1000     1000     2912 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0     1000     1000    33240 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0     1000     1000      537 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0     1000     1000      156 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0     1000     1000     5872 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0     1000     1000     1583 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0     1000     1000    17592 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0     1000     1000     4794 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0     1000     1000     5944 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0     1000     1000     8808 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0     1000     1000    10096 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0     1000     1000   140235 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0     1000     1000     1064 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0     1000     1000     2114 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0     1000     1000      265 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0     1000     1000     9695 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0     1000     1000     3225 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0     1000     1000     1236 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0     1000     1000     7063 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0     1000     1000      423 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0     1000     1000     5472 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0     1000     1000    19919 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0     1000     1000      351 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0     1000     1000      417 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0     1000     1000    22820 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0     1000     1000     1926 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0     1000     1000     2783 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0     1000     1000     1840 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0     1000     1000      890 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0     1000     1000    10368 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0     1000     1000     6820 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0     1000     1000     3264 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0     1000     1000     9864 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0     1000     1000     4503 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0     1000     1000    17957 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0     1000     1000     1054 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0     1000     1000     7131 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0     1000     1000    95885 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0     1000     1000     1288 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0     1000     1000     5497 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0     1000     1000     6630 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0     1000     1000     7954 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0     1000     1000      972 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0     1000     1000     2501 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0     1000     1000      642 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0     1000     1000     1616 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0     1000     1000     2507 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0     1000     1000     9585 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0     1000     1000     5051 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0     1000     1000     3252 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0     1000     1000    14074 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0     1000     1000    14172 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0     1000     1000     3667 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0     1000     1000    11471 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0     1000     1000     8198 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0     1000     1000     5305 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0     1000     1000     4970 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0     1000     1000      828 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0     1000     1000     3396 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0     1000     1000     8744 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0     1000     1000    36576 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0     1000     1000    59746 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0     1000     1000     8161 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0     1000     1000    11303 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0     1000     1000     1391 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0     1000     1000      166 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0     1000     1000     4449 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0     1000     1000     4773 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0     1000     1000     2842 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0     1000     1000     1591 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0     1000     1000    24224 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0     1000     1000     4374 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0     1000     1000     4425 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0     1000     1000    26240 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0     1000     1000     1258 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0     1000     1000    34697 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0     1000     1000    39515 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0     1000     1000     3370 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0     1000     1000    44666 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0     1000     1000     3627 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0     1000     1000      102 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0     1000     1000    26060 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0     1000     1000     9169 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0     1000     1000    34549 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/six.py
+-rw-r--r--   0     1000     1000    18364 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0     1000     1000     3314 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0     1000     1000     1944 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0     1000     1000     1496 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0     1000     1000     1376 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0     1000     1000     1908 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0     1000     1000     1383 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0     1000     1000     7550 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0     1000     1000     2790 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0     1000     1000     2145 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0     1000     1000     8011 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0     1000     1000      396 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0     1000     1000    22633 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0     1000     1000     2943 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0     1000     1000      254 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0     1000     1000    80114 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0     1000     1000     3333 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0     1000     1000    10811 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0     1000     1000       64 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0     1000     1000    20070 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0     1000     1000    39093 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0     1000     1000      957 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0     1000     1000    17632 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0     1000     1000    13922 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0     1000     1000    11034 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0     1000     1000     4538 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0     1000     1000    17182 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0     1000     1000    34448 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0     1000     1000     7097 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0     1000     1000     8217 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0     1000     1000     8579 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0     1000     1000     2440 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0     1000     1000     1417 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0     1000     1000    34665 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0     1000     1000    19786 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0     1000     1000     5985 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0     1000     1000    30109 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0     1000     1000     1155 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0     1000     1000     4901 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0     1000     1000     1605 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0     1000     1000      498 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0     1000     1000     3997 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0     1000     1000     3510 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0     1000     1000    22001 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0     1000     1000    17177 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0     1000     1000     5758 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0     1000     1000     6895 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0     1000     1000    10003 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0     1000     1000    14287 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0     1000     1000     5403 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0     1000     1000      469 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0     1000     1000    10579 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0     1000     1000     8979 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0     1000     1000     1305 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0     1000     1000     6563 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0     1000     1000     4307 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0     1000     1000      286 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/py.typed
+-rw-r--r--   0     1000     1000        4 2023-01-17 08:30:19.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/INSTALLER
+-rw-r--r--   0     1000     1000     1093 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt
+-rw-r--r--   0     1000     1000     4072 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/METADATA
+-rw-r--r--   0     1000     1000    76117 2023-01-17 08:30:19.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/RECORD
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:19.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/REQUESTED
+-rw-r--r--   0     1000     1000       92 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/WHEEL
+-rw-r--r--   0     1000     1000      125 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/entry_points.txt
+-rw-r--r--   0     1000     1000        4 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/top_level.txt
+-rw-r--r--   0     1000     1000   108568 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0     1000     1000    24701 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0     1000     1000      506 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0     1000     1000     4504 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0     1000     1000     2741 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0     1000     1000     2706 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0     1000     1000      884 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0     1000     1000     3494 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0     1000     1000     3886 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0     1000     1000     3566 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0     1000     1000     2836 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0     1000     1000     5420 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0     1000     1000    13515 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0     1000     1000    15526 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0     1000     1000       83 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0     1000     1000   132569 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0     1000     1000    18410 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0     1000     1000      661 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0     1000     1000      497 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0     1000     1000    11488 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0     1000     1000     4378 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0     1000     1000     1431 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0     1000     1000     8496 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0     1000     1000     4706 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0     1000     1000    30110 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0     1000     1000    15699 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0     1000     1000     4200 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0     1000     1000    14665 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0     1000     1000     9159 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0     1000     1000     6426 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0     1000     1000    12936 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0     1000     1000   213310 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/core.py
+-rw-r--r--   0     1000     1000    23668 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0     1000     1000     9023 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0     1000     1000    39129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0     1000     1000    25341 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0     1000     1000    13402 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0     1000     1000    10787 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0     1000     1000     6805 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0     1000     1000     8425 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0     1000     1000     2426 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0     1000     1000      119 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia/__init__.py
+-rw-r--r--   0     1000     1000        4 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/INSTALLER
+-rw-r--r--   0     1000     1000     3895 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/METADATA
+-rw-r--r--   0     1000     1000      735 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/RECORD
+-rw-r--r--   0     1000     1000        0 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/REQUESTED
+-rw-r--r--   0     1000     1000      101 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/WHEEL
+-rw-r--r--   0     1000     1000       98 2023-02-01 09:23:25.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/direct_url.json
+-rw-r--r--   0     1000     1000     8429 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/__init__.py
+-rw-r--r--   0     1000     1000      218 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0     1000     1000      537 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0     1000     1000     1330 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0     1000     1000      411 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0     1000     1000      239 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0     1000     1000    19672 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0     1000     1000     8603 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0     1000     1000    14789 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0     1000     1000    47369 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0     1000     1000    17973 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0     1000     1000      430 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0     1000     1000     1614 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0     1000     1000     5441 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0     1000     1000     4701 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0     1000     1000    22051 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0     1000     1000     5617 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0     1000     1000     7728 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0     1000     1000    31558 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0     1000     1000    16568 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0     1000     1000     5624 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0     1000     1000     4888 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0     1000     1000     2603 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0     1000     1000    13137 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0     1000     1000    30221 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0     1000     1000     2779 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0     1000     1000     2785 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0     1000     1000     1189 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0     1000     1000     8434 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0     1000     1000     1936 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0     1000     1000      672 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0     1000     1000    11765 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0     1000     1000    19241 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0     1000     1000     7477 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0     1000     1000     4920 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0     1000     1000     9451 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0     1000     1000    12537 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0     1000     1000      139 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0     1000     1000     3423 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0     1000     1000     8082 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0     1000     1000    50186 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0     1000     1000     3589 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0     1000     1000    10270 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0     1000     1000    17910 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0     1000     1000     8226 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0     1000     1000    13713 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0     1000     1000     1972 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0     1000     1000    30235 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0     1000     1000    23602 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0     1000     1000      217 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0     1000     1000      639 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0     1000     1000     3517 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0     1000     1000    18858 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0     1000     1000    12096 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0     1000     1000    15641 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0     1000     1000    18128 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0     1000     1000    12952 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0     1000     1000     5248 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0     1000     1000     1972 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0     1000     1000     2392 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_imp.py
+-rw-r--r--   0     1000     1000     1311 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_importlib.py
+-rw-r--r--   0     1000     1000      675 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_itertools.py
+-rw-r--r--   0     1000     1000      749 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_path.py
+-rw-r--r--   0     1000     1000      501 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_reqs.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0     1000     1000    30130 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0     1000     1000     1862 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0     1000     1000      743 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0     1000     1000     1828 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0     1000     1000     2895 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0     1000     1000     2068 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0     1000     1000     1154 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0     1000     1000     2166 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0     1000     1000      506 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0     1000     1000     4504 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0     1000     1000     2741 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0     1000     1000     2706 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0     1000     1000      884 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0     1000     1000     3494 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0     1000     1000     3886 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0     1000     1000     3566 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0     1000     1000     2836 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0     1000     1000     5420 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0     1000     1000    13512 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0     1000     1000    15517 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0     1000     1000       82 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0     1000     1000   117959 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0     1000     1000    16256 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0     1000     1000    15130 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0     1000     1000      661 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0     1000     1000      497 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0     1000     1000    11488 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0     1000     1000     4378 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0     1000     1000     1431 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0     1000     1000     8493 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0     1000     1000     4700 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0     1000     1000    30110 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0     1000     1000    15699 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0     1000     1000     4200 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0     1000     1000    14665 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0     1000     1000     9159 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0     1000     1000     6426 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0     1000     1000    12936 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0     1000     1000   213310 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/core.py
+-rw-r--r--   0     1000     1000    23668 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0     1000     1000     9023 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0     1000     1000    39129 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0     1000     1000    25341 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0     1000     1000    13402 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0     1000     1000    10787 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0     1000     1000     6805 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/util.py
+-rw-r--r--   0     1000     1000      396 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0     1000     1000    22633 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0     1000     1000     2943 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0     1000     1000      254 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0     1000     1000    87149 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0     1000     1000     8425 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0     1000     1000     7346 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/archive_util.py
+-rw-r--r--   0     1000     1000    19539 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/build_meta.py
+-rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0     1000     1000    74752 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0     1000     1000   137216 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli.exe
+-rw-r--r--   0     1000     1000      396 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0     1000     1000     2381 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/alias.py
+-rw-r--r--   0     1000     1000    16623 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0     1000     1000     1182 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0     1000     1000     6595 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build.py
+-rw-r--r--   0     1000     1000     4415 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0     1000     1000    15821 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0     1000     1000    14115 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0     1000     1000     7012 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/develop.py
+-rw-r--r--   0     1000     1000     4800 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0     1000     1000    85662 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0     1000     1000    31188 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0     1000     1000    26795 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0     1000     1000     5163 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install.py
+-rw-r--r--   0     1000     1000     2226 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0     1000     1000     3875 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0     1000     1000     2612 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0     1000     1000      628 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0     1000     1000     4946 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0     1000     1000      468 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/register.py
+-rw-r--r--   0     1000     1000     2128 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0     1000     1000      658 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0     1000     1000     7071 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0     1000     1000     5086 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0     1000     1000     8102 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/test.py
+-rw-r--r--   0     1000     1000      462 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/upload.py
+-rw-r--r--   0     1000     1000     7494 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0     1000     1000     1121 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0     1000     1000    13398 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0     1000     1000     1038 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0     1000     1000    11266 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0     1000     1000     1153 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0     1000     1000     1612 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0     1000     1000   269900 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0     1000     1000     8736 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0     1000     1000    16319 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/expand.py
+-rw-r--r--   0     1000     1000    19304 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0     1000     1000    25198 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0     1000     1000      949 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/dep_util.py
+-rw-r--r--   0     1000     1000     5499 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/depends.py
+-rw-r--r--   0     1000     1000    20799 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/discovery.py
+-rw-r--r--   0     1000     1000    45578 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/dist.py
+-rw-r--r--   0     1000     1000     2464 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/errors.py
+-rw-r--r--   0     1000     1000     5591 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/extension.py
+-rw-r--r--   0     1000     1000     2512 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0     1000     1000     4873 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/glob.py
+-rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0     1000     1000    75264 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0     1000     1000   137728 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0     1000     1000    65536 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui.exe
+-rw-r--r--   0     1000     1000     3824 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/installer.py
+-rw-r--r--   0     1000     1000      812 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/launch.py
+-rw-r--r--   0     1000     1000     1210 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/logging.py
+-rw-r--r--   0     1000     1000     4857 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/monkey.py
+-rw-r--r--   0     1000     1000    47724 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/msvc.py
+-rw-r--r--   0     1000     1000     3093 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/namespaces.py
+-rw-r--r--   0     1000     1000    40020 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/package_index.py
+-rw-r--r--   0     1000     1000      245 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/py34compat.py
+-rw-r--r--   0     1000     1000    14348 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/sandbox.py
+-rw-r--r--   0     1000     1000      218 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0     1000     1000      138 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/script.tmpl
+-rw-r--r--   0     1000     1000      941 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0     1000     1000      144 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/version.py
+-rw-r--r--   0     1000     1000     8376 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/wheel.py
+-rw-r--r--   0     1000     1000      718 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/windows_support.py
+-rw-r--r--   0     1000     1000        4 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/INSTALLER
+-rw-r--r--   0     1000     1000     1050 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/LICENSE
+-rw-r--r--   0     1000     1000     6301 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/METADATA
+-rw-r--r--   0     1000     1000    37694 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/RECORD
+-rw-r--r--   0     1000     1000        0 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/REQUESTED
+-rw-r--r--   0     1000     1000       92 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/WHEEL
+-rw-r--r--   0     1000     1000     2740 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-r--r--   0     1000     1000       41 2023-01-17 08:30:18.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+-rw-r--r--   0     1000     1000      396 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/__init__.py
+-rw-r--r--   0     1000     1000    22633 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/_parser.py
+-rw-r--r--   0     1000     1000     2943 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/_re.py
+-rw-r--r--   0     1000     1000      254 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/_types.py
+-rw-r--r--   0     1000     1000       26 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/py.typed
+-rw-r--r--   0     1000     1000        4 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rw-r--r--   0     1000     1000     1072 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0     1000     1000     8875 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA
+-rw-r--r--   0     1000     1000      913 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD
+-rw-r--r--   0     1000     1000       81 2023-01-25 10:59:02.000000 pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rw-r--r--   0     1000     1000       70 2023-01-25 11:53:47.000000 pysequoia-0.1.9/.env/pyvenv.cfg
+-rw-r--r--   0     1000     1000      710 2023-01-19 11:23:14.000000 pysequoia-0.1.9/.gitignore
+-rw-r--r--   0     1000     1000      469 2023-01-19 11:23:14.000000 pysequoia-0.1.9/.gitlab-ci.yml
+-rw-r--r--   0     1000     1000     1257 2023-01-19 13:30:28.000000 pysequoia-0.1.9/.woodpecker.yml
+-rw-r--r--   0     1000     1000     3567 2023-01-31 11:32:51.000000 pysequoia-0.1.9/README.md
+-rw-r--r--   0     1000     1000      416 2023-01-31 11:53:11.000000 pysequoia-0.1.9/ci/build.dockerfile
+-rw-r--r--   0     1000     1000      361 2023-01-19 11:23:14.000000 pysequoia-0.1.9/ci/docs.dockerfile
+-rw-r--r--   0     1000     1000      533 2023-01-31 11:48:00.000000 pysequoia-0.1.9/ci/e2e.dockerfile
+-rw-r--r--   0     1000     1000     8334 2023-01-19 11:23:14.000000 pysequoia-0.1.9/doc/tufte.min.css
+-rw-r--r--   0     1000     1000      317 2023-01-25 10:57:15.000000 pysequoia-0.1.9/pyproject.toml
+-rw-r--r--   0     1000     1000      428 2023-01-19 11:23:14.000000 pysequoia-0.1.9/signing-key.asc
+-rw-r--r--   0     1000     1000    14560 2023-02-01 09:20:54.000000 pysequoia-0.1.9/src/lib.rs
+-rw-r--r--   0     1000     1000    32600 2023-01-19 11:23:14.000000 pysequoia-0.1.9/wiktor-fresh.asc
+-rw-r--r--   0     1000     1000   199223 2023-01-19 11:23:14.000000 pysequoia-0.1.9/wiktor.asc
+-rw-r--r--   0     1000     1000    73407 2023-02-01 09:22:55.000000 pysequoia-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 pysequoia-0.1.9/PKG-INFO
```

### Comparing `pysequoia-0.1.8/Cargo.toml` & `pysequoia-0.1.9/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [package]
 name = "pysequoia"
-version = "0.1.8"
+version = "0.1.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pysequoia"
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0.66"
+openpgp-card-pcsc = { version = "0.3.0", path = "local_dependencies/openpgp-card-pcsc" }
+openpgp-card-sequoia = { version = "0.1.0", path = "local_dependencies/openpgp-card-sequoia", default-features = false }
 openpgp-cert-d = "0.1.0"
 pyo3 = { version = "0.17", features = ["extension-module", "anyhow"] }
 pyo3-asyncio = { version = "0.17", features = ["tokio-runtime"] }
 sequoia-net = "0.26.0"
-sequoia-openpgp = { version = "1.13", default-features = false, features = ["crypto-rust", "allow-experimental-crypto", "allow-variable-time-crypto", "compression-deflate"] }
+sequoia-openpgp = { version = "1.13", default-features = false, features = ["crypto-rust", "allow-variable-time-crypto", "allow-experimental-crypto"] }
 testresult = "0.2"
```

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/_distutils_hack/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin/__main__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin/__main__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin/import_hook.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin/import_hook.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/METADATA` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/RECORD` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/maturin-0.14.10.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/__main__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/__pip-runner__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/build_env.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cache.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/autocompletion.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/base_command.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/cmdoptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/command_context.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/main.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/main_parser.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/parser.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/progress_bars.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/req_command.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/cli/spinners.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/cache.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/check.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/completion.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/configuration.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/debug.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/download.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/freeze.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/hash.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/help.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/index.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/inspect.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/install.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/list.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/search.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/show.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/uninstall.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/commands/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/configuration.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/base.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/installed.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/sdist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/distributions/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/collector.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/package_finder.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/index/sources.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/_distutils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/_sysconfig.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/locations/base.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/_json.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/base.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/candidate.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/direct_url.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/format_control.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/index.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/installation_report.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/link.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/scheme.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/search_scope.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/selection_prefs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/target_python.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/models/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/auth.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/cache.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/download.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/lazy_wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/session.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/network/xmlrpc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/check.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/freeze.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/legacy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/operations/prepare.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/pyproject.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/constructors.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_file.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_install.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_set.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/req/req_uninstall.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/base.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/self_outdated_check.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/_log.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/appdirs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/deprecation.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/distutils_args.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/egg_link.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/encoding.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/entrypoints.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/filesystem.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/filetypes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/glibc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/hashes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/logging.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/misc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/models.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/packaging.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/setuptools_build.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/subprocess.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/temp_dir.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/unpacking.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/urls.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/virtualenv.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/utils/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/bazaar.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/git.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/mercurial.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/subversion.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_internal/wheel_builder.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/cacert.pem` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/core.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5freq.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5prober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/enums.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escsm.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansi.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/initialise.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/win32.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/winterm.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/database.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/index.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/locators.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/manifest.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/markers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/metadata.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/resources.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/scripts.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t32.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/version.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w32.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distro/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/distro/distro.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/codec.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/core.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/idnadata.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/intranges.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/idna/uts46data.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/ext.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/fallback.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/__about__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_structures.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/markers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/requirements.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/specifiers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/tags.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/version.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/build.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/check.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/colorlog.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/dirtools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/envbuild.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/meta.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/wrappers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/android.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/api.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/macos.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/unix.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/windows.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/cmdline.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/console.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filter.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatter.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexer.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/modeline.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/plugin.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/regexopt.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/scanner.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/style.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/token.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/unistring.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/actions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/common.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/core.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/results.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/testing.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/adapters.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/api.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/auth.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/certs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/cookies.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/help.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/hooks.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/models.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/packages.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/sessions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/status_codes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/structures.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/requests/utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/providers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/structs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__main__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_export_format.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_inspect.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_log_render.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_loop.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_palettes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_ratio.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_spinners.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_win32_console.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_wrap.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/abc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/align.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/ansi.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/bar.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/box.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/cells.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color_triplet.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/columns.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/console.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/constrain.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/containers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/control.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/default_styles.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/diagnose.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/emoji.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/errors.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/file_proxy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/filesize.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/highlighter.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/json.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/jupyter.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/layout.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live_render.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/logging.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/markup.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/measure.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/padding.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pager.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/palette.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/panel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pretty.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress_bar.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/prompt.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/protocol.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/repr.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/rule.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/scope.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/screen.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/segment.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/spinner.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/status.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/style.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/styled.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/syntax.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/table.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/text.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/theme.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/traceback.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/rich/tree.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/six.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/after.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/nap.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/retry.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/stop.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/wait.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_parser.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_re.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/typing_extensions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/_collections.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connection.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/fields.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/filepost.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/request.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/response.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/request.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/response.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/url.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/labels.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/tests.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/METADATA` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/RECORD` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pip-22.3.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/appdirs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/zipp.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pkg_resources/extern/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/METADATA` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysequoia
-Version: 0.1.4
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PySequoia
@@ -36,14 +36,25 @@
 ```python
 s = Cert.from_file("signing-key.asc")
 r = Cert.from_bytes(open("wiktor.asc", "rb").read())
 encrypted = Context.standard().encrypt(s, r, "content to encrypt")
 print(f"Encrypted data: {encrypted}")
 ```
 
+### sign
+
+Signs the data and returns armored output:
+
+```python
+from pysequoia import sign
+
+s = Cert.from_file("signing-key.asc")
+signed = sign(s.signer(), "data to be signed")
+```
+
 ### merge
 
 Merges data from old certificate with new packets:
 
 ```python
 old = Cert.from_file("wiktor.asc")
 new = Cert.from_file("wiktor-fresh.asc")
@@ -139,7 +150,29 @@
 retrieved later by its fingerprint:
 
 ```python
 s = Store("/tmp/store")
 assert s.get("653909a2f0e37c106f5faf546c8857e0d8e8f074") != None
 ```
 
+### OpenPGP Cards
+
+There's an experimental feature allowing communication with OpenPGP
+Cards (like Yubikey or Nitrokey).
+
+```py
+from pysequoia import Card
+
+# enumerate all cards
+all = Card.all()
+
+# open card by card ident
+card = Card.open("card ident")
+
+print(card.ident)
+print(card.cardholder)
+
+signer = card.signer(input("PIN: "))
+
+signed = sign(signer, "data to be signed")
+```
+
```

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/pysequoia-0.1.4.dist-info/RECORD` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/pysequoia-0.1.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pysequoia-0.1.4.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
-pysequoia-0.1.4.dist-info/METADATA,sha256=_ud6aPKuMpjSgQewUq0mhS8cmiYJeI2RhSPjqslsCeE,3331
-pysequoia-0.1.4.dist-info/RECORD,,
-pysequoia-0.1.4.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pysequoia-0.1.4.dist-info/WHEEL,sha256=__RdKO0gfeLBAOIdHSG_JNwFPIJt5rjlyYRjPgXoELM,101
-pysequoia-0.1.4.dist-info/direct_url.json,sha256=Tcfh49Ka2ZUR0mMKcG3B6PzR--Fxk3O56h3F7mCL4UQ,98
+pysequoia-0.1.9.dist-info/INSTALLER,sha256=zuuue4knoyJ-UwPPXg8fezS7VCrXJQrAP7zeNuwvFQg,4
+pysequoia-0.1.9.dist-info/METADATA,sha256=gRPkWcuWwFM9x1PlSY4Mjg4vfHzXU3sqVCaK1XAToXE,3895
+pysequoia-0.1.9.dist-info/RECORD,,
+pysequoia-0.1.9.dist-info/REQUESTED,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+pysequoia-0.1.9.dist-info/WHEEL,sha256=__RdKO0gfeLBAOIdHSG_JNwFPIJt5rjlyYRjPgXoELM,101
+pysequoia-0.1.9.dist-info/direct_url.json,sha256=l3Gd8Ai2l_7AYCPqFbZHLHb0J4go8_rE6uTWXuKdYqs,98
 pysequoia/__init__.py,sha256=t3pi6oXWy4xLuPamz-dU-TTVZUfRqsKYEOa3IpQQKIk,119
 pysequoia/__pycache__/__init__.cpython-310.pyc,,
-pysequoia/pysequoia.cpython-310-x86_64-linux-gnu.so,sha256=0fuBWEIxmcVIo-B2DMw2wUw6oyRpJVXwlp4VZoAzufI,186481585
+pysequoia/pysequoia.cpython-310-x86_64-linux-gnu.so,sha256=KzWJUtan5iNWLuE9Dy1-QJex_44A7m6bvMpkVV_CIPM,205425729
```

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/_collections.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/archive_util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/ccompiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/cmd.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_clib.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_ext.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_py.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/check.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/clean.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/config.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_data.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_headers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_lib.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/py37compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/register.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/sdist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/upload.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/config.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/core.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/dep_util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/dir_util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/dist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/errors.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/extension.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/file_util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/filelist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/log.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvccompiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/py39compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/spawn.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/sysconfig.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/text_file.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/unixccompiler.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/version.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_distutils/versionpredicate.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_entry_points.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_imp.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_importlib.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_itertools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_path.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/context.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/ordered_set.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/markers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/tags.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/version.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/actions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/common.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/core.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/results.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/testing.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_re.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/typing_extensions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/_vendor/zipp.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/archive_util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/build_meta.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli-32.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli-64.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli-arm64.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/cli.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/alias.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/bdist_egg.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/bdist_rpm.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build_clib.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build_ext.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/build_py.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/develop.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/dist_info.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/easy_install.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/editable_wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/egg_info.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install_egg_info.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install_lib.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/install_scripts.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/launcher manifest.xml` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/py36compat.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/rotate.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/saveopts.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/sdist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/setopt.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/test.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/command/upload_docs.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/expand.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/pyprojecttoml.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/config/setupcfg.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/dep_util.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/depends.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/discovery.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/dist.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/errors.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/extension.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/extern/__init__.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/glob.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui-32.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui-64.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui-arm64.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/gui.exe` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/installer.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/launch.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/logging.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/monkey.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/msvc.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/namespaces.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/package_index.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/sandbox.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/unicode_utils.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/wheel.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools/windows_support.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/LICENSE` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/METADATA` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/RECORD` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/entry_points.txt` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/setuptools-65.5.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/_parser.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli/_re.py` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD` & `pysequoia-0.1.9/.env/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.gitignore` & `pysequoia-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/.woodpecker.yml` & `pysequoia-0.1.9/.woodpecker.yml`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/README.md` & `pysequoia-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 ```python
 s = Cert.from_file("signing-key.asc")
 r = Cert.from_bytes(open("wiktor.asc", "rb").read())
 encrypted = Context.standard().encrypt(s, r, "content to encrypt")
 print(f"Encrypted data: {encrypted}")
 ```
 
+### sign
+
+Signs the data and returns armored output:
+
+```python
+from pysequoia import sign
+
+s = Cert.from_file("signing-key.asc")
+signed = sign(s.signer(), "data to be signed")
+```
+
 ### merge
 
 Merges data from old certificate with new packets:
 
 ```python
 old = Cert.from_file("wiktor.asc")
 new = Cert.from_file("wiktor-fresh.asc")
@@ -129,7 +140,29 @@
 The certificate is now stored in the given directory and can be
 retrieved later by its fingerprint:
 
 ```python
 s = Store("/tmp/store")
 assert s.get("653909a2f0e37c106f5faf546c8857e0d8e8f074") != None
 ```
+
+### OpenPGP Cards
+
+There's an experimental feature allowing communication with OpenPGP
+Cards (like Yubikey or Nitrokey).
+
+```py
+from pysequoia import Card
+
+# enumerate all cards
+all = Card.all()
+
+# open card by card ident
+card = Card.open("card ident")
+
+print(card.ident)
+print(card.cardholder)
+
+signer = card.signer(input("PIN: "))
+
+signed = sign(signer, "data to be signed")
+```
```

### Comparing `pysequoia-0.1.8/doc/tufte.min.css` & `pysequoia-0.1.9/doc/tufte.min.css`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/src/lib.rs` & `pysequoia-0.1.9/src/lib.rs`

 * *Files 25% similar despite different names*

```diff
@@ -59,14 +59,32 @@
         format!("<Cert fingerprint={}>", self.cert.fingerprint())
     }
 
     #[getter]
     pub fn fingerprint(&self) -> PyResult<String> {
         Ok(format!("{:x}", self.cert.fingerprint()))
     }
+
+    pub fn signer(&self) -> PyResult<PySigner> {
+        let policy = StandardPolicy::new();
+        let keypair = self
+            .cert
+            .keys()
+            .unencrypted_secret()
+            .with_policy(&policy, None)
+            .alive()
+            .revoked(false)
+            .for_signing()
+            .next()
+            .unwrap()
+            .key()
+            .clone()
+            .into_keypair()?;
+        Ok(PySigner::new(Box::new(keypair)))
+    }
 }
 
 #[pyclass]
 pub struct KeyServer {
     uri: String,
 }
 
@@ -97,14 +115,55 @@
     }
 
     pub fn __repr__(&self) -> String {
         format!("<KeyServer uri={}>", self.uri)
     }
 }
 
+use std::sync::{Arc, Mutex};
+
+#[pyclass]
+#[derive(Clone)]
+pub struct PySigner {
+    inner: Arc<Mutex<Box<dyn openpgp::crypto::Signer + Send + Sync + 'static>>>,
+    public: openpgp::packet::Key<
+        openpgp::packet::key::PublicParts,
+        openpgp::packet::key::UnspecifiedRole,
+    >,
+}
+
+impl PySigner {
+    pub fn new(inner: Box<dyn openpgp::crypto::Signer + Send + Sync + 'static>) -> Self {
+        let public = inner.public().clone();
+        Self {
+            inner: Arc::new(Mutex::new(inner)),
+            public,
+        }
+    }
+}
+
+impl openpgp::crypto::Signer for PySigner {
+    fn public(
+        &self,
+    ) -> &openpgp::packet::Key<
+        openpgp::packet::key::PublicParts,
+        openpgp::packet::key::UnspecifiedRole,
+    > {
+        &self.public
+    }
+
+    fn sign(
+        &mut self,
+        hash_algo: openpgp::types::HashAlgorithm,
+        digest: &[u8],
+    ) -> openpgp::Result<openpgp::crypto::mpi::Signature> {
+        self.inner.lock().unwrap().sign(hash_algo, digest)
+    }
+}
+
 #[pyclass]
 struct Context {
     policy: Box<dyn Policy + 'static>,
 }
 
 #[pymethods]
 impl Context {
@@ -201,21 +260,144 @@
     }
 
     pub fn __repr__(&self) -> String {
         format!("<Store base={}>", self.loc.display())
     }
 }
 
+use openpgp_card_pcsc::PcscBackend;
+
+#[pyclass]
+struct Card {
+    open: openpgp_card_sequoia::Card<openpgp_card_sequoia::state::Open>,
+}
+
+#[pymethods]
+impl Card {
+    #[staticmethod]
+    pub fn open(ident: &str) -> anyhow::Result<Self> {
+        Ok(Self {
+            open: PcscBackend::open_by_ident(ident, None)?.into(),
+        })
+    }
+
+    #[getter]
+    pub fn cardholder(&mut self) -> anyhow::Result<Option<String>> {
+        let mut transaction = self.open.transaction()?;
+        Ok(transaction.cardholder_name()?)
+    }
+
+    #[getter]
+    pub fn ident(&mut self) -> anyhow::Result<String> {
+        let transaction = self.open.transaction()?;
+        Ok(transaction.application_identifier()?.ident())
+    }
+
+    #[staticmethod]
+    pub fn all() -> anyhow::Result<Vec<Card>> {
+        Ok(PcscBackend::cards(None)?
+            .into_iter()
+            .map(|card| Self { open: card.into() })
+            .collect())
+    }
+
+    pub fn signer(&mut self, pin: String) -> anyhow::Result<PySigner> {
+        use sequoia_openpgp::crypto::Signer;
+
+        struct CardSigner {
+            public: openpgp::packet::Key<
+                openpgp::packet::key::PublicParts,
+                openpgp::packet::key::UnspecifiedRole,
+            >,
+            ident: String,
+            pin: String,
+        }
+
+        impl openpgp::crypto::Signer for CardSigner {
+            fn public(
+                &self,
+            ) -> &openpgp::packet::Key<
+                openpgp::packet::key::PublicParts,
+                openpgp::packet::key::UnspecifiedRole,
+            > {
+                &self.public
+            }
+
+            fn sign(
+                &mut self,
+                hash_algo: openpgp::types::HashAlgorithm,
+                digest: &[u8],
+            ) -> openpgp::Result<openpgp::crypto::mpi::Signature> {
+                let backend = openpgp_card_pcsc::PcscBackend::open_by_ident(&self.ident, None)?;
+                let mut card: openpgp_card_sequoia::Card<openpgp_card_sequoia::state::Open> =
+                    backend.into();
+                let mut transaction = card.transaction()?;
+
+                transaction.verify_user_for_signing(self.pin.as_bytes())?;
+                let mut user = transaction.signing_card().expect("This should not fail");
+
+                let mut signer = user.signer(&|| {})?;
+                signer.sign(hash_algo, digest)
+            }
+        }
+
+        let public = {
+            let mut transaction = self.open.transaction()?;
+
+            transaction.verify_user_for_signing(pin.as_bytes())?;
+
+            let mut user = transaction.signing_card().expect("This should not fail");
+
+            let signer = user.signer(&|| {})?;
+            signer.public().clone()
+        };
+        Ok(PySigner::new(Box::new(CardSigner {
+            public,
+            ident: self.ident()?,
+            pin,
+        })))
+    }
+
+    pub fn __repr__(&mut self) -> anyhow::Result<String> {
+        Ok(format!("<Card ident={}>", self.ident()?))
+    }
+}
+
+#[pyfunction]
+fn sign(signer: PySigner, data: String) -> PyResult<String> {
+    use openpgp::serialize::stream::Signer;
+
+    let mut sink = vec![];
+    {
+        let message = Message::new(&mut sink);
+
+        let message = Armorer::new(message)
+            .kind(openpgp::armor::Kind::Signature)
+            .build()?;
+        let message = Signer::new(message, signer).build()?;
+
+        let mut message = LiteralWriter::new(message).build()?;
+
+        message.write_all(data.as_bytes())?;
+
+        message.finalize()?;
+    }
+
+    Ok(String::from_utf8_lossy(&sink).into())
+}
+
 #[pymodule]
 fn pysequoia(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<Cert>()?;
     m.add_class::<Context>()?;
     m.add_class::<KeyServer>()?;
     m.add_class::<WKD>()?;
     m.add_class::<Store>()?;
+    m.add_class::<Card>()?;
+    m.add_function(wrap_pyfunction!(sign, m)?)?;
     Ok(())
 }
 
 pub fn encrypt_for<U>(
     signing_cert: &Cert,
     recipient_certs: &Cert,
     content: U,
```

### Comparing `pysequoia-0.1.8/wiktor-fresh.asc` & `pysequoia-0.1.9/wiktor-fresh.asc`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/wiktor.asc` & `pysequoia-0.1.9/wiktor.asc`

 * *Files identical despite different names*

### Comparing `pysequoia-0.1.8/Cargo.lock` & `pysequoia-0.1.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "adler"
-version = "1.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
-
-[[package]]
 name = "aead"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fc95d1bdb8e6666b2b217308eeeb09f2d6728d104be3e31916cc74d15420331"
 dependencies = [
  "generic-array",
 ]
@@ -121,14 +115,34 @@
 [[package]]
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
+name = "bindgen"
+version = "0.63.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "36d860121800b2a9a94f9b5604b332d5cffb234ce17609ea479d723dbc9d3885"
+dependencies = [
+ "bitflags",
+ "cexpr",
+ "clang-sys",
+ "lazy_static",
+ "lazycell",
+ "peeking_take_while",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "rustc-hash",
+ "shlex",
+ "syn",
+]
+
+[[package]]
 name = "bit-set"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0700ddab506f33b20a03b13996eccd309a48e5ff77d0d95926aa0210fb4e95f1"
 dependencies = [
  "bit-vec",
 ]
@@ -154,14 +168,25 @@
  "funty",
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
+name = "blanket"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b04ce3d2372d05d1ef4ea3fdf427da6ae3c17ca06d688a107b5344836276bc3"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "block-buffer"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
 dependencies = [
  "generic-array",
 ]
@@ -195,15 +220,14 @@
 
 [[package]]
 name = "buffered-reader"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9f82920285502602088677aeb65df0909b39c347b38565e553ba0363c242f65"
 dependencies = [
- "flate2",
  "libc",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -235,14 +259,23 @@
 [[package]]
 name = "cc"
 version = "1.0.77"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9f73505338f7d905b19d18738976aae232eb46b8efc15554ffc56deb5d9ebe4"
 
 [[package]]
+name = "cexpr"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
@@ -265,14 +298,25 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "12f8e7987cbd042a63249497f41aed09f8e65add917ea6566effbc56578d6801"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
+name = "clang-sys"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fa2e27ae6ab525c3d369ded447057bca5438d86dc3a68f6faafb8269ba82ebf3"
+dependencies = [
+ "glob",
+ "libc",
+ "libloading",
+]
+
+[[package]]
 name = "cmac"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73d4de4f7724e5fe70addfb2bd37c2abd2f95084a429d7773b0b9645499b4272"
 dependencies = [
  "crypto-mac 0.10.1",
  "dbl",
@@ -316,23 +360,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
 dependencies = [
  "libc",
 ]
 
 [[package]]
-name = "crc32fast"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "crypto-mac"
@@ -670,24 +705,14 @@
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
-name = "flate2"
-version = "1.0.25"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
-dependencies = [
- "crc32fast",
- "miniz_oxide",
-]
-
-[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "foreign-types"
@@ -841,14 +866,20 @@
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "group"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61b3c1e8b4f1ca07e6605ea1be903a5f6956aec5c8a67fd44d56076631675ed8"
 dependencies = [
  "ff",
  "rand_core 0.6.4",
@@ -901,14 +932,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hex-slice"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5491a308e0214554f07a81d8944abe45f552871c12e3c3c6e7e5d354039a6c4c"
+
+[[package]]
 name = "hmac"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a2a2320eb7ec0ebe8da8f744d7812d9fc4cb4d09344ac01898dbcb6a20ae69b"
 dependencies = [
  "crypto-mac 0.11.1",
  "digest",
@@ -1101,14 +1138,23 @@
 [[package]]
 name = "ipnet"
 version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30e22bd8629359895450b59ea7a776c850561b96a3b1d31321c1949d9e6c9146"
 
 [[package]]
+name = "iso7816-tlv"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "395d8e0ae63eb5016fbcf4a72864155880e34bce0158206fcfa7218efdd52e82"
+dependencies = [
+ "untrusted 0.9.0",
+]
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -1162,20 +1208,36 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 dependencies = [
  "spin",
 ]
 
 [[package]]
+name = "lazycell"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
+
+[[package]]
 name = "libc"
 version = "0.2.137"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc7fcc620a3bff7cdd7a365be3376c97191aeaccc2a603e600951e452615bf89"
 
 [[package]]
+name = "libloading"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
+dependencies = [
+ "cfg-if",
+ "winapi",
+]
+
+[[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "link-cplusplus"
@@ -1267,21 +1329,18 @@
 [[package]]
 name = "memsec"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ac78937f19a0c7807e45a931eac41f766f210173ec664ec046d58e6d388a5cb"
 
 [[package]]
-name = "miniz_oxide"
-version = "0.6.2"
+name = "minimal-lexical"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
-dependencies = [
- "adler",
-]
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "mio"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
 dependencies = [
@@ -1306,14 +1365,40 @@
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
+name = "nettle"
+version = "7.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f5d193a809310369c5d16e45bc0a88cb27935edd5d3375bcfc2371b167694035"
+dependencies = [
+ "getrandom 0.2.8",
+ "libc",
+ "nettle-sys",
+ "thiserror",
+]
+
+[[package]]
+name = "nettle-sys"
+version = "2.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5df7cd7e8d5d2997055f31318d1ec648c84886e662bbef7b4a60e3cbc899522b"
+dependencies = [
+ "bindgen",
+ "cc",
+ "libc",
+ "pkg-config",
+ "tempfile",
+ "vcpkg",
+]
+
+[[package]]
 name = "new_debug_unreachable"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
 
 [[package]]
 name = "nibble_vec"
@@ -1321,14 +1406,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a5d83df9f36fe23f0c3648c6bbb8b0298bb5f1939c8f2704431371f4b84d43"
 dependencies = [
  "smallvec",
 ]
 
 [[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "num-bigint"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090c7f9998ee0ff65aa5b723e4009f7b217707f1fb5ea551329cc4d6231fb304"
 dependencies = [
  "autocfg 1.1.0",
  "num-integer",
@@ -1403,14 +1498,49 @@
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
+name = "openpgp-card"
+version = "0.3.3"
+dependencies = [
+ "blanket",
+ "chrono",
+ "hex-slice",
+ "log",
+ "nom",
+ "thiserror",
+]
+
+[[package]]
+name = "openpgp-card-pcsc"
+version = "0.3.0"
+dependencies = [
+ "iso7816-tlv",
+ "log",
+ "openpgp-card",
+ "pcsc",
+]
+
+[[package]]
+name = "openpgp-card-sequoia"
+version = "0.1.0"
+dependencies = [
+ "anyhow",
+ "chrono",
+ "log",
+ "nettle",
+ "openpgp-card",
+ "sequoia-openpgp",
+ "thiserror",
+]
+
+[[package]]
 name = "openpgp-cert-d"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccaa2a2e4502a5daf19c5753250fc6e37daa1d06f866ec97cd5e3416e6d05883"
 dependencies = [
  "anyhow",
  "dirs",
@@ -1496,14 +1626,39 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
+name = "pcsc"
+version = "2.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "37cab0be9d04e808a8d8059fa54befcd71dc8b168f9f0c04bdb7e59832abbab4"
+dependencies = [
+ "bitflags",
+ "pcsc-sys",
+]
+
+[[package]]
+name = "pcsc-sys"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1b7bfecba2c0f1b5efb0e7caf7533ab1c295024165bcbb066231f60d33e23ea"
+dependencies = [
+ "pkg-config",
+]
+
+[[package]]
+name = "peeking_take_while"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
+
+[[package]]
 name = "pem"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd56cbd21fea48d0c440b41cd69c589faacade08c992d9a54e471b79d0fd13eb"
 dependencies = [
  "base64",
  "once_cell",
@@ -1656,17 +1811,19 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pysequoia"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "anyhow",
+ "openpgp-card-pcsc",
+ "openpgp-card-sequoia",
  "openpgp-cert-d",
  "pyo3",
  "pyo3-asyncio",
  "sequoia-net",
  "sequoia-openpgp",
  "testresult",
 ]
@@ -1835,15 +1992,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
  "cc",
  "libc",
  "once_cell",
  "spin",
- "untrusted",
+ "untrusted 0.7.1",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "ripemd160"
 version = "0.9.1"
@@ -1874,14 +2031,20 @@
  "simple_asn1",
  "subtle",
  "thiserror",
  "zeroize",
 ]
 
 [[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
 name = "rustix"
 version = "0.36.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4fdebc4b395b7fbb9ab11e462e20ed9051e7b16e42d24042c776eca0ac81b03"
 dependencies = [
  "bitflags",
  "errno",
@@ -1984,15 +2147,14 @@
  "cipher",
  "des",
  "digest",
  "dyn-clone",
  "eax",
  "ecdsa",
  "ed25519-dalek",
- "flate2",
  "generic-array",
  "getrandom 0.2.8",
  "idea",
  "idna 0.3.0",
  "lalrpop",
  "lalrpop-util",
  "lazy_static",
@@ -2056,14 +2218,20 @@
  "cfg-if",
  "cpufeatures",
  "digest",
  "opaque-debug",
 ]
 
 [[package]]
+name = "shlex"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
+
+[[package]]
 name = "signal-hook-registry"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
 dependencies = [
  "libc",
 ]
@@ -2524,14 +2692,20 @@
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
+name = "untrusted"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
+
+[[package]]
 name = "url"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
 dependencies = [
  "form_urlencoded",
  "idna 0.3.0",
```

### Comparing `pysequoia-0.1.8/PKG-INFO` & `pysequoia-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysequoia
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PySequoia
@@ -36,14 +36,25 @@
 ```python
 s = Cert.from_file("signing-key.asc")
 r = Cert.from_bytes(open("wiktor.asc", "rb").read())
 encrypted = Context.standard().encrypt(s, r, "content to encrypt")
 print(f"Encrypted data: {encrypted}")
 ```
 
+### sign
+
+Signs the data and returns armored output:
+
+```python
+from pysequoia import sign
+
+s = Cert.from_file("signing-key.asc")
+signed = sign(s.signer(), "data to be signed")
+```
+
 ### merge
 
 Merges data from old certificate with new packets:
 
 ```python
 old = Cert.from_file("wiktor.asc")
 new = Cert.from_file("wiktor-fresh.asc")
@@ -139,7 +150,29 @@
 retrieved later by its fingerprint:
 
 ```python
 s = Store("/tmp/store")
 assert s.get("653909a2f0e37c106f5faf546c8857e0d8e8f074") != None
 ```
 
+### OpenPGP Cards
+
+There's an experimental feature allowing communication with OpenPGP
+Cards (like Yubikey or Nitrokey).
+
+```py
+from pysequoia import Card
+
+# enumerate all cards
+all = Card.all()
+
+# open card by card ident
+card = Card.open("card ident")
+
+print(card.ident)
+print(card.cardholder)
+
+signer = card.signer(input("PIN: "))
+
+signed = sign(signer, "data to be signed")
+```
+
```

