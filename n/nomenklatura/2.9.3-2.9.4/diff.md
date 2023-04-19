# Comparing `tmp/nomenklatura-2.9.3.tar.gz` & `tmp/nomenklatura-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-2.9.3.tar", last modified: Sat Apr 15 16:29:41 2023, max compression
+gzip compressed data, was "nomenklatura-2.9.4.tar", last modified: Wed Apr 19 19:57:50 2023, max compression
```

## Comparing `nomenklatura-2.9.3.tar` & `nomenklatura-2.9.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/data/match-regression.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/judgement.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/matching/features/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/features/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/matching/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 16:29:41.027504 nomenklatura-2.9.3/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 16:29:03.000000 nomenklatura-2.9.3/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 16:29:40.000000 nomenklatura-2.9.3/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 16:29:41.031504 nomenklatura-2.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-15 16:27:29.000000 nomenklatura-2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/data/match-regression.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15759 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/judgement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/matching/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/features/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/matching/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:57:50.563531 nomenklatura-2.9.4/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:57:10.000000 nomenklatura-2.9.4/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 19:57:50.000000 nomenklatura-2.9.4/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:57:50.567531 nomenklatura-2.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-19 19:55:37.000000 nomenklatura-2.9.4/setup.py
```

### Comparing `nomenklatura-2.9.3/LICENSE` & `nomenklatura-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/PKG-INFO` & `nomenklatura-2.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.3
+Version: 2.9.4
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # nomenklatura
 
 Nomenklatura de-duplicates and integrates different [Follow the Money](https://followthemoney.rtfd.org/) entities. It serves to clean up messy data and to find links between different datasets.
@@ -91,9 +90,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-2.9.3/README.md` & `nomenklatura-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/cache.py` & `nomenklatura-2.9.4/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/cli.py` & `nomenklatura-2.9.4/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/data/match-regression.pkl` & `nomenklatura-2.9.4/nomenklatura/data/match-regression.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/dataset/catalog.py` & `nomenklatura-2.9.4/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/dataset/coverage.py` & `nomenklatura-2.9.4/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/dataset/dataset.py` & `nomenklatura-2.9.4/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/dataset/publisher.py` & `nomenklatura-2.9.4/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/dataset/resource.py` & `nomenklatura-2.9.4/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/dataset/util.py` & `nomenklatura-2.9.4/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/db.py` & `nomenklatura-2.9.4/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/__init__.py` & `nomenklatura-2.9.4/nomenklatura/enrich/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,19 +3,27 @@
 from typing import Iterable, Generator, Optional, Type, cast
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.matching import compare_scored
 from nomenklatura.enrich.common import Enricher, EnricherConfig
+from nomenklatura.enrich.common import EnrichmentAbort, EnrichmentException
 from nomenklatura.judgement import Judgement
 from nomenklatura.resolver import Resolver
 
 log = logging.getLogger(__name__)
-__all__ = ["Enricher", "make_enricher", "enrich", "match"]
+__all__ = [
+    "Enricher",
+    "EnrichmentAbort",
+    "EnrichmentException",
+    "make_enricher",
+    "enrich",
+    "match",
+]
 
 
 def make_enricher(
     dataset: DS, cache: Cache, config: EnricherConfig
 ) -> Optional[Enricher]:
     enricher = get_enricher(config.pop("type"))
     if enricher is not None:
@@ -27,47 +35,53 @@
 # then:
 # nk dedupe -i entities-with-matches.json -r resolver.json
 def match(
     enricher: Enricher, resolver: Resolver[CE], entities: Iterable[CE]
 ) -> Generator[CE, None, None]:
     for entity in entities:
         yield entity
-        for match in enricher.match_wrapped(entity):
-            if entity.id is None or match.id is None:
-                continue
-            if not resolver.check_candidate(entity.id, match.id):
-                continue
-            if not entity.schema.can_match(match.schema):
-                continue
-            result = compare_scored(entity, match)
-            score = result["score"]
-            log.info("Match [%s]: %.2f -> %s", entity, score, match)
-            resolver.suggest(entity.id, match.id, score)
-            match.datasets.add(enricher.dataset.name)
-            match = resolver.apply(match)
-            yield match
+        try:
+            for match in enricher.match_wrapped(entity):
+                if entity.id is None or match.id is None:
+                    continue
+                if not resolver.check_candidate(entity.id, match.id):
+                    continue
+                if not entity.schema.can_match(match.schema):
+                    continue
+                result = compare_scored(entity, match)
+                score = result["score"]
+                log.info("Match [%s]: %.2f -> %s", entity, score, match)
+                resolver.suggest(entity.id, match.id, score)
+                match.datasets.add(enricher.dataset.name)
+                match = resolver.apply(match)
+                yield match
+        except EnrichmentException:
+            log.exception("Failed to match: %r" % entity)
 
 
 # nk enrich -i entities.json -r resolver.json -o combined.json
 def enrich(
     enricher: Enricher, resolver: Resolver[CE], entities: Iterable[CE]
 ) -> Generator[CE, None, None]:
     for entity in entities:
-        for match in enricher.match_wrapped(entity):
-            if entity.id is None or match.id is None:
-                continue
-            judgement = resolver.get_judgement(match.id, entity.id)
-            if judgement != Judgement.POSITIVE:
-                continue
-
-            log.info("Enrich [%s]: %r", entity, match)
-            for adjacent in enricher.expand_wrapped(entity, match):
-                adjacent.datasets.add(enricher.dataset.name)
-                adjacent = resolver.apply(adjacent)
-                yield adjacent
+        try:
+            for match in enricher.match_wrapped(entity):
+                if entity.id is None or match.id is None:
+                    continue
+                judgement = resolver.get_judgement(match.id, entity.id)
+                if judgement != Judgement.POSITIVE:
+                    continue
+
+                log.info("Enrich [%s]: %r", entity, match)
+                for adjacent in enricher.expand_wrapped(entity, match):
+                    adjacent.datasets.add(enricher.dataset.name)
+                    adjacent = resolver.apply(adjacent)
+                    yield adjacent
+        except EnrichmentException:
+            log.exception("Failed to enrich: %r" % entity)
 
 
 def get_enricher(import_path: str) -> Optional[Type[Enricher]]:
     if ":" not in import_path:
         raise RuntimeError("Invalid import path: %r" % import_path)
     module_name, clazz_name = import_path.split(":", 1)
     module = import_module(module_name)
```

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/aleph.py` & `nomenklatura-2.9.4/nomenklatura/enrich/aleph.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,20 +114,15 @@
             url = normalize_url(url, {"collection_ids": self.collection_id})
         query = {
             "schema": entity.schema.name,
             "properties": entity.properties,
         }
         cache_id = entity.id or hash_data(query)
         cache_key = f"{url}:{cache_id}"
-        response = self.cache.get_json(cache_key, max_age=self.cache_days)
-        if response is None:
-            resp = self.session.post(url, json=query)
-            resp.raise_for_status()
-            response = resp.json()
-            self.cache.set_json(cache_key, response)
+        response = self.http_post_json_cached(url, cache_key, query)
         for result in response.get("results", []):
             proxy = self.load_aleph_entity(entity, result)
             if proxy is not None:
                 if self._ns is not None:
                     entity = self._ns.apply(entity)
                 yield proxy
```

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/common.py` & `nomenklatura-2.9.4/nomenklatura/enrich/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import os
 import json
 from banal import as_bool
 from typing import Union, Any, Dict, Optional, Generator
 from abc import ABC, abstractmethod
 from requests import Session
+from requests.exceptions import RequestException, HTTPError
 from followthemoney import model
 
 from nomenklatura import __version__
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.util import ParamsType, normalize_url
 
 EnricherConfig = Dict[str, Any]
 
 
+class EnrichmentException(Exception):
+    pass
+
+
+class EnrichmentAbort(Exception):
+    pass
+
+
 class Enricher(ABC):
     def __init__(self, dataset: DS, cache: Cache, config: EnricherConfig):
         self.dataset = dataset
         self.cache = cache
         self.config = config
         self.cache_days = int(config.pop("cache_days", 90))
         self.schemata = config.pop("schemata", [])
@@ -53,16 +62,22 @@
         cache_days: Optional[int] = None,
     ) -> str:
         url = normalize_url(url, params=params)
         cache_days_ = cache_days or self.cache_days
         response = self.cache.get(url, max_age=cache_days_)
         if response is None:
             hidden_url = normalize_url(url, params=hidden)
-            resp = self.session.get(hidden_url)
-            resp.raise_for_status()
+            try:
+                resp = self.session.get(hidden_url)
+                resp.raise_for_status()
+            except RequestException as rex:
+                if rex.response is not None and rex.response.status_code in (401, 403):
+                    raise EnrichmentAbort("Authorization failure: %s" % url) from rex
+                msg = "HTTP fetch failed [%s]: %s" % (url, rex)
+                raise EnrichmentException(msg) from rex
             response = resp.text
             self.cache.set(url, response)
         return response
 
     def http_remove_cache(self, url: str, params: ParamsType = None) -> None:
         url = normalize_url(url, params=params)
         self.cache.delete(url)
@@ -73,14 +88,36 @@
         params: ParamsType = None,
         hidden: ParamsType = None,
         cache_days: Optional[int] = None,
     ) -> Any:
         res = self.http_get_cached(url, params, hidden=hidden, cache_days=cache_days)
         return json.loads(res)
 
+    def http_post_json_cached(
+        self,
+        url: str,
+        cache_key: str,
+        json: Any,
+        cache_days: Optional[int] = None,
+    ) -> Any:
+        cache_days_ = cache_days or self.cache_days
+        resp_data = self.cache.get_json(cache_key, max_age=cache_days_)
+        if resp_data is None:
+            try:
+                resp = self.session.post(url, json=json)
+                resp.raise_for_status()
+            except RequestException as rex:
+                if rex.response is not None and rex.response.status_code in (401, 403):
+                    raise EnrichmentAbort("Authorization failure: %s" % url) from rex
+                msg = "HTTP POST failed [%s]: %s" % (url, rex)
+                raise EnrichmentException(msg) from rex
+            resp_data = resp.json()
+            self.cache.set_json(cache_key, resp_data)
+        return resp_data
+
     def load_entity(self, entity: CE, data: Dict[str, Any]) -> CE:
         proxy = type(entity).from_dict(model, data, cleaned=False)
         for prop in proxy.iterprops():
             if prop.stub:
                 proxy.pop(prop)
         return proxy
```

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/nominatim.py` & `nomenklatura-2.9.4/nomenklatura/enrich/nominatim.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import json
 import logging
 from normality import collapse_spaces
 from typing import Any, Dict, Iterable, Generator
-from requests.exceptions import HTTPError
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.enrich.common import Enricher, EnricherConfig
 
 
@@ -25,20 +23,15 @@
             params = {
                 "q": full_norm,
                 "countrycodes": address.get("country"),
                 "format": "jsonv2",
                 "accept-language": "en",
                 "addressdetails": 1,
             }
-            try:
-                response = self.http_get_cached(NOMINATIM, params)
-            except HTTPError as exc:
-                log.error("Failed to geocode [%s]: %s", exc.response.status_code, full)
-                continue
-            results = json.loads(response)
+            results = self.http_get_json_cached(NOMINATIM, params)
             log.info("OpenStreetMap geocoded [%s]: %d results", full, len(results))
             for result in results:
                 yield result
                 # FIXME: only best result for now.
                 return
 
     def match(self, entity: CE) -> Generator[CE, None, None]:
```

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/opencorporates.py` & `nomenklatura-2.9.4/nomenklatura/enrich/opencorporates.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from followthemoney.types import registry
 from requests.exceptions import HTTPError
 
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.enrich.common import Enricher, EnricherConfig
+from nomenklatura.enrich.common import EnrichmentAbort
 
 
 log = logging.getLogger(__name__)
 
 
 class OpenCorporatesEnricher(Enricher):
     COMPANY_SEARCH_API = "https://api.opencorporates.com/v0.4/companies/search"
@@ -126,23 +127,20 @@
 
     def search_companies(self, entity: CE) -> Generator[CE, None, None]:
         countries = entity.get_type_values(registry.country)
         q = self.names_query(entity)
         params = {"q": q, "sparse": True, "country_codes": countries}
         for page in range(1, 9):
             params["page"] = page
-            try:
-                results = self.http_get_json_cached(
-                    self.COMPANY_SEARCH_API,
-                    params=params,
-                    hidden={"api_token": self.api_token},
-                )
-            except HTTPError as exc:
-                log.error("Failed to search [%s]: %s", exc.response.status_code, q)
-                break
+            results = self.http_get_json_cached(
+                self.COMPANY_SEARCH_API,
+                params=params,
+                hidden={"api_token": self.api_token},
+            )
+
             # print(results)
             for company in results.get("results", {}).get("companies", []):
                 proxy = self.company_entity(entity, company)
                 yield proxy
             if page >= results.get("total_pages", 0):
                 break
```

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-2.9.4/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/enrich/yente.py` & `nomenklatura-2.9.4/nomenklatura/enrich/yente.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     """Uses the `yente` match API to look up entities in a specific dataset."""
 
     def __init__(self, dataset: DS, cache: Cache, config: EnricherConfig):
         super().__init__(dataset, cache, config)
         self._api: str = config.pop("api")
         self._dataset: str = config.pop("dataset", "default")
         self._threshold: Optional[float] = config.pop("threshold", None)
+        self._nested: bool = config.pop("expand_nested", True)
         self._ns: Optional[Namespace] = None
         if self.get_config_bool("strip_namespace"):
             self._ns = Namespace()
 
         api_key: Optional[str] = os.path.expandvars(config.pop("api_key", "")).strip()
         if api_key is None or not len(api_key):
             api_key = os.environ.get("YENTE_API_KEY")
@@ -43,35 +44,31 @@
     def match(self, entity: CE) -> Generator[CE, None, None]:
         if not entity.schema.matchable:
             return
         url = urljoin(self._api, f"match/{self._dataset}")
         if self._threshold is not None:
             url = normalize_url(url, {"threshold": self._threshold})
         cache_key = f"{url}:{entity.id}"
-        response = self.cache.get_json(cache_key, max_age=self.cache_days)
-        if response is None:
-            props: Dict[str, List[str]] = {}
-            for prop in entity.iterprops():
-                if prop.type == registry.entity:
-                    continue
-                if prop.matchable:
-                    props[prop.name] = entity.get(prop)
-            data = {
-                "queries": {
-                    "entity": {
-                        "schema": entity.schema.name,
-                        "properties": props,
-                    }
+        props: Dict[str, List[str]] = {}
+        for prop in entity.iterprops():
+            if prop.type == registry.entity:
+                continue
+            if prop.matchable:
+                props[prop.name] = entity.get(prop)
+        query = {
+            "queries": {
+                "entity": {
+                    "schema": entity.schema.name,
+                    "properties": props,
                 }
             }
-            resp = self.session.post(url, json=data)
-            resp.raise_for_status()
-            response = resp.json().get("responses", {}).get("entity", {})
-            self.cache.set_json(cache_key, response)
-        for result in response.get("results", []):
+        }
+        response = self.http_post_json_cached(url, cache_key, query)
+        inner_resp = response.get("responses", {}).get("entity", {})
+        for result in inner_resp.get("results", []):
             proxy = self.load_entity(entity, result)
             proxy.add("sourceUrl", self.make_url(proxy))
             if self._ns is not None:
                 proxy = self._ns.apply(proxy)
             yield proxy
 
     def _traverse_nested(self, entity: CE, response: Any) -> Generator[CE, None, None]:
@@ -93,10 +90,10 @@
                     yield from self._traverse_nested(entity, value)
 
     def expand(self, entity: CE, match: CE) -> Generator[CE, None, None]:
         url = self.make_url(match)
         for source_url in match.get("sourceUrl", quiet=True):
             if source_url.startswith(self._api):
                 url = source_url
-        url = normalize_url(url, {"nested": True})
+        url = normalize_url(url, {"nested": self._nested})
         response = self.http_get_json_cached(url)
         yield from self._traverse_nested(match, response)
```

### Comparing `nomenklatura-2.9.3/nomenklatura/entity.py` & `nomenklatura-2.9.4/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/index/entry.py` & `nomenklatura-2.9.4/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/index/index.py` & `nomenklatura-2.9.4/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/index/tokenizer.py` & `nomenklatura-2.9.4/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/judgement.py` & `nomenklatura-2.9.4/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/loader.py` & `nomenklatura-2.9.4/nomenklatura/loader.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/features/__init__.py` & `nomenklatura-2.9.4/nomenklatura/matching/features/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/features/dates.py` & `nomenklatura-2.9.4/nomenklatura/matching/features/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/features/misc.py` & `nomenklatura-2.9.4/nomenklatura/matching/features/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/features/names.py` & `nomenklatura-2.9.4/nomenklatura/matching/features/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/features/util.py` & `nomenklatura-2.9.4/nomenklatura/matching/features/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/model.py` & `nomenklatura-2.9.4/nomenklatura/matching/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/pairs.py` & `nomenklatura-2.9.4/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/matching/train.py` & `nomenklatura-2.9.4/nomenklatura/matching/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/publish/dates.py` & `nomenklatura-2.9.4/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/publish/edges.py` & `nomenklatura-2.9.4/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/publish/names.py` & `nomenklatura-2.9.4/nomenklatura/publish/names.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if len(chars) == 0:
         return 0.0
     return float(len(asciis)) / float(len(chars))
 
 
 def pick_name(names: List[str]) -> Optional[str]:
     forms: List[Tuple[str, str, float]] = []
-    for name in names:
+    for name in sorted(names):
         norm = normalize(name, ascii=True, lowercase=False)
         if norm is not None:
             weight = 2 - ascii_share(name)
             forms.append((norm, name, weight))
             forms.append((norm.title(), name, weight))
 
     edits: Dict[str, float] = defaultdict(float)
```

### Comparing `nomenklatura-2.9.3/nomenklatura/resolver/edge.py` & `nomenklatura-2.9.4/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/resolver/identifier.py` & `nomenklatura-2.9.4/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/resolver/resolver.py` & `nomenklatura-2.9.4/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/senzing.py` & `nomenklatura-2.9.4/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/statement/serialize.py` & `nomenklatura-2.9.4/nomenklatura/statement/serialize.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/statement/statement.py` & `nomenklatura-2.9.4/nomenklatura/statement/statement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/tui/app.py` & `nomenklatura-2.9.4/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/tui/comparison.py` & `nomenklatura-2.9.4/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/tui/util.py` & `nomenklatura-2.9.4/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/util.py` & `nomenklatura-2.9.4/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura/xref.py` & `nomenklatura-2.9.4/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-2.9.4/nomenklatura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 2.9.3
+Version: 2.9.4
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # nomenklatura
 
 Nomenklatura de-duplicates and integrates different [Follow the Money](https://followthemoney.rtfd.org/) entities. It serves to clean up messy data and to find links between different datasets.
@@ -91,9 +90,7 @@
 ## Contact, contributions etc.
 
 This codebase is licensed under the terms of an MIT license (see LICENSE).
 
 We're keen for any contributions, bug fixes and feature suggestions, please use the GitHub issue tracker for this repository. 
 
 Nomenklatura is currently developed thanks to a Prototypefund grant for [OpenSanctions](https://opensanctions.org). Previous iterations of the package were developed with support from [Knight-Mozilla OpenNews](http://opennews.org) and the [Open Knowledge Foundation Labs](http://okfnlabs.org).
-
-
```

### Comparing `nomenklatura-2.9.3/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-2.9.4/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-2.9.3/setup.py` & `nomenklatura-2.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="2.9.3",
+    version="2.9.4",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

