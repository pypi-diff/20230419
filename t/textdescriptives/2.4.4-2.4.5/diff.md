# Comparing `tmp/textdescriptives-2.4.4.tar.gz` & `tmp/textdescriptives-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdescriptives-2.4.4.tar", last modified: Tue Mar 28 15:06:31 2023, max compression
+gzip compressed data, was "textdescriptives-2.4.5.tar", last modified: Wed Apr 19 20:55:45 2023, max compression
```

## Comparing `textdescriptives-2.4.4.tar` & `textdescriptives-2.4.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.010877 textdescriptives-2.4.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.994877 textdescriptives-2.4.4/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.994877 textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      582 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/01_bugs.md
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/02_docs.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/03_feature-request.md
--rw-r--r--   0 root         (0) root         (0)      632 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)      776 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.994877 textdescriptives-2.4.4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)     1161 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      669 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/workflows/draft-pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1673 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)      867 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/workflows/stale.yml
--rw-r--r--   0 root         (0) root         (0)     2261 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.github/workflows/tests.yml
--rw-r--r--   0 root         (0) root         (0)     2140 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1388 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      907 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)     6114 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/CITATION.cff
--rw-r--r--   0 root         (0) root         (0)     5242 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4473 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23468 2023-03-28 15:06:31.010877 textdescriptives-2.4.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9111 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.998877 textdescriptives-2.4.4/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.998877 textdescriptives-2.4.4/docs/_static/
--rw-r--r--   0 root         (0) root         (0)   642030 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)   139565 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/_static/icon_dark_old.png
--rw-r--r--   0 root         (0) root         (0)   125611 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/_static/icon_old.png
--rw-r--r--   0 root         (0) root         (0)     3540 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/coherence.rst
--rw-r--r--   0 root         (0) root         (0)     3548 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     3189 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/dependencydistance.rst
--rw-r--r--   0 root         (0) root         (0)     3198 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/descriptivestats.rst
--rw-r--r--   0 root         (0) root         (0)      477 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/extractors.rst
--rw-r--r--   0 root         (0) root         (0)     1909 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     2627 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     2140 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/information_theory.rst
--rw-r--r--   0 root         (0) root         (0)      859 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      795 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      987 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/news.rst
--rw-r--r--   0 root         (0) root         (0)     2082 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/posstats.rst
--rw-r--r--   0 root         (0) root         (0)     8242 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/quality.rst
--rw-r--r--   0 root         (0) root         (0)     1869 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/readability.rst
--rw-r--r--   0 root         (0) root         (0)      349 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/tutorial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.998877 textdescriptives-2.4.4/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)    96577 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/tutorials/filter_corpus_using_quality.ipynb
--rw-r--r--   0 root         (0) root         (0)   115694 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/tutorials/introductory_tutorial.ipynb
--rw-r--r--   0 root         (0) root         (0)      273 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/tutorials/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     7465 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/docs/usingthepackage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.002877 textdescriptives-2.4.4/paper/
--rw-r--r--   0 root         (0) root         (0)    23688 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     8736 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)    42220 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/paper/paper_quarto.pdf
--rw-r--r--   0 root         (0) root         (0)     9724 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/paper/paper_quarto.qmd
--rw-r--r--   0 root         (0) root         (0)      473 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/paper/readme.md
--rw-r--r--   0 root         (0) root         (0)     3059 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-28 15:06:31.010877 textdescriptives-2.4.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:30.990877 textdescriptives-2.4.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.002877 textdescriptives-2.4.4/src/textdescriptives/
--rw-r--r--   0 root         (0) root         (0)      328 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/__init__.py
--rw-r--r--   0 root         (0) root         (0)      492 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/about.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.006877 textdescriptives-2.4.4/src/textdescriptives/components/
--rw-r--r--   0 root         (0) root         (0)      396 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5351 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/coherence.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     7504 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5515 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/information_theory.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)    22190 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/quality.py
--rw-r--r--   0 root         (0) root         (0)    10426 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/quality_data_classes.py
--rw-r--r--   0 root         (0) root         (0)     7713 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/readability.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/components/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.006877 textdescriptives-2.4.4/src/textdescriptives/data/
--rw-r--r--   0 root         (0) root         (0)   503663 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/data/spam.csv
--rw-r--r--   0 root         (0) root         (0)     6024 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/extractors.py
--rw-r--r--   0 root         (0) root         (0)     1330 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/load_components.py
--rw-r--r--   0 root         (0) root         (0)     6197 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/src/textdescriptives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.002877 textdescriptives-2.4.4/src/textdescriptives.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23468 2023-03-28 15:06:30.000000 textdescriptives-2.4.4/src/textdescriptives.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2365 2023-03-28 15:06:30.000000 textdescriptives-2.4.4/src/textdescriptives.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 15:06:30.000000 textdescriptives-2.4.4/src/textdescriptives.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      493 2023-03-28 15:06:30.000000 textdescriptives-2.4.4/src/textdescriptives.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-03-28 15:06:30.000000 textdescriptives-2.4.4/src/textdescriptives.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 15:06:31.010877 textdescriptives-2.4.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28399 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/books.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     2816 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_coherence.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_dependency_distance.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_descriptive_stats.py
--rw-r--r--   0 root         (0) root         (0)     5283 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_extractors.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_information.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_load_components.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_pos_proportions.py
--rw-r--r--   0 root         (0) root         (0)     9246 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_quality.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_readability.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-03-28 15:06:20.000000 textdescriptives-2.4.4/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/01_bugs.md
+-rw-r--r--   0 root         (0) root         (0)      418 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/02_docs.md
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/03_feature-request.md
+-rw-r--r--   0 root         (0) root         (0)      632 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      776 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/dependabot.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      669 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/draft-pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)      867 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/stale.yml
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.github/workflows/tests.yml
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)     6703 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1150 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/CITATION.cff
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23998 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9641 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)   642030 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)   139565 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/_static/icon_dark_old.png
+-rw-r--r--   0 root         (0) root         (0)   125611 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/_static/icon_old.png
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/coherence.rst
+-rw-r--r--   0 root         (0) root         (0)     3548 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/dependencydistance.rst
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/descriptivestats.rst
+-rw-r--r--   0 root         (0) root         (0)      477 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/extractors.rst
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/information_theory.rst
+-rw-r--r--   0 root         (0) root         (0)      859 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      795 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      987 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/news.rst
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/posstats.rst
+-rw-r--r--   0 root         (0) root         (0)     8242 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/quality.rst
+-rw-r--r--   0 root         (0) root         (0)     1869 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/readability.rst
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)    96689 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorials/filter_corpus_using_quality.ipynb
+-rw-r--r--   0 root         (0) root         (0)   115780 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorials/introductory_tutorial.ipynb
+-rw-r--r--   0 root         (0) root         (0)      273 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/tutorials/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     7465 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/docs/usingthepackage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/paper/
+-rw-r--r--   0 root         (0) root         (0)    23688 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)    42220 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper_quarto.pdf
+-rw-r--r--   0 root         (0) root         (0)     9724 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/paper_quarto.qmd
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/paper/readme.md
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.565709 textdescriptives-2.4.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.569709 textdescriptives-2.4.5/src/textdescriptives/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-04-19 20:55:34.000000 textdescriptives-2.4.5/src/textdescriptives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      492 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/about.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.573709 textdescriptives-2.4.5/src/textdescriptives/components/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5353 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/coherence.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     7504 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5515 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/information_theory.py
+-rw-r--r--   0 root         (0) root         (0)     3380 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)    22254 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/quality.py
+-rw-r--r--   0 root         (0) root         (0)    10426 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/quality_data_classes.py
+-rw-r--r--   0 root         (0) root         (0)     7713 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/readability.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/components/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.573709 textdescriptives-2.4.5/src/textdescriptives/data/
+-rw-r--r--   0 root         (0) root         (0)   503663 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/data/spam.csv
+-rw-r--r--   0 root         (0) root         (0)     6042 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/load_components.py
+-rw-r--r--   0 root         (0) root         (0)     6203 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/src/textdescriptives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.573709 textdescriptives-2.4.5/src/textdescriptives.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23998 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      493 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-19 20:55:45.000000 textdescriptives-2.4.5/src/textdescriptives.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 20:55:45.577709 textdescriptives-2.4.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28399 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/books.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_coherence.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_dependency_distance.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_descriptive_stats.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_extractors.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_information.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_load_components.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_pos_proportions.py
+-rw-r--r--   0 root         (0) root         (0)     9305 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_quality.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_readability.py
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-19 20:55:35.000000 textdescriptives-2.4.5/tests/test_utils.py
```

### Comparing `textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/01_bugs.md` & `textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/01_bugs.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/ISSUE_TEMPLATE/config.yml` & `textdescriptives-2.4.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/dependabot.yml` & `textdescriptives-2.4.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/workflows/dependabot_automerge.yml` & `textdescriptives-2.4.5/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/workflows/documentation.yml` & `textdescriptives-2.4.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/workflows/draft-pdf.yml` & `textdescriptives-2.4.5/.github/workflows/draft-pdf.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/workflows/release.yml` & `textdescriptives-2.4.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/workflows/stale.yml` & `textdescriptives-2.4.5/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.github/workflows/tests.yml` & `textdescriptives-2.4.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.gitignore` & `textdescriptives-2.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/.pre-commit-config.yaml` & `textdescriptives-2.4.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
   #           --wrap-descriptions,
   #           "80",
   #           --wrap-summaries,
   #           "80",
   #         ]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
         #args: [--line-length, "88"]
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.257
+    rev: v0.0.261
     hooks:
       - id: ruff
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
```

### Comparing `textdescriptives-2.4.4/.zenodo.json` & `textdescriptives-2.4.5/.zenodo.json`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/CHANGELOG.md` & `textdescriptives-2.4.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.4.5 (2023-04-19)
+### Fix
+* Dep dist. test ([`a3b54a6`](https://github.com/HLasse/TextDescriptives/commit/a3b54a6b3e3d57acc140b0f9afd72406a88104f8))
+* Coherence model now handles empty strings as intended ([`abfa507`](https://github.com/HLasse/TextDescriptives/commit/abfa5071ba075f25ff8c170f5cee4f84ef648ea5))
+* Dep distance test ([`2bed2c1`](https://github.com/HLasse/TextDescriptives/commit/2bed2c194b98062aad66d6ca0985fb92af6be977))
+
+### Documentation
+* Added demo to docs ([`6121eeb`](https://github.com/HLasse/TextDescriptives/commit/6121eebc0a125e68979591f6c585d19fae70746b))
+
 ## v2.4.4 (2023-03-28)
 ### Fix
 * Add .zenodo.json ([`3cc463c`](https://github.com/HLasse/TextDescriptives/commit/3cc463c5bcc236bb5c49fc51eaba0b419d84ffcc))
 
 ### Documentation
 * Add test requirements to faq ([`1550de7`](https://github.com/HLasse/TextDescriptives/commit/1550de7c4815779f53cc8ba260ddedcdbf8f0358))
```

### Comparing `textdescriptives-2.4.4/CITATION.cff` & `textdescriptives-2.4.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/CODE_OF_CONDUCT.md` & `textdescriptives-2.4.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/CONTRIBUTING.md` & `textdescriptives-2.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/LICENSE` & `textdescriptives-2.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/PKG-INFO` & `textdescriptives-2.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.4.4
+Version: 2.4.5
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -238,22 +238,24 @@
 # TextDescriptives
 
 [![spacy](https://img.shields.io/badge/built%20with-spaCy-09a3d5.svg)](https://spacy.io)
 [![github actions pytest](https://github.com/hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://github.com/hlasse/textdescriptives/actions)
 [![github actions docs](https://github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/badge.svg)](https://hlasse.github.io/TextDescriptives/)
 [![arXiv](https://img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/2301.02057)
 [![status](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24)
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://huggingface.co/spaces/HLasse/textdescriptives)
 
 A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
+* We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
 * Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://github.com/HLasse/TextDescriptives) for tutorials and more information!  
 
 
 
 # ⚡ Quick Start
 
 Use `extract_metrics` to quickly extract your desired metrics. To see available methods you can simply run:
@@ -316,17 +318,19 @@
 TextDescriptives has a detailed documentation as well as a series of Jupyter notebook tutorials.
 All the tutorials are located in the `docs/tutorials` folder and can also be found on the documentation website.
 
 
 | Documentation              |                                                                                    |
 | -------------------------- | ---------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use TextDescriptives and its features.           |
+| 👩‍💻 **[Demo]**               | A live demo of TextDescriptives.                                                   |
 | 😎 **[Tutorials]**          | Detailed tutorials on how to make the most of TextDescriptives                     |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                        |
 | 🎛 **[API References]**     | The detailed reference for TextDescriptive's API. Including function documentation |
 | 📄 **[Paper]**              | The preprint of the TextDescriptives paper.                                        |
 
 [Paper]: https://arxiv.org/abs/2301.02057
 [Tutorials]: https://hlasse.github.io/TextDescriptives/tutorial.html
 [Getting started]: https://hlasse.github.io/TextDescriptives/usingthepackage.html
 [API References]: https://hlasse.github.io/TextDescriptives/index.html
 [News and changelog]: https://hlasse.github.io/TextDescriptives/news.html
+[Demo]: https://huggingface.co/spaces/HLasse/textdescriptives
```

### Comparing `textdescriptives-2.4.4/README.md` & `textdescriptives-2.4.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 # TextDescriptives
 
 [![spacy](https://img.shields.io/badge/built%20with-spaCy-09a3d5.svg)](https://spacy.io)
 [![github actions pytest](https://github.com/hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://github.com/hlasse/textdescriptives/actions)
 [![github actions docs](https://github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/badge.svg)](https://hlasse.github.io/TextDescriptives/)
 [![arXiv](https://img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/2301.02057)
 [![status](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24)
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://huggingface.co/spaces/HLasse/textdescriptives)
 
 A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
+* We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
 * Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://github.com/HLasse/TextDescriptives) for tutorials and more information!  
 
 
 
 # ⚡ Quick Start
 
 Use `extract_metrics` to quickly extract your desired metrics. To see available methods you can simply run:
@@ -83,17 +85,19 @@
 TextDescriptives has a detailed documentation as well as a series of Jupyter notebook tutorials.
 All the tutorials are located in the `docs/tutorials` folder and can also be found on the documentation website.
 
 
 | Documentation              |                                                                                    |
 | -------------------------- | ---------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use TextDescriptives and its features.           |
+| 👩‍💻 **[Demo]**               | A live demo of TextDescriptives.                                                   |
 | 😎 **[Tutorials]**          | Detailed tutorials on how to make the most of TextDescriptives                     |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                        |
 | 🎛 **[API References]**     | The detailed reference for TextDescriptive's API. Including function documentation |
 | 📄 **[Paper]**              | The preprint of the TextDescriptives paper.                                        |
 
 [Paper]: https://arxiv.org/abs/2301.02057
 [Tutorials]: https://hlasse.github.io/TextDescriptives/tutorial.html
 [Getting started]: https://hlasse.github.io/TextDescriptives/usingthepackage.html
 [API References]: https://hlasse.github.io/TextDescriptives/index.html
 [News and changelog]: https://hlasse.github.io/TextDescriptives/news.html
+[Demo]: https://huggingface.co/spaces/HLasse/textdescriptives
```

#### html2text {}

```diff
@@ -4,50 +4,54 @@
 hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://
 github.com/hlasse/textdescriptives/actions) [![github actions docs](https://
 github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/
 badge.svg)](https://hlasse.github.io/TextDescriptives/) [![arXiv](https://
 img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/
 2301.02057) [![status](https://joss.theoj.org/papers/
 06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/
-06447337ee61969b5a64de484199df24) A Python library for calculating a large
-variety of metrics from text(s) using spaCy v.3 pipeline components and
+06447337ee61969b5a64de484199df24) [![Open in Streamlit](https://
+static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://
+huggingface.co/spaces/HLasse/textdescriptives) A Python library for calculating
+a large variety of metrics from text(s) using spaCy v.3 pipeline components and
 extensions. TextDescriptives can be used to calculate several descriptive
 statistics, readability metrics, and metrics related to dependency distance. #
-ð§ Installation `pip install textdescriptives` # ð° News * Version 2.0 out
-with a new API, a new component, updated documentation, and tutorials!
-Components are now called by "`textdescriptives/{metric_name}`. New `coherence`
-component for calculating the semantic coherence between sentences. See the
-[documentation](https://github.com/HLasse/TextDescriptives) for tutorials and
-more information! # â¡ Quick Start Use `extract_metrics` to quickly extract
-your desired metrics. To see available methods you can simply run: ```python
-import textdescriptives as td td.get_valid_metrics() # {'quality',
-'readability', 'all', 'descriptive_stats', 'dependency_distance',
-'pos_proportions', 'information_theory', 'coherence'} ``` Set the `spacy_model`
-parameter to specify which spaCy model to use, otherwise, TextDescriptives will
-auto-download an appropriate one based on `lang`. If `lang` is set,
-`spacy_model` is not necessary and vice versa. Specify which metrics to extract
-in the `metrics` argument. `None` extracts all metrics. ```py import
-textdescriptives as td text = "The world is changed. I feel it in the water. I
-feel it in the earth. I smell it in the air. Much that once was is lost, for
-none now live who remember it." # will automatically download the relevant
-model (Â´en_core_web_lgÂ´) and extract all metrics df = td.extract_metrics
-(text=text, lang="en", metrics=None) # specify spaCy model and which metrics to
-extract df = td.extract_metrics(text=text, spacy_model="en_core_web_lg",
-metrics=["readability", "coherence"]) ``` ## Usage with spaCy To integrate with
-other spaCy pipelines, import the library and add the component(s) to your
-pipeline using the standard spaCy syntax. Available components are
-*descriptive_stats*, *readability*, *dependency_distance*, *pos_proportions*,
-*coherence*, and *quality* prefixed with `textdescriptives/`. If you want to
-add all components you can use the shorthand `textdescriptives/all`. ```py
-import spacy import textdescriptives as td # load your favourite spacy model
-(remember to install it first using e.g. `python -m spacy download
-en_core_web_sm`) nlp = spacy.load("en_core_web_sm") nlp.add_pipe
-("textdescriptives/all") doc = nlp("The world is changed. I feel it in the
-water. I feel it in the earth. I smell it in the air. Much that once was is
-lost, for none now live who remember it.") # access some of the values
+ð§ Installation `pip install textdescriptives` # ð° News * We now have a
+TextDescriptives-powered web-app so you can extract and downloads metrics
+without a single line of code! Check it out [here](https://huggingface.co/
+spaces/HLasse/textdescriptives) * Version 2.0 out with a new API, a new
+component, updated documentation, and tutorials! Components are now called by
+"`textdescriptives/{metric_name}`. New `coherence` component for calculating
+the semantic coherence between sentences. See the [documentation](https://
+github.com/HLasse/TextDescriptives) for tutorials and more information! # â¡
+Quick Start Use `extract_metrics` to quickly extract your desired metrics. To
+see available methods you can simply run: ```python import textdescriptives as
+td td.get_valid_metrics() # {'quality', 'readability', 'all',
+'descriptive_stats', 'dependency_distance', 'pos_proportions',
+'information_theory', 'coherence'} ``` Set the `spacy_model` parameter to
+specify which spaCy model to use, otherwise, TextDescriptives will auto-
+download an appropriate one based on `lang`. If `lang` is set, `spacy_model` is
+not necessary and vice versa. Specify which metrics to extract in the `metrics`
+argument. `None` extracts all metrics. ```py import textdescriptives as td text
+= "The world is changed. I feel it in the water. I feel it in the earth. I
+smell it in the air. Much that once was is lost, for none now live who remember
+it." # will automatically download the relevant model (Â´en_core_web_lgÂ´) and
+extract all metrics df = td.extract_metrics(text=text, lang="en", metrics=None)
+# specify spaCy model and which metrics to extract df = td.extract_metrics
+(text=text, spacy_model="en_core_web_lg", metrics=["readability", "coherence"])
+``` ## Usage with spaCy To integrate with other spaCy pipelines, import the
+library and add the component(s) to your pipeline using the standard spaCy
+syntax. Available components are *descriptive_stats*, *readability*,
+*dependency_distance*, *pos_proportions*, *coherence*, and *quality* prefixed
+with `textdescriptives/`. If you want to add all components you can use the
+shorthand `textdescriptives/all`. ```py import spacy import textdescriptives as
+td # load your favourite spacy model (remember to install it first using e.g.
+`python -m spacy download en_core_web_sm`) nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("textdescriptives/all") doc = nlp("The world is changed. I feel it
+in the water. I feel it in the earth. I smell it in the air. Much that once was
+is lost, for none now live who remember it.") # access some of the values
 doc._.readability doc._.token_length ``` TextDescriptives includes convenience
 functions for extracting metrics from a `Doc` to a Pandas DataFrame or a
 dictionary. ```py td.extract_dict(doc) td.extract_df(doc) ``` | | text |
 first_order_coherence | second_order_coherence | pos_prop_DET | pos_prop_NOUN |
 pos_prop_AUX | pos_prop_VERB | pos_prop_PUNCT | pos_prop_PRON | pos_prop_ADP |
 pos_prop_ADV | pos_prop_SCONJ | flesch_reading_ease | flesch_kincaid_grade |
 smog | gunning_fog | automated_readability_index | coleman_liau_index | lix |
@@ -89,17 +93,19 @@
 0.0722806 | 3.28571 | 3 | 1.54127 | 7 | 6 | 3.09839 | 1.08571 | 1 | 0.368117 |
 35 | 23 | 0.657143 | 121 | 5 | # ð Documentation TextDescriptives has a
 detailed documentation as well as a series of Jupyter notebook tutorials. All
 the tutorials are located in the `docs/tutorials` folder and can also be found
 on the documentation website. | Documentation | | | -------------------------
 - | ---------------------------------------------------------------------------
 ------- | | ð **[Getting started]** | Guides and instructions on how to use
-TextDescriptives and its features. | | ð **[Tutorials]** | Detailed
-tutorials on how to make the most of TextDescriptives | | ð° **[News and
-changelog]** | New additions, changes and version history. | | ð **[API
-References]** | The detailed reference for TextDescriptive's API. Including
-function documentation | | ð **[Paper]** | The preprint of the
-TextDescriptives paper. | [Paper]: https://arxiv.org/abs/2301.02057
-[Tutorials]: https://hlasse.github.io/TextDescriptives/tutorial.html [Getting
-started]: https://hlasse.github.io/TextDescriptives/usingthepackage.html [API
-References]: https://hlasse.github.io/TextDescriptives/index.html [News and
-changelog]: https://hlasse.github.io/TextDescriptives/news.html
+TextDescriptives and its features. | | ð©âð» **[Demo]** | A live demo of
+TextDescriptives. | | ð **[Tutorials]** | Detailed tutorials on how to make
+the most of TextDescriptives | | ð° **[News and changelog]** | New additions,
+changes and version history. | | ð **[API References]** | The detailed
+reference for TextDescriptive's API. Including function documentation | | ð
+**[Paper]** | The preprint of the TextDescriptives paper. | [Paper]: https://
+arxiv.org/abs/2301.02057 [Tutorials]: https://hlasse.github.io/
+TextDescriptives/tutorial.html [Getting started]: https://hlasse.github.io/
+TextDescriptives/usingthepackage.html [API References]: https://
+hlasse.github.io/TextDescriptives/index.html [News and changelog]: https://
+hlasse.github.io/TextDescriptives/news.html [Demo]: https://huggingface.co/
+spaces/HLasse/textdescriptives
```

### Comparing `textdescriptives-2.4.4/docs/Makefile` & `textdescriptives-2.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/_static/icon.png` & `textdescriptives-2.4.5/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/_static/icon_dark_old.png` & `textdescriptives-2.4.5/docs/_static/icon_dark_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/_static/icon_old.png` & `textdescriptives-2.4.5/docs/_static/icon_old.png`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/coherence.rst` & `textdescriptives-2.4.5/docs/coherence.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/conf.py` & `textdescriptives-2.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/dependencydistance.rst` & `textdescriptives-2.4.5/docs/dependencydistance.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/descriptivestats.rst` & `textdescriptives-2.4.5/docs/descriptivestats.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/faq.rst` & `textdescriptives-2.4.5/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/index.rst` & `textdescriptives-2.4.5/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ================================
 
 .. image:: https://img.shields.io/github/stars/hlasse/textdescriptives.svg?style=social&label=Star&maxAge=2592000
    :target: https://github.com/hlasse/textdescriptives
 
 TextDescriptives is Python library for calculating a large variety of statistics from text(s) using spaCy v.3 pipeline components and extensions. 
 TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
+If you wish to try out the package, you can use the `online demo <https://huggingface.co/spaces/HLasse/textdescriptives>`__.
   
 The documentation is organized in two parts:
 
 - **Getting Started** contains the installation instructions, guides, and tutorials on how to use the package.
 - **Package References** contains the documentation of each public class and function.
```

### Comparing `textdescriptives-2.4.4/docs/information_theory.rst` & `textdescriptives-2.4.5/docs/information_theory.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/installation.rst` & `textdescriptives-2.4.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/make.bat` & `textdescriptives-2.4.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/news.rst` & `textdescriptives-2.4.5/docs/news.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/posstats.rst` & `textdescriptives-2.4.5/docs/posstats.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Part-of-Speech Proportions
 -----------------------------
 
-The *pos_stats* component adds one attribute to a Doc or Span:
+The *pos_proportions* component adds one attribute to a Doc or Span:
 
 * :code:`Doc._.pos_proportions` 
     * Dict of :code:`{pos_prop_POSTAG: proportion of all tokens tagged with POSTAG}`. Does not create a key if no tokens in the document fit the POSTAG.
 
 * :code:`Span._.pos_proportions`
 * 
     * Dict of :code:`{pos_prop_POSTAG: proportion of all tokens tagged with POSTAG}`. Does not create a key if no tokens in the document fit the POSTAG.
@@ -37,8 +37,8 @@
 
 -----
 
 
 Component
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. autofunction:: textdescriptives.components.pos_proportions.create_pos_stats_component
+.. autofunction:: textdescriptives.components.pos_proportions.create_pos_proportions_component
```

### Comparing `textdescriptives-2.4.4/docs/quality.rst` & `textdescriptives-2.4.5/docs/quality.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/readability.rst` & `textdescriptives-2.4.5/docs/readability.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/docs/tutorials/filter_corpus_using_quality.ipynb` & `textdescriptives-2.4.5/docs/tutorials/filter_corpus_using_quality.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989214652846287%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(3, \'dataset = load_dataset("mc4", "en", streaming=True, '*

 * *            'split="train")\\n\'), (9, \'texts = [sample["text"] for sample in dataset]\')], '*

 * *            "delete: [9, 3]}}, 6: {'source': {insert: [(1, 'print(texts[0][:400])')], delete: "*

 * *            '[1]}}, 20: {\'source\': [\'print(\\n\', \'    f"A total of {len(docs)} texts were '*

 * *            'processed and {len(filtered_texts)} passed the quality check."\\n\', \')\']}, 22: '*

 * *            "{'source': {in […]*

```diff
@@ -69,21 +69,21 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from datasets import load_dataset\n",
                 "\n",
                 "# stream in the dataset\n",
-                "dataset = load_dataset(\"mc4\", \"en\", streaming = True, split = \"train\")\n",
+                "dataset = load_dataset(\"mc4\", \"en\", streaming=True, split=\"train\")\n",
                 "\n",
                 "# download the first 1 000\n",
                 "dataset = dataset.take(1000)\n",
                 "\n",
                 "# extract the text\n",
-                "texts = [sample [\"text\"] for sample in dataset]\n"
+                "texts = [sample[\"text\"] for sample in dataset]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
@@ -94,15 +94,15 @@
                         "Posts 4,362\tMore Info\n",
                         "Okay so to those of you that were very helpful this is not to you but for those of you that laugh when I ask about ohms or powering LSi15's this is to you. If you know a book, website, or someone to talk to to get more info that I seek so I know what some of you are talking about please share it with me. I ask questions to gain more info on audio thats all. Not to get laughed\n"
                     ]
                 }
             ],
             "source": [
                 "# let us look at the first part (400 characters) of the first text\n",
-                "print(texts[0][:400])\n"
+                "print(texts[0][:400])"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -309,15 +309,17 @@
                     "output_type": "stream",
                     "text": [
                         "A total of 1000 texts were processed and 572 passed the quality check.\n"
                     ]
                 }
             ],
             "source": [
-                "print(f\"A total of {len(docs)} texts were processed and {len(filtered_texts)} passed the quality check.\")"
+                "print(\n",
+                "    f\"A total of {len(docs)} texts were processed and {len(filtered_texts)} passed the quality check.\"\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -328,26 +330,28 @@
         {
             "cell_type": "code",
             "execution_count": 42,
             "metadata": {},
             "outputs": [],
             "source": [
                 "new_thresholds = td.QualityThresholds(\n",
-                "    n_stop_words=(2, None), # at least 2 stop words, no upper bound\n",
-                "    alpha_ratio= (0.7, None),\n",
-                "    mean_word_length= (3, 10), # mean word length between 3 and 10 characters\n",
-                "    doc_length = (10, 100_000),\n",
-                "    symbol_to_word_ratio = {}, # don't filter based on symbol to word ratio.\n",
-                "    proportion_ellipsis = (None, 0.3),\n",
-                "    proportion_bullet_points = (None, 0.8),\n",
-                "    contains = {\"lorem ipsum\": False}, # remove texts which contain the string \"lorem ipsum\"\n",
-                "    duplicate_line_chr_fraction = (None, 0.2),\n",
-                "    duplicate_paragraph_chr_fraction = (None, 0.2),\n",
-                "    duplicate_ngram_chr_fraction = {}, # don't filter based on duplicate n-grams\n",
-                "    top_ngram_chr_fraction = {\"2\": (None, 0.2), \"3\": (None, 0.18), \"4\": (None, 0.16)}\n",
+                "    n_stop_words=(2, None),  # at least 2 stop words, no upper bound\n",
+                "    alpha_ratio=(0.7, None),\n",
+                "    mean_word_length=(3, 10),  # mean word length between 3 and 10 characters\n",
+                "    doc_length=(10, 100_000),\n",
+                "    symbol_to_word_ratio={},  # don't filter based on symbol to word ratio.\n",
+                "    proportion_ellipsis=(None, 0.3),\n",
+                "    proportion_bullet_points=(None, 0.8),\n",
+                "    contains={\n",
+                "        \"lorem ipsum\": False\n",
+                "    },  # remove texts which contain the string \"lorem ipsum\"\n",
+                "    duplicate_line_chr_fraction=(None, 0.2),\n",
+                "    duplicate_paragraph_chr_fraction=(None, 0.2),\n",
+                "    duplicate_ngram_chr_fraction={},  # don't filter based on duplicate n-grams\n",
+                "    top_ngram_chr_fraction={\"2\": (None, 0.2), \"3\": (None, 0.18), \"4\": (None, 0.16)},\n",
                 ")\n",
                 "\n",
                 "# overwrite the existing thresholds\n",
                 "quality_pipe.set_quality_thresholds(new_thresholds)"
             ]
         },
         {
@@ -767,15 +771,17 @@
             "execution_count": 18,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# 1. Crease a blank spaCy model with a sentencizer as that's the only component required for the quality metrics\n",
                 "nlp = spacy.blank(\"da\")\n",
                 "nlp.add_pipe(\"sentencizer\")\n",
-                "nlp.max_length = 2000000  # as some of the documents are quite long we can increase the max length\n",
+                "nlp.max_length = (\n",
+                "    2000000  # as some of the documents are quite long we can increase the max length\n",
+                ")\n",
                 "# however it might be worth filtering out these documents beforehand for very very long documents.\n",
                 "\n",
                 "# 2. Add the textdescriptives pipeline\n",
                 "quality_pipe = nlp.add_pipe(\"textdescriptives/quality\")\n",
                 "\n",
                 "# 3. Apply the pipeline to the legal documents\n",
                 "legal_docs = nlp.pipe(legal[\"text\"])"
@@ -855,15 +861,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "legal_doc = legal_docs[0]\n",
                 "\n",
-                "print(legal_doc[:100]) # print the first 100 tokens\n",
+                "print(legal_doc[:100])  # print the first 100 tokens\n",
                 "print(\"----\")\n",
                 "print(\"This passed the quality filter:\")\n",
                 "legal_doc._.passed_quality_check"
             ]
         },
         {
             "attachments": {},
@@ -913,15 +919,15 @@
         {
             "cell_type": "code",
             "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# 4. Filter out the documents that do not pass the quality\n",
-                "legal_docs_filtered = [doc for doc in legal_docs if doc._.passed_quality_check]\n"
+                "legal_docs_filtered = [doc for doc in legal_docs if doc._.passed_quality_check]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 24,
             "metadata": {},
             "outputs": [
@@ -930,15 +936,17 @@
                     "output_type": "stream",
                     "text": [
                         "We had a total of 1000 which we filtered down to 264.\n"
                     ]
                 }
             ],
             "source": [
-                "print(f\"We had a total of {len(legal['text'])} which we filtered down to {len(legal_docs_filtered)}.\")"
+                "print(\n",
+                "    f\"We had a total of {len(legal['text'])} which we filtered down to {len(legal_docs_filtered)}.\"\n",
+                ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -970,19 +978,21 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import seaborn as sns\n",
                 "\n",
+                "\n",
                 "def get_duplicate_10_gram_fraction(doc):\n",
                 "    quality = doc._.quality\n",
                 "    duplicate_10_gram_fraction = quality.duplicate_ngram_chr_fraction[\"10\"]\n",
                 "    return duplicate_10_gram_fraction.value\n",
                 "\n",
+                "\n",
                 "duplicate_10_gram_fraction = [get_duplicate_10_gram_fraction(doc) for doc in legal_docs]\n",
                 "sns.histplot(duplicate_10_gram_fraction)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -1093,14 +1103,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import matplotlib.pyplot as plt\n",
+                "\n",
                 "# histogram\n",
                 "sns.histplot(news_alpha_ratio, label=\"News\", alpha=0.5, binwidth=0.05)\n",
                 "sns.histplot(alpha_ratio, label=\"Legal\", alpha=0.5, binwidth=0.05)\n",
                 "sns.histplot(speech_alpha_ratio, label=\"Speech\", alpha=0.5, binwidth=0.05)\n",
                 "\n",
                 "# add labels\n",
                 "plt.xlabel(\"Alpha ratio\")\n",
```

### Comparing `textdescriptives-2.4.4/docs/tutorials/introductory_tutorial.ipynb` & `textdescriptives-2.4.5/docs/tutorials/introductory_tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988821866539257%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(1, 'metrics = td.extract_metrics(\\n'), (2, '    "*

 * *            'text=df["message"],\\n\'), (3, \'    spacy_model="en_core_web_sm",\\n\'), (4, \'    '*

 * *            'metrics=["readability", "dependency_distance"],\\n\'), (5, \')\\n\')], delete: [1]}}, '*

 * *            "9: {'source': {delete: [0]}}, 17: {'source': {insert: [(1, '\\n')]}}, 19: {'source': "*

 * *            "{insert: [(3, 'metrics_correlations = "*

 * *            'metrics.corrwith(metrics_df["is_ham"]).sort_values(\\n\' […]*

```diff
@@ -403,15 +403,19 @@
                     "execution_count": 3,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# assumes you have downloaded the \u00b4en_core_web_model\u00b4\n",
-                "metrics = td.extract_metrics(text=df[\"message\"], spacy_model=\"en_core_web_sm\", metrics=[\"readability\", \"dependency_distance\"])\n",
+                "metrics = td.extract_metrics(\n",
+                "    text=df[\"message\"],\n",
+                "    spacy_model=\"en_core_web_sm\",\n",
+                "    metrics=[\"readability\", \"dependency_distance\"],\n",
+                ")\n",
                 "# alternatively, you can specify the language and (optionally) the model size\n",
                 "# metrics = td.extract_metrics(text=df[\"message\"], lang=\"en\", spacy_model_size=\"sm\", metrics=[\"readability, dependency_distance\"])\n",
                 "\n",
                 "# join the metrics to the original dataframe to get the label\n",
                 "metrics_df = df.join(metrics.drop(columns=[\"text\"]))\n",
                 "metrics_df.head()"
             ]
@@ -463,15 +467,14 @@
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "\n",
                 "nlp.add_pipe(\"textdescriptives/readability\")\n",
                 "nlp.add_pipe(\"textdescriptives/dependency_distance\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -805,14 +808,15 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import seaborn as sns\n",
+                "\n",
                 "sns.boxplot(x=\"label\", y=\"lix\", data=metrics_df)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -845,15 +849,17 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# encode the label as a boolean\n",
                 "metrics_df[\"is_ham\"] = metrics_df[\"label\"] == \"ham\"\n",
                 "# compute the correlation between all metrics and the label\n",
-                "metrics_correlations = metrics.corrwith(metrics_df[\"is_ham\"]).sort_values(key=abs, ascending=False)\n",
+                "metrics_correlations = metrics.corrwith(metrics_df[\"is_ham\"]).sort_values(\n",
+                "    key=abs, ascending=False\n",
+                ")\n",
                 "metrics_correlations[:10]"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -875,15 +881,16 @@
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# plot a kde plot for the top 3 metrics\n",
                 "import matplotlib.pyplot as plt\n",
-                "fig, ax = plt.subplots(1,3, figsize=(10, 5), sharey=False)\n",
+                "\n",
+                "fig, ax = plt.subplots(1, 3, figsize=(10, 5), sharey=False)\n",
                 "for i, metric in enumerate(metrics_correlations.index[:3]):\n",
                 "    sns.kdeplot(metrics_df, x=metric, hue=\"label\", ax=ax[i])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `textdescriptives-2.4.4/docs/usingthepackage.rst` & `textdescriptives-2.4.5/docs/usingthepackage.rst`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/paper/paper.bib` & `textdescriptives-2.4.5/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/paper/paper.md` & `textdescriptives-2.4.5/paper/paper.md`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/paper/paper_quarto.pdf` & `textdescriptives-2.4.5/paper/paper_quarto.pdf`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/paper/paper_quarto.qmd` & `textdescriptives-2.4.5/paper/paper_quarto.qmd`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/pyproject.toml` & `textdescriptives-2.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textdescriptives"
-version = "2.4.4"
+version = "2.4.5"
 description = "A library for calculating a variety of features from text using spaCy"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"},
              {name = "Kenneth Enevoldsen"}]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -32,39 +32,39 @@
     "text mining",
 ]
 
 dependencies = [
     "spacy[lookups]>=3.1.0,<3.6.0",
     "numpy>=1.20.0,<1.25.0",
     "pandas>=1.0.0,<1.6.0",
-    "pyphen>=0.11.0,<0.12.0",
+    "pyphen>=0.11.0,<0.15.0",
     "ftfy>=6.0.3,<6.1.0",
 ]
 
 requires-python = ">=3.7"
 
 [project.urls]
 homepage = "https://hlasse.github.io/TextDescriptives/"
 repository = "https://github.com/HLasse/textdescriptives"
 documentation = "https://hlasse.github.io/TextDescriptives/"
 
 [project.optional-dependencies]
 style = [
-    "black==22.8.0",
+    "black==23.3.0",
     "pre-commit==3.1.1",
-    "ruff==0.0.253",
-    "mypy==1.0.1"
+    "ruff==0.0.260",
+    "mypy==1.1.1"
 ]
 tests = [
     "pytest>=7.1.3,<7.3.0",
     "pytest-cov>=3.0.0,<3.0.1",
 ]
 docs = [
     "sphinx>=5.3.0,<6.2.0",
-    "furo==2022.12.7",
+    "furo==2023.3.27",
     "sphinx-copybutton>=0.5.1,<0.5.2",
     "sphinxext-opengraph>=0.7.3,<0.8.2",
     "myst-nb>=0.6.0,<1.17.0",
     "sphinx_design>=0.3.0,<0.3.1",
     "autodoc_pydantic>=1.1.0,<1.9.0",
 ]
 tutorials = [
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/coherence.py` & `textdescriptives-2.4.5/src/textdescriptives/components/coherence.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,31 +14,33 @@
             calculate the semantic similarity between consecutive sentences. And
             order=2 will calculate the semantic similarity between sentences that
             are two sentences apart.
 
     Returns:
         A list of floats representing the semantic similarity between sentences
     """
-    if doc.vector.size == 0:
-        raise ValueError(
-            "Sentence vectors are not available. Thus it is not possible to "
-            + "calculate the coherence between sentences. Please add a component "
-            + "that includes word vectors or sentence embeddings."
-            + "See https://spacy.io/usage/vectors-similarity for more details.",
-        )
+
     if not doc.has_annotation("SENT_START"):
         raise ValueError(
             "A sentence boundary detector has not been run on this Doc, which is "
             + "required to calculate coherence. Have you added a model with a "
             + "sentencizer and word vectors to the pipeline?",
         )
-
     sents = list(doc.sents)
     if len(sents) < order + 1:
         return [np.nan]
+
+    if doc.vector.size == 0:
+        raise ValueError(
+            "Sentence vectors are not available. Thus it is not possible to "
+            + "calculate the coherence between sentences. Please add a component "
+            + "that includes word vectors or sentence embeddings."
+            + "See https://spacy.io/usage/vectors-similarity for more details.",
+        )
+
     similarities: List[float] = []
     for i, sent in enumerate(sents):
         if i == len(sents) - order:
             break
         similarities.append(sent.similarity(sents[i + order]))
     return similarities
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/dependency_distance.py` & `textdescriptives-2.4.5/src/textdescriptives/components/dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/descriptive_stats.py` & `textdescriptives-2.4.5/src/textdescriptives/components/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/information_theory.py` & `textdescriptives-2.4.5/src/textdescriptives/components/information_theory.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/pos_proportions.py` & `textdescriptives-2.4.5/src/textdescriptives/components/pos_proportions.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 
 @Language.factory(
     "textdescriptives/pos_proportions",
     assigns=["doc._.pos_proportions", "span._.pos_proportions"],
     default_config={"use_pos": True},
 )
-def create_pos_stats_component(
+def create_pos_proportions_component(
     nlp: Language,
     name: str,
     use_pos: bool,
 ) -> Callable[[Doc], Doc]:
     """Allows PosPropotions to be added to a spaCy pipe using
     nlp.add_pipe("textdescriptives/pos_proportions")
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/quality.py` & `textdescriptives-2.4.5/src/textdescriptives/components/quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,17 +342,20 @@
         vocab (Optional[Mapping], optional): A vocabulary to check against.
             If None, will use the spaCy vocab. Note that the spaCy vocab
             is not defined for small models. Defaults to None.
 
     Returns:
         float: the out-of-vocabulary ratio
     """
+    len_span = len(span)
+    if len_span == 0:
+        return 0.0
     if vocab is None:
-        return len([token for token in span if token.is_oov]) / len(span)
-    return len([token for token in span if token.text not in vocab]) / len(span)
+        return len([token for token in span if token.is_oov]) / len_span
+    return len([token for token in span if token.text not in vocab]) / len_span
 
 
 class Quality:
     """spaCy component for adding text quality metrics to the `Doc` and `Span`
     objects.
 
     Extracts metrics and returns them as a dictionary as the ._.quality
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/quality_data_classes.py` & `textdescriptives-2.4.5/src/textdescriptives/components/quality_data_classes.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/readability.py` & `textdescriptives-2.4.5/src/textdescriptives/components/readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/components/utils.py` & `textdescriptives-2.4.5/src/textdescriptives/components/utils.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/data/spam.csv` & `textdescriptives-2.4.5/src/textdescriptives/data/spam.csv`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/extractors.py` & `textdescriptives-2.4.5/src/textdescriptives/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """Extract calculated metrics from a spaCy Doc or an iterable of Docs to a
     list of dictionaries.
 
     Args:
         docs (Union[Iterable[Doc],  Doc]): An iterable of spaCy Docs or a single Doc
         metrics (Union[list[str], str, None], optional): Which metrics to extract.
                 One or more of ["descriptive_stats", "readability",
-                "dependency_distance", "pos_stats", "information_theory"].
+                "dependency_distance", "pos_proportions", "information_theory"].
                 Defaults to None in which case it will extract metrics for which a
                 pipeline compoenent has been set.
         include_text (bool, optional): Whether to add an entry containing the text.
             Defaults to True.
 
     Returns:
         List[Dict[str, Any]]: List of dictionaries for each Doc with extracted metrics.
@@ -91,15 +91,15 @@
     """Extract calculated metrics from a spaCy Doc object or a generator of Docs
     from nlp.pipe to a Pandas DataFrame.
 
     Args:
         docs (Union[Iterable[Doc],  Doc]): An iterable of spaCy Docs or a single Doc
         metrics (Union[list[str], str], optional): Which metrics to extract.
                 One or more of ["descriptive_stats", "readability",
-                "dependency_distance", "pos_stats"]. Defaults to None in which
+                "dependency_distance", "pos_proportions"]. Defaults to None in which
                 case it will extract metrics for which a pipeline compoenent has been
                 set.
         include_text (bool, optional): Whether to add a column containing the text.
             Defaults to True.
 
     Returns:
         pd.DataFrame: DataFrame with a row for each doc and column for each metric.
@@ -121,15 +121,15 @@
         spacy_model (str, optional): The spacy model to use. If not set,
             will download one based on lang. Defaults to None.
         lang (str, optional): Language of the text. If lang is set and no spacy
             model is provided, will automatically download and use a spacy
             model for the language. Defaults to None.
         metrics (List[str]): Which metrics to extract.
             One or more of ["descriptive_stats", "readability",
-            "dependency_distance", "pos_stats", "coherence", "quality"]. If None,
+            "dependency_distance", "pos_proportions", "coherence", "quality"]. If None,
             will extract all metrics from textdescriptives. Defaults to None.
         spacy_model_size (str, optional): Size of the spacy model to download.
 
     Returns:
         pd.DataFrame: DataFrame with a row for each text and column for each metric.
     """
     if isinstance(metrics, str):
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives/load_components.py` & `textdescriptives-2.4.5/src/textdescriptives/load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/src/textdescriptives/utils.py` & `textdescriptives-2.4.5/src/textdescriptives/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
     Returns:
         Language: a spacy pipeline
     """
 
     metrics_requiring_spacy_model = {
         "dependency_distance",
-        "pos_stats",
+        "pos_proportions",
         "coherence",
         "pos_proportions",
     }
     # if no spacy model is necessary for the metrics, return a blank model
     # for the language
     if not bool(metrics_requiring_spacy_model.intersection(metrics)):
         # always load spacy model if specified (if e.g. custom tokenizer)
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives.egg-info/PKG-INFO` & `textdescriptives-2.4.5/src/textdescriptives.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdescriptives
-Version: 2.4.4
+Version: 2.4.5
 Summary: A library for calculating a variety of features from text using spaCy
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -238,22 +238,24 @@
 # TextDescriptives
 
 [![spacy](https://img.shields.io/badge/built%20with-spaCy-09a3d5.svg)](https://spacy.io)
 [![github actions pytest](https://github.com/hlasse/textdescriptives/actions/workflows/tests.yml/badge.svg)](https://github.com/hlasse/textdescriptives/actions)
 [![github actions docs](https://github.com/hlasse/textdescriptives/actions/workflows/documentation.yml/badge.svg)](https://hlasse.github.io/TextDescriptives/)
 [![arXiv](https://img.shields.io/badge/arXiv-2301.02057-b31b1b.svg)](https://arxiv.org/abs/2301.02057)
 [![status](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24/status.svg)](https://joss.theoj.org/papers/06447337ee61969b5a64de484199df24)
+[![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://huggingface.co/spaces/HLasse/textdescriptives)
 
 A Python library for calculating a large variety of metrics from text(s) using spaCy v.3 pipeline components and extensions. TextDescriptives can be used to calculate several descriptive statistics, readability metrics, and metrics related to dependency distance. 
 
 # 🔧 Installation
 `pip install textdescriptives`
 
 # 📰 News
 
+* We now have a TextDescriptives-powered web-app so you can extract and downloads metrics without a single line of code! Check it out [here](https://huggingface.co/spaces/HLasse/textdescriptives)
 * Version 2.0 out with a new API, a new component, updated documentation, and tutorials! Components are now called by "`textdescriptives/{metric_name}`. New `coherence` component for calculating the semantic coherence between sentences. See the [documentation](https://github.com/HLasse/TextDescriptives) for tutorials and more information!  
 
 
 
 # ⚡ Quick Start
 
 Use `extract_metrics` to quickly extract your desired metrics. To see available methods you can simply run:
@@ -316,17 +318,19 @@
 TextDescriptives has a detailed documentation as well as a series of Jupyter notebook tutorials.
 All the tutorials are located in the `docs/tutorials` folder and can also be found on the documentation website.
 
 
 | Documentation              |                                                                                    |
 | -------------------------- | ---------------------------------------------------------------------------------- |
 | 📚 **[Getting started]**    | Guides and instructions on how to use TextDescriptives and its features.           |
+| 👩‍💻 **[Demo]**               | A live demo of TextDescriptives.                                                   |
 | 😎 **[Tutorials]**          | Detailed tutorials on how to make the most of TextDescriptives                     |
 | 📰 **[News and changelog]** | New additions, changes and version history.                                        |
 | 🎛 **[API References]**     | The detailed reference for TextDescriptive's API. Including function documentation |
 | 📄 **[Paper]**              | The preprint of the TextDescriptives paper.                                        |
 
 [Paper]: https://arxiv.org/abs/2301.02057
 [Tutorials]: https://hlasse.github.io/TextDescriptives/tutorial.html
 [Getting started]: https://hlasse.github.io/TextDescriptives/usingthepackage.html
 [API References]: https://hlasse.github.io/TextDescriptives/index.html
 [News and changelog]: https://hlasse.github.io/TextDescriptives/news.html
+[Demo]: https://huggingface.co/spaces/HLasse/textdescriptives
```

### Comparing `textdescriptives-2.4.4/src/textdescriptives.egg-info/SOURCES.txt` & `textdescriptives-2.4.5/src/textdescriptives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/books.py` & `textdescriptives-2.4.5/tests/books.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_coherence.py` & `textdescriptives-2.4.5/tests/test_coherence.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     nlp = spacy.blank("en")
     nlp.add_pipe("textdescriptives/coherence")
 
     text = "This is a short and simple sentence. Here is yet another one."
     # check that an exception is raised
     with pytest.raises(ValueError) as e:
         doc = nlp(text)  # noqa F841
-    assert "Sentence vectors are not available" in str(e.value)
+    assert "sentence boundary detector has not been" in str(e.value)
 
     # add a sentencizer
     nlp.add_pipe("sentencizer", before="textdescriptives/coherence")
 
     with pytest.raises(ValueError) as e:
         doc = nlp(text)  # noqa F841
     assert "Sentence vectors are not available" in str(e.value)
```

### Comparing `textdescriptives-2.4.4/tests/test_dependency_distance.py` & `textdescriptives-2.4.5/tests/test_dependency_distance.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_descriptive_stats.py` & `textdescriptives-2.4.5/tests/test_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_extractors.py` & `textdescriptives-2.4.5/tests/test_extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,12 +182,14 @@
         metrics=["readability", "dependency_distance"],
         spacy_model="en_core_web_sm",
     )
     assert "lix" in df.columns
     assert "dependency_distance_mean" in df.columns
 
 
-def test_extract_metrics_all_metrics():
-    text = "just a little test"
-
+@pytest.mark.parametrize(
+    "text",
+    ["just a little test", ""],
+)
+def test_extract_metrics_all_metrics(text: str):
     df = td.extract_metrics(text=text, spacy_model="en_core_web_sm", metrics=None)
     assert "n_tokens" in df.columns
```

### Comparing `textdescriptives-2.4.4/tests/test_information.py` & `textdescriptives-2.4.5/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_load_components.py` & `textdescriptives-2.4.5/tests/test_load_components.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_pos_proportions.py` & `textdescriptives-2.4.5/tests/test_pos_proportions.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_quality.py` & `textdescriptives-2.4.5/tests/test_quality.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
         ),
         (
             "This is repitious text, This is repitious text, This is repitious text.",
             False,
         ),
         ("This test has many symbols #!@#$%^&*()_+.", False),
         ("- this is a text of \n - bullet points", False),
+        ("", False),  # test that it handles empty strings
     ],
 )
 def test_passed_quality_check(text: str, passed: bool, nlp: spacy.Language):
     """Test the passed_quality_check attribute."""
     nlp.add_pipe("textdescriptives/quality", config={"force": True})
     doc = nlp(text)
     assert doc._.passed_quality_check == passed
```

### Comparing `textdescriptives-2.4.4/tests/test_readability.py` & `textdescriptives-2.4.5/tests/test_readability.py`

 * *Files identical despite different names*

### Comparing `textdescriptives-2.4.4/tests/test_utils.py` & `textdescriptives-2.4.5/tests/test_utils.py`

 * *Files identical despite different names*

