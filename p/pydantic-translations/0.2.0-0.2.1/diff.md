# Comparing `tmp/pydantic-translations-0.2.0.tar.gz` & `tmp/pydantic-translations-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-translations-0.2.0.tar", last modified: Tue Apr 18 09:37:21 2023, max compression
+gzip compressed data, was "pydantic-translations-0.2.1.tar", last modified: Wed Apr 19 10:10:39 2023, max compression
```

## Comparing `pydantic-translations-0.2.0.tar` & `pydantic-translations-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,30 @@
--rw-r--r--   0        0        0     1121 2023-04-03 10:57:30.267939 pydantic-translations-0.2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0      128 2023-03-31 09:09:46.066607 pydantic-translations-0.2.0/.gitignore
--rw-r--r--   0        0        0      325 2023-03-31 07:34:53.564133 pydantic-translations-0.2.0/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2023-03-31 07:35:20.203909 pydantic-translations-0.2.0/LICENSE
--rw-r--r--   0        0        0     2679 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/README.md
--rw-r--r--   0        0        0     3967 2023-03-31 10:15:59.804031 pydantic-translations-0.2.0/Taskfile.yml
--rw-r--r--   0        0        0    13300 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/locales/de.po
--rw-r--r--   0        0        0    13115 2023-03-31 12:39:04.197605 pydantic-translations-0.2.0/locales/en.po
--rw-r--r--   0        0        0    13520 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/locales/es.po
--rw-r--r--   0        0        0    13769 2023-04-18 09:37:06.902758 pydantic-translations-0.2.0/locales/fr.po
--rw-r--r--   0        0        0    13470 2023-04-18 09:37:06.906758 pydantic-translations-0.2.0/locales/it.po
--rw-r--r--   0        0        0    13007 2023-04-18 09:37:06.906758 pydantic-translations-0.2.0/locales/nl.po
--rw-r--r--   0        0        0    14950 2023-04-03 07:03:56.036022 pydantic-translations-0.2.0/locales/ru.po
--rw-r--r--   0        0        0      126 2023-04-18 09:37:06.906758 pydantic-translations-0.2.0/pydantic_translations/__init__.py
--rw-r--r--   0        0        0      136 2023-03-31 08:42:52.417332 pydantic-translations-0.2.0/pydantic_translations/_constants.py
--rw-r--r--   0        0        0     9016 2023-03-31 10:10:09.219762 pydantic-translations-0.2.0/pydantic_translations/_messages.py
--rw-r--r--   0        0        0     4868 2023-03-31 12:50:11.309343 pydantic-translations-0.2.0/pydantic_translations/_translator.py
--rw-r--r--   0        0        0     1701 2023-03-31 09:09:16.931060 pydantic-translations-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-31 07:34:31.548319 pydantic-translations-0.2.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-30 11:42:57.498741 pydantic-translations-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2126 2023-03-31 07:43:14.475910 pydantic-translations-0.2.0/tests/test_messages.py
--rw-r--r--   0        0        0     1464 2023-03-31 10:12:59.705748 pydantic-translations-0.2.0/tests/test_translate.py
--rw-r--r--   0        0        0     3682 1970-01-01 00:00:00.000000 pydantic-translations-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-04-03 10:57:30.267939 pydantic-translations-0.2.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/.gitignore
+-rw-r--r--   0        0        0      325 2023-03-31 07:34:53.564133 pydantic-translations-0.2.1/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2023-03-31 07:35:20.203909 pydantic-translations-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2679 2023-04-18 09:37:06.902758 pydantic-translations-0.2.1/README.md
+-rw-r--r--   0        0        0     3967 2023-03-31 10:15:59.804031 pydantic-translations-0.2.1/Taskfile.yml
+-rw-r--r--   0        0        0    13300 2023-04-18 09:37:06.902758 pydantic-translations-0.2.1/locales/de.po
+-rw-r--r--   0        0        0    13115 2023-03-31 12:39:04.197605 pydantic-translations-0.2.1/locales/en.po
+-rw-r--r--   0        0        0    13520 2023-04-18 09:37:06.902758 pydantic-translations-0.2.1/locales/es.po
+-rw-r--r--   0        0        0    13769 2023-04-18 09:37:06.902758 pydantic-translations-0.2.1/locales/fr.po
+-rw-r--r--   0        0        0    13470 2023-04-18 09:37:06.906758 pydantic-translations-0.2.1/locales/it.po
+-rw-r--r--   0        0        0    13007 2023-04-18 09:37:06.906758 pydantic-translations-0.2.1/locales/nl.po
+-rw-r--r--   0        0        0    14950 2023-04-03 07:03:56.036022 pydantic-translations-0.2.1/locales/ru.po
+-rw-r--r--   0        0        0      126 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/__init__.py
+-rw-r--r--   0        0        0      136 2023-03-31 08:42:52.417332 pydantic-translations-0.2.1/pydantic_translations/_constants.py
+-rw-r--r--   0        0        0     9016 2023-03-31 10:10:09.219762 pydantic-translations-0.2.1/pydantic_translations/_messages.py
+-rw-r--r--   0        0        0     4868 2023-03-31 12:50:11.309343 pydantic-translations-0.2.1/pydantic_translations/_translator.py
+-rw-r--r--   0        0        0     8772 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/locales/de.mo
+-rw-r--r--   0        0        0     8517 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/locales/en.mo
+-rw-r--r--   0        0        0     8984 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/locales/es.mo
+-rw-r--r--   0        0        0     9233 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/locales/fr.mo
+-rw-r--r--   0        0        0     8932 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/locales/it.mo
+-rw-r--r--   0        0        0     8471 2023-04-19 10:10:33.727516 pydantic-translations-0.2.1/pydantic_translations/locales/nl.mo
+-rw-r--r--   0        0        0     9194 2023-04-19 10:10:33.731516 pydantic-translations-0.2.1/pydantic_translations/locales/ru.mo
+-rw-r--r--   0        0        0     1701 2023-04-19 10:07:07.062436 pydantic-translations-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-31 07:34:31.548319 pydantic-translations-0.2.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-30 11:42:57.498741 pydantic-translations-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2126 2023-03-31 07:43:14.475910 pydantic-translations-0.2.1/tests/test_messages.py
+-rw-r--r--   0        0        0     1464 2023-03-31 10:12:59.705748 pydantic-translations-0.2.1/tests/test_translate.py
+-rw-r--r--   0        0        0     3682 1970-01-01 00:00:00.000000 pydantic-translations-0.2.1/PKG-INFO
```

### Comparing `pydantic-translations-0.2.0/.github/workflows/main.yml` & `pydantic-translations-0.2.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/LICENSE` & `pydantic-translations-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/README.md` & `pydantic-translations-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/Taskfile.yml` & `pydantic-translations-0.2.1/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/de.po` & `pydantic-translations-0.2.1/locales/de.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/en.po` & `pydantic-translations-0.2.1/locales/en.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/es.po` & `pydantic-translations-0.2.1/locales/es.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/fr.po` & `pydantic-translations-0.2.1/locales/fr.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/it.po` & `pydantic-translations-0.2.1/locales/it.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/nl.po` & `pydantic-translations-0.2.1/locales/nl.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/locales/ru.po` & `pydantic-translations-0.2.1/locales/ru.po`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/pydantic_translations/_messages.py` & `pydantic-translations-0.2.1/pydantic_translations/_messages.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/pydantic_translations/_translator.py` & `pydantic-translations-0.2.1/pydantic_translations/_translator.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/pyproject.toml` & `pydantic-translations-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/tests/test_messages.py` & `pydantic-translations-0.2.1/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/tests/test_translate.py` & `pydantic-translations-0.2.1/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `pydantic-translations-0.2.0/PKG-INFO` & `pydantic-translations-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-translations
-Version: 0.2.0
+Version: 0.2.1
 Summary: Translations for pydantic errors.
 Keywords: mypy,typing,annotations,type annotations
 Author-email: Gram <git@orsinium.dev>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

