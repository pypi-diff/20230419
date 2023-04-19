# Comparing `tmp/dkist_fits_specifications-3.6.0rc2.tar.gz` & `tmp/dkist_fits_specifications-3.6.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_fits_specifications-3.6.0rc2.tar", last modified: Wed Apr 19 19:33:18 2023, max compression
+gzip compressed data, was "dkist_fits_specifications-3.6.0rc3.tar", last modified: Wed Apr 19 19:59:51 2023, max compression
```

## Comparing `dkist_fits_specifications-3.6.0rc2.tar` & `dkist_fits_specifications-3.6.0rc3.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.655733 dkist_fits_specifications-3.6.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     3334 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     4276 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     6509 2023-04-19 19:33:18.655733 dkist_fits_specifications-3.6.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6089 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2283 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.643733 dkist_fits_specifications-3.6.0rc2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/changelog/35.spec_change.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.647733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/py.typed
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.647733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/
--rw-rw-rw-   0 root         (0) root         (0)     3584 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.647733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    10244 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     4395 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)     2653 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)      930 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/ws.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.647733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/
--rw-rw-rw-   0 root         (0) root         (0)    11880 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/level0.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.651733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     5886 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    13479 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/datacenter.yml
--rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dataset.yml
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dkist-op.yml
--rw-rw-rw-   0 root         (0) root         (0)     8355 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/stats.yml
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3660 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/ws.yml
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/spec214_full_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec_validation_schema.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.651733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1044 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     2687 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_level0_214.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.651733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/frozendict.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/spec.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.651733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/sphinx/spec_table.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.647733 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6509 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-19 19:33:18.000000 dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.655733 dkist_fits_specifications-3.6.0rc2/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/level_one.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/reference.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/release_history.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.655733 dkist_fits_specifications-3.6.0rc2/docs/specs/
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/specs/spec-122.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/docs/specs/spec-214.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:33:18.655733 dkist_fits_specifications-3.6.0rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-04-19 19:33:18.655733 dkist_fits_specifications-3.6.0rc2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      612 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-19 19:33:01.000000 dkist_fits_specifications-3.6.0rc2/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6089 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.710378 dkist_fits_specifications-3.6.0rc3/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/changelog/35.spec_change.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.710378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/
+-rw-rw-rw-   0 root         (0) root         (0)     3584 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2951 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10244 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4395 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ws.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)    11880 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/level0.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6341 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13479 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/datacenter.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dataset.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-op.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8355 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/stats.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3660 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ws.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/spec214_full_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec_validation_schema.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_level0_214.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/frozendict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/spec.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.718378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8553 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/spec_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.714378 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      205 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-19 19:59:51.000000 dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/level_one.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/release_history.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/docs/specs/
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/specs/spec-122.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/docs/specs/spec-214.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-04-19 19:59:51.722378 dkist_fits_specifications-3.6.0rc3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      612 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-04-19 19:59:31.000000 dkist_fits_specifications-3.6.0rc3/tox.ini
```

### Comparing `dkist_fits_specifications-3.6.0rc2/.gitignore` & `dkist_fits_specifications-3.6.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/.pre-commit-config.yaml` & `dkist_fits_specifications-3.6.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/CHANGELOG.rst` & `dkist_fits_specifications-3.6.0rc3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/PKG-INFO` & `dkist_fits_specifications-3.6.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_fits_specifications
-Version: 3.6.0rc2
+Version: 3.6.0rc3
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-3.6.0rc2/README.rst` & `dkist_fits_specifications-3.6.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/bitbucket-pipelines.yml` & `dkist_fits_specifications-3.6.0rc3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/check_changelog_updated.sh` & `dkist_fits_specifications-3.6.0rc3/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/__init__.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/__init__.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/ao.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/camera.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/dkist-id.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/fits.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/pac.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/telescope.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/vbi.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vbi.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/visp.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/vtf.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/wfc.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec122/schemas/ws.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec122/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/__init__.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/level0.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/level0.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/ao.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ao.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/camera.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/camera.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/compression.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/compression.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/cryonirsp.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/cryonirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/datacenter.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/datacenter.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dataset.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dataset.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dkist-id.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-id.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dkist-op.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dkist-op.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/dlnirsp.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/dlnirsp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/fits.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/fits.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/pac.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/pac.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/stats.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/stats.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/telescope.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/telescope.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/vbi.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vbi.yml`

 * *Files 10% similar despite different names*

```diff
@@ -104,26 +104,28 @@
 00000670: 656e 6162 6c65 6420 6275 7420 6e6f 2072  enabled but no r
 00000680: 3020 6973 2061 7661 696c 6162 6c65 2e22  0 is available."
 00000690: 0a56 4249 4e4d 4f53 433a 0a20 2064 6573  .VBINMOSC:.  des
 000006a0: 6372 6970 7469 6f6e 3a20 2254 6f74 616c  cription: "Total
 000006b0: 206e 756d 6265 7220 6f66 206d 6f73 6169   number of mosai
 000006c0: 6320 7265 7065 6174 7320 696e 2064 6174  c repeats in dat
 000006d0: 6173 6574 2e22 0a20 2074 7970 653a 2069  aset.".  type: i
-000006e0: 6e74 0a56 4249 434d 4f53 433a 0a20 2064  nt.VBICMOSC:.  d
-000006f0: 6573 6372 6970 7469 6f6e 3a20 2243 7572  escription: "Cur
-00000700: 7265 6e74 206d 6f73 6169 6320 7265 7065  rent mosaic repe
-00000710: 6174 2e22 0a20 2074 7970 653a 2069 6e74  at.".  type: int
-00000720: 0a56 4249 464f 563a 0a20 2064 6573 6372  .VBIFOV:.  descr
-00000730: 6970 7469 6f6e 3a20 2243 7572 7265 6e74  iption: "Current
-00000740: 2046 6965 6c64 4f66 5669 6577 2073 6361   FieldOfView sca
-00000750: 6e20 6e75 6d62 6572 220a 2020 636f 6d6d  n number".  comm
-00000760: 656e 743a 2046 4f56 5363 616e 4e75 6d62  ent: FOVScanNumb
-00000770: 6572 0a20 2074 7970 653a 2069 6e74 0a20  er.  type: int. 
-00000780: 2063 6f70 793a 2046 616c 7365 0a56 4249   copy: False.VBI
-00000790: 4e46 4f56 533a 0a20 2064 6573 6372 6970  NFOVS:.  descrip
-000007a0: 7469 6f6e 3a20 224e 756d 6265 7220 6f66  tion: "Number of
-000007b0: 2073 6361 6e6e 6564 2046 6965 6c64 734f   scanned FieldsO
-000007c0: 6656 6965 7720 696e 2074 6865 2064 6174  fView in the dat
-000007d0: 6173 6574 220a 2020 636f 6d6d 656e 743a  aset".  comment:
-000007e0: 2054 6f74 616c 464f 5653 6361 6e73 0a20   TotalFOVScans. 
-000007f0: 2074 7970 653a 2069 6e74 0a20 2063 6f70   type: int.  cop
-00000800: 793a 2046 616c 7365 0a                   y: False.
+000006e0: 6e74 0a20 2063 6f70 793a 2046 616c 7365  nt.  copy: False
+000006f0: 0a56 4249 434d 4f53 433a 0a20 2064 6573  .VBICMOSC:.  des
+00000700: 6372 6970 7469 6f6e 3a20 2243 7572 7265  cription: "Curre
+00000710: 6e74 206d 6f73 6169 6320 7265 7065 6174  nt mosaic repeat
+00000720: 2e22 0a20 2074 7970 653a 2069 6e74 0a20  .".  type: int. 
+00000730: 2063 6f70 793a 2046 616c 7365 0a56 4249   copy: False.VBI
+00000740: 464f 563a 0a20 2064 6573 6372 6970 7469  FOV:.  descripti
+00000750: 6f6e 3a20 2243 7572 7265 6e74 2046 6965  on: "Current Fie
+00000760: 6c64 4f66 5669 6577 2073 6361 6e20 6e75  ldOfView scan nu
+00000770: 6d62 6572 220a 2020 636f 6d6d 656e 743a  mber".  comment:
+00000780: 2046 4f56 5363 616e 4e75 6d62 6572 0a20   FOVScanNumber. 
+00000790: 2074 7970 653a 2069 6e74 0a20 2063 6f70   type: int.  cop
+000007a0: 793a 2046 616c 7365 0a56 4249 4e46 4f56  y: False.VBINFOV
+000007b0: 533a 0a20 2064 6573 6372 6970 7469 6f6e  S:.  description
+000007c0: 3a20 224e 756d 6265 7220 6f66 2073 6361  : "Number of sca
+000007d0: 6e6e 6564 2046 6965 6c64 734f 6656 6965  nned FieldsOfVie
+000007e0: 7720 696e 2074 6865 2064 6174 6173 6574  w in the dataset
+000007f0: 220a 2020 636f 6d6d 656e 743a 2054 6f74  ".  comment: Tot
+00000800: 616c 464f 5653 6361 6e73 0a20 2074 7970  alFOVScans.  typ
+00000810: 653a 2069 6e74 0a20 2063 6f70 793a 2046  e: int.  copy: F
+00000820: 616c 7365 0a                             alse.
```

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/visp.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/visp.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/vtf.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/vtf.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/wfc.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/wfc.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/schemas/ws.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/schemas/ws.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec214/spec214_full_schema.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec214/spec214_full_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/spec_validation_schema.yml` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/spec_validation_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_122.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_214.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/tests/test_expansions.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/tests/test_expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/formatter.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/frozendict.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/spec.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/spec.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications/utils/sphinx/spec_table.py` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications/utils/sphinx/spec_table.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/PKG-INFO` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-fits-specifications
-Version: 3.6.0rc2
+Version: 3.6.0rc3
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-3.6.0rc2/dkist_fits_specifications.egg-info/SOURCES.txt` & `dkist_fits_specifications-3.6.0rc3/dkist_fits_specifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/Makefile` & `dkist_fits_specifications-3.6.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/conf.py` & `dkist_fits_specifications-3.6.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/index.rst` & `dkist_fits_specifications-3.6.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/level_one.rst` & `dkist_fits_specifications-3.6.0rc3/docs/level_one.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/make.bat` & `dkist_fits_specifications-3.6.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/specs/spec-122.rst` & `dkist_fits_specifications-3.6.0rc3/docs/specs/spec-122.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/docs/specs/spec-214.rst` & `dkist_fits_specifications-3.6.0rc3/docs/specs/spec-214.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/licenses/LICENSE.rst` & `dkist_fits_specifications-3.6.0rc3/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/licenses/TEMPLATE_LICENSE.rst` & `dkist_fits_specifications-3.6.0rc3/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/pyproject.toml` & `dkist_fits_specifications-3.6.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/setup.cfg` & `dkist_fits_specifications-3.6.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/setup.py` & `dkist_fits_specifications-3.6.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-3.6.0rc2/tox.ini` & `dkist_fits_specifications-3.6.0rc3/tox.ini`

 * *Files identical despite different names*

