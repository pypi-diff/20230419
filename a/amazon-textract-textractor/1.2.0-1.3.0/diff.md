# Comparing `tmp/amazon-textract-textractor-1.2.0.tar.gz` & `tmp/amazon-textract-textractor-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-textractor-1.2.0.tar", last modified: Wed Apr 12 15:25:42 2023, max compression
+gzip compressed data, was "amazon-textract-textractor-1.3.0.tar", last modified: Tue Apr 18 22:36:15 2023, max compression
```

## Comparing `amazon-textract-textractor-1.2.0.tar` & `amazon-textract-textractor-1.3.0.tar`

### file list

```diff
@@ -1,70 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-12 15:25:25.000000 amazon-textract-textractor-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.670259 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 15:25:42.000000 amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/pandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/pdf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/extras/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/textractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/textractor/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.674259 amazon-textract-textractor-1.2.0/textractor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.678259 amazon-textract-textractor-1.2.0/textractor/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/document_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/expense_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/expense_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/identity_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/identity_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/key_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/lazy_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/line.py
--rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/selection_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/table_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/entities/word.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.678259 amazon-textract-textractor-1.2.0/textractor/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35493 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/parsers/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/textractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/textractor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/utils/search_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/textractor/validate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/validate/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 15:25:42.682259 amazon-textract-textractor-1.2.0/textractor/visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/visualizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/visualizers/arial.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-04-12 15:25:26.000000 amazon-textract-textractor-1.2.0/textractor/visualizers/entitylist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 22:36:15.000000 amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/pandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/extras/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/textractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/textractor/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.528288 amazon-textract-textractor-1.3.0/textractor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/data/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/expense_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/expense_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/identity_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/identity_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/key_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/lazy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/selection_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/table_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/entities/word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35059 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/parsers/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/textractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/utils/search_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:36:15.532288 amazon-textract-textractor-1.3.0/textractor/visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/visualizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/visualizers/arial.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-04-18 22:36:08.000000 amazon-textract-textractor-1.3.0/textractor/visualizers/entitylist.py
```

### Comparing `amazon-textract-textractor-1.2.0/LICENSE` & `amazon-textract-textractor-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/PKG-INFO` & `amazon-textract-textractor-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.2.0
+Version: 1.3.0
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: pandas
```

### Comparing `amazon-textract-textractor-1.2.0/README.md` & `amazon-textract-textractor-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/PKG-INFO` & `amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.2.0
+Version: 1.3.0
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: pandas
```

### Comparing `amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/SOURCES.txt` & `amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -47,12 +47,10 @@
 textractor/entities/word.py
 textractor/parsers/__init__.py
 textractor/parsers/response_parser.py
 textractor/utils/__init__.py
 textractor/utils/geometry_util.py
 textractor/utils/s3_utils.py
 textractor/utils/search_utils.py
-textractor/validate/__init__.py
-textractor/validate/validation.py
 textractor/visualizers/__init__.py
 textractor/visualizers/arial.ttf
 textractor/visualizers/entitylist.py
```

### Comparing `amazon-textract-textractor-1.2.0/amazon_textract_textractor.egg-info/requires.txt` & `amazon-textract-textractor-1.3.0/amazon_textract_textractor.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Pillow
 XlsxWriter==3.0.*
 amazon-textract-caller<0.1.0,>=0.0.27
 amazon-textract-pipeline-pagedimensions
-amazon-textract-response-parser<0.2.0,>=0.1.37
+amazon-textract-response-parser<0.2.0,>=0.1.45
 editdistance==0.6.2
-jsonschema
 tabulate==0.9.*
 
 [dev]
-jsonschema
 jupyterlab
 numpy==1.21.*
 pandas
 pdf2image==1.16.*
 pytest
 sentence-transformers==2.2.*
 sphinx-rtd-theme==1.0.*
 
 [docs]
 Sphinx==5.1.*
-jsonschema
 jupyterlab
 nbsphinx==0.8.*
 numpy==1.21.*
 pandas
 pdf2image==1.16.0
 pytest
 sphinx-argparse
```

### Comparing `amazon-textract-textractor-1.2.0/setup.py` & `amazon-textract-textractor-1.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,22 @@
         requirements = [line for line in f.readlines()]
     return requirements
 
 
 setup(
     # include data files
     name="amazon-textract-textractor",
-    version="1.2.0",
+    version="1.3.0",
     license="Apache 2.0",
     description="A package to use AWS Textract services.",
     url="https://github.com/aws-samples/amazon-textract-textractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     keywords="amazon textract aws ocr document",
     packages=find_packages(exclude=["docs", "tests"], ),
     include_package_data=True,
```

### Comparing `amazon-textract-textractor-1.2.0/textractor/cli/cli.py` & `amazon-textract-textractor-1.3.0/textractor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/data/constants.py` & `amazon-textract-textractor-1.3.0/textractor/data/constants.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/bbox.py` & `amazon-textract-textractor-1.3.0/textractor/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/document.py` & `amazon-textract-textractor-1.3.0/textractor/entities/document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/document_entity.py` & `amazon-textract-textractor-1.3.0/textractor/entities/document_entity.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/expense_document.py` & `amazon-textract-textractor-1.3.0/textractor/entities/expense_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/expense_field.py` & `amazon-textract-textractor-1.3.0/textractor/entities/expense_field.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/identity_document.py` & `amazon-textract-textractor-1.3.0/textractor/entities/identity_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/key_value.py` & `amazon-textract-textractor-1.3.0/textractor/entities/key_value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/lazy_document.py` & `amazon-textract-textractor-1.3.0/textractor/entities/lazy_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/line.py` & `amazon-textract-textractor-1.3.0/textractor/entities/line.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/page.py` & `amazon-textract-textractor-1.3.0/textractor/entities/page.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/query.py` & `amazon-textract-textractor-1.3.0/textractor/entities/query.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/query_result.py` & `amazon-textract-textractor-1.3.0/textractor/entities/query_result.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/selection_element.py` & `amazon-textract-textractor-1.3.0/textractor/entities/selection_element.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/signature.py` & `amazon-textract-textractor-1.3.0/textractor/entities/signature.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/table.py` & `amazon-textract-textractor-1.3.0/textractor/entities/table.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/table_cell.py` & `amazon-textract-textractor-1.3.0/textractor/entities/table_cell.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/table_footer.py` & `amazon-textract-textractor-1.3.0/textractor/entities/table_footer.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/table_title.py` & `amazon-textract-textractor-1.3.0/textractor/entities/table_title.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/value.py` & `amazon-textract-textractor-1.3.0/textractor/entities/value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/entities/word.py` & `amazon-textract-textractor-1.3.0/textractor/entities/word.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/exceptions.py` & `amazon-textract-textractor-1.3.0/textractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/parsers/response_parser.py` & `amazon-textract-textractor-1.3.0/textractor/parsers/response_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from textractor.entities.bbox import BoundingBox
 from textractor.entities.document import Document
 from textractor.entities.key_value import KeyValue
 from textractor.entities.table_cell import TableCell
 from textractor.entities.table_title import TableTitle
 from textractor.entities.table_footer import TableFooter
 from textractor.entities.query import Query
-from textractor.validate.validation import validate_entity_schema
 from textractor.entities.document_entity import DocumentEntity
 from textractor.entities.selection_element import SelectionElement
 from textractor.data.constants import (
     TABLE_FOOTER,
     TABLE_TITLE,
     COLUMN_HEADER,
     TABLE_SUMMARY,
@@ -181,15 +180,14 @@
 
     :return: Returns a list of Word objects for the IDs passed in word_ids.
     :rtype: list
     """
     word_elements = []
 
     for word_id in word_ids:
-        validate_entity_schema(id_json_map[word_id], entity=WORD)
         word_elements.append(id_json_map[word_id])
 
     text_type = {PRINTED: TextTypes.PRINTED, HANDWRITING: TextTypes.HANDWRITING}
 
     words = []
     for elem in word_elements:
         word = Word(
@@ -228,15 +226,14 @@
              belonging to the corresponding Line objects.
     :rtype: List[Line], List[Word]
     """
     page_lines = []
 
     for line_id in line_ids:
         if line_id in page.child_ids:
-            validate_entity_schema(id_json_map[line_id], entity=LINE)
             page_lines.append(id_json_map[line_id])
 
     lines = []
     page_words = []
     for line in page_lines:
         if _get_relationship_ids(line, relationship="CHILD"):
             line_words = _create_word_objects(
@@ -278,16 +275,14 @@
     :type page: Page
 
     :return: Returns a dictionary mapping of SelectionElement IDs with SelectionElement objects for the IDs present in
              selection_ids.
     :rtype: Dict[str, SelectionElement]
     """
     checkbox_elements = [id_json_map[selection_id] for selection_id in selection_ids]
-    for checkbox_info in checkbox_elements:
-        validate_entity_schema(checkbox_info, entity=SELECTION_ELEMENT)
 
     status = {
         "SELECTED": SelectionStatus.SELECTED,
         "NOT_SELECTED": SelectionStatus.NOT_SELECTED,
     }
 
     checkboxes = {}
@@ -374,15 +369,14 @@
     id_json_map: Dict[str, str],
     entity_id_map: Dict[str, list],
     page: Page,
 ) -> List[Query]:
     page_queries = []
     for query_id in query_ids:
         if query_id in page.child_ids:
-            validate_entity_schema(id_json_map[query_id], entity=QUERY)
             page_queries.append(id_json_map[query_id])
 
     query_result_id_map = {}
     for block in page_queries:
         answer = _get_relationship_ids(block, relationship="ANSWER")
         query_result_id_map[block["Id"]] = answer[0] if answer else None
 
@@ -411,15 +405,14 @@
     id_json_map: Dict[str, str],
     entity_id_map: Dict[str, list],
     page: Page,
 ) -> Dict[str, QueryResult]:
     page_query_results = []
     for query_result_id in query_result_ids:
         if query_result_id in page.child_ids:
-            validate_entity_schema(id_json_map[query_result_id], entity=QueryResult)
             page_query_results.append(id_json_map[query_result_id])
 
     query_results = {}
     for block in page_query_results:
         query_results[block["Id"]] = QueryResult(
             entity_id=block["Id"],
             confidence=block["Confidence"],
@@ -441,15 +434,14 @@
     id_json_map: Dict[str, str],
     entity_id_map: Dict[str, list],
     page: Page,
 ) -> Dict[str, Signature]:
     page_signatures = []
     for signature_id in signature_ids:
         if signature_id in page.child_ids:
-            validate_entity_schema(id_json_map[signature_id], entity=Signature)
             page_signatures.append(id_json_map[signature_id])
 
     signatures = {}
     for block in page_signatures:
         signatures[block["Id"]] = Signature(
             entity_id=block["Id"],
             confidence=block["Confidence"],
@@ -489,15 +481,14 @@
     :return: Returns a list of KeyValue objects and list of Word objects with CHILD relationship
              to the KeyValue objects.
     :rtype: List[KeyValue], List[Word]
     """
     page_kv = []
     for kv_id in key_value_ids:
         if kv_id in page.child_ids:
-            validate_entity_schema(id_json_map[kv_id], entity=KEY_VALUE_SET)
             page_kv.append(id_json_map[kv_id])
 
     keys_info = _filter_by_entity(page_kv, entity_type="KEY")
 
     key_value_id_map = {
         block["Id"]: _get_relationship_ids(block, relationship="VALUE")[0]
         for block in keys_info.values()
@@ -578,15 +569,14 @@
     :return: Returns a dictionary containing TableCells mapped with their IDs and dictionary containing ID: CELL JSON mapping.
     :rtype: Dict[str, TableCell], Dict[str, Any]
     """
     all_table_cells_info = {}
     for table in page_tables:
         for cell_id in _get_relationship_ids(table, relationship="CHILD"):
             if id_entity_map[cell_id] == CELL:
-                validate_entity_schema(id_json_map[cell_id], entity=CELL)
                 all_table_cells_info[cell_id] = id_json_map[cell_id]
 
     table_cells = {}
     for elem_id, elem in all_table_cells_info.items():
         table_cells[elem_id] = TableCell(
             entity_id=elem_id,
             bbox=BoundingBox.from_normalized_dict(
@@ -637,15 +627,14 @@
     :return: Returns a list of table objects and list of words present in tables.
     :rtype: List[Table], List[Word]
     """
     # Create Tables
     page_tables = []
     for table_id in table_ids:
         if table_id in page.child_ids:
-            validate_entity_schema(id_json_map[table_id], entity=TABLE)
             page_tables.append(id_json_map[table_id])
 
     tables = {}
     for val in page_tables:
         tables[val["Id"]] = Table(
             entity_id=val["Id"],
             bbox=BoundingBox.from_normalized_dict(
@@ -907,15 +896,14 @@
         currency = field["Currency"]["Code"]
     else:
         currency = None
     return ExpenseField(type_expense, value_expense, group_properties=group_properties, label=label_expense,
                         currency=currency, page=page.page_num)
 
 
-
 def parser_analyze_expense_response(response):
     response["Blocks"] = [b for doc in response["ExpenseDocuments"] for b in doc.get("Blocks", [])]
     document = parse_document_api_response(response)
     for doc in response["ExpenseDocuments"]:
         # FIXME
         if len(doc["SummaryFields"]) == 0:
             continue
@@ -956,14 +944,19 @@
 
     :param response: JSON response data in a format readable by the ResponseParser.
     :type response: dict
 
     :return: Document object returned after making respective parse function calls.
     :rtype: Document
     """
-
     if "IdentityDocuments" in response:
+        from trp.trp2_analyzeid import TAnalyzeIdDocumentSchema
+        t_doc = TAnalyzeIdDocumentSchema().load(response)
         return parse_analyze_id_response(response)
     if "ExpenseDocuments" in response:
+        from trp.trp2_expense import TAnalyzeExpenseDocumentSchema
+        t_doc = TAnalyzeExpenseDocumentSchema().load(response)
         return parser_analyze_expense_response(response)
     else:
+        from trp.trp2 import TDocumentSchema
+        t_doc = TDocumentSchema().load(response)
         return parse_document_api_response(response)
```

### Comparing `amazon-textract-textractor-1.2.0/textractor/textractor.py` & `amazon-textract-textractor-1.3.0/textractor/textractor.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/utils/geometry_util.py` & `amazon-textract-textractor-1.3.0/textractor/utils/geometry_util.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/utils/s3_utils.py` & `amazon-textract-textractor-1.3.0/textractor/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/utils/search_utils.py` & `amazon-textract-textractor-1.3.0/textractor/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/visualizers/arial.ttf` & `amazon-textract-textractor-1.3.0/textractor/visualizers/arial.ttf`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.2.0/textractor/visualizers/entitylist.py` & `amazon-textract-textractor-1.3.0/textractor/visualizers/entitylist.py`

 * *Files identical despite different names*

