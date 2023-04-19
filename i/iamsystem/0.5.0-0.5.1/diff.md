# Comparing `tmp/iamsystem-0.5.0.tar.gz` & `tmp/iamsystem-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/cossin/workspace/iamsystem_python/dist/.tmp-saem5_my/iamsystem-0.5.0.tar", last modified: Wed Mar 22 00:20:15 2023, max compression
+gzip compressed data, was "/home/cossin/workspace/iamsystem_python/dist/.tmp-e0be22mt/iamsystem-0.5.1.tar", last modified: Wed Apr 19 14:18:39 2023, max compression
```

## Comparing `iamsystem-0.5.0.tar` & `iamsystem-0.5.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1074 2023-01-31 22:56:40.000000 iamsystem-0.5.0/LICENSE
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4358 2023-03-22 00:20:15.000000 iamsystem-0.5.0/PKG-INFO
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3475 2023-02-12 19:19:20.000000 iamsystem-0.5.0/README.md
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1665 2023-03-21 23:57:09.000000 iamsystem-0.5.0/pyproject.toml
--rw-rw-r--   0 cossin    (1000) cossin    (1000)       38 2023-03-22 00:20:15.000000 iamsystem-0.5.0/setup.cfg
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4070 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/__init__.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/brat/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/brat/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     8882 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/brat/adapter.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3479 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/brat/formatter.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      508 2023-02-19 14:10:43.000000 iamsystem-0.5.0/src/iamsystem/brat/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3324 2023-02-22 21:30:19.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/abbreviations.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     7075 2023-03-12 15:37:04.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2625 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/cache.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      650 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/exact.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2261 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/norm_fun.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2764 2023-03-11 20:19:38.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/regex.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4182 2023-02-12 19:19:20.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/simstring.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4594 2023-02-12 19:19:20.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/spellwise.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1286 2023-02-26 21:30:37.000000 iamsystem-0.5.0/src/iamsystem/fuzzy/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/keywords/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/keywords/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      705 2023-02-12 19:19:20.000000 iamsystem-0.5.0/src/iamsystem/keywords/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1803 2023-02-19 14:03:03.000000 iamsystem-0.5.0/src/iamsystem/keywords/collection.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1116 2023-02-19 14:03:03.000000 iamsystem-0.5.0/src/iamsystem/keywords/keywords.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      877 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/keywords/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/matcher/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/matcher/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    11783 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/matcher/annotation.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4214 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/matcher/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    19387 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/matcher/matcher.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1648 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/matcher/printannot.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    14119 2023-03-21 23:38:49.000000 iamsystem-0.5.0/src/iamsystem/matcher/strategy.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2985 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/matcher/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/spacy/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      487 2023-02-19 14:03:03.000000 iamsystem-0.5.0/src/iamsystem/spacy/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     8073 2023-02-19 14:10:43.000000 iamsystem-0.5.0/src/iamsystem/spacy/component.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      424 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/spacy/stopwords.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1051 2023-02-19 14:10:43.000000 iamsystem-0.5.0/src/iamsystem/spacy/token.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1380 2023-02-19 14:10:43.000000 iamsystem-0.5.0/src/iamsystem/spacy/tokenizer.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/stopwords/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/stopwords/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1629 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/stopwords/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3983 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/stopwords/negative.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1492 2023-02-17 17:50:31.000000 iamsystem-0.5.0/src/iamsystem/stopwords/simple.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/tokenization/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/tokenization/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2162 2023-02-19 14:10:43.000000 iamsystem-0.5.0/src/iamsystem/tokenization/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      506 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/tokenization/normalize.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3110 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/tokenization/span.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     1873 2023-02-19 14:10:43.000000 iamsystem-0.5.0/src/iamsystem/tokenization/token.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4254 2023-02-25 00:38:50.000000 iamsystem-0.5.0/src/iamsystem/tokenization/tokenize.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     5664 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/tokenization/util.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem/tree/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.0/src/iamsystem/tree/__init__.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      275 2023-02-12 19:19:20.000000 iamsystem-0.5.0/src/iamsystem/tree/api.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     7732 2023-03-11 22:49:04.000000 iamsystem-0.5.0/src/iamsystem/tree/nodes.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3502 2023-02-12 19:19:20.000000 iamsystem-0.5.0/src/iamsystem/tree/trie.py
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem.egg-info/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     4358 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem.egg-info/PKG-INFO
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     2022 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem.egg-info/SOURCES.txt
--rw-rw-r--   0 cossin    (1000) cossin    (1000)        1 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem.egg-info/dependency_links.txt
--rw-rw-r--   0 cossin    (1000) cossin    (1000)      126 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem.egg-info/requires.txt
--rw-rw-r--   0 cossin    (1000) cossin    (1000)       10 2023-03-22 00:20:15.000000 iamsystem-0.5.0/src/iamsystem.egg-info/top_level.txt
-drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-03-22 00:20:15.000000 iamsystem-0.5.0/tests/
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    10966 2023-03-11 22:49:04.000000 iamsystem-0.5.0/tests/test_annotation.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    12681 2023-03-11 22:49:04.000000 iamsystem-0.5.0/tests/test_brat.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    11902 2023-03-11 22:49:04.000000 iamsystem-0.5.0/tests/test_detect.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    38661 2023-03-11 22:49:04.000000 iamsystem-0.5.0/tests/test_doc.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    13519 2023-02-27 22:35:29.000000 iamsystem-0.5.0/tests/test_fuzzy.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)    23629 2023-03-21 23:46:39.000000 iamsystem-0.5.0/tests/test_matcher.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     5524 2023-02-12 19:19:20.000000 iamsystem-0.5.0/tests/test_simstring.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     6324 2023-02-19 14:03:03.000000 iamsystem-0.5.0/tests/test_spacy.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     6818 2023-02-12 19:19:20.000000 iamsystem-0.5.0/tests/test_spellwise.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3768 2023-02-19 14:10:43.000000 iamsystem-0.5.0/tests/test_stopwords.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     3092 2023-02-12 19:19:20.000000 iamsystem-0.5.0/tests/test_terminology.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     5704 2023-03-11 22:49:04.000000 iamsystem-0.5.0/tests/test_toknorm.py
--rw-rw-r--   0 cossin    (1000) cossin    (1000)     9402 2023-03-11 22:49:04.000000 iamsystem-0.5.0/tests/test_tree.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1074 2023-01-31 22:56:40.000000 iamsystem-0.5.1/LICENSE
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4358 2023-04-19 14:18:39.000000 iamsystem-0.5.1/PKG-INFO
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3475 2023-02-12 19:19:20.000000 iamsystem-0.5.1/README.md
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1665 2023-04-19 14:18:10.000000 iamsystem-0.5.1/pyproject.toml
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)       38 2023-04-19 14:18:39.000000 iamsystem-0.5.1/setup.cfg
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4070 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/__init__.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/brat/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/brat/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     8882 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/brat/adapter.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3479 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/brat/formatter.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      508 2023-02-19 14:10:43.000000 iamsystem-0.5.1/src/iamsystem/brat/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3324 2023-02-22 21:30:19.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/abbreviations.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     7075 2023-03-22 00:25:08.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2625 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/cache.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      650 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/exact.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2261 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/norm_fun.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2764 2023-03-11 20:19:38.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/regex.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4182 2023-02-12 19:19:20.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/simstring.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4594 2023-02-12 19:19:20.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/spellwise.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1286 2023-02-26 21:30:37.000000 iamsystem-0.5.1/src/iamsystem/fuzzy/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/keywords/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/keywords/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      705 2023-02-12 19:19:20.000000 iamsystem-0.5.1/src/iamsystem/keywords/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1803 2023-02-19 14:03:03.000000 iamsystem-0.5.1/src/iamsystem/keywords/collection.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1116 2023-02-19 14:03:03.000000 iamsystem-0.5.1/src/iamsystem/keywords/keywords.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      877 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/keywords/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/matcher/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/matcher/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    11783 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/matcher/annotation.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4214 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/matcher/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    19387 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/matcher/matcher.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1648 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/matcher/printannot.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    14119 2023-03-22 00:27:49.000000 iamsystem-0.5.1/src/iamsystem/matcher/strategy.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2985 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/matcher/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/spacy/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      487 2023-02-19 14:03:03.000000 iamsystem-0.5.1/src/iamsystem/spacy/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     8151 2023-04-19 14:18:10.000000 iamsystem-0.5.1/src/iamsystem/spacy/component.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      424 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/spacy/stopwords.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1051 2023-02-19 14:10:43.000000 iamsystem-0.5.1/src/iamsystem/spacy/token.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1437 2023-04-19 14:18:10.000000 iamsystem-0.5.1/src/iamsystem/spacy/tokenizer.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/stopwords/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/stopwords/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1629 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/stopwords/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3983 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/stopwords/negative.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1492 2023-02-17 17:50:31.000000 iamsystem-0.5.1/src/iamsystem/stopwords/simple.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/tokenization/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/tokenization/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2162 2023-02-19 14:10:43.000000 iamsystem-0.5.1/src/iamsystem/tokenization/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      506 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/tokenization/normalize.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3110 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/tokenization/span.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     1873 2023-02-19 14:10:43.000000 iamsystem-0.5.1/src/iamsystem/tokenization/token.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4254 2023-02-25 00:38:50.000000 iamsystem-0.5.1/src/iamsystem/tokenization/tokenize.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     5664 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/tokenization/util.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem/tree/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        0 2023-01-31 22:56:40.000000 iamsystem-0.5.1/src/iamsystem/tree/__init__.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      275 2023-02-12 19:19:20.000000 iamsystem-0.5.1/src/iamsystem/tree/api.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     7732 2023-03-11 22:49:04.000000 iamsystem-0.5.1/src/iamsystem/tree/nodes.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3502 2023-02-12 19:19:20.000000 iamsystem-0.5.1/src/iamsystem/tree/trie.py
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem.egg-info/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     4358 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem.egg-info/PKG-INFO
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     2022 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem.egg-info/SOURCES.txt
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)        1 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem.egg-info/dependency_links.txt
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)      126 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem.egg-info/requires.txt
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)       10 2023-04-19 14:18:39.000000 iamsystem-0.5.1/src/iamsystem.egg-info/top_level.txt
+drwxrwxr-x   0 cossin    (1000) cossin    (1000)        0 2023-04-19 14:18:39.000000 iamsystem-0.5.1/tests/
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    10966 2023-03-11 22:49:04.000000 iamsystem-0.5.1/tests/test_annotation.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    12681 2023-03-11 22:49:04.000000 iamsystem-0.5.1/tests/test_brat.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    11902 2023-03-11 22:49:04.000000 iamsystem-0.5.1/tests/test_detect.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    38661 2023-03-11 22:49:04.000000 iamsystem-0.5.1/tests/test_doc.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    13519 2023-02-27 22:35:29.000000 iamsystem-0.5.1/tests/test_fuzzy.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)    23629 2023-03-22 00:27:49.000000 iamsystem-0.5.1/tests/test_matcher.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     5524 2023-02-12 19:19:20.000000 iamsystem-0.5.1/tests/test_simstring.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     7437 2023-04-19 14:18:10.000000 iamsystem-0.5.1/tests/test_spacy.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     6818 2023-02-12 19:19:20.000000 iamsystem-0.5.1/tests/test_spellwise.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3768 2023-02-19 14:10:43.000000 iamsystem-0.5.1/tests/test_stopwords.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     3092 2023-02-12 19:19:20.000000 iamsystem-0.5.1/tests/test_terminology.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     5704 2023-03-11 22:49:04.000000 iamsystem-0.5.1/tests/test_toknorm.py
+-rw-rw-r--   0 cossin    (1000) cossin    (1000)     9402 2023-03-11 22:49:04.000000 iamsystem-0.5.1/tests/test_tree.py
```

### Comparing `iamsystem-0.5.0/LICENSE` & `iamsystem-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/PKG-INFO` & `iamsystem-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamsystem
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python implementation of IAMsystem algorithm
 Author-email: Sebastien Cossin <cossin.sebastien@gmail.com>
 Project-URL: Homepage, https://github.com/scossin/iamsystem_python
 Project-URL: Bug Tracker, https://github.com/scossin/iamsystem_python/issues
 Keywords: NLP,semantic annotation,entity linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `iamsystem-0.5.0/README.md` & `iamsystem-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/pyproject.toml` & `iamsystem-0.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iamsystem"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Sebastien Cossin", email="cossin.sebastien@gmail.com" },
 ]
 description = "A python implementation of IAMsystem algorithm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `iamsystem-0.5.0/src/iamsystem/__init__.py` & `iamsystem-0.5.1/src/iamsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/brat/adapter.py` & `iamsystem-0.5.1/src/iamsystem/brat/adapter.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/brat/formatter.py` & `iamsystem-0.5.1/src/iamsystem/brat/formatter.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/abbreviations.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/abbreviations.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/api.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/cache.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/cache.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/exact.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/exact.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/norm_fun.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/norm_fun.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/regex.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/regex.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/simstring.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/simstring.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/spellwise.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/spellwise.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/fuzzy/util.py` & `iamsystem-0.5.1/src/iamsystem/fuzzy/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/keywords/api.py` & `iamsystem-0.5.1/src/iamsystem/keywords/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/keywords/collection.py` & `iamsystem-0.5.1/src/iamsystem/keywords/collection.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/keywords/keywords.py` & `iamsystem-0.5.1/src/iamsystem/keywords/keywords.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/keywords/util.py` & `iamsystem-0.5.1/src/iamsystem/keywords/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/matcher/annotation.py` & `iamsystem-0.5.1/src/iamsystem/matcher/annotation.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/matcher/api.py` & `iamsystem-0.5.1/src/iamsystem/matcher/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/matcher/matcher.py` & `iamsystem-0.5.1/src/iamsystem/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/matcher/printannot.py` & `iamsystem-0.5.1/src/iamsystem/matcher/printannot.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/matcher/strategy.py` & `iamsystem-0.5.1/src/iamsystem/matcher/strategy.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/matcher/util.py` & `iamsystem-0.5.1/src/iamsystem/matcher/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/spacy/component.py` & `iamsystem-0.5.1/src/iamsystem/spacy/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,19 @@
         """Add an extension to the spaCy Span class to store iamsystem's
         annotations."""
         if not Span.has_extension(self.attr):
             Span.set_extension(self.attr, default=None)
 
     def __call__(self, doc: Doc) -> Doc:
         """Function called by spaCy to execute this component."""
-        spans = self.process(doc)
         if self.attr not in doc.spans:
-            doc.spans[self.attr] = spans
+            doc.spans[self.attr] = []
+        iam_spans = self.process(doc)
+        for span in iam_spans:
+            doc.spans[self.attr].append(span)
         return doc
 
     def process(self, doc) -> List[Span]:
         """Annotate a document. Call IAMsystem algorithm."""
         tokens = self.matcher.tokenize(text=doc)
         anns: List[IAnnotation[TokenSpacyAdapter]] = self.matcher.annot_tokens(
             tokens=tokens
```

### Comparing `iamsystem-0.5.0/src/iamsystem/spacy/token.py` & `iamsystem-0.5.1/src/iamsystem/spacy/token.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/spacy/tokenizer.py` & `iamsystem-0.5.1/src/iamsystem/spacy/tokenizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,13 +28,14 @@
         """Tokenize a text. This function is used only to tokenize the
         keywords by the matcher since this custom component receives
         from spaCy the document already tokenized.
 
         :param text: a string to tokenize with spaCy component.
         :return: an ordered sequence of tokens.
         """
-        doc = self.nlp(text, disable=["iamsystem"])
-        tokens = [
-            TokenSpacyAdapter(spacy_token=token, norm_fun=self.norm_fun)
-            for token in doc
-        ]
-        return tokens
+        with self.nlp.select_pipes(enable="tokenizer"):
+            doc = self.nlp(text)
+            tokens = [
+                TokenSpacyAdapter(spacy_token=token, norm_fun=self.norm_fun)
+                for token in doc
+            ]
+            return tokens
```

### Comparing `iamsystem-0.5.0/src/iamsystem/stopwords/api.py` & `iamsystem-0.5.1/src/iamsystem/stopwords/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/stopwords/negative.py` & `iamsystem-0.5.1/src/iamsystem/stopwords/negative.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/stopwords/simple.py` & `iamsystem-0.5.1/src/iamsystem/stopwords/simple.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tokenization/api.py` & `iamsystem-0.5.1/src/iamsystem/tokenization/api.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tokenization/span.py` & `iamsystem-0.5.1/src/iamsystem/tokenization/span.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tokenization/token.py` & `iamsystem-0.5.1/src/iamsystem/tokenization/token.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tokenization/tokenize.py` & `iamsystem-0.5.1/src/iamsystem/tokenization/tokenize.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tokenization/util.py` & `iamsystem-0.5.1/src/iamsystem/tokenization/util.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tree/nodes.py` & `iamsystem-0.5.1/src/iamsystem/tree/nodes.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem/tree/trie.py` & `iamsystem-0.5.1/src/iamsystem/tree/trie.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/src/iamsystem.egg-info/PKG-INFO` & `iamsystem-0.5.1/src/iamsystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamsystem
-Version: 0.5.0
+Version: 0.5.1
 Summary: A python implementation of IAMsystem algorithm
 Author-email: Sebastien Cossin <cossin.sebastien@gmail.com>
 Project-URL: Homepage, https://github.com/scossin/iamsystem_python
 Project-URL: Bug Tracker, https://github.com/scossin/iamsystem_python/issues
 Keywords: NLP,semantic annotation,entity linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `iamsystem-0.5.0/src/iamsystem.egg-info/SOURCES.txt` & `iamsystem-0.5.1/src/iamsystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_annotation.py` & `iamsystem-0.5.1/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_brat.py` & `iamsystem-0.5.1/tests/test_brat.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_detect.py` & `iamsystem-0.5.1/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_doc.py` & `iamsystem-0.5.1/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_fuzzy.py` & `iamsystem-0.5.1/tests/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_matcher.py` & `iamsystem-0.5.1/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_simstring.py` & `iamsystem-0.5.1/tests/test_simstring.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_spacy.py` & `iamsystem-0.5.1/tests/test_spacy.py`

 * *Files 13% similar despite different names*

```diff
@@ -144,14 +144,46 @@
                 },
                 "build_params": {"w": 1},
             },
         )
         doc = nlp("insuffisance cardiaque gauche")
         self.assertEqual(1, len(doc.spans["iamsystem"]))
 
+    def test_component_name(self):
+        """Rename iamsystem component
+        https://github.com/scossin/iamsystem_python/issues/20"""
+        nlp = spacy.blank("fr")
+        nlp.add_pipe(
+            "iamsystem_matcher",
+            name="my_custom_name",
+            last=True,
+            config={"build_params": {"keywords": ["cancer"]}},
+        )
+        doc = nlp("prostate cancer")
+        self.assertEqual(1, len(doc.spans["iamsystem"]))
+
+    def test_multiple_components(self):
+        """Add several iam components.
+        Annotations are appended to the same attribute 'iamsystem'."""
+        nlp = spacy.blank("fr")
+        nlp.add_pipe(
+            "iamsystem_matcher",
+            name="first_iam_component",
+            last=True,
+            config={"build_params": {"keywords": ["cancer"]}},
+        )
+        nlp.add_pipe(
+            "iamsystem_matcher",
+            name="second_iam_component",
+            last=True,
+            config={"build_params": {"keywords": ["prostate"]}},
+        )
+        doc = nlp("prostate cancer")
+        self.assertEqual(2, len(doc.spans["iamsystem"]))
+
     def test_all_params(self):
         """Test it words with all the parameters."""
         nlp = French()
         nlp.add_pipe(
             "iamsystem_matcher",
             name="iamsystem",
             last=True,
```

### Comparing `iamsystem-0.5.0/tests/test_spellwise.py` & `iamsystem-0.5.1/tests/test_spellwise.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_stopwords.py` & `iamsystem-0.5.1/tests/test_stopwords.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_terminology.py` & `iamsystem-0.5.1/tests/test_terminology.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_toknorm.py` & `iamsystem-0.5.1/tests/test_toknorm.py`

 * *Files identical despite different names*

### Comparing `iamsystem-0.5.0/tests/test_tree.py` & `iamsystem-0.5.1/tests/test_tree.py`

 * *Files identical despite different names*

