# Comparing `tmp/study_id_generator-0.0.4.tar.gz` & `tmp/study_id_generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "study_id_generator-0.0.4.tar", last modified: Wed Apr 19 12:49:40 2023, max compression
+gzip compressed data, was "study_id_generator-0.0.5.tar", last modified: Wed Apr 19 13:17:32 2023, max compression
```

## Comparing `study_id_generator-0.0.4.tar` & `study_id_generator-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.330704 study_id_generator-0.0.4/
--rw-rw-rw-   0        0        0     1380 2023-04-19 12:49:40.329706 study_id_generator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.4/README.md
--rw-rw-rw-   0        0        0      873 2023-04-19 12:07:41.000000 study_id_generator-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 12:49:40.330704 study_id_generator-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.311765 study_id_generator-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.318742 study_id_generator-0.0.4/src/study_id_generator/
--rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.4/src/study_id_generator/__init__.py
--rw-rw-rw-   0        0        0     6117 2023-04-19 12:44:02.000000 study_id_generator-0.0.4/src/study_id_generator/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:49:40.327713 study_id_generator-0.0.4/src/study_id_generator.egg-info/
--rw-rw-rw-   0        0        0     1380 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-19 12:49:40.000000 study_id_generator-0.0.4/src/study_id_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 13:17:32.356165 study_id_generator-0.0.5/
+-rw-rw-rw-   0        0        0     1380 2023-04-19 13:17:32.355168 study_id_generator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.5/README.md
+-rw-rw-rw-   0        0        0      873 2023-04-19 13:02:39.000000 study_id_generator-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 13:17:32.357163 study_id_generator-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 13:17:32.338227 study_id_generator-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 13:17:32.343209 study_id_generator-0.0.5/src/study_id_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.5/src/study_id_generator/__init__.py
+-rw-rw-rw-   0        0        0     6117 2023-04-19 13:00:54.000000 study_id_generator-0.0.5/src/study_id_generator/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:17:32.354172 study_id_generator-0.0.5/src/study_id_generator.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-04-19 13:17:32.000000 study_id_generator-0.0.5/src/study_id_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-19 13:17:32.000000 study_id_generator-0.0.5/src/study_id_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:17:32.000000 study_id_generator-0.0.5/src/study_id_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 13:17:32.000000 study_id_generator-0.0.5/src/study_id_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-19 13:17:32.000000 study_id_generator-0.0.5/src/study_id_generator.egg-info/top_level.txt
```

### Comparing `study_id_generator-0.0.4/PKG-INFO` & `study_id_generator-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: study_id_generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Study ID Generator.
 Author-email: Sushant Obeja <sobeja@umich.edu>, Adam Patterson <adpatter@umich.edu>
 Project-URL: Homepage, https://git.umms.med.umich.edu/feldman-lab/study_id_generator
 Project-URL: Bug Tracker, https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `study_id_generator-0.0.4/README.md` & `study_id_generator-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `study_id_generator-0.0.4/pyproject.toml` & `study_id_generator-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "study_id_generator"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name="Sushant Obeja", email="sobeja@umich.edu" },
     { name="Adam Patterson", email="adpatter@umich.edu" },
 ]
 description = "Study ID Generator."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `study_id_generator-0.0.4/src/study_id_generator/__main__.py` & `study_id_generator-0.0.5/src/study_id_generator/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,20 +97,20 @@
 
                 df = df.loc[df[section['FIELD_NAME']].str.contains(section['ID_REGEX']) == True]
 
                 ids.append(df[section['FIELD_NAME']])
 
             ds = pd.concat(ids)
 
-            ds = ds.drop_duplicates()
-
             df = ds.to_frame(name='id')  # type: ignore
 
             df['id'] = df['id'].astype(str).str.pad(self._ID_WIDTH, side='left', fillchar=self._ID_FILLCHAR)
 
+            df = df.drop_duplicates()
+
             id_variants = pd.Series(range(self._MIN_ID, self._MAX_ID))
 
             id_variants = id_variants.astype(str).str.pad(self._ID_WIDTH, side='left', fillchar=self._ID_FILLCHAR)
 
             id_variants = id_variants.loc[~id_variants.isin(df['id'])]
 
             id_variants = id_variants.sample(frac=self._SAMPLE_FRAC)
```

### Comparing `study_id_generator-0.0.4/src/study_id_generator.egg-info/PKG-INFO` & `study_id_generator-0.0.5/src/study_id_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: study-id-generator
-Version: 0.0.4
+Version: 0.0.5
 Summary: Study ID Generator.
 Author-email: Sushant Obeja <sobeja@umich.edu>, Adam Patterson <adpatter@umich.edu>
 Project-URL: Homepage, https://git.umms.med.umich.edu/feldman-lab/study_id_generator
 Project-URL: Bug Tracker, https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

