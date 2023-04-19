# Comparing `tmp/tsinfer-0.3.0.tar.gz` & `tmp/tsinfer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsinfer-0.3.0.tar", last modified: Tue Oct 25 22:14:53 2022, max compression
+gzip compressed data, was "tsinfer-0.3.1.tar", last modified: Wed Apr 19 14:30:03 2023, max compression
```

## Comparing `tsinfer-0.3.0.tar` & `tsinfer-0.3.1.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.597930 tsinfer-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.573930 tsinfer-0.3.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.circleci/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.569930 tsinfer-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.573930 tsinfer-0.3.0/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.573930 tsinfer-0.3.0/.github/workflows/docker/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.github/workflows/docker/buildwheel.sh
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.github/workflows/docker/shared.env
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3983 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5399 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.mergify.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-10-25 22:14:37.000000 tsinfer-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     8344 2022-10-25 22:14:37.000000 tsinfer-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-10-25 22:14:37.000000 tsinfer-0.3.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (121)    35121 2022-10-25 22:14:37.000000 tsinfer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-10-25 22:14:37.000000 tsinfer-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-10-25 22:14:37.000000 tsinfer-0.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-10-25 22:14:53.597930 tsinfer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-10-25 22:14:37.000000 tsinfer-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)    52276 2022-10-25 22:14:37.000000 tsinfer-0.3.0/_tsinfermodule.c
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-10-25 22:14:37.000000 tsinfer-0.3.0/convert_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)    10035 2022-10-25 22:14:37.000000 tsinfer-0.3.0/dev.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.577930 tsinfer-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     8344 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2385 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.577930 tsinfer-0.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_static/.README
--rw-r--r--   0 runner    (1001) docker     (121)   127385 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_static/P_dom_chr24_phased.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (121)     3423 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_static/P_dom_chr24_phased.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (121)    14459 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_static/tree_at_1Mb.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.577930 tsinfer-0.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_templates/.README
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      506 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/build.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/file_formats.rst
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (121)    13652 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/inference.md
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)    24900 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/notebook-simulation.trees
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/simulation-example.py
--rw-r--r--   0 runner    (1001) docker     (121)     6832 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/tsinfer_logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)    31635 2022-10-25 22:14:37.000000 tsinfer-0.3.0/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (121)    77033 2022-10-25 22:14:37.000000 tsinfer-0.3.0/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.577930 tsinfer-0.3.0/lib/
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/.clang-format
--rw-r--r--   0 runner    (1001) docker     (121)    19708 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/ancestor_builder.c
--rw-r--r--   0 runner    (1001) docker     (121)    35768 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/ancestor_matcher.c
--rw-r--r--   0 runner    (1001) docker     (121)    13960 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/avl.c
--rw-r--r--   0 runner    (1001) docker     (121)     6766 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/avl.h
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/err.c
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/err.h
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/meson.build
--rw-r--r--   0 runner    (1001) docker     (121)     4869 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/object_heap.c
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/object_heap.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.577930 tsinfer-0.3.0/lib/subprojects/
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.581930 tsinfer-0.3.0/lib/subprojects/tskit/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    20759 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.581930 tsinfer-0.3.0/lib/subprojects/tskit/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/api_structure.c
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/cpp_sorting_example.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/error_handling.c
--rw-r--r--   0 runner    (1001) docker     (121)     3641 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/haploid_wright_fisher.c
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/streaming.c
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/take_ownership.c
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/tree_iteration.c
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/examples/tree_traversal.c
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/meson.build
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/meson_options.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.569930 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.585930 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (121)    33757 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/kastore.c
--rw-r--r--   0 runner    (1001) docker     (121)    21452 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/kastore.h
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.585930 tsinfer-0.3.0/lib/subprojects/tskit/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4466 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_convert.c
--rw-r--r--   0 runner    (1001) docker     (121)    18767 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_core.c
--rw-r--r--   0 runner    (1001) docker     (121)    51752 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_file_format.c
--rw-r--r--   0 runner    (1001) docker     (121)    42613 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_genotypes.c
--rw-r--r--   0 runner    (1001) docker     (121)    20332 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_haplotype_matching.c
--rw-r--r--   0 runner    (1001) docker     (121)     8267 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_minimal_cpp.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    59429 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_stats.c
--rw-r--r--   0 runner    (1001) docker     (121)   453278 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_tables.c
--rw-r--r--   0 runner    (1001) docker     (121)   290106 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/test_trees.c
--rw-r--r--   0 runner    (1001) docker     (121)    38877 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/testlib.c
--rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tests/testlib.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.589930 tsinfer-0.3.0/lib/subprojects/tskit/tskit/
--rw-r--r--   0 runner    (1001) docker     (121)     6245 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/convert.c
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/convert.h
--rw-r--r--   0 runner    (1001) docker     (121)    39079 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/core.c
--rw-r--r--   0 runner    (1001) docker     (121)    31098 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/core.h
--rw-r--r--   0 runner    (1001) docker     (121)    21534 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/genotypes.c
--rw-r--r--   0 runner    (1001) docker     (121)     7275 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/genotypes.h
--rw-r--r--   0 runner    (1001) docker     (121)    54813 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/haplotype_matching.c
--rw-r--r--   0 runner    (1001) docker     (121)     6210 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/haplotype_matching.h
--rw-r--r--   0 runner    (1001) docker     (121)     8164 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/stats.c
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/stats.h
--rw-r--r--   0 runner    (1001) docker     (121)   415146 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/tables.c
--rw-r--r--   0 runner    (1001) docker     (121)   168953 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/tables.h
--rw-r--r--   0 runner    (1001) docker     (121)   193425 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/trees.c
--rw-r--r--   0 runner    (1001) docker     (121)    58013 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit/trees.h
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit/tskit.h
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/subprojects/tskit.wrap
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.589930 tsinfer-0.3.0/lib/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    33383 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/tests/tests.c
--rw-r--r--   0 runner    (1001) docker     (121)    33142 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/tree_sequence_builder.c
--rw-r--r--   0 runner    (1001) docker     (121)     8963 2022-10-25 22:14:37.000000 tsinfer-0.3.0/lib/tsinfer.h
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-10-25 22:14:37.000000 tsinfer-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.589930 tsinfer-0.3.0/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.589930 tsinfer-0.3.0/requirements/CI-docs/
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-10-25 22:14:37.000000 tsinfer-0.3.0/requirements/CI-docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.593930 tsinfer-0.3.0/requirements/CI-tests-complete/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-10-25 22:14:37.000000 tsinfer-0.3.0/requirements/CI-tests-complete/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.593930 tsinfer-0.3.0/requirements/CI-tests-conda/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-25 22:14:37.000000 tsinfer-0.3.0/requirements/CI-tests-conda/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.593930 tsinfer-0.3.0/requirements/CI-tests-pip/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-25 22:14:37.000000 tsinfer-0.3.0/requirements/CI-tests-pip/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-10-25 22:14:37.000000 tsinfer-0.3.0/requirements/CI-tests-pip/requirements3.7.txt
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-10-25 22:14:37.000000 tsinfer-0.3.0/requirements/development.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-10-25 22:14:53.597930 tsinfer-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-10-25 22:14:37.000000 tsinfer-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.593930 tsinfer-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.569930 tsinfer-0.3.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.593930 tsinfer-0.3.0/tests/data/bugs/
--rw-r--r--   0 runner    (1001) docker     (121)    65536 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/data/bugs/invalid_pc_ancestor_time.samples
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.593930 tsinfer-0.3.0/tests/data/old_formats/
--rw-r--r--   0 runner    (1001) docker     (121)    53248 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/data/old_formats/medium_sd_fixture_0.2.3.samples
--rw-r--r--   0 runner    (1001) docker     (121)    20251 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    42700 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)    18712 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_extend.py
--rw-r--r--   0 runner    (1001) docker     (121)   117609 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (121)   182064 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_low_level.py
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/test_provenance.py
--rw-r--r--   0 runner    (1001) docker     (121)     6802 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tests/tsutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.597930 tsinfer-0.3.0/tsinfer/
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    42068 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)    18212 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    34242 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/eval_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)   121693 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/formats.py
--rw-r--r--   0 runner    (1001) docker     (121)   103168 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/progress.py
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/provenance.py
--rw-r--r--   0 runner    (1001) docker     (121)     3405 2022-10-25 22:14:37.000000 tsinfer-0.3.0/tsinfer/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 22:14:53.597930 tsinfer-0.3.0/tsinfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-25 22:14:53.000000 tsinfer-0.3.0/tsinfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19516 2022-10-25 22:14:37.000000 tsinfer-0.3.0/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.926569 tsinfer-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.906569 tsinfer-0.3.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.circleci/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.902569 tsinfer-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.906569 tsinfer-0.3.1/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.906569 tsinfer-0.3.1/.github/workflows/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.github/workflows/docker/buildwheel.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.github/workflows/docker/shared.env
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.mergify.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-19 14:29:50.000000 tsinfer-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-19 14:29:50.000000 tsinfer-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 14:29:50.000000 tsinfer-0.3.1/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-19 14:29:50.000000 tsinfer-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-19 14:29:50.000000 tsinfer-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-19 14:29:50.000000 tsinfer-0.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 14:30:03.926569 tsinfer-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-19 14:29:50.000000 tsinfer-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    52276 2023-04-19 14:29:50.000000 tsinfer-0.3.1/_tsinfermodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-19 14:29:50.000000 tsinfer-0.3.1/convert_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-04-19 14:29:50.000000 tsinfer-0.3.1/dev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.910569 tsinfer-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.910569 tsinfer-0.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_static/.README
+-rw-r--r--   0 runner    (1001) docker     (123)   127385 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_static/P_dom_chr24_phased.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_static/P_dom_chr24_phased.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)    14459 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_static/tree_at_1Mb.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.910569 tsinfer-0.3.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_templates/.README
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      506 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/file_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/inference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24868 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/notebook-simulation.trees
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/simulation-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/tsinfer_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31635 2023-04-19 14:29:50.000000 tsinfer-0.3.1/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)    77033 2023-04-19 14:29:50.000000 tsinfer-0.3.1/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.914569 tsinfer-0.3.1/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/ancestor_builder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35768 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/ancestor_matcher.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/avl.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/avl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/err.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/err.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/meson.build
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/object_heap.c
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/object_heap.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.914569 tsinfer-0.3.1/lib/subprojects/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.914569 tsinfer-0.3.1/lib/subprojects/tskit/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.914569 tsinfer-0.3.1/lib/subprojects/tskit/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/api_structure.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/cpp_sorting_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/error_handling.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/haploid_wright_fisher.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/streaming.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/take_ownership.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/tree_iteration.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/examples/tree_traversal.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/meson.build
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/meson_options.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.902569 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.914569 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    33757 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/kastore.c
+-rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/kastore.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.918569 tsinfer-0.3.1/lib/subprojects/tskit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_convert.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18767 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_core.c
+-rw-r--r--   0 runner    (1001) docker     (123)    51752 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_file_format.c
+-rw-r--r--   0 runner    (1001) docker     (123)    42613 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_genotypes.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_haplotype_matching.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_minimal_cpp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    59429 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)   453278 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_tables.c
+-rw-r--r--   0 runner    (1001) docker     (123)   290106 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/test_trees.c
+-rw-r--r--   0 runner    (1001) docker     (123)    38877 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/testlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tests/testlib.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.918569 tsinfer-0.3.1/lib/subprojects/tskit/tskit/
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/convert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/convert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39079 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/core.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31098 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21534 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/genotypes.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/genotypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    54813 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/haplotype_matching.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/haplotype_matching.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/stats.h
+-rw-r--r--   0 runner    (1001) docker     (123)   415146 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/tables.c
+-rw-r--r--   0 runner    (1001) docker     (123)   168953 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/tables.h
+-rw-r--r--   0 runner    (1001) docker     (123)   193425 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/trees.c
+-rw-r--r--   0 runner    (1001) docker     (123)    58013 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit/trees.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit/tskit.h
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/subprojects/tskit.wrap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.918569 tsinfer-0.3.1/lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    33383 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/tests/tests.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33142 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/tree_sequence_builder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-04-19 14:29:50.000000 tsinfer-0.3.1/lib/tsinfer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-19 14:29:50.000000 tsinfer-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.918569 tsinfer-0.3.1/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/requirements/CI-docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-19 14:29:50.000000 tsinfer-0.3.1/requirements/CI-docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/requirements/CI-tests-complete/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-19 14:29:50.000000 tsinfer-0.3.1/requirements/CI-tests-complete/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/requirements/CI-tests-conda/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 14:29:50.000000 tsinfer-0.3.1/requirements/CI-tests-conda/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/requirements/CI-tests-pip/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 14:29:50.000000 tsinfer-0.3.1/requirements/CI-tests-pip/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-19 14:29:50.000000 tsinfer-0.3.1/requirements/CI-tests-pip/requirements3.7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-19 14:29:50.000000 tsinfer-0.3.1/requirements/development.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-19 14:30:03.926569 tsinfer-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-19 14:29:50.000000 tsinfer-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.906569 tsinfer-0.3.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/tests/data/bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)    65536 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/data/bugs/invalid_pc_ancestor_time.samples
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.922569 tsinfer-0.3.1/tests/data/old_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)    53248 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/data/old_formats/medium_sd_fixture_0.2.3.samples
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42700 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117609 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182064 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_low_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/test_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tests/tsutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.926569 tsinfer-0.3.1/tsinfer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42068 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34242 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/eval_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121693 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-19 14:29:50.000000 tsinfer-0.3.1/tsinfer/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 14:30:03.926569 tsinfer-0.3.1/tsinfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 14:30:03.000000 tsinfer-0.3.1/tsinfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-04-19 14:29:50.000000 tsinfer-0.3.1/visualisation.py
```

### Comparing `tsinfer-0.3.0/.circleci/config.yml` & `tsinfer-0.3.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/.github/workflows/docker/buildwheel.sh` & `tsinfer-0.3.1/.github/workflows/docker/buildwheel.sh`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/.github/workflows/docs.yml` & `tsinfer-0.3.1/.github/workflows/docs.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,52 +12,54 @@
   MAKE_TARGET: all
   OWNER: tskit-dev
   REPO: tsinfer
 
 jobs:
   build-deploy-docs:
     name: Docs
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
       - name: Cancel Previous Runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
 
       - uses: actions/checkout@v3
-        # As we are using pull-request-target which uses the workflow from the base
-        # of the PR, we need to be specific
         with:
-            ref: ${{ github.event.pull_request.head.ref }}
-            repository: ${{ github.event.pull_request.head.repo.full_name }}
             submodules: true
 
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.8
+          python-version: "3.10"
 
       - uses: actions/cache@v3
-        id: cache
+        id: venv-cache
         with:
           path: venv
-          key: docs-venv-v1-${{ hashFiles('requirements/CI-docs/requirements.txt') }}
+          key: docs-venv-v3-${{ hashFiles('requirements/CI-docs/requirements.txt') }}
 
-      - name: Build virtualenv
-        if: steps.cache.outputs.cache-hit != 'true'
-        run: python -m venv venv
-
-      - name: Install deps
-        run: venv/bin/activate && pip install -r requirements/CI-docs/requirements.txt
+      - name: Create venv and install deps (one by one to avoid conflict errors)
+        if: steps.venv-cache.outputs.cache-hit != 'true'
+        run: |
+          python -m venv venv
+          . venv/bin/activate
+          pip install --upgrade pip wheel
+          cat requirements/CI-docs/requirements.txt | sed -e '/^\s*#.*$/d' -e '/^\s*$/d' | xargs -n 1 pip install --no-dependencies          
+          
 
       - name: Build C module
         if: env.MAKE_TARGET
-        run: venv/bin/activate && make $MAKE_TARGET
+        run: |
+          . venv/bin/activate
+          make $MAKE_TARGET
 
       - name: Build Docs
-        run: venv/bin/activate && cd docs && make dist
+        run: |
+          . venv/bin/activate
+          cd docs && make dist
 
       - name: Trigger docs site rebuild
         if: github.ref == 'refs/heads/main'
         run: |
           curl -X POST https://api.github.com/repos/tskit-dev/tskit-site/dispatches \
                     -H 'Accept: application/vnd.github.everest-preview+json' \
                     -u AdminBot-tskit:${{ secrets.ADMINBOT_TOKEN }} \
```

### Comparing `tsinfer-0.3.0/.github/workflows/tests.yml` & `tsinfer-0.3.1/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 name: Tests
 
 on:
   pull_request:
   push:
     branches: [main]
+    tags:
 
 jobs:
   pre-commit:
     name: Lint
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-latest
     steps:
       - name: Cancel Previous Runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: "3.10"
       - name: install clang-format
         run: |
-          sudo apt-get remove -y clang-6.0 libclang-common-6.0-dev libclang1-6.0 libllvm6.0
-          sudo apt-get autoremove
-          sudo apt-get install clang-format clang-format-6.0
+          pip install clang-format==6.0.1
       - uses: pre-commit/action@v3.0.0
 
   test:
     name: Python
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
```

### Comparing `tsinfer-0.3.0/.github/workflows/wheels.yml` & `tsinfer-0.3.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/.gitignore` & `tsinfer-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/.mergify.yml` & `tsinfer-0.3.1/.mergify.yml`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/.pre-commit-config.yaml` & `tsinfer-0.3.1/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.4.0
     hooks:
       - id: check-merge-conflict
       - id: debug-statements
       - id: mixed-line-ending
       - id: check-case-conflict
       - id: check-yaml
   - repo: https://github.com/benjeffery/pre-commit-clang-format
-    rev: c21a74d089aaeb86c2c19df371c7e7bf40c07207
+    rev: '1.0'
     hooks:
     - id: clang-format
       exclude: avl
       verbose: true
   - repo: https://github.com/asottile/reorder_python_imports
-    rev: v3.0.1
+    rev: v3.9.0
     hooks:
       - id: reorder-python-imports
         args: [ --unclassifiable-application-module=_tsinfer ]
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.31.1
+    rev: v3.2.2
     hooks:
       - id: pyupgrade
         args: [ --py3-plus, --py37-plus ]
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 22.10.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/asottile/blacken-docs
     rev: v1.12.1
     hooks:
       - id: blacken-docs
         args: [--skip-errors]
         additional_dependencies: [black==22.3.0]
         language_version: python3
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         args: [--config=.flake8]
-        additional_dependencies: ["flake8-bugbear==22.3.23", "flake8-builtins==1.5.3"]
+        additional_dependencies: ["flake8-bugbear==22.10.27", "flake8-builtins==2.0.1"]
```

### Comparing `tsinfer-0.3.0/CHANGELOG.md` & `tsinfer-0.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## [0.3.1] - 2023-04-19
+
+Bug fix release for a bad dependency specification.
+
+
 ## [0.3.0] - 2022-10-25
 
 **Features**
 
 - When calling `sample_data.add_site()` the ancestral state does not need to be the
   first allele (index 0): alternatively, an ancestral allele index can be given
   (and if `MISSING_DATA`, the ancestral state will be imputed). ({pr}`718`,
```

### Comparing `tsinfer-0.3.0/CITATION.md` & `tsinfer-0.3.1/CITATION.md`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/LICENSE` & `tsinfer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/PKG-INFO` & `tsinfer-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsinfer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Infer tree sequences from genetic variation data.
 Home-page: https://tskit.dev/tsinfer
 Author: Tskit Developers
 Author-email: admin@tskit.dev
 License: GNU GPLv3+
 Project-URL: Documentation, https://tskit.dev/tsinfer/docs/stable
 Project-URL: Changelog, https://tskit.dev/tsinfer/docs/stable/CHANGELOG.html
```

### Comparing `tsinfer-0.3.0/README.md` & `tsinfer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/_tsinfermodule.c` & `tsinfer-0.3.1/_tsinfermodule.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/convert_hdf5.py` & `tsinfer-0.3.1/convert_hdf5.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/dev.py` & `tsinfer-0.3.1/dev.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/CHANGELOG.md` & `tsinfer-0.3.1/docs/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## [0.3.1] - 2023-04-19
+
+Bug fix release for a bad dependency specification.
+
+
 ## [0.3.0] - 2022-10-25
 
 **Features**
 
 - When calling `sample_data.add_site()` the ancestral state does not need to be the
   first allele (index 0): alternatively, an ancestral allele index can be given
   (and if `MISSING_DATA`, the ancestral state will be imputed). ({pr}`718`,
```

### Comparing `tsinfer-0.3.0/docs/CITATION.md` & `tsinfer-0.3.1/docs/CITATION.md`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/_config.yml` & `tsinfer-0.3.1/docs/_config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     - sphinx.ext.autodoc
     - sphinx.ext.autosummary
     - sphinx.ext.todo
     - sphinx.ext.viewcode
     - sphinx.ext.intersphinx
     - sphinx_issues
     - sphinxarg.ext
+    - IPython.sphinxext.ipython_console_highlighting
 
     config:
       html_theme: tskit_book_theme
       pygments_style: monokai
       myst_enable_extensions:
       - colon_fence
       - deflist
```

### Comparing `tsinfer-0.3.0/docs/_static/P_dom_chr24_phased.vcf.gz` & `tsinfer-0.3.1/docs/_static/P_dom_chr24_phased.vcf.gz`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/_static/P_dom_chr24_phased.vcf.gz.tbi` & `tsinfer-0.3.1/docs/_static/P_dom_chr24_phased.vcf.gz.tbi`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/_static/tree_at_1Mb.svg` & `tsinfer-0.3.1/docs/_static/tree_at_1Mb.svg`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/api.rst` & `tsinfer-0.3.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/cli.rst` & `tsinfer-0.3.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/file_formats.rst` & `tsinfer-0.3.1/docs/file_formats.rst`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/index.md` & `tsinfer-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/inference.md` & `tsinfer-0.3.1/docs/inference.md`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/installation.rst` & `tsinfer-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/introduction.rst` & `tsinfer-0.3.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/notebook-simulation.trees` & `tsinfer-0.3.1/docs/notebook-simulation.trees`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 894b 4153 0d0a 1a0a 0100 0000 3e00 0000  .KAS........>...
-00000010: 4461 0000 0000 0000 0000 0000 0000 0000  Da..............
+00000010: 2461 0000 0000 0000 0000 0000 0000 0000  $a..............
 00000020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000040: 0400 0000 0000 0000 c00f 0000 0000 0000  ................
 00000050: 0b00 0000 0000 0000 4014 0000 0000 0000  ........@.......
 00000060: e200 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0900 0000 0000 0000 cb0f 0000 0000 0000  ................
@@ -196,62 +196,62 @@
 00000c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c40: 0100 0000 0000 0000 3413 0000 0000 0000  ........4.......
 00000c50: 1b00 0000 0000 0000 205b 0000 0000 0000  ........ [......
 00000c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000c80: 0100 0000 0000 0000 4f13 0000 0000 0000  ........O.......
 00000c90: 1200 0000 0000 0000 205b 0000 0000 0000  ........ [......
-00000ca0: 3402 0000 0000 0000 0000 0000 0000 0000  4...............
+00000ca0: 1302 0000 0000 0000 0000 0000 0000 0000  ................
 00000cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000cc0: 0500 0000 0000 0000 6113 0000 0000 0000  ........a.......
-00000cd0: 1900 0000 0000 0000 585d 0000 0000 0000  ........X]......
+00000cd0: 1900 0000 0000 0000 385d 0000 0000 0000  ........8]......
 00000ce0: 0200 0000 0000 0000 0000 0000 0000 0000  ................
 00000cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d00: 0100 0000 0000 0000 7a13 0000 0000 0000  ........z.......
-00000d10: 1500 0000 0000 0000 605d 0000 0000 0000  ........`]......
+00000d10: 1500 0000 0000 0000 405d 0000 0000 0000  ........@]......
 00000d20: 1a00 0000 0000 0000 0000 0000 0000 0000  ................
 00000d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d40: 0500 0000 0000 0000 8f13 0000 0000 0000  ................
-00000d50: 1c00 0000 0000 0000 805d 0000 0000 0000  .........]......
+00000d50: 1c00 0000 0000 0000 605d 0000 0000 0000  ........`]......
 00000d60: 0200 0000 0000 0000 0000 0000 0000 0000  ................
 00000d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d80: 0900 0000 0000 0000 ab13 0000 0000 0000  ................
-00000d90: 0f00 0000 0000 0000 885d 0000 0000 0000  .........]......
+00000d90: 0f00 0000 0000 0000 685d 0000 0000 0000  ........h]......
 00000da0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00000db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000dc0: 0100 0000 0000 0000 ba13 0000 0000 0000  ................
-00000dd0: 1500 0000 0000 0000 905d 0000 0000 0000  .........]......
+00000dd0: 1500 0000 0000 0000 705d 0000 0000 0000  ........p]......
 00000de0: 1400 0000 0000 0000 0000 0000 0000 0000  ................
 00000df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e00: 0500 0000 0000 0000 cf13 0000 0000 0000  ................
-00000e10: 1c00 0000 0000 0000 a85d 0000 0000 0000  .........]......
+00000e10: 1c00 0000 0000 0000 885d 0000 0000 0000  .........]......
 00000e20: 1500 0000 0000 0000 0000 0000 0000 0000  ................
 00000e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e40: 0100 0000 0000 0000 eb13 0000 0000 0000  ................
-00000e50: 0e00 0000 0000 0000 005e 0000 0000 0000  .........^......
+00000e50: 0e00 0000 0000 0000 e05d 0000 0000 0000  .........]......
 00000e60: 1702 0000 0000 0000 0000 0000 0000 0000  ................
 00000e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000e80: 0500 0000 0000 0000 f913 0000 0000 0000  ................
-00000e90: 1500 0000 0000 0000 1860 0000 0000 0000  .........`......
+00000e90: 1500 0000 0000 0000 f85f 0000 0000 0000  ........._......
 00000ea0: 1500 0000 0000 0000 0000 0000 0000 0000  ................
 00000eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ec0: 0100 0000 0000 0000 0e14 0000 0000 0000  ................
-00000ed0: 1500 0000 0000 0000 7060 0000 0000 0000  ........p`......
+00000ed0: 1500 0000 0000 0000 5060 0000 0000 0000  ........P`......
 00000ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f00: 0900 0000 0000 0000 2314 0000 0000 0000  ........#.......
-00000f10: 0e00 0000 0000 0000 7060 0000 0000 0000  ........p`......
+00000f10: 0e00 0000 0000 0000 5060 0000 0000 0000  ........P`......
 00000f20: 1400 0000 0000 0000 0000 0000 0000 0000  ................
 00000f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f40: 0000 0000 0000 0000 3114 0000 0000 0000  ........1.......
-00000f50: 0a00 0000 0000 0000 1061 0000 0000 0000  .........a......
+00000f50: 0a00 0000 0000 0000 f060 0000 0000 0000  .........`......
 00000f60: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
 00000f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000f80: 0000 0000 0000 0000 3b14 0000 0000 0000  ........;.......
-00000f90: 0400 0000 0000 0000 2061 0000 0000 0000  ........ a......
+00000f90: 0400 0000 0000 0000 0061 0000 0000 0000  .........a......
 00000fa0: 2400 0000 0000 0000 0000 0000 0000 0000  $...............
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 6564 6765 732f 6368 696c 6465 6467 6573  edges/childedges
 00000fd0: 2f6c 6566 7465 6467 6573 2f6d 6574 6164  /leftedges/metad
 00000fe0: 6174 6165 6467 6573 2f6d 6574 6164 6174  ataedges/metadat
 00000ff0: 615f 6f66 6673 6574 6564 6765 732f 6d65  a_offsetedges/me
 00001000: 7461 6461 7461 5f73 6368 656d 6165 6467  tadata_schemaedg
@@ -322,20 +322,20 @@
 00001410: 7465 732f 6d65 7461 6461 7461 5f73 6368  tes/metadata_sch
 00001420: 656d 6173 6974 6573 2f70 6f73 6974 696f  emasites/positio
 00001430: 6e74 696d 655f 756e 6974 7375 7569 6400  ntime_unitsuuid.
 00001440: 2000 0000 5500 0000 a200 0000 0c00 0000   ...U...........
 00001450: 6800 0000 8200 0000 0300 0000 2600 0000  h...........&...
 00001460: 8400 0000 4d00 0000 5100 0000 5d00 0000  ....M...Q...]...
 00001470: 7300 0000 2200 0000 2900 0000 4900 0000  s..."...)...I...
-00001480: 7500 0000 c200 0000 0000 0000 0400 0000  u...............
-00001490: 0d00 0000 1000 0000 1700 0000 1800 0000  ................
-000014a0: 3a00 0000 3e00 0000 4400 0000 4600 0000  :...>...D...F...
-000014b0: 5400 0000 7900 0000 9800 0000 9b00 0000  T...y...........
-000014c0: a900 0000 ae00 0000 b900 0000 be00 0000  ................
-000014d0: c400 0000 c900 0000 2800 0000 3400 0000  ........(...4...
+00001480: 7500 0000 c200 0000 0400 0000 0d00 0000  u...............
+00001490: 1000 0000 1700 0000 1800 0000 3a00 0000  ............:...
+000014a0: 3e00 0000 4400 0000 4600 0000 5400 0000  >...D...F...T...
+000014b0: 7900 0000 9800 0000 9b00 0000 a900 0000  y...............
+000014c0: ae00 0000 b900 0000 be00 0000 c400 0000  ................
+000014d0: c700 0000 c900 0000 2800 0000 3400 0000  ........(...4...
 000014e0: 3b00 0000 6d00 0000 7b00 0000 9d00 0000  ;...m...{.......
 000014f0: cd00 0000 1400 0000 2100 0000 2400 0000  ........!...$...
 00001500: 5200 0000 8600 0000 8700 0000 8800 0000  R...............
 00001510: 8d00 0000 ca00 0000 0100 0000 0800 0000  ................
 00001520: 1100 0000 1300 0000 3f00 0000 4100 0000  ........?...A...
 00001530: 4b00 0000 6100 0000 7c00 0000 8000 0000  K...a...|.......
 00001540: 9300 0000 9700 0000 b000 0000 b800 0000  ................
@@ -346,21 +346,21 @@
 00001590: 4e00 0000 5600 0000 5900 0000 5a00 0000  N...V...Y...Z...
 000015a0: 6400 0000 6700 0000 7100 0000 7e00 0000  d...g...q...~...
 000015b0: 9100 0000 9c00 0000 a000 0000 a100 0000  ................
 000015c0: ab00 0000 ac00 0000 af00 0000 ba00 0000  ................
 000015d0: c100 0000 c300 0000 0600 0000 1a00 0000  ................
 000015e0: 1f00 0000 2700 0000 4500 0000 7000 0000  ....'...E...p...
 000015f0: 8c00 0000 8e00 0000 9500 0000 9600 0000  ................
-00001600: a600 0000 0900 0000 1200 0000 1c00 0000  ................
-00001610: 2c00 0000 3600 0000 4800 0000 5300 0000  ,...6...H...S...
-00001620: 6900 0000 6f00 0000 7200 0000 7600 0000  i...o...r...v...
-00001630: 7f00 0000 8100 0000 8300 0000 8f00 0000  ................
-00001640: a500 0000 a700 0000 aa00 0000 ad00 0000  ................
-00001650: b700 0000 bb00 0000 bd00 0000 c500 0000  ................
-00001660: c700 0000 d200 0000 d100 0000 d200 0000  ................
+00001600: a600 0000 0000 0000 0900 0000 1200 0000  ................
+00001610: 1c00 0000 2c00 0000 3600 0000 4800 0000  ....,...6...H...
+00001620: 5300 0000 6900 0000 6f00 0000 7200 0000  S...i...o...r...
+00001630: 7600 0000 7f00 0000 8100 0000 8300 0000  v...............
+00001640: 8f00 0000 a500 0000 a700 0000 aa00 0000  ................
+00001650: ad00 0000 b700 0000 bb00 0000 bd00 0000  ................
+00001660: c500 0000 d200 0000 d100 0000 d200 0000  ................
 00001670: 0200 0000 0a00 0000 0b00 0000 0f00 0000  ................
 00001680: 1500 0000 1d00 0000 2d00 0000 3000 0000  ........-...0...
 00001690: 3500 0000 3d00 0000 4300 0000 4a00 0000  5...=...C...J...
 000016a0: 4f00 0000 5800 0000 5c00 0000 5e00 0000  O...X...\...^...
 000016b0: 5f00 0000 6000 0000 6200 0000 6500 0000  _...`...b...e...
 000016c0: 6a00 0000 6e00 0000 7800 0000 8a00 0000  j...n...x.......
 000016d0: 9000 0000 9200 0000 9400 0000 9a00 0000  ................
@@ -1456,102 +1456,100 @@
 00005af0: 0000 0000 0000 d83f 3333 3333 3333 e73f  .......?333333.?
 00005b00: c10f fcc0 0ffc e83f c10f fcc0 0ffc e83f  .......?.......?
 00005b10: c10f fcc0 0ffc e83f 0000 0000 0000 0000  .......?........
 00005b20: 7b22 7363 6865 6d61 5f76 6572 7369 6f6e  {"schema_version
 00005b30: 223a 2022 312e 302e 3022 2c20 2273 6f66  ": "1.0.0", "sof
 00005b40: 7477 6172 6522 3a20 7b22 6e61 6d65 223a  tware": {"name":
 00005b50: 2022 7473 696e 6665 7222 2c20 2276 6572   "tsinfer", "ver
-00005b60: 7369 6f6e 223a 2022 302e 322e 342e 6465  sion": "0.2.4.de
-00005b70: 7635 382b 6765 3433 6437 3439 227d 2c20  v58+ge43d749"}, 
-00005b80: 2270 6172 616d 6574 6572 7322 3a20 7b22  "parameters": {"
-00005b90: 636f 6d6d 616e 6422 3a20 2269 6e66 6572  command": "infer
-00005ba0: 227d 2c20 2265 6e76 6972 6f6e 6d65 6e74  "}, "environment
-00005bb0: 223a 207b 226c 6962 7261 7269 6573 223a  ": {"libraries":
-00005bc0: 207b 227a 6172 7222 3a20 7b22 7665 7273   {"zarr": {"vers
-00005bd0: 696f 6e22 3a20 2232 2e38 2e33 227d 2c20  ion": "2.8.3"}, 
-00005be0: 226e 756d 636f 6465 6373 223a 207b 2276  "numcodecs": {"v
-00005bf0: 6572 7369 6f6e 223a 2022 302e 372e 3322  ersion": "0.7.3"
-00005c00: 7d2c 2022 6c6d 6462 223a 207b 2276 6572  }, "lmdb": {"ver
-00005c10: 7369 6f6e 223a 2022 312e 322e 3122 7d2c  sion": "1.2.1"},
-00005c20: 2022 7473 6b69 7422 3a20 7b22 7665 7273   "tskit": {"vers
-00005c30: 696f 6e22 3a20 2230 2e35 2e33 227d 7d2c  ion": "0.5.3"}},
-00005c40: 2022 6f73 223a 207b 2273 7973 7465 6d22   "os": {"system"
-00005c50: 3a20 2244 6172 7769 6e22 2c20 226e 6f64  : "Darwin", "nod
-00005c60: 6522 3a20 2259 616e 732d 4e65 772d 4169  e": "Yans-New-Ai
-00005c70: 7222 2c20 2272 656c 6561 7365 223a 2022  r", "release": "
-00005c80: 3230 2e36 2e30 222c 2022 7665 7273 696f  20.6.0", "versio
-00005c90: 6e22 3a20 2244 6172 7769 6e20 4b65 726e  n": "Darwin Kern
-00005ca0: 656c 2056 6572 7369 6f6e 2032 302e 362e  el Version 20.6.
-00005cb0: 303a 2054 7565 204a 756e 2032 3120 3230  0: Tue Jun 21 20
-00005cc0: 3a35 303a 3238 2050 4454 2032 3032 323b  :50:28 PDT 2022;
-00005cd0: 2072 6f6f 743a 786e 752d 3731 3935 2e31   root:xnu-7195.1
-00005ce0: 3431 2e33 327e 312f 5245 4c45 4153 455f  41.32~1/RELEASE_
-00005cf0: 5838 365f 3634 222c 2022 6d61 6368 696e  X86_64", "machin
-00005d00: 6522 3a20 2278 3836 5f36 3422 7d2c 2022  e": "x86_64"}, "
-00005d10: 7079 7468 6f6e 223a 207b 2269 6d70 6c65  python": {"imple
-00005d20: 6d65 6e74 6174 696f 6e22 3a20 2243 5079  mentation": "CPy
-00005d30: 7468 6f6e 222c 2022 7665 7273 696f 6e22  thon", "version"
-00005d40: 3a20 5b22 3322 2c20 2239 222c 2022 3422  : ["3", "9", "4"
-00005d50: 5d7d 7d7d 0000 0000 0000 0000 3402 0000  ]}}}........4...
-00005d60: 3230 3232 2d31 302d 3139 5431 383a 3337  2022-10-19T18:37
-00005d70: 3a31 322e 3337 3131 3232 0000 0000 0000  :12.371122......
-00005d80: 0000 0000 1a00 0000 0000 0000 0088 c340  ...............@
-00005d90: 4341 4347 4747 4743 4147 4347 5447 4141  CACGGGGCAGCGTGAA
-00005da0: 5454 4354 0000 0000 0000 0000 0100 0000  TTCT............
-00005db0: 0200 0000 0300 0000 0400 0000 0500 0000  ................
-00005dc0: 0600 0000 0700 0000 0800 0000 0900 0000  ................
-00005dd0: 0a00 0000 0b00 0000 0c00 0000 0d00 0000  ................
-00005de0: 0e00 0000 0f00 0000 1000 0000 1100 0000  ................
-00005df0: 1200 0000 1300 0000 1400 0000 0000 0000  ................
-00005e00: 7b22 696e 6665 7265 6e63 655f 7479 7065  {"inference_type
-00005e10: 223a 2022 6675 6c6c 227d 7b22 696e 6665  ": "full"}{"infe
-00005e20: 7265 6e63 655f 7479 7065 223a 2022 7061  rence_type": "pa
-00005e30: 7273 696d 6f6e 7922 7d7b 2269 6e66 6572  rsimony"}{"infer
-00005e40: 656e 6365 5f74 7970 6522 3a20 2266 756c  ence_type": "ful
-00005e50: 6c22 7d7b 2269 6e66 6572 656e 6365 5f74  l"}{"inference_t
-00005e60: 7970 6522 3a20 2266 756c 6c22 7d7b 2269  ype": "full"}{"i
-00005e70: 6e66 6572 656e 6365 5f74 7970 6522 3a20  nference_type": 
-00005e80: 2266 756c 6c22 7d7b 2269 6e66 6572 656e  "full"}{"inferen
-00005e90: 6365 5f74 7970 6522 3a20 2266 756c 6c22  ce_type": "full"
-00005ea0: 7d7b 2269 6e66 6572 656e 6365 5f74 7970  }{"inference_typ
-00005eb0: 6522 3a20 2270 6172 7369 6d6f 6e79 227d  e": "parsimony"}
-00005ec0: 7b22 696e 6665 7265 6e63 655f 7479 7065  {"inference_type
-00005ed0: 223a 2022 6675 6c6c 227d 7b22 696e 6665  ": "full"}{"infe
-00005ee0: 7265 6e63 655f 7479 7065 223a 2022 6675  rence_type": "fu
-00005ef0: 6c6c 227d 7b22 696e 6665 7265 6e63 655f  ll"}{"inference_
-00005f00: 7479 7065 223a 2022 6675 6c6c 227d 7b22  type": "full"}{"
-00005f10: 696e 6665 7265 6e63 655f 7479 7065 223a  inference_type":
-00005f20: 2022 6675 6c6c 227d 7b22 696e 6665 7265   "full"}{"infere
-00005f30: 6e63 655f 7479 7065 223a 2022 6675 6c6c  nce_type": "full
-00005f40: 227d 7b22 696e 6665 7265 6e63 655f 7479  "}{"inference_ty
-00005f50: 7065 223a 2022 7061 7273 696d 6f6e 7922  pe": "parsimony"
-00005f60: 7d7b 2269 6e66 6572 656e 6365 5f74 7970  }{"inference_typ
-00005f70: 6522 3a20 2266 756c 6c22 7d7b 2269 6e66  e": "full"}{"inf
-00005f80: 6572 656e 6365 5f74 7970 6522 3a20 2266  erence_type": "f
-00005f90: 756c 6c22 7d7b 2269 6e66 6572 656e 6365  ull"}{"inference
-00005fa0: 5f74 7970 6522 3a20 2266 756c 6c22 7d7b  _type": "full"}{
-00005fb0: 2269 6e66 6572 656e 6365 5f74 7970 6522  "inference_type"
-00005fc0: 3a20 2266 756c 6c22 7d7b 2269 6e66 6572  : "full"}{"infer
-00005fd0: 656e 6365 5f74 7970 6522 3a20 2266 756c  ence_type": "ful
-00005fe0: 6c22 7d7b 2269 6e66 6572 656e 6365 5f74  l"}{"inference_t
-00005ff0: 7970 6522 3a20 2266 756c 6c22 7d7b 2269  ype": "full"}{"i
-00006000: 6e66 6572 656e 6365 5f74 7970 6522 3a20  nference_type": 
-00006010: 2266 756c 6c22 7d00 0000 0000 1a00 0000  "full"}.........
-00006020: 3900 0000 5300 0000 6d00 0000 8700 0000  9...S...m.......
-00006030: a100 0000 c000 0000 da00 0000 f400 0000  ................
-00006040: 0e01 0000 2801 0000 4201 0000 6101 0000  ....(...B...a...
-00006050: 7b01 0000 9501 0000 af01 0000 c901 0000  {...............
-00006060: e301 0000 fd01 0000 1702 0000 0000 0000  ................
-00006070: 0000 0000 0078 8440 0000 0000 0068 8640  .....x.@.....h.@
-00006080: 0000 0000 00a8 9140 0000 0000 006c 9740  .......@.....l.@
-00006090: 0000 0000 00bc 9a40 0000 0000 0028 a040  .......@.....(.@
-000060a0: 0000 0000 006c a540 0000 0000 0062 a640  .....l.@.....b.@
-000060b0: 0000 0000 00bb b240 0000 0000 00ac b340  .......@.......@
-000060c0: 0000 0000 0039 b440 0000 0000 0070 b440  .....9.@.....p.@
-000060d0: 0000 0000 008a b540 0000 0000 0093 b740  .......@.......@
-000060e0: 0000 0000 005a b840 0000 0000 00a2 ba40  .....Z.@.......@
-000060f0: 0000 0000 00eb bd40 0000 0000 00fb bf40  .......@.......@
-00006100: 0000 0000 0007 c040 0000 0000 8007 c040  .......@.......@
-00006110: 756e 6361 6c69 6272 6174 6564 0000 0000  uncalibrated....
-00006120: 3663 6237 6636 6238 2d36 6234 352d 3732  6cb7f6b8-6b45-72
-00006130: 3965 2d38 6330 642d 3230 3436 3639 3364  9e-8c0d-2046693d
-00006140: 6565 3738                                ee78
+00005b60: 7369 6f6e 223a 2022 302e 332e 312e 6465  sion": "0.3.1.de
+00005b70: 7635 322b 6763 6239 3765 3830 2e64 3230  v52+gcb97e80.d20
+00005b80: 3233 3034 3132 227d 2c20 2270 6172 616d  230412"}, "param
+00005b90: 6574 6572 7322 3a20 7b22 636f 6d6d 616e  eters": {"comman
+00005ba0: 6422 3a20 2269 6e66 6572 227d 2c20 2265  d": "infer"}, "e
+00005bb0: 6e76 6972 6f6e 6d65 6e74 223a 207b 226c  nvironment": {"l
+00005bc0: 6962 7261 7269 6573 223a 207b 227a 6172  ibraries": {"zar
+00005bd0: 7222 3a20 7b22 7665 7273 696f 6e22 3a20  r": {"version": 
+00005be0: 2232 2e31 342e 3222 7d2c 2022 6e75 6d63  "2.14.2"}, "numc
+00005bf0: 6f64 6563 7322 3a20 7b22 7665 7273 696f  odecs": {"versio
+00005c00: 6e22 3a20 2230 2e31 312e 3022 7d2c 2022  n": "0.11.0"}, "
+00005c10: 6c6d 6462 223a 207b 2276 6572 7369 6f6e  lmdb": {"version
+00005c20: 223a 2022 312e 342e 3022 7d2c 2022 7473  ": "1.4.0"}, "ts
+00005c30: 6b69 7422 3a20 7b22 7665 7273 696f 6e22  kit": {"version"
+00005c40: 3a20 2230 2e35 2e34 227d 7d2c 2022 6f73  : "0.5.4"}}, "os
+00005c50: 223a 207b 2273 7973 7465 6d22 3a20 224c  ": {"system": "L
+00005c60: 696e 7578 222c 2022 6e6f 6465 223a 2022  inux", "node": "
+00005c70: 7472 6565 6265 6172 6422 2c20 2272 656c  treebeard", "rel
+00005c80: 6561 7365 223a 2022 352e 342e 302d 3130  ease": "5.4.0-10
+00005c90: 392d 6765 6e65 7269 6322 2c20 2276 6572  9-generic", "ver
+00005ca0: 7369 6f6e 223a 2022 2331 3233 2d55 6275  sion": "#123-Ubu
+00005cb0: 6e74 7520 534d 5020 4672 6920 4170 7220  ntu SMP Fri Apr 
+00005cc0: 3820 3039 3a31 303a 3534 2055 5443 2032  8 09:10:54 UTC 2
+00005cd0: 3032 3222 2c20 226d 6163 6869 6e65 223a  022", "machine":
+00005ce0: 2022 7838 365f 3634 227d 2c20 2270 7974   "x86_64"}, "pyt
+00005cf0: 686f 6e22 3a20 7b22 696d 706c 656d 656e  hon": {"implemen
+00005d00: 7461 7469 6f6e 223a 2022 4350 7974 686f  tation": "CPytho
+00005d10: 6e22 2c20 2276 6572 7369 6f6e 223a 205b  n", "version": [
+00005d20: 2233 222c 2022 3130 222c 2022 3130 225d  "3", "10", "10"]
+00005d30: 7d7d 7d00 0000 0000 0000 0000 1302 0000  }}}.............
+00005d40: 3230 3233 2d30 342d 3139 5431 343a 3436  2023-04-19T14:46
+00005d50: 3a33 372e 3031 3035 3834 0000 0000 0000  :37.010584......
+00005d60: 0000 0000 1a00 0000 0000 0000 0088 c340  ...............@
+00005d70: 4341 4347 4747 4743 4147 4347 5447 4141  CACGGGGCAGCGTGAA
+00005d80: 5454 4354 0000 0000 0000 0000 0100 0000  TTCT............
+00005d90: 0200 0000 0300 0000 0400 0000 0500 0000  ................
+00005da0: 0600 0000 0700 0000 0800 0000 0900 0000  ................
+00005db0: 0a00 0000 0b00 0000 0c00 0000 0d00 0000  ................
+00005dc0: 0e00 0000 0f00 0000 1000 0000 1100 0000  ................
+00005dd0: 1200 0000 1300 0000 1400 0000 0000 0000  ................
+00005de0: 7b22 696e 6665 7265 6e63 655f 7479 7065  {"inference_type
+00005df0: 223a 2022 6675 6c6c 227d 7b22 696e 6665  ": "full"}{"infe
+00005e00: 7265 6e63 655f 7479 7065 223a 2022 7061  rence_type": "pa
+00005e10: 7273 696d 6f6e 7922 7d7b 2269 6e66 6572  rsimony"}{"infer
+00005e20: 656e 6365 5f74 7970 6522 3a20 2266 756c  ence_type": "ful
+00005e30: 6c22 7d7b 2269 6e66 6572 656e 6365 5f74  l"}{"inference_t
+00005e40: 7970 6522 3a20 2266 756c 6c22 7d7b 2269  ype": "full"}{"i
+00005e50: 6e66 6572 656e 6365 5f74 7970 6522 3a20  nference_type": 
+00005e60: 2266 756c 6c22 7d7b 2269 6e66 6572 656e  "full"}{"inferen
+00005e70: 6365 5f74 7970 6522 3a20 2266 756c 6c22  ce_type": "full"
+00005e80: 7d7b 2269 6e66 6572 656e 6365 5f74 7970  }{"inference_typ
+00005e90: 6522 3a20 2270 6172 7369 6d6f 6e79 227d  e": "parsimony"}
+00005ea0: 7b22 696e 6665 7265 6e63 655f 7479 7065  {"inference_type
+00005eb0: 223a 2022 6675 6c6c 227d 7b22 696e 6665  ": "full"}{"infe
+00005ec0: 7265 6e63 655f 7479 7065 223a 2022 6675  rence_type": "fu
+00005ed0: 6c6c 227d 7b22 696e 6665 7265 6e63 655f  ll"}{"inference_
+00005ee0: 7479 7065 223a 2022 6675 6c6c 227d 7b22  type": "full"}{"
+00005ef0: 696e 6665 7265 6e63 655f 7479 7065 223a  inference_type":
+00005f00: 2022 6675 6c6c 227d 7b22 696e 6665 7265   "full"}{"infere
+00005f10: 6e63 655f 7479 7065 223a 2022 6675 6c6c  nce_type": "full
+00005f20: 227d 7b22 696e 6665 7265 6e63 655f 7479  "}{"inference_ty
+00005f30: 7065 223a 2022 7061 7273 696d 6f6e 7922  pe": "parsimony"
+00005f40: 7d7b 2269 6e66 6572 656e 6365 5f74 7970  }{"inference_typ
+00005f50: 6522 3a20 2266 756c 6c22 7d7b 2269 6e66  e": "full"}{"inf
+00005f60: 6572 656e 6365 5f74 7970 6522 3a20 2266  erence_type": "f
+00005f70: 756c 6c22 7d7b 2269 6e66 6572 656e 6365  ull"}{"inference
+00005f80: 5f74 7970 6522 3a20 2266 756c 6c22 7d7b  _type": "full"}{
+00005f90: 2269 6e66 6572 656e 6365 5f74 7970 6522  "inference_type"
+00005fa0: 3a20 2266 756c 6c22 7d7b 2269 6e66 6572  : "full"}{"infer
+00005fb0: 656e 6365 5f74 7970 6522 3a20 2266 756c  ence_type": "ful
+00005fc0: 6c22 7d7b 2269 6e66 6572 656e 6365 5f74  l"}{"inference_t
+00005fd0: 7970 6522 3a20 2266 756c 6c22 7d7b 2269  ype": "full"}{"i
+00005fe0: 6e66 6572 656e 6365 5f74 7970 6522 3a20  nference_type": 
+00005ff0: 2266 756c 6c22 7d00 0000 0000 1a00 0000  "full"}.........
+00006000: 3900 0000 5300 0000 6d00 0000 8700 0000  9...S...m.......
+00006010: a100 0000 c000 0000 da00 0000 f400 0000  ................
+00006020: 0e01 0000 2801 0000 4201 0000 6101 0000  ....(...B...a...
+00006030: 7b01 0000 9501 0000 af01 0000 c901 0000  {...............
+00006040: e301 0000 fd01 0000 1702 0000 0000 0000  ................
+00006050: 0000 0000 0078 8440 0000 0000 0068 8640  .....x.@.....h.@
+00006060: 0000 0000 00a8 9140 0000 0000 006c 9740  .......@.....l.@
+00006070: 0000 0000 00bc 9a40 0000 0000 0028 a040  .......@.....(.@
+00006080: 0000 0000 006c a540 0000 0000 0062 a640  .....l.@.....b.@
+00006090: 0000 0000 00bb b240 0000 0000 00ac b340  .......@.......@
+000060a0: 0000 0000 0039 b440 0000 0000 0070 b440  .....9.@.....p.@
+000060b0: 0000 0000 008a b540 0000 0000 0093 b740  .......@.......@
+000060c0: 0000 0000 005a b840 0000 0000 00a2 ba40  .....Z.@.......@
+000060d0: 0000 0000 00eb bd40 0000 0000 00fb bf40  .......@.......@
+000060e0: 0000 0000 0007 c040 0000 0000 8007 c040  .......@.......@
+000060f0: 756e 6361 6c69 6272 6174 6564 0000 0000  uncalibrated....
+00006100: 3561 3961 3030 3230 2d30 3832 362d 3239  5a9a0020-0826-29
+00006110: 3363 2d37 3034 342d 6634 3830 3732 3466  3c-7044-f480724f
+00006120: 3963 3339                                9c39
```

### Comparing `tsinfer-0.3.0/docs/simulation-example.py` & `tsinfer-0.3.1/docs/simulation-example.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/tsinfer_logo.svg` & `tsinfer-0.3.1/docs/tsinfer_logo.svg`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/docs/tutorial.md` & `tsinfer-0.3.1/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/evaluation.py` & `tsinfer-0.3.1/evaluation.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/.clang-format` & `tsinfer-0.3.1/lib/.clang-format`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/ancestor_builder.c` & `tsinfer-0.3.1/lib/ancestor_builder.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/ancestor_matcher.c` & `tsinfer-0.3.1/lib/ancestor_matcher.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/avl.c` & `tsinfer-0.3.1/lib/avl.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/avl.h` & `tsinfer-0.3.1/lib/avl.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/err.c` & `tsinfer-0.3.1/lib/err.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/err.h` & `tsinfer-0.3.1/lib/err.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/meson.build` & `tsinfer-0.3.1/lib/meson.build`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/object_heap.c` & `tsinfer-0.3.1/lib/object_heap.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/object_heap.h` & `tsinfer-0.3.1/lib/object_heap.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/CHANGELOG.rst` & `tsinfer-0.3.1/lib/subprojects/tskit/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/Makefile` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/Makefile`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/api_structure.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/api_structure.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/cpp_sorting_example.cpp` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/cpp_sorting_example.cpp`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/error_handling.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/error_handling.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/haploid_wright_fisher.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/haploid_wright_fisher.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/streaming.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/streaming.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/take_ownership.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/take_ownership.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/tree_iteration.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/tree_iteration.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/examples/tree_traversal.c` & `tsinfer-0.3.1/lib/subprojects/tskit/examples/tree_traversal.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/meson.build` & `tsinfer-0.3.1/lib/subprojects/tskit/meson.build`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/kastore.c` & `tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/kastore.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/kastore.h` & `tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/kastore.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/subprojects/kastore/meson.build` & `tsinfer-0.3.1/lib/subprojects/tskit/subprojects/kastore/meson.build`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_convert.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_convert.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_core.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_core.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_file_format.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_file_format.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_genotypes.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_genotypes.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_haplotype_matching.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_haplotype_matching.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_minimal_cpp.cpp` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_minimal_cpp.cpp`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_stats.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_stats.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_tables.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_tables.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/test_trees.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/test_trees.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/testlib.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/testlib.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tests/testlib.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tests/testlib.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/convert.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/convert.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/convert.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/convert.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/core.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/core.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/core.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/core.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/genotypes.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/genotypes.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/genotypes.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/genotypes.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/haplotype_matching.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/haplotype_matching.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/haplotype_matching.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/haplotype_matching.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/stats.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/stats.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/stats.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/stats.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/tables.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/tables.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/tables.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/tables.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/trees.c` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/trees.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit/trees.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit/trees.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/subprojects/tskit/tskit.h` & `tsinfer-0.3.1/lib/subprojects/tskit/tskit.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/tests/tests.c` & `tsinfer-0.3.1/lib/tests/tests.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/tree_sequence_builder.c` & `tsinfer-0.3.1/lib/tree_sequence_builder.c`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/lib/tsinfer.h` & `tsinfer-0.3.1/lib/tsinfer.h`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/requirements/development.txt` & `tsinfer-0.3.1/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/setup.cfg` & `tsinfer-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 	numpy
 	six
 	tqdm
 	humanize
 	daiquiri
 	tskit>=0.5.3
 	numcodecs>=0.6
-	zarr>=2.2!=2.11.0!=2.11.1!=2.11.2
+	zarr>=2.2,!=2.11.0,!=2.11.1,!=2.11.2
 	lmdb
 	sortedcontainers
 	attrs>=19.2.0
 
 [options.entry_points]
 console_scripts = 
 	tsinfer = tsinfer.__main__:main
```

### Comparing `tsinfer-0.3.0/setup.py` & `tsinfer-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/conftest.py` & `tsinfer-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/data/bugs/invalid_pc_ancestor_time.samples` & `tsinfer-0.3.1/tests/data/bugs/invalid_pc_ancestor_time.samples`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/data/old_formats/medium_sd_fixture_0.2.3.samples` & `tsinfer-0.3.1/tests/data/old_formats/medium_sd_fixture_0.2.3.samples`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/test_cli.py` & `tsinfer-0.3.1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,50 @@
                 "-A",
                 augmented_ancestors,
             ]
         )
         self.verify_output(output_trees)
 
 
+class TestCommandsExtra(TestCli):
+    """
+    Test miscellaneous extra options for standard commands
+    """
+
+    def test_filenames_without_keeping_intermediates(self):
+        output_anc = os.path.join(self.tempdir.name, "test1")
+        output_anc_ts = os.path.join(self.tempdir.name, "test2")
+        with pytest.raises(ValueError, match="--keep-intermediates"):
+            self.run_command(["infer", self.sample_file, "-a", output_anc])
+        with pytest.raises(ValueError, match="--keep-intermediates"):
+            self.run_command(["infer", self.sample_file, "-A", output_anc_ts])
+
+    def test_keep_intermediates(self):
+        output_anc = os.path.join(self.tempdir.name, "test1")
+        output_anc_ts = os.path.join(self.tempdir.name, "test2")
+        self.run_command(
+            [
+                "infer",
+                self.sample_file,
+                "--keep-intermediates",
+                "-a",
+                output_anc,
+                "-A",
+                output_anc_ts,
+            ]
+        )
+        assert os.path.exists(output_anc)
+        ancestors = tsinfer.load(output_anc)
+        assert ancestors.num_ancestors > 0
+
+        assert os.path.exists(output_anc_ts)
+        anc_ts = tskit.load(output_anc_ts)
+        assert anc_ts.num_samples > 0
+
+
 class TestProgress(TestCli):
     """
     Tests that we get some output when we use the progress bar.
     """
 
     # Need to mock out setup_logging here or we spew logging to the console
     # in later tests.
@@ -399,15 +435,15 @@
 
     @pytest.mark.skip(reason="https://github.com/tskit-dev/tsinfer/issues/753")
     @pytest.mark.skipif(
         sys.platform == "win32", reason="windows simultaneous file permissions issue"
     )
     def test_map(self):
         ratemap = os.path.join(self.tempdir.name, "ratemap.txt")
-        with open(ratemap, "wt") as map:
+        with open(ratemap, "w") as map:
             print("Chromosome  Position(bp)  Rate(cM/Mb)  Map(cM)", file=map)
             print("chr1 0 0.1 0", file=map)
             print("chr1 1 0.2 0.002", file=map)
         command = [
             "infer",
             self.sample_file,
             "--recombination-map",
@@ -424,15 +460,15 @@
     )
     def test_fails_on_bad_map(self):
         output_trees = os.path.join(self.tempdir.name, "output_test_map.trees")
         ratemap = os.path.join(self.tempdir.name, "ratemap.txt")
         sd = tsinfer.load(self.sample_file)
         last_pos = sd.sites_position[-1]
         assert last_pos > 2
-        with open(ratemap, "wt") as map:
+        with open(ratemap, "w") as map:
             print("Chromosome  Position(bp)  Rate(cM/Mb)  Map(cM)", file=map)
             print("chr1 0 0.1 0.0", file=map)
             print(f"chr1 {int(last_pos) - 1} 0.2 0.001", file=map)
         command = [
             "infer",
             self.sample_file,
             "--recombination-map",
```

### Comparing `tsinfer-0.3.0/tests/test_evaluation.py` & `tsinfer-0.3.1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/test_extend.py` & `tsinfer-0.3.1/tests/test_extend.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/test_formats.py` & `tsinfer-0.3.1/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/test_inference.py` & `tsinfer-0.3.1/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/test_low_level.py` & `tsinfer-0.3.1/tests/test_low_level.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/test_provenance.py` & `tsinfer-0.3.1/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tests/tsutil.py` & `tsinfer-0.3.1/tests/tsutil.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/__init__.py` & `tsinfer-0.3.1/tsinfer/__init__.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/algorithm.py` & `tsinfer-0.3.1/tsinfer/algorithm.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/cli.py` & `tsinfer-0.3.1/tsinfer/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,45 +158,61 @@
         except tskit.FileFormatError:
             raise e  # Re-raise the original error
         raise exceptions.FileFormatError(
             "Expecting a sample data file, not a tree sequence (you can create one "
             "via the Python function `tsinfer.SampleData.from_tree_sequence()`)."
         )
     sample_data = tsinfer.SampleData.load(args.samples)
-    ts = tsinfer.infer(
-        sample_data,
-        progress_monitor=args.progress,
-        num_threads=args.num_threads,
-        recombination_rate=get_recombination_map(args),
-        mismatch_ratio=args.mismatch_ratio,
-        record_provenance=False,
-    )
-    output_trees = get_output_trees_path(args.output_trees, args.samples)
-    write_ts(ts, output_trees)
+    if args.keep_intermediates:
+        run_generate_ancestors(args, usage_summary=False)
+        run_match_ancestors(args, usage_summary=False)
+        run_match_samples(args, usage_summary=False)
+    else:
+        if args.ancestors is not None:
+            raise ValueError(
+                "Must specify --keep-intermediates to save an ancestors file"
+            )
+        if args.ancestors_trees is not None:
+            raise ValueError(
+                "Must specify --keep-intermediates to save an ancestors tree sequence"
+            )
+
+        ts = tsinfer.infer(
+            sample_data,
+            progress_monitor=args.progress,
+            num_threads=args.num_threads,
+            recombination_rate=get_recombination_map(args),
+            mismatch_ratio=args.mismatch_ratio,
+            path_compression=not args.no_path_compression,
+            record_provenance=False,
+        )
+        output_trees = get_output_trees_path(args.output_trees, args.samples)
+        write_ts(ts, output_trees)
     summarise_usage()
 
 
-def run_generate_ancestors(args):
+def run_generate_ancestors(args, usage_summary=True):
     setup_logging(args)
     ancestors_path = get_ancestors_path(args.ancestors, args.samples)
     sample_data = tsinfer.SampleData.load(args.samples)
     tsinfer.generate_ancestors(
         sample_data,
         progress_monitor=args.progress,
-        num_flush_threads=args.num_flush_threads,
+        num_flush_threads=getattr(args, "num_flush_threads", 0),
         num_threads=args.num_threads,
         path=ancestors_path,
         record_provenance=False,
     )
     # NB: ideally we should store the cli provenance in here, but this creates
     # perf issues - see https://github.com/tskit-dev/tsinfer/issues/743
-    summarise_usage()
+    if usage_summary:
+        summarise_usage()
 
 
-def run_match_ancestors(args):
+def run_match_ancestors(args, usage_summary=True):
     setup_logging(args)
     ancestors_path = get_ancestors_path(args.ancestors, args.samples)
     logger.info(f"Loading ancestral haplotypes from {ancestors_path}")
     ancestors_trees = get_ancestors_trees_path(args.ancestors_trees, args.samples)
     sample_data = tsinfer.SampleData.load(args.samples)
     ancestor_data = tsinfer.AncestorData.load(ancestors_path)
     ts = tsinfer.match_ancestors(
@@ -206,18 +222,19 @@
         progress_monitor=args.progress,
         recombination_rate=get_recombination_map(args),
         mismatch_ratio=args.mismatch_ratio,
         path_compression=not args.no_path_compression,
         record_provenance=False,
     )
     write_ts(ts, ancestors_trees)
-    summarise_usage()
+    if usage_summary:
+        summarise_usage()
 
 
-def run_augment_ancestors(args):
+def run_augment_ancestors(args, usage_summary=True):
     setup_logging(args)
 
     sample_data = tsinfer.SampleData.load(args.samples)
     ancestors_trees = get_ancestors_trees_path(args.ancestors_trees, args.samples)
     output_path = args.augmented_ancestors
     logger.info(f"Loading ancestral genealogies from {ancestors_trees}")
     ancestors_trees = tskit.load(ancestors_trees)
@@ -237,18 +254,19 @@
         progress_monitor=args.progress,
         recombination_rate=get_recombination_map(args),
         mismatch_ratio=args.mismatch_ratio,
         record_provenance=False,
     )
     logger.info(f"Writing output tree sequence to {output_path}")
     ts.dump(output_path)
-    summarise_usage()
+    if usage_summary:
+        summarise_usage()
 
 
-def run_match_samples(args):
+def run_match_samples(args, usage_summary=True):
     setup_logging(args)
 
     sample_data = tsinfer.SampleData.load(args.samples)
     ancestors_trees = get_ancestors_trees_path(args.ancestors_trees, args.samples)
     output_trees = get_output_trees_path(args.output_trees, args.samples)
     logger.info(f"Loading ancestral genealogies from {ancestors_trees}")
     ancestors_trees = tskit.load(ancestors_trees)
@@ -260,15 +278,16 @@
         post_process=not args.no_post_process,
         progress_monitor=args.progress,
         recombination_rate=get_recombination_map(args),
         mismatch_ratio=args.mismatch_ratio,
         record_provenance=False,
     )
     write_ts(ts, output_trees)
-    summarise_usage()
+    if usage_summary:
+        summarise_usage()
 
 
 def run_verify(args):
     setup_logging(args)
     samples = tsinfer.SampleData.load(args.samples)
     ts = tskit.load(args.tree_sequence)
     tsinfer.verify(samples, ts, progress_monitor=args.progress)
@@ -421,14 +440,27 @@
         help=(
             "The number of data flush threads to use. If < 1, all data is flushed "
             "synchronously in the main thread (default=2)"
         ),
     )
 
 
+def add_keep_intermediates_argument(parser):
+    parser.add_argument(
+        "--keep-intermediates",
+        "-k",
+        action="store_true",
+        help=(
+            "Keep the intermediate ancestors and ancestors-tree-sequence files. "
+            "To override the default locations where these files are saved, use the "
+            "--ancestors and --ancestors-trees options"
+        ),
+    )
+
+
 def get_cli_parser():
     top_parser = argparse.ArgumentParser(
         description="Command line interface for tsinfer."
     )
     top_parser.add_argument(
         "-V",
         "--version",
@@ -521,25 +553,29 @@
     add_mismatch_argument(parser)
     parser.set_defaults(runner=run_match_samples)
 
     parser = subparsers.add_parser(
         "infer",
         help=(
             "Runs the generate-ancestors, match-ancestors and match-samples "
-            "commands without writing the intermediate files to disk. Not "
-            "recommended for large inferences."
+            "steps in one go. Not recommended for large inferences."
         ),
     )
     add_samples_file_argument(parser)
     add_logging_arguments(parser)
     add_output_trees_argument(parser)
+    add_path_compression_argument(parser)
     add_num_threads_argument(parser)
     add_progress_argument(parser)
+    add_postprocess_argument(parser)
     add_recombination_arguments(parser)
     add_mismatch_argument(parser)
+    add_keep_intermediates_argument(parser)
+    add_ancestors_file_argument(parser)  # Only used if keep-intermediates
+    add_ancestors_trees_argument(parser)  # Only used if keep-intermediates
     parser.set_defaults(runner=run_infer)
 
     parser = subparsers.add_parser(
         "list",
         aliases=["ls"],
         help=("Show a summary of the specified tsinfer related file."),
     )
```

### Comparing `tsinfer-0.3.0/tsinfer/constants.py` & `tsinfer-0.3.1/tsinfer/constants.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/eval_util.py` & `tsinfer-0.3.1/tsinfer/eval_util.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/exceptions.py` & `tsinfer-0.3.1/tsinfer/exceptions.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/formats.py` & `tsinfer-0.3.1/tsinfer/formats.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/inference.py` & `tsinfer-0.3.1/tsinfer/inference.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/progress.py` & `tsinfer-0.3.1/tsinfer/progress.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/provenance.py` & `tsinfer-0.3.1/tsinfer/provenance.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer/threads.py` & `tsinfer-0.3.1/tsinfer/threads.py`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/tsinfer.egg-info/PKG-INFO` & `tsinfer-0.3.1/tsinfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsinfer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Infer tree sequences from genetic variation data.
 Home-page: https://tskit.dev/tsinfer
 Author: Tskit Developers
 Author-email: admin@tskit.dev
 License: GNU GPLv3+
 Project-URL: Documentation, https://tskit.dev/tsinfer/docs/stable
 Project-URL: Changelog, https://tskit.dev/tsinfer/docs/stable/CHANGELOG.html
```

### Comparing `tsinfer-0.3.0/tsinfer.egg-info/SOURCES.txt` & `tsinfer-0.3.1/tsinfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tsinfer-0.3.0/visualisation.py` & `tsinfer-0.3.1/visualisation.py`

 * *Files identical despite different names*

