# Comparing `tmp/robotframework-tidy-4.1.0.tar.gz` & `tmp/robotframework-tidy-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-tidy-4.1.0.tar", last modified: Fri Apr  7 18:36:45 2023, max compression
+gzip compressed data, was "robotframework-tidy-4.2.0.tar", last modified: Wed Apr 19 08:55:50 2023, max compression
```

## Comparing `robotframework-tidy-4.1.0.tar` & `robotframework-tidy-4.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.818516 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotframework_tidy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.822517 robotframework-tidy-4.1.0/robotidy/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.822517 robotframework-tidy-4.1.0/robotidy/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotidy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 18:36:45.000000 robotframework-tidy-4.1.0/robotidy/__pycache__/version.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    19515 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/rich_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/skip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/robotidy/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AddMissingEnd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignKeywordsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignTemplatedTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignTestCasesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/AlignVariablesSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/DiscardEmptySections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/GenerateDocumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/IndentNestedKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/InlineIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/MergeAndOrderSections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeAssignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeComments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeNewLines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSectionHeaderName.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSeparators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSettingName.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/NormalizeTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/OrderSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/OrderSettingsSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/OrderTags.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RemoveEmptySettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RenameKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RenameTestCases.py
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/RenameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceBreakContinue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceEmptyValues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceReturns.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/ReplaceRunKeywordIf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/SmartSortKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/SplitTooLongLine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/Translate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19572 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/aligners_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/transformers/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13418 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/robotidy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 18:36:45.826517 robotframework-tidy-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-07 18:36:28.000000 robotframework-tidy-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.501036 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotframework_tidy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.505035 robotframework-tidy-4.2.0/robotidy/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.509036 robotframework-tidy-4.2.0/robotidy/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotidy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-19 08:55:50.000000 robotframework-tidy-4.2.0/robotidy/__pycache__/version.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14328 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/rich_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/robotidy/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AddMissingEnd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignKeywordsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignTemplatedTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignTestCasesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/AlignVariablesSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/DiscardEmptySections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/GenerateDocumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9875 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/IndentNestedKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/InlineIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/MergeAndOrderSections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeAssignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeComments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeNewLines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSectionHeaderName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSeparators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSettingName.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/NormalizeTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/OrderSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/OrderSettingsSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/OrderTags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RemoveEmptySettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RenameKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RenameTestCases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/RenameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceBreakContinue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceEmptyValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceReturns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/ReplaceRunKeywordIf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/SmartSortKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/SplitTooLongLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10020 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/Translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23065 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/aligners_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/transformers/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13625 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/robotidy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 08:55:50.517036 robotframework-tidy-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-19 08:55:31.000000 robotframework-tidy-4.2.0/setup.py
```

### Comparing `robotframework-tidy-4.1.0/LICENSE` & `robotframework-tidy-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/PKG-INFO` & `robotframework-tidy-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.1.0
+Version: 4.2.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.1.0/README.md` & `robotframework-tidy-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotframework_tidy.egg-info/PKG-INFO` & `robotframework-tidy-4.2.0/robotframework_tidy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-tidy
-Version: 4.1.0
+Version: 4.2.0
 Summary: Code autoformatter for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-tidy
 Author: MarketSquare - Robot Framework community
 Author-email: bartek.hirsz@gmail.com
 License: Apache License 2.0
 Keywords: robotframework
 Platform: any
```

### Comparing `robotframework-tidy-4.1.0/robotframework_tidy.egg-info/SOURCES.txt` & `robotframework-tidy-4.2.0/robotframework_tidy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/app.py` & `robotframework-tidy-4.2.0/robotidy/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import os
 import sys
 from difflib import unified_diff
+from typing import Dict
 
 try:
     import rich_click as click
 except ImportError:  # Fails on vendored-in LSP plugin
     import click
 
 from robot.api import get_model
 from robot.errors import DataError
 
 from robotidy import utils
-from robotidy.config import Config
+from robotidy.config import MainConfig
 from robotidy.disablers import RegisterDisablers
 from robotidy.rich_console import console
 
 
 class Robotidy:
-    def __init__(self, config: Config):
-        self.config = config
+    def __init__(self, main_config: "MainConfig"):
+        self.main_config = main_config
+        self.config = main_config.default_loaded
 
     def get_model(self, source):
         if utils.rf_supports_lang():
             return get_model(source, lang=self.config.language)
         return get_model(source)
 
     def transform_files(self):
         changed_files = 0
-        disabler_finder = RegisterDisablers(self.config.formatting.start_line, self.config.formatting.end_line)
-        for source in self.config.sources:
+        for source, config in self.main_config.get_sources_with_configs():
+            self.config = config
+            disabler_finder = RegisterDisablers(self.config.formatting.start_line, self.config.formatting.end_line)
             try:
                 stdin = False
                 if str(source) == "-":
                     stdin = True
                     if self.config.verbose:
                         click.echo("Loading file from stdin")
                     source = self.load_from_stdin()
@@ -102,18 +105,15 @@
                 if isinstance(f.newlines, str):
                     return f.newlines
                 else:
                     return f.newlines[0]
         return self.config.formatting.line_sep
 
     def output_diff(
-        self,
-        path: str,
-        old_model: utils.StatementLinesCollector,
-        new_model: utils.StatementLinesCollector,
+        self, path: str, old_model: utils.StatementLinesCollector, new_model: utils.StatementLinesCollector
     ):
         if not self.config.show_diff:
             return
         old = [l + "\n" for l in old_model.text.splitlines()]
         new = [l + "\n" for l in new_model.text.splitlines()]
         lines = list(unified_diff(old, new, fromfile=f"{path}\tbefore", tofile=f"{path}\tafter"))
         if not lines:
```

### Comparing `robotframework-tidy-4.1.0/robotidy/cli.py` & `robotframework-tidy-4.2.0/robotidy/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import os
-import re
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Pattern, Tuple, Union
+from typing import List, Optional, Pattern, Tuple, Union
 
 try:
     import rich_click as click
 
     RICH_PRESENT = True
 except ImportError:  # Fails on vendored-in LSP plugin
     import click
 
     RICH_PRESENT = False
 
-from robotidy import app, decorators, files, skip, utils, version
-from robotidy.config import Config, FormattingConfig
+from robotidy import app
+from robotidy import config as config_module
+from robotidy import decorators, files, skip, utils, version
+from robotidy.config import RawConfig, csv_list_type, validate_target_version
 from robotidy.rich_console import console
-from robotidy.transformers import TransformConfig, TransformConfigMap, TransformConfigParameter, load_transformers
+from robotidy.transformers import TransformConfigMap, TransformConfigParameter, load_transformers
 
 CLI_OPTIONS_LIST = [
     {
         "name": "Run only selected transformers",
         "options": ["--transform"],
     },
     {
@@ -33,15 +33,15 @@
     },
     {
         "name": "Documentation",
         "options": ["--list", "--desc"],
     },
     {
         "name": "Configuration",
-        "options": ["--configure", "--config"],
+        "options": ["--configure", "--config", "--ignore-git-dir"],
     },
     {
         "name": "Global formatting settings",
         "options": [
             "--spacecount",
             "--indent",
             "--continuation-indent",
@@ -52,21 +52,31 @@
             "--endline",
         ],
     },
     {"name": "File exclusion", "options": ["--exclude", "--extend-exclude", "--skip-gitignore"]},
     skip.option_group,
     {
         "name": "Other",
-        "options": ["--target-version", "--language", "--verbose", "--color", "--output", "--version", "--help"],
+        "options": [
+            "--target-version",
+            "--language",
+            "--reruns",
+            "--verbose",
+            "--color",
+            "--output",
+            "--version",
+            "--help",
+        ],
     },
 ]
 
 if RICH_PRESENT:
     click.rich_click.USE_RICH_MARKUP = True
     click.rich_click.USE_MARKDOWN = True
+    click.rich_click.FORCE_TERMINAL = None  # workaround rich_click trying to force color in GitHub Actions
     click.rich_click.STYLE_OPTION = "bold sky_blue3"
     click.rich_click.STYLE_SWITCH = "bold sky_blue3"
     click.rich_click.STYLE_METAVAR = "bold white"
     click.rich_click.STYLE_OPTION_DEFAULT = "grey37"
     click.rich_click.STYLE_OPTIONS_PANEL_BORDER = "grey66"
     click.rich_click.STYLE_USAGE = "magenta"
     click.rich_click.OPTION_GROUPS = {
@@ -74,96 +84,37 @@
         "python -m robotidy": CLI_OPTIONS_LIST,
     }
 
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 
 
-def parse_opt(opt):
-    while opt and opt[0] == "-":
-        opt = opt[1:]
-    return opt.replace("-", "_")
-
-
-def validate_config_options(params, config):
-    if params is None:
-        return
-    allowed = {parse_opt(opt) for param in params for opt in param.opts}
-    for conf in config:
-        if conf not in allowed:
-            rec_finder = utils.RecommendationFinder()
-            similar = rec_finder.find(conf, list(allowed))
-            raise click.NoSuchOption(conf, possibilities=similar)
-
-
-def read_config(ctx: click.Context, param: click.Parameter, value: Optional[str]) -> Optional[str]:
-    # if --config was not used, try to find pyproject.toml or robotidy.toml file
-    if value:
-        config = files.read_pyproject_config(value)
-    else:
-        src = ctx.params["src"] or (str(Path(".").resolve()),)
-        ignore_git_dir = ctx.params["ignore_git_dir"]
-        config = files.find_and_read_config(src, ignore_git_dir)
-    if not config:
-        return
-    # Sanitize the values to be Click friendly. For more information please see:
-    # https://github.com/psf/black/issues/1458
-    # https://github.com/pallets/click/issues/1567
-    config = {k: str(v) if not isinstance(v, (list, dict)) else v for k, v in config.items()}
-    if "src" in config:
-        config["src"] = tuple(config["src"])
-    validate_config_options(ctx.command.params, config)
-    default_map: Dict[str, Any] = {}
-    if ctx.default_map:
-        default_map.update(ctx.default_map)
-    default_map.update(config)
-    ctx.default_map = default_map
-
-
-def validate_regex_callback(
-    ctx: click.Context,
-    param: click.Parameter,
-    value: Optional[str],
-) -> Optional[Pattern]:
+def validate_regex_callback(ctx: click.Context, param: click.Parameter, value: Optional[str]) -> Optional[Pattern]:
     return utils.validate_regex(value)
 
 
-def validate_target_version(
-    ctx: click.Context,
-    param: Union[click.Option, click.Parameter],
-    value: Optional[str],
+def validate_target_version_callback(
+    ctx: click.Context, param: Union[click.Option, click.Parameter], value: Optional[str]
 ) -> Optional[int]:
-    if value is None:
-        return utils.ROBOT_VERSION.major
-    version = utils.TargetVersion[value.upper()].value
-    if version > utils.ROBOT_VERSION.major:
-        raise click.BadParameter(
-            f"Target Robot Framework version ({version}) should not be higher than "
-            f"installed version ({utils.ROBOT_VERSION})."
-        )
-    return version
-
-
-def validate_list_optional_value(
-    ctx: click.Context,
-    param: Union[click.Option, click.Parameter],
-    value: Optional[str],
-):
+    return validate_target_version(value)
+
+
+def validate_list_optional_value(ctx: click.Context, param: Union[click.Option, click.Parameter], value: Optional[str]):
     if not value:
         return value
     allowed = ["all", "enabled", "disabled"]
     if value not in allowed:
         raise click.BadParameter(f"Not allowed value. Allowed values are: {', '.join(allowed)}")
     return value
 
 
-def csv_list_type(ctx: click.Context, param: Union[click.Option, click.Parameter], value: Optional[str]) -> List[str]:
-    if not value:
-        return []
-    return value.split(",")
+def csv_list_type_callback(
+    ctx: click.Context, param: Union[click.Option, click.Parameter], value: Optional[str]
+) -> List[str]:
+    return csv_list_type(value)
 
 
 def print_transformer_docs(transformer):
     from rich.markdown import Markdown
 
     md = Markdown(str(transformer), code_theme="native", inline_code_lexer="robotframework")
     console.print(md)
@@ -194,27 +145,29 @@
     for transformer in transformers_from_conf:
         if transformer.name not in transformers_names:
             external.append(transformer)
     return external
 
 
 @decorators.optional_rich
-def print_transformers_list(
-    transformers_config: TransformConfigMap, config: Config, target_version: int, list_transformers: str
-):
+def print_transformers_list(global_config: config_module.MainConfig):
     from rich.table import Table
 
+    target_version = global_config.default.target_version
+    list_transformers = global_config.default.list_transformers
     table = Table(title="Transformers", header_style="bold red")
     table.add_column("Name", justify="left", no_wrap=True)
     table.add_column("Enabled")
     transformers = load_transformers(TransformConfigMap([], [], []), allow_disabled=True, target_version=target_version)
-    transformers.extend(_load_external_transformers(transformers, transformers_config, target_version))
+    transformers.extend(
+        _load_external_transformers(transformers, global_config.default_loaded.transformers_config, target_version)
+    )
 
     for transformer in transformers:
-        enabled = transformer.name in config.transformers_lookup
+        enabled = transformer.name in global_config.default_loaded.transformers_lookup
         if list_transformers != "all":
             filter_by = list_transformers == "enabled"
             if enabled != filter_by:
                 continue
         decorated_enable = "Yes" if enabled else "No"
         if enabled != transformer.enabled_by_default:
             decorated_enable = f"[bold magenta]{decorated_enable}*"
@@ -259,15 +212,14 @@
     metavar="TRANSFORMER_NAME:PARAM=VALUE",
     help="Configure transformers",
 )
 @click.argument(
     "src",
     nargs=-1,
     type=click.Path(exists=True, file_okay=True, dir_okay=True, readable=True, allow_dash=True),
-    is_eager=True,
     metavar="[PATH(S)]",
 )
 @click.option(
     "--exclude",
     type=str,
     callback=validate_regex_callback,
     help=(
@@ -291,40 +243,30 @@
     is_flag=True,
     show_default=True,
     help="Skip **.gitignore** files and do not ignore files listed inside.",
 )
 @click.option(
     "--ignore-git-dir",
     is_flag=True,
-    is_eager=True,
-    help="Ignore .git directories when searching for the default configuration file. "
-    "By default first parent directory with .git directory is returned and this flag disables this behaviour.",
+    help="Ignore **.git** directories when searching for the default configuration file. "
+    "By default first parent directory with **.git** directory is returned and this flag disables this behaviour.",
     show_default=True,
 )
 @click.option(
     "--config",
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=False,
         readable=True,
         allow_dash=False,
         path_type=str,
     ),
-    is_eager=True,
-    callback=read_config,
     help="Read configuration from FILE path.",
 )
-# This option is workaround to make it possible to pass configuration directory when reading config.
-# We first load the config file and then map every value from it as cli option defaults. The option must exist, so we
-# cannot pass additional info, ie the directory where config file was found.
-@click.option(
-    "--config-directory",
-    hidden=True,
-)
 @click.option(
     "--overwrite/--no-overwrite",
     default=None,
     help="Write changes back to file",
     show_default=True,
 )
 @click.option(
@@ -416,15 +358,14 @@
     show_default=True,
 )
 @click.option(
     "--list",
     "-l",
     "list_transformers",
     callback=validate_list_optional_value,
-    is_eager=True,
     is_flag=False,
     default="",
     flag_value="all",
     help="List available transformers and exit. "
     "Pass optional value **enabled** or **disabled** to filter out list by transformer status.",
 )
 @click.option(
@@ -448,22 +389,22 @@
     is_flag=True,
     help="Transform files using transformers in order provided in cli",
 )
 @click.option(
     "--target-version",
     "-tv",
     type=click.Choice([v.name.lower() for v in utils.TargetVersion], case_sensitive=False),
-    callback=validate_target_version,
+    callback=validate_target_version_callback,
     help="Only enable transformers supported in set target version",
     show_default="installed Robot Framework version",
 )
 @click.option(
     "--language",
     "--lang",
-    callback=csv_list_type,
+    callback=csv_list_type_callback,
     help="Parse Robot Framework files using additional languages.",
     show_default="en",
 )
 @click.option(
     "--reruns",
     "-r",
     type=int,
@@ -484,140 +425,24 @@
 @skip.return_option
 @skip.tags_option
 @skip.sections_option
 @skip.block_comments_option
 @click.version_option(version=version.__version__, prog_name="robotidy")
 @click.pass_context
 @decorators.catch_exceptions
-def cli(
-    ctx: click.Context,
-    transform: List[TransformConfig],
-    custom_transformers: List[TransformConfig],
-    configure: List[TransformConfig],
-    src: Tuple[str, ...],
-    exclude: Optional[Pattern],
-    extend_exclude: Optional[Pattern],
-    skip_gitignore: bool,
-    overwrite: bool,
-    diff: bool,
-    color: bool,
-    check: bool,
-    spacecount: int,
-    indent: Optional[int],
-    continuation_indent: Optional[int],
-    lineseparator: str,
-    verbose: bool,
-    config: Optional[str],
-    config_directory: Optional[str],
-    separator: Optional[str],
-    startline: Optional[int],
-    endline: Optional[int],
-    line_length: int,
-    list_transformers: str,
-    desc: Optional[str],
-    output: Optional[Path],
-    force_order: bool,
-    target_version: int,
-    language: Optional[List[str]],
-    reruns: int,
-    ignore_git_dir: bool,
-    skip_comments: bool,
-    skip_documentation: bool,
-    skip_return_values: bool,
-    skip_keyword_call: List[str],
-    skip_keyword_call_pattern: List[str],
-    skip_settings: bool,
-    skip_arguments: bool,
-    skip_setup: bool,
-    skip_teardown: bool,
-    skip_timeout: bool,
-    skip_template: bool,
-    skip_return: bool,
-    skip_tags: bool,
-    skip_block_comments: bool,
-    skip_sections: str,
-):
+def cli(ctx: click.Context, **kwargs):
     """
     Robotidy is a tool for formatting Robot Framework source code.
     Full documentation available at <https://robotidy.readthedocs.io> .
     """
-    if not src and not (list_transformers or desc):
-        if ctx.default_map is not None:
-            src = ctx.default_map.get("src", None)
-        if not src:
-            print("No source path provided. Run robotidy --help to see how to use robotidy")
-            sys.exit(1)
-
-    if exclude is None:
-        exclude = re.compile(files.DEFAULT_EXCLUDES)
-
-    if config and verbose:
-        click.echo(f"Loaded {config} configuration file")
-
-    if overwrite is None:
-        # None is default, with check not set -> overwrite, with check set -> overwrite only when overwrite flag is set
-        overwrite = not check
-
-    if color:
-        color = "NO_COLOR" not in os.environ
-
-    skip_config = skip.SkipConfig(
-        documentation=skip_documentation,
-        return_values=skip_return_values,
-        keyword_call=skip_keyword_call,
-        keyword_call_pattern=skip_keyword_call_pattern,
-        settings=skip_settings,
-        arguments=skip_arguments,
-        setup=skip_setup,
-        teardown=skip_teardown,
-        template=skip_template,
-        timeout=skip_timeout,
-        return_statement=skip_return,
-        tags=skip_tags,
-        comments=skip_comments,
-        block_comments=skip_block_comments,
-        sections=skip_sections,
-    )
-
-    formatting = FormattingConfig(
-        space_count=spacecount,
-        indent=indent,
-        continuation_indent=continuation_indent,
-        line_sep=lineseparator,
-        start_line=startline,
-        separator=separator,
-        end_line=endline,
-        line_length=line_length,
-    )
-
-    transformers_config = TransformConfigMap(transform, custom_transformers, configure)
-    config = Config(
-        formatting=formatting,
-        skip=skip_config,
-        transformers_config=transformers_config,
-        src=src,
-        exclude=exclude,
-        extend_exclude=extend_exclude,
-        skip_gitignore=skip_gitignore,
-        overwrite=overwrite,
-        show_diff=diff,
-        verbose=verbose,
-        check=check,
-        output=output,
-        force_order=force_order,
-        target_version=target_version,
-        color=color,
-        language=language,
-        reruns=reruns,
-        config_directory=config_directory,
-    )
-
-    if list_transformers:
-        print_transformers_list(transformers_config, config, target_version, list_transformers)
+    cli_config = RawConfig.from_cli(ctx=ctx, **kwargs)
+    global_config = config_module.MainConfig(cli_config)
+    global_config.validate_src_is_required()
+    if global_config.default.list_transformers:
+        print_transformers_list(global_config)
         sys.exit(0)
-    if desc is not None:
-        return_code = print_description(desc, target_version)
+    if global_config.default.desc is not None:
+        return_code = print_description(global_config.default.desc, global_config.default.target_version)
         sys.exit(return_code)
-
-    tidy = app.Robotidy(config=config)
+    tidy = app.Robotidy(global_config)
     status = tidy.transform_files()
     sys.exit(status)
```

### Comparing `robotframework-tidy-4.1.0/robotidy/decorators.py` & `robotframework-tidy-4.2.0/robotidy/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import functools
-import sys
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
 from robotidy import exceptions
```

### Comparing `robotframework-tidy-4.1.0/robotidy/disablers.py` & `robotframework-tidy-4.2.0/robotidy/disablers.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/exceptions.py` & `robotframework-tidy-4.2.0/robotidy/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 import sys
+from typing import List
+
+from click import NoSuchOption
+
+from robotidy import utils
 
 
 class RobotidyConfigError(Exception):
     def __init__(self, err):
         print(f"Error: {err}")
         sys.exit(1)
 
@@ -31,7 +36,14 @@
     pass
 
 
 class MissingOptionalRichDependencyError(RobotidyConfigError):
     def __init__(self):
         msg = "It looks like you have rich module uninstalled. Install it to be able to use robotidy in the cli mode."
         super().__init__(msg)
+
+
+class NoSuchOptionError(NoSuchOption):
+    def __init__(self, option_name: str, allowed_options: List[str]):
+        rec_finder = utils.RecommendationFinder()
+        similar = rec_finder.find(option_name, allowed_options)
+        super().__init__(option_name, possibilities=similar)
```

### Comparing `robotframework-tidy-4.1.0/robotidy/files.py` & `robotframework-tidy-4.2.0/robotidy/files.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,38 @@
     import click
 
 import tomli
 from pathspec import PathSpec
 
 DEFAULT_EXCLUDES = r"/(\.direnv|\.eggs|\.git|\.hg|\.nox|\.tox|\.venv|venv|\.svn)/"
 INCLUDE_EXT = (".robot", ".resource")
+DOTFILE_CONFIG = ".robotidy"
+CONFIG_NAMES = ("robotidy.toml", "pyproject.toml", DOTFILE_CONFIG)
+
+
+@lru_cache()
+def find_source_config_file(src: Path, ignore_git_dir: bool = False) -> Optional[Path]:
+    """Find and return configuration file for the source path.
+
+    This method looks iteratively in source parents for directory that contains configuration file and
+    returns its path. The lru_cache speeds up searching if there are multiple files in the same directory (they will
+    have the same configuration file).
+
+    If ``.git`` directory is found and ``ignore_git_dir`` is set to ``False``, or top directory is reached, this method
+    returns ``None``.
+    """
+    if src.is_dir():
+        if not ignore_git_dir and src.name == ".git":
+            return None
+        for config_filename in CONFIG_NAMES:
+            if (src / config_filename).is_file():
+                return src / config_filename
+        if not src.parents:
+            return None
+    return find_source_config_file(src.parent, ignore_git_dir)
 
 
 @lru_cache()
 def find_project_root(srcs: Iterable[str], ignore_git_dir: bool = False) -> Path:
     """Return a directory containing .git, or robotidy.toml.
     That directory will be a common parent of all files and directories
     passed in `srcs`.
@@ -35,51 +59,32 @@
         set.intersection(*(set(parents) for parents in src_parents)),
         key=lambda path: path.parts,
     )
 
     for directory in (common_base, *common_base.parents):
         if not ignore_git_dir and (directory / ".git").exists():
             return directory
-
-        if (directory / "robotidy.toml").is_file():
-            return directory
-
-        if (directory / "pyproject.toml").is_file():
+        if any((directory / config_name).is_file() for config_name in CONFIG_NAMES):
             return directory
-
     return directory
 
 
-def find_and_read_config(src_paths: Iterable[str], ignore_git_dir: bool = False) -> Dict[str, Any]:
-    project_root = find_project_root(src_paths, ignore_git_dir)
-    config_path = project_root / "robotidy.toml"
-    if config_path.is_file():
-        return read_pyproject_config(str(config_path))
-    pyproject_path = project_root / "pyproject.toml"
-    if pyproject_path.is_file():
-        return read_pyproject_config(str(pyproject_path))
-    return {}
-
-
 def load_toml_file(config_path: Path) -> Dict[str, Any]:
     try:
         with config_path.open("rb") as tf:
             config = tomli.load(tf)
         return config
     except (tomli.TOMLDecodeError, OSError) as e:
         raise click.FileError(filename=str(config_path), hint=f"Error reading configuration file: {e}")
 
 
-def read_pyproject_config(path: str) -> Dict[str, Any]:
-    config_path = Path(path)
+def read_pyproject_config(config_path: Path) -> Dict[str, Any]:
     config = load_toml_file(config_path)
-    config = config.get("tool", {}).get("robotidy", {})
-    if config:
-        config["config_directory"] = str(config_path.parent)
-        click.echo(f"Loaded configuration from {path}")
+    if config_path.name != DOTFILE_CONFIG or "tool" in config:
+        config = config.get("tool", {}).get("robotidy", {})
     return {k.replace("--", "").replace("-", "_"): v for k, v in config.items()}
 
 
 @lru_cache()
 def get_gitignore(root: Path) -> PathSpec:
     """Return a PathSpec matching gitignore content if present."""
     gitignore = root / ".gitignore"
```

### Comparing `robotframework-tidy-4.1.0/robotidy/skip.py` & `robotframework-tidy-4.2.0/robotidy/skip.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,9 +190,10 @@
         "--skip-teardown",
         "--skip-timeout",
         "--skip-template",
         "--skip-return",
         "--skip-tags",
         "--skip-comments",
         "--skip-block-comments",
+        "--skip-sections",
     ],
 }
```

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/AddMissingEnd.py` & `robotframework-tidy-4.2.0/robotidy/transformers/AddMissingEnd.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/AlignKeywordsSection.py` & `robotframework-tidy-4.2.0/robotidy/transformers/AlignKeywordsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/AlignSettingsSection.py` & `robotframework-tidy-4.2.0/robotidy/transformers/AlignSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/AlignTemplatedTestCases.py` & `robotframework-tidy-4.2.0/robotidy/transformers/AlignTemplatedTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/AlignTestCasesSection.py` & `robotframework-tidy-4.2.0/robotidy/transformers/AlignTestCasesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/AlignVariablesSection.py` & `robotframework-tidy-4.2.0/robotidy/transformers/AlignVariablesSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/DiscardEmptySections.py` & `robotframework-tidy-4.2.0/robotidy/transformers/DiscardEmptySections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/GenerateDocumentation.py` & `robotframework-tidy-4.2.0/robotidy/transformers/GenerateDocumentation.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/IndentNestedKeywords.py` & `robotframework-tidy-4.2.0/robotidy/transformers/IndentNestedKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/InlineIf.py` & `robotframework-tidy-4.2.0/robotidy/transformers/InlineIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/MergeAndOrderSections.py` & `robotframework-tidy-4.2.0/robotidy/transformers/MergeAndOrderSections.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeAssignments.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeAssignments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeComments.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeComments.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeNewLines.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeNewLines.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSectionHeaderName.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSectionHeaderName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSeparators.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSeparators.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 except ImportError:
     InlineIfHeader = None
     ReturnStatement = None
 
 from robotidy.disablers import skip_if_disabled, skip_section_if_disabled
 from robotidy.skip import Skip
 from robotidy.transformers import Transformer
+from robotidy.utils import join_comments
 
 
 class NormalizeSeparators(Transformer):
     """
     Normalize separators and indents.
 
     All separators (pipes included) are converted to fixed length of 4 spaces (configurable via global argument
@@ -28,17 +29,18 @@
             "skip_keyword_call_pattern",
             "skip_comments",
             "skip_block_comments",
             "skip_sections",
         }
     )
 
-    def __init__(self, skip: Skip = None):
+    def __init__(self, flatten_lines: bool = False, skip: Skip = None):
         super().__init__(skip=skip)
         self.indent = 0
+        self.flatten_lines = flatten_lines
         self.is_inline = False
 
     def visit_File(self, node):  # noqa
         self.indent = 0
         return self.generic_visit(node)
 
     @skip_section_if_disabled
@@ -81,41 +83,83 @@
         if node.orelse:
             self.visit(node.orelse)
         if node.end:
             self.visit_Statement(node.end)
         self.is_inline = False
         return node
 
+    @skip_if_disabled
     def visit_Documentation(self, doc):  # noqa
-        if self.skip.documentation:
+        if self.skip.documentation or self.flatten_lines:
             has_pipes = doc.tokens[0].value.startswith("|")
-            return self._handle_spaces(doc, has_pipes, only_indent=True)
+            return self.handle_spaces(doc, has_pipes, only_indent=True)
         return self.visit_Statement(doc)
 
     def visit_KeywordCall(self, keyword):  # noqa
         if self.skip.keyword_call(keyword):
             return keyword
         return self.visit_Statement(keyword)
 
+    @skip_if_disabled
     def visit_Comment(self, node):  # noqa
         if self.skip.comment(node):
             return node
-        return self.visit_Statement(node)
+        has_pipes = node.tokens[0].value.startswith("|")
+        return self.handle_spaces(node, has_pipes)
 
     def is_keyword_inside_inline_if(self, node):
         return self.is_inline and not isinstance(node, InlineIfHeader)
 
     @skip_if_disabled
     def visit_Statement(self, statement):  # noqa
         if statement is None:
             return None
         has_pipes = statement.tokens[0].value.startswith("|")
-        return self._handle_spaces(statement, has_pipes)
+        if has_pipes or not self.flatten_lines:
+            return self.handle_spaces(statement, has_pipes)
+        else:
+            return self.handle_spaces_and_flatten_lines(statement)
+
+    def handle_spaces_and_flatten_lines(self, statement):
+        """Normalize separators and flatten multiline statements to one line."""
+        add_eol, prev_sep = False, False
+        add_indent = not self.is_keyword_inside_inline_if(statement)
+        new_tokens, comments = [], []
+        for token in statement.tokens:
+            if token.type == Token.SEPARATOR:
+                if prev_sep:
+                    continue
+                prev_sep = True
+                if add_indent:
+                    token.value = self.formatting_config.indent * self.indent
+                else:
+                    token.value = self.formatting_config.separator
+            elif token.type == Token.EOL:
+                add_eol = True
+                continue
+            elif token.type == Token.CONTINUATION:
+                continue
+            elif token.type == Token.COMMENT:
+                comments.append(token)
+                continue
+            else:
+                prev_sep = False
+            new_tokens.append(token)
+            add_indent = False
+        if new_tokens and new_tokens[-1].type == Token.SEPARATOR:
+            new_tokens.pop()
+        if comments:
+            new_tokens.extend(join_comments(comments))
+        if add_eol:
+            new_tokens.append(Token(Token.EOL))
+        statement.tokens = new_tokens
+        self.generic_visit(statement)
+        return statement
 
-    def _handle_spaces(self, statement, has_pipes, only_indent=False):
+    def handle_spaces(self, statement, has_pipes, only_indent=False):
         new_tokens = []
         prev_token = None
         for line in statement.lines:
             prev_sep = False
             for index, token in enumerate(line):
                 if token.type == Token.SEPARATOR:
                     if prev_sep:
```

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeSettingName.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeSettingName.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/NormalizeTags.py` & `robotframework-tidy-4.2.0/robotidy/transformers/NormalizeTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/OrderSettings.py` & `robotframework-tidy-4.2.0/robotidy/transformers/OrderSettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/OrderSettingsSection.py` & `robotframework-tidy-4.2.0/robotidy/transformers/OrderSettingsSection.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/OrderTags.py` & `robotframework-tidy-4.2.0/robotidy/transformers/OrderTags.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/RemoveEmptySettings.py` & `robotframework-tidy-4.2.0/robotidy/transformers/RemoveEmptySettings.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/RenameKeywords.py` & `robotframework-tidy-4.2.0/robotidy/transformers/RenameKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/RenameTestCases.py` & `robotframework-tidy-4.2.0/robotidy/transformers/RenameTestCases.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/RenameVariables.py` & `robotframework-tidy-4.2.0/robotidy/transformers/RenameVariables.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,17 +353,26 @@
                 error_var.value = self.rename_value(error_var.value, variable_case="lower", is_var=True)
         return self.generic_visit(node)
 
     @skip_if_disabled
     def visit_If(self, node):  # noqa
         if node.errors:
             return node
-        for assign in node.header.get_tokens(Token.ASSIGN):
-            self.variables_scope.add_local(assign.value)
-            assign.value = self.rename_value(assign.value, variable_case="lower", is_var=False)
+        for token in node.header.data_tokens:
+            if token.type == Token.ASSIGN:
+                self.variables_scope.add_local(token.value)
+                token.value = self.rename_value(token.value, variable_case="lower", is_var=False)
+            elif token.type == Token.ARGUMENT:
+                token.value = self.rename_value(token.value, variable_case="auto", is_var=False)
+        return self.generic_visit(node)
+
+    @skip_if_disabled
+    def visit_While(self, node):  # noqa
+        for arg in node.header.get_tokens(Token.ARGUMENT):
+            arg.value = self.rename_value(arg.value, variable_case="auto", is_var=False)
         return self.generic_visit(node)
 
     def rename_value(self, value: str, variable_case: str, is_var: bool = False):
         try:
             variables = list(VariableIterator(value))
         except VariableError:  # for example ${variable which wasn't closed properly
             variables = []
```

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceBreakContinue.py` & `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceBreakContinue.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceEmptyValues.py` & `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceEmptyValues.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceReturns.py` & `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceReturns.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/ReplaceRunKeywordIf.py` & `robotframework-tidy-4.2.0/robotidy/transformers/ReplaceRunKeywordIf.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/SmartSortKeywords.py` & `robotframework-tidy-4.2.0/robotidy/transformers/SmartSortKeywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/SplitTooLongLine.py` & `robotframework-tidy-4.2.0/robotidy/transformers/SplitTooLongLine.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/Translate.py` & `robotframework-tidy-4.2.0/robotidy/transformers/Translate.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/__init__.py` & `robotframework-tidy-4.2.0/robotidy/transformers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,28 +193,32 @@
             transformer_names = [name for name, transf in self.transformers.items() if not transf.is_config_only]
             similar = similar_finder.find_similar(transf_name, transformer_names)
             raise ImportTransformerError(
                 f"Configuring transformer '{transf_name}' failed. " f"Verify if correct name was provided.{similar}"
             ) from None
 
 
+def convert_transform_config(value: str, param_name: str) -> TransformConfig:
+    force_included = param_name == "transform"
+    custom_transformer = param_name == "custom_transformers"
+    is_config = param_name == "configure"
+    return TransformConfig(
+        value, force_include=force_included, custom_transformer=custom_transformer, is_config=is_config
+    )
+
+
 class TransformConfigParameter(click.ParamType):
     """
     Click parameter that holds the name of the transformer and optional configuration.
     """
 
     name = "transform"
 
     def convert(self, value, param, ctx):
-        force_included = param.name == "transform"
-        custom_transformer = param.name == "custom_transformers"
-        is_config = param.name == "configure"
-        return TransformConfig(
-            value, force_include=force_included, custom_transformer=custom_transformer, is_config=is_config
-        )
+        return convert_transform_config(value, param.name)
 
 
 class TransformerParameter:
     def __init__(self, name, default_value):
         self.name = name
         self.value = default_value
```

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/aligners_core.py` & `robotframework-tidy-4.2.0/robotidy/transformers/aligners_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     InlineIfHeader, TryHeader = None, None
 
 from robotidy.disablers import skip_if_disabled
 from robotidy.exceptions import InvalidParameterValueError
 from robotidy.skip import Skip
 from robotidy.transformers import Transformer
-from robotidy.utils import is_blank_multiline, round_to_four
+from robotidy.utils import is_blank_multiline, join_comments, round_to_four
 
 WHITESPACE_TOKENS = frozenset({Token.SEPARATOR, Token.EOS})
 
 
 class AlignKeywordsTestsSection(Transformer):
 
     ENABLED = False
@@ -470,23 +470,14 @@
         if token.type == Token.COMMENT:
             comments.append(token)
         else:
             non_comments.append(token)
     return non_comments, comments
 
 
-def join_comments(comments):
-    tokens = []
-    separator = get_separator(2)
-    for token in comments:
-        tokens.append(separator)
-        tokens.append(token)
-    return tokens
-
-
 def align_fixed(tokens, sep_len, start_sep=False):
     """Align tokens with fixed spacing."""
     sep_token = get_separator(sep_len)
     aligned = [sep_token] if start_sep else []
     for token in tokens:
         aligned.append(token)
         aligned.append(sep_token)
```

### Comparing `robotframework-tidy-4.1.0/robotidy/transformers/run_keywords.py` & `robotframework-tidy-4.2.0/robotidy/transformers/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-tidy-4.1.0/robotidy/utils.py` & `robotframework-tidy-4.2.0/robotidy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,7 +433,16 @@
 
 def get_line_length(tokens):
     return sum(len(token.value) for token in tokens)
 
 
 def get_line_length_with_sep(tokens, sep_len: int):
     return get_line_length(tokens) + ((len(tokens) - 1) * sep_len)
+
+
+def join_comments(comments) -> List:
+    tokens = []
+    separator = Token(Token.SEPARATOR, "  ")
+    for token in comments:
+        tokens.append(separator)
+        tokens.append(token)
+    return tokens
```

### Comparing `robotframework-tidy-4.1.0/setup.py` & `robotframework-tidy-4.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,34 +38,34 @@
     classifiers=CLASSIFIERS,
     keywords="robotframework",
     packages=["robotidy"],
     include_package_data=True,
     python_requires=">=3.7",
     install_requires=[
         "robotframework>=4.0",
-        "click>=8.1.3",
-        "colorama>=0.4.3",
-        "pathspec>=0.9.0,<0.12.0",
-        "tomli>=2.0.0",
-        "rich_click==1.4",
+        "click==8.1.*",
+        "colorama>=0.4.3,<0.4.7",
+        "pathspec>=0.9.0,<0.11.2",
+        "tomli==2.0.*",
+        "rich_click>=1.4,<1.6.2",
         "jinja2>=3.0,<4.0",
     ],
     extras_require={
         "dev": [
             "coverage",
             "invoke",
             "jinja2",
             "packaging>=21.0",
-            "pyflakes==2.4.*",  #  FIXME https://github.com/klen/pylama/issues/224
+            "pyflakes>=2.4,<3.1",  #  FIXME https://github.com/klen/pylama/issues/224
             "pylama",
             "pytest",
             "pre-commit",
         ],
         "doc": [
             "sphinx",
             "furo",
             "sphinx-design",
-            "sphinx-copybutton==0.3.3",
+            "sphinx-copybutton==0.5.2",
         ],
     },
     entry_points={"console_scripts": ["robotidy=robotidy.cli:cli"]},
 )
```

