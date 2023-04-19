# Comparing `tmp/pdb-toolkit-0.3.tar.gz` & `tmp/pdb-toolkit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb-toolkit-0.3.tar", last modified: Wed Apr 19 14:15:40 2023, max compression
+gzip compressed data, was "pdb-toolkit-0.3.1.tar", last modified: Wed Apr 19 14:54:36 2023, max compression
```

## Comparing `pdb-toolkit-0.3.tar` & `pdb-toolkit-0.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1064 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/LICENSE
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      400 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/PKG-INFO
--rw-rw-r--   0 raouf     (1000) raouf     (1000)    11323 2023-04-19 14:01:55.000000 pdb-toolkit-0.3/README.md
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.504857 pdb-toolkit-0.3/pdb_toolkit/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)        0 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1190 2023-04-14 09:08:12.000000 pdb-toolkit-0.3/pdb_toolkit/constants.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit/editor/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      241 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1949 2023-04-14 14:54:32.000000 pdb-toolkit-0.3/pdb_toolkit/editor/fix_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      922 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/keep_only_atoms.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      944 2023-04-17 13:21:20.000000 pdb-toolkit-0.3/pdb_toolkit/editor/protonate_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1976 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/renumber_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      857 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/sort_atoms.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      742 2023-04-17 09:44:44.000000 pdb-toolkit-0.3/pdb_toolkit/editor/unprotonate_pdb.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit/generic/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      201 2023-04-17 15:58:54.000000 pdb-toolkit-0.3/pdb_toolkit/generic/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1452 2023-04-18 14:52:03.000000 pdb-toolkit-0.3/pdb_toolkit/generic/align.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      703 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/generic/concat_pdbs.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2602 2023-04-19 08:53:47.000000 pdb-toolkit-0.3/pdb_toolkit/generic/download_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2557 2023-04-18 12:27:11.000000 pdb-toolkit-0.3/pdb_toolkit/generic/extract_chains_from_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1096 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/generic/split_chains.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit/parser/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      282 2023-04-19 10:41:27.000000 pdb-toolkit-0.3/pdb_toolkit/parser/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1991 2023-04-18 09:20:44.000000 pdb-toolkit-0.3/pdb_toolkit/parser/get_atoms_residues.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1101 2023-04-18 08:36:06.000000 pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_centroid.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2514 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_sequence.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1661 2023-04-14 09:07:20.000000 pdb-toolkit-0.3/pdb_toolkit/parser/split_residues_surface_boundary_core.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2814 2023-04-19 10:41:27.000000 pdb-toolkit-0.3/pdb_toolkit/parser/steric_clashes.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit.egg-info/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      400 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      951 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)        1 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)        5 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/requires.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)       12 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)       38 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/setup.cfg
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      667 2023-04-19 14:15:26.000000 pdb-toolkit-0.3/setup.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1064 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/LICENSE
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      402 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/PKG-INFO
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)    11323 2023-04-19 14:01:55.000000 pdb-toolkit-0.3.1/README.md
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.713484 pdb-toolkit-0.3.1/pdb_toolkit/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)        0 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1190 2023-04-14 09:08:12.000000 pdb-toolkit-0.3.1/pdb_toolkit/constants.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.717484 pdb-toolkit-0.3.1/pdb_toolkit/editor/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      241 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1949 2023-04-14 14:54:32.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/fix_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      922 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/keep_only_atoms.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      944 2023-04-17 13:21:20.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/protonate_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1976 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/renumber_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      857 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/sort_atoms.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      742 2023-04-17 09:44:44.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/unprotonate_pdb.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.721484 pdb-toolkit-0.3.1/pdb_toolkit/generic/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      201 2023-04-17 15:58:54.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1452 2023-04-18 14:52:03.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/align.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      703 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/concat_pdbs.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2602 2023-04-19 08:53:47.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/download_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2557 2023-04-18 12:27:11.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/extract_chains_from_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1096 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/split_chains.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/pdb_toolkit/parser/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      282 2023-04-19 10:41:27.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1991 2023-04-18 09:20:44.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/get_atoms_residues.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1101 2023-04-18 08:36:06.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_centroid.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2514 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_sequence.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1661 2023-04-14 09:07:20.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/split_residues_surface_boundary_core.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2814 2023-04-19 10:41:27.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/steric_clashes.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.717484 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      402 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      951 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)        1 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)        5 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)       12 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)       38 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/setup.cfg
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      669 2023-04-19 14:48:09.000000 pdb-toolkit-0.3.1/setup.py
```

### Comparing `pdb-toolkit-0.3/LICENSE` & `pdb-toolkit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/README.md` & `pdb-toolkit-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/constants.py` & `pdb-toolkit-0.3.1/pdb_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/editor/fix_pdb.py` & `pdb-toolkit-0.3.1/pdb_toolkit/editor/fix_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/editor/keep_only_atoms.py` & `pdb-toolkit-0.3.1/pdb_toolkit/editor/keep_only_atoms.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/editor/protonate_pdb.py` & `pdb-toolkit-0.3.1/pdb_toolkit/editor/protonate_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/editor/renumber_pdb.py` & `pdb-toolkit-0.3.1/pdb_toolkit/editor/renumber_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/editor/sort_atoms.py` & `pdb-toolkit-0.3.1/pdb_toolkit/editor/sort_atoms.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/editor/unprotonate_pdb.py` & `pdb-toolkit-0.3.1/pdb_toolkit/editor/unprotonate_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/generic/align.py` & `pdb-toolkit-0.3.1/pdb_toolkit/generic/align.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/generic/concat_pdbs.py` & `pdb-toolkit-0.3.1/pdb_toolkit/generic/concat_pdbs.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/generic/download_pdb.py` & `pdb-toolkit-0.3.1/pdb_toolkit/generic/download_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/generic/extract_chains_from_pdb.py` & `pdb-toolkit-0.3.1/pdb_toolkit/generic/extract_chains_from_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/generic/split_chains.py` & `pdb-toolkit-0.3.1/pdb_toolkit/generic/split_chains.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/parser/get_atoms_residues.py` & `pdb-toolkit-0.3.1/pdb_toolkit/parser/get_atoms_residues.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_centroid.py` & `pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_centroid.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_sequence.py` & `pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_sequence.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/parser/split_residues_surface_boundary_core.py` & `pdb-toolkit-0.3.1/pdb_toolkit/parser/split_residues_surface_boundary_core.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit/parser/steric_clashes.py` & `pdb-toolkit-0.3.1/pdb_toolkit/parser/steric_clashes.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/pdb_toolkit.egg-info/SOURCES.txt` & `pdb-toolkit-0.3.1/pdb_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3/setup.py` & `pdb-toolkit-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of your README file
 with open('README.md', encoding='utf-8') as f:
     description = f.read()
 
 setup(
     name='pdb-toolkit',
-    version='0.3',
+    version='0.3.1',
     packages=find_packages(),
     url='https://github.com/raoufkeskes/pdb_toolkit',
     license='MIT Licence',
     author='raouf-ks',
     author_email='raouf.keskes@mabsilico.com',
     description=description,
     python_requires='>=3.6',
```

