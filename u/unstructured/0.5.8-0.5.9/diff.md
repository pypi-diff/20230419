# Comparing `tmp/unstructured-0.5.8.tar.gz` & `tmp/unstructured-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.5.8.tar", last modified: Thu Mar 30 20:59:00 2023, max compression
+gzip compressed data, was "unstructured-0.5.9.tar", last modified: Mon Apr  3 18:19:40 2023, max compression
```

## Comparing `unstructured-0.5.8.tar` & `unstructured-0.5.9.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.083874 unstructured-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-03-30 20:58:52.000000 unstructured-0.5.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-03-30 20:59:00.083874 unstructured-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15598 2023-03-30 20:58:52.000000 unstructured-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-30 20:59:00.083874 unstructured-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-03-30 20:58:52.000000 unstructured-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.071874 unstructured-0.5.8/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.071874 unstructured-0.5.8/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-30 20:58:52.000000 unstructured-0.5.8/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-30 20:58:52.000000 unstructured-0.5.8/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-30 20:58:52.000000 unstructured-0.5.8/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-30 20:58:52.000000 unstructured-0.5.8/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.071874 unstructured-0.5.8/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.071874 unstructured-0.5.8/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.075874 unstructured-0.5.8/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.075874 unstructured-0.5.8/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.075874 unstructured-0.5.8/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.075874 unstructured-0.5.8/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.075874 unstructured-0.5.8/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23278 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.075874 unstructured-0.5.8/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.079874 unstructured-0.5.8/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.083874 unstructured-0.5.8/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.083874 unstructured-0.5.8/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-30 20:58:52.000000 unstructured-0.5.8/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:59:00.071874 unstructured-0.5.8/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-03-30 20:58:59.000000 unstructured-0.5.8/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-30 20:59:00.000000 unstructured-0.5.8/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:58:59.000000 unstructured-0.5.8/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-30 20:58:59.000000 unstructured-0.5.8/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-30 20:58:59.000000 unstructured-0.5.8/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-30 20:58:59.000000 unstructured-0.5.8/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.363400 unstructured-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-03 18:19:33.000000 unstructured-0.5.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-04-03 18:19:40.363400 unstructured-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-04-03 18:19:33.000000 unstructured-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-03 18:19:40.363400 unstructured-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-03 18:19:33.000000 unstructured-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.351400 unstructured-0.5.9/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.351400 unstructured-0.5.9/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-03 18:19:33.000000 unstructured-0.5.9/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10853 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23278 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.359400 unstructured-0.5.9/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.363400 unstructured-0.5.9/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.363400 unstructured-0.5.9/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-03 18:19:33.000000 unstructured-0.5.9/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 18:19:40.355400 unstructured-0.5.9/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-03 18:19:40.000000 unstructured-0.5.9/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.5.8/LICENSE.md` & `unstructured-0.5.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/PKG-INFO` & `unstructured-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.5.8
+Version: 0.5.9
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -90,27 +90,27 @@
         ```
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
         
-        NOTE: the image is only supported for x86_64 hardware and known to have issues on Apple silicon.
+        NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
         
         We build Docker images for all pushes to `main`. We tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`. To leverage this, `docker pull` from our image repository.
         
         ```bash
         docker pull quay.io/unstructured-io/unstructured:latest
         ```
         
         Once pulled, you can create a container from this image and shell to it.
         
         ```bash
         # create the container
-        docker run --platform linux/amd64 -d -t --name unstructured quay.io/unstructured-io/unstructured:latest
+        docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
         
         # this will drop you into a bash shell where the Docker image is running
         docker exec -it unstructured bash
         ```
         
         You can also build your own Docker image.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.5.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.5.9 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -44,46 +44,48 @@
 [str(el) for el in elements])) ``` And if you installed with `local-inference`,
 you should be able to run this as well: ```python from
 unstructured.partition.auto import partition elements = partition("example-
 docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
 ``` ## :dizzy: Instructions for using the docker image The following
 instructions are intended to help you get up and running using Docker to
 interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
-) if you don't already have docker installed on your machine. NOTE: the image
-is only supported for x86_64 hardware and known to have issues on Apple
-silicon. We build Docker images for all pushes to `main`. We tag each image
-with the corresponding short commit hash (e.g. `fbc7a69`) and the application
+) if you don't already have docker installed on your machine. NOTE: we build
+multi-platform images to support both x86_64 and Apple silicon hardware.
+`docker pull` should download the corresponding image for your architecture,
+but you can specify with `--platform` (e.g. `--platform linux/amd64`) if
+needed. We build Docker images for all pushes to `main`. We tag each image with
+the corresponding short commit hash (e.g. `fbc7a69`) and the application
 version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`.
 To leverage this, `docker pull` from our image repository. ```bash docker pull
 quay.io/unstructured-io/unstructured:latest ``` Once pulled, you can create a
 container from this image and shell to it. ```bash # create the container
-docker run --platform linux/amd64 -d -t --name unstructured quay.io/
-unstructured-io/unstructured:latest # this will drop you into a bash shell
-where the Docker image is running docker exec -it unstructured bash ``` You can
-also build your own Docker image. If you only plan on parsing one type of data
-you can speed up building the image by commenting out some of the packages/
-requirements necessary for other data types. See Dockerfile to know which lines
-are necessary for your use case. ```bash make docker-build # this will drop you
-into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
-interpreter's interactive mode. ```bash # this will drop you into a python
-console so you can run the below partition functions python3 >>> from
-unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
-(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
-unstructured.partition.text import partition_text >>> elements = partition_text
-(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
-Instructions for Local Development The following instructions are intended to
-help you get up and running with `unstructured` locally if you are planning to
-contribute to the project. * Using `pyenv` to manage virtualenv's is
-recommended but not necessary * Mac install instructions. See [here](https://
-github.com/Unstructured-IO/community#mac--homebrew) for more detailed
-instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
-Linux instructions are available [here](https://github.com/Unstructured-IO/
-community#linux). * Create a virtualenv to work in and activate it, e.g. for
-one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
+docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
+# this will drop you into a bash shell where the Docker image is running docker
+exec -it unstructured bash ``` You can also build your own Docker image. If you
+only plan on parsing one type of data you can speed up building the image by
+commenting out some of the packages/requirements necessary for other data
+types. See Dockerfile to know which lines are necessary for your use case.
+```bash make docker-build # this will drop you into a bash shell where the
+Docker image is running make docker-start-bash ``` Once in the running
+container, you can try things out directly in Python interpreter's interactive
+mode. ```bash # this will drop you into a python console so you can run the
+below partition functions python3 >>> from unstructured.partition.pdf import
+partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
+parser-paper-fast.pdf") >>> from unstructured.partition.text import
+partition_text >>> elements = partition_text(filename="example-docs/fake-
+text.txt") ``` ## :coffee: Installation Instructions for Local Development The
+following instructions are intended to help you get up and running with
+`unstructured` locally if you are planning to contribute to the project. *
+Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
+install instructions. See [here](https://github.com/Unstructured-IO/
+community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
+virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
+(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
+work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
+3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
```

### Comparing `unstructured-0.5.8/README.md` & `unstructured-0.5.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,27 +82,27 @@
 ```
 
 ## :dizzy: Instructions for using the docker image
 
 The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
 See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
 
-NOTE: the image is only supported for x86_64 hardware and known to have issues on Apple silicon.
+NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
 
 We build Docker images for all pushes to `main`. We tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`. To leverage this, `docker pull` from our image repository.
 
 ```bash
 docker pull quay.io/unstructured-io/unstructured:latest
 ```
 
 Once pulled, you can create a container from this image and shell to it.
 
 ```bash
 # create the container
-docker run --platform linux/amd64 -d -t --name unstructured quay.io/unstructured-io/unstructured:latest
+docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
 
 # this will drop you into a bash shell where the Docker image is running
 docker exec -it unstructured bash
 ```
 
 You can also build your own Docker image.
```

#### html2text {}

```diff
@@ -40,46 +40,48 @@
 [str(el) for el in elements])) ``` And if you installed with `local-inference`,
 you should be able to run this as well: ```python from
 unstructured.partition.auto import partition elements = partition("example-
 docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
 ``` ## :dizzy: Instructions for using the docker image The following
 instructions are intended to help you get up and running using Docker to
 interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
-) if you don't already have docker installed on your machine. NOTE: the image
-is only supported for x86_64 hardware and known to have issues on Apple
-silicon. We build Docker images for all pushes to `main`. We tag each image
-with the corresponding short commit hash (e.g. `fbc7a69`) and the application
+) if you don't already have docker installed on your machine. NOTE: we build
+multi-platform images to support both x86_64 and Apple silicon hardware.
+`docker pull` should download the corresponding image for your architecture,
+but you can specify with `--platform` (e.g. `--platform linux/amd64`) if
+needed. We build Docker images for all pushes to `main`. We tag each image with
+the corresponding short commit hash (e.g. `fbc7a69`) and the application
 version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`.
 To leverage this, `docker pull` from our image repository. ```bash docker pull
 quay.io/unstructured-io/unstructured:latest ``` Once pulled, you can create a
 container from this image and shell to it. ```bash # create the container
-docker run --platform linux/amd64 -d -t --name unstructured quay.io/
-unstructured-io/unstructured:latest # this will drop you into a bash shell
-where the Docker image is running docker exec -it unstructured bash ``` You can
-also build your own Docker image. If you only plan on parsing one type of data
-you can speed up building the image by commenting out some of the packages/
-requirements necessary for other data types. See Dockerfile to know which lines
-are necessary for your use case. ```bash make docker-build # this will drop you
-into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
-interpreter's interactive mode. ```bash # this will drop you into a python
-console so you can run the below partition functions python3 >>> from
-unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
-(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
-unstructured.partition.text import partition_text >>> elements = partition_text
-(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
-Instructions for Local Development The following instructions are intended to
-help you get up and running with `unstructured` locally if you are planning to
-contribute to the project. * Using `pyenv` to manage virtualenv's is
-recommended but not necessary * Mac install instructions. See [here](https://
-github.com/Unstructured-IO/community#mac--homebrew) for more detailed
-instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
-Linux instructions are available [here](https://github.com/Unstructured-IO/
-community#linux). * Create a virtualenv to work in and activate it, e.g. for
-one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
+docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
+# this will drop you into a bash shell where the Docker image is running docker
+exec -it unstructured bash ``` You can also build your own Docker image. If you
+only plan on parsing one type of data you can speed up building the image by
+commenting out some of the packages/requirements necessary for other data
+types. See Dockerfile to know which lines are necessary for your use case.
+```bash make docker-build # this will drop you into a bash shell where the
+Docker image is running make docker-start-bash ``` Once in the running
+container, you can try things out directly in Python interpreter's interactive
+mode. ```bash # this will drop you into a python console so you can run the
+below partition functions python3 >>> from unstructured.partition.pdf import
+partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
+parser-paper-fast.pdf") >>> from unstructured.partition.text import
+partition_text >>> elements = partition_text(filename="example-docs/fake-
+text.txt") ``` ## :coffee: Installation Instructions for Local Development The
+following instructions are intended to help you get up and running with
+`unstructured` locally if you are planning to contribute to the project. *
+Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
+install instructions. See [here](https://github.com/Unstructured-IO/
+community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
+virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
+(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
+work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
+3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
```

### Comparing `unstructured-0.5.8/setup.py` & `unstructured-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.5.9/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.5.9/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/test_unstructured/test_utils.py` & `unstructured-0.5.9/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/cleaners/core.py` & `unstructured-0.5.9/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/cleaners/extract.py` & `unstructured-0.5.9/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/cleaners/translate.py` & `unstructured-0.5.9/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/documents/base.py` & `unstructured-0.5.9/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/documents/elements.py` & `unstructured-0.5.9/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/documents/email_elements.py` & `unstructured-0.5.9/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/documents/html.py` & `unstructured-0.5.9/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/documents/xml.py` & `unstructured-0.5.9/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/file_utils/exploration.py` & `unstructured-0.5.9/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/file_utils/file_conversion.py` & `unstructured-0.5.9/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/file_utils/filetype.py` & `unstructured-0.5.9/unstructured/file_utils/filetype.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/file_utils/metadata.py` & `unstructured-0.5.9/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/azure.py` & `unstructured-0.5.9/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/biomed.py` & `unstructured-0.5.9/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/fsspec.py` & `unstructured-0.5.9/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/git.py` & `unstructured-0.5.9/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/github.py` & `unstructured-0.5.9/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/gitlab.py` & `unstructured-0.5.9/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/google_drive.py` & `unstructured-0.5.9/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/local.py` & `unstructured-0.5.9/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/reddit.py` & `unstructured-0.5.9/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/s3.py` & `unstructured-0.5.9/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.5.9/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.5.9/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/interfaces.py` & `unstructured-0.5.9/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/ingest/main.py` & `unstructured-0.5.9/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/nlp/english-words.txt` & `unstructured-0.5.9/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/nlp/english_words.py` & `unstructured-0.5.9/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/nlp/patterns.py` & `unstructured-0.5.9/unstructured/nlp/patterns.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/nlp/tokenize.py` & `unstructured-0.5.9/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/__init__.py` & `unstructured-0.5.9/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/auto.py` & `unstructured-0.5.9/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/common.py` & `unstructured-0.5.9/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/doc.py` & `unstructured-0.5.9/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/docx.py` & `unstructured-0.5.9/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/email.py` & `unstructured-0.5.9/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/epub.py` & `unstructured-0.5.9/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/html.py` & `unstructured-0.5.9/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/image.py` & `unstructured-0.5.9/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/json.py` & `unstructured-0.5.9/unstructured/partition/json.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/md.py` & `unstructured-0.5.9/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/msg.py` & `unstructured-0.5.9/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/pdf.py` & `unstructured-0.5.9/unstructured/partition/pdf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/ppt.py` & `unstructured-0.5.9/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/pptx.py` & `unstructured-0.5.9/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/partition/text.py` & `unstructured-0.5.9/unstructured/partition/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
             try:
                 file_text = f.read()
             except (UnicodeDecodeError, UnicodeError) as error:
                 raise error
 
     elif file is not None:
         file_text = file.read()
+        if isinstance(file_text, bytes):
+            file_text = file_text.decode(encoding)
 
     elif text is not None:
         file_text = str(text)
 
     file_content = split_by_paragraph(file_text)
 
     elements: List[Element] = []
```

### Comparing `unstructured-0.5.8/unstructured/partition/text_type.py` & `unstructured-0.5.9/unstructured/partition/text_type.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/argilla.py` & `unstructured-0.5.9/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/base.py` & `unstructured-0.5.9/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/datasaur.py` & `unstructured-0.5.9/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/huggingface.py` & `unstructured-0.5.9/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/label_box.py` & `unstructured-0.5.9/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/label_studio.py` & `unstructured-0.5.9/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/staging/prodigy.py` & `unstructured-0.5.9/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured/utils.py` & `unstructured-0.5.9/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.5.8/unstructured.egg-info/PKG-INFO` & `unstructured-0.5.9/unstructured.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.5.8
+Version: 0.5.9
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -90,27 +90,27 @@
         ```
         
         ## :dizzy: Instructions for using the docker image
         
         The following instructions are intended to help you get up and running using Docker to interact with `unstructured`.
         See [here](https://docs.docker.com/get-docker/) if you don't already have docker installed on your machine.
         
-        NOTE: the image is only supported for x86_64 hardware and known to have issues on Apple silicon.
+        NOTE: we build multi-platform images to support both x86_64 and Apple silicon hardware. `docker pull` should download the corresponding image for your architecture, but you can specify with `--platform` (e.g. `--platform linux/amd64`) if needed.
         
         We build Docker images for all pushes to `main`. We tag each image with the corresponding short commit hash (e.g. `fbc7a69`) and the application version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`. To leverage this, `docker pull` from our image repository.
         
         ```bash
         docker pull quay.io/unstructured-io/unstructured:latest
         ```
         
         Once pulled, you can create a container from this image and shell to it.
         
         ```bash
         # create the container
-        docker run --platform linux/amd64 -d -t --name unstructured quay.io/unstructured-io/unstructured:latest
+        docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
         
         # this will drop you into a bash shell where the Docker image is running
         docker exec -it unstructured bash
         ```
         
         You can also build your own Docker image.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.5.8 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.5.9 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
@@ -44,46 +44,48 @@
 [str(el) for el in elements])) ``` And if you installed with `local-inference`,
 you should be able to run this as well: ```python from
 unstructured.partition.auto import partition elements = partition("example-
 docs/layout-parser-paper.pdf") print("\n\n".join([str(el) for el in elements]))
 ``` ## :dizzy: Instructions for using the docker image The following
 instructions are intended to help you get up and running using Docker to
 interact with `unstructured`. See [here](https://docs.docker.com/get-docker/
-) if you don't already have docker installed on your machine. NOTE: the image
-is only supported for x86_64 hardware and known to have issues on Apple
-silicon. We build Docker images for all pushes to `main`. We tag each image
-with the corresponding short commit hash (e.g. `fbc7a69`) and the application
+) if you don't already have docker installed on your machine. NOTE: we build
+multi-platform images to support both x86_64 and Apple silicon hardware.
+`docker pull` should download the corresponding image for your architecture,
+but you can specify with `--platform` (e.g. `--platform linux/amd64`) if
+needed. We build Docker images for all pushes to `main`. We tag each image with
+the corresponding short commit hash (e.g. `fbc7a69`) and the application
 version (e.g. `0.5.5-dev1`). We also tag the most recent image with `latest`.
 To leverage this, `docker pull` from our image repository. ```bash docker pull
 quay.io/unstructured-io/unstructured:latest ``` Once pulled, you can create a
 container from this image and shell to it. ```bash # create the container
-docker run --platform linux/amd64 -d -t --name unstructured quay.io/
-unstructured-io/unstructured:latest # this will drop you into a bash shell
-where the Docker image is running docker exec -it unstructured bash ``` You can
-also build your own Docker image. If you only plan on parsing one type of data
-you can speed up building the image by commenting out some of the packages/
-requirements necessary for other data types. See Dockerfile to know which lines
-are necessary for your use case. ```bash make docker-build # this will drop you
-into a bash shell where the Docker image is running make docker-start-bash ```
-Once in the running container, you can try things out directly in Python
-interpreter's interactive mode. ```bash # this will drop you into a python
-console so you can run the below partition functions python3 >>> from
-unstructured.partition.pdf import partition_pdf >>> elements = partition_pdf
-(filename="example-docs/layout-parser-paper-fast.pdf") >>> from
-unstructured.partition.text import partition_text >>> elements = partition_text
-(filename="example-docs/fake-text.txt") ``` ## :coffee: Installation
-Instructions for Local Development The following instructions are intended to
-help you get up and running with `unstructured` locally if you are planning to
-contribute to the project. * Using `pyenv` to manage virtualenv's is
-recommended but not necessary * Mac install instructions. See [here](https://
-github.com/Unstructured-IO/community#mac--homebrew) for more detailed
-instructions. * `brew install pyenv-virtualenv` * `pyenv install 3.8.15` *
-Linux instructions are available [here](https://github.com/Unstructured-IO/
-community#linux). * Create a virtualenv to work in and activate it, e.g. for
-one named `unstructured`: `pyenv virtualenv 3.8.15 unstructured`
+docker run -dt --name unstructured quay.io/unstructured-io/unstructured:latest
+# this will drop you into a bash shell where the Docker image is running docker
+exec -it unstructured bash ``` You can also build your own Docker image. If you
+only plan on parsing one type of data you can speed up building the image by
+commenting out some of the packages/requirements necessary for other data
+types. See Dockerfile to know which lines are necessary for your use case.
+```bash make docker-build # this will drop you into a bash shell where the
+Docker image is running make docker-start-bash ``` Once in the running
+container, you can try things out directly in Python interpreter's interactive
+mode. ```bash # this will drop you into a python console so you can run the
+below partition functions python3 >>> from unstructured.partition.pdf import
+partition_pdf >>> elements = partition_pdf(filename="example-docs/layout-
+parser-paper-fast.pdf") >>> from unstructured.partition.text import
+partition_text >>> elements = partition_text(filename="example-docs/fake-
+text.txt") ``` ## :coffee: Installation Instructions for Local Development The
+following instructions are intended to help you get up and running with
+`unstructured` locally if you are planning to contribute to the project. *
+Using `pyenv` to manage virtualenv's is recommended but not necessary * Mac
+install instructions. See [here](https://github.com/Unstructured-IO/
+community#mac--homebrew) for more detailed instructions. * `brew install pyenv-
+virtualenv` * `pyenv install 3.8.15` * Linux instructions are available [here]
+(https://github.com/Unstructured-IO/community#linux). * Create a virtualenv to
+work in and activate it, e.g. for one named `unstructured`: `pyenv virtualenv
+3.8.15 unstructured`
 `pyenv activate unstructured` * Run `make install` * Optional: * To install
 models and dependencies for processing images and PDFs locally, run `make
 install-local-inference`. * For processing image files, `tesseract` is
 required. See [here](https://tesseract-ocr.github.io/tessdoc/Installation.html)
 for installation instructions. * For processing PDF files, `tesseract` and
 `poppler` are required. The [pdf2image docs](https://pdf2image.readthedocs.io/
 en/latest/installation.html) have instructions on installing `poppler` across
```

### Comparing `unstructured-0.5.8/unstructured.egg-info/SOURCES.txt` & `unstructured-0.5.9/unstructured.egg-info/SOURCES.txt`

 * *Files identical despite different names*

