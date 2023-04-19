# Comparing `tmp/PRauto-0.112.tar.gz` & `tmp/PRauto-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PRauto-0.112.tar", last modified: Tue Apr 18 12:06:16 2023, max compression
+gzip compressed data, was "PRauto-0.12.tar", last modified: Wed Apr 19 01:55:00 2023, max compression
```

## Comparing `PRauto-0.112.tar` & `PRauto-0.12.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.576630 PRauto-0.112/
--rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.112/LICENSE
--rw-rw-rw-   0        0        0      365 2023-04-18 12:06:16.575629 PRauto-0.112/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.564630 PRauto-0.112/PRauto.egg-info/
--rw-rw-rw-   0        0        0      365 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 12:06:16.000000 PRauto-0.112/PRauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 06:21:00.000000 PRauto-0.112/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.568630 PRauto-0.112/prauto/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.112/prauto/__init__.py
--rw-rw-rw-   0        0        0     1790 2023-04-18 12:03:28.000000 PRauto-0.112/prauto/__main__.py
--rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.112/prauto/get_preprocess.py
-drwxrwxrwx   0        0        0        0 2023-04-18 12:06:16.573629 PRauto-0.112/prauto/retriever/
--rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.112/prauto/retriever/__init__.py
--rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.112/prauto/retriever/get_fasta.py
--rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.112/prauto/retriever/get_ligand.py
--rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.112/prauto/retriever/get_pdb.py
--rw-rw-rw-   0        0        0       42 2023-04-18 12:06:16.576630 PRauto-0.112/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-04-18 12:04:08.000000 PRauto-0.112/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.071836 PRauto-0.12/
+-rw-rw-rw-   0        0        0     1098 2023-04-18 06:21:00.000000 PRauto-0.12/LICENSE
+-rw-rw-rw-   0        0        0      364 2023-04-19 01:55:00.071319 PRauto-0.12/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.049898 PRauto-0.12/PRauto.egg-info/
+-rw-rw-rw-   0        0        0      364 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-19 01:54:59.000000 PRauto-0.12/PRauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 06:21:00.000000 PRauto-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.051903 PRauto-0.12/prauto/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:34:40.000000 PRauto-0.12/prauto/__init__.py
+-rw-rw-rw-   0        0        0     2279 2023-04-19 01:41:22.000000 PRauto-0.12/prauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.055314 PRauto-0.12/prauto/prepauto/
+-rw-rw-rw-   0        0        0        0 2023-04-19 01:47:21.000000 PRauto-0.12/prauto/prepauto/__init__.py
+-rw-rw-rw-   0        0        0    12324 2023-04-18 10:56:42.000000 PRauto-0.12/prauto/prepauto/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 01:55:00.069318 PRauto-0.12/prauto/retriever/
+-rw-rw-rw-   0        0        0        0 2023-04-17 00:31:39.000000 PRauto-0.12/prauto/retriever/__init__.py
+-rw-rw-rw-   0        0        0     4848 2023-04-18 07:55:44.000000 PRauto-0.12/prauto/retriever/get_fasta.py
+-rw-rw-rw-   0        0        0     2749 2023-04-18 10:56:42.000000 PRauto-0.12/prauto/retriever/get_ligand.py
+-rw-rw-rw-   0        0        0     4274 2023-04-18 10:56:42.000000 PRauto-0.12/prauto/retriever/get_pdb.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 01:55:00.071836 PRauto-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2023-04-19 01:07:08.000000 PRauto-0.12/setup.py
```

### Comparing `PRauto-0.112/LICENSE` & `PRauto-0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `PRauto-0.112/prauto/__main__.py` & `PRauto-0.12/prauto/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,34 +6,40 @@
 from tqdm.auto import tqdm
 from tkinter import Tk
 from tkinter import filedialog
 
 root = Tk()
 root.withdraw()
 
-mult = '\n' * 5
+mult = '\n' * 3
 global search_key
 
 
 def main():
     global search_key
     target_dir = filedialog.askdirectory(title='Select a directory to work with')
     os.chdir(target_dir)
-    print(f"""{mult}
+    print(f'Step1: Retrieve FASTA files{mult}')
+    print(f"""
     
-    ########################## Search with Protein Name and Gene Name ##########################
+########################################################################################################
 
-    input 1  Protein Name subtype : ex. 5-hydroxytryptamine receptor 2A
-    input 2  Gene Name : ex. HTR2A
-                                                                                            """)
+ > Please input [ Protein Name ] and [ Gene Name ] of your target.
 
-    print(f'Step1: Retrieve FASTA files{mult}')
 
-    search_key = input('input Protein Name with subtype: ').replace(' ', '%20')
-    gene_name = input('input Gene Name with subtype: ').replace(' ', '%20')
+    input 1  Protein Name with subtype :  ex. 5-hydroxytryptamine receptor 2A   
+                                                                             / Search term(uniprot API)
+                                                                               
+    input 2  Gene Name :  ex. HTR2A                                 
+                                     / Filtering term for Integrity of data 
+                                                  
+#########################################################################################################
+                                                                                            """)
+    search_key = input('input 1  Protein Name with subtype :')
+    gene_name = input('input 2  Gene Name :')
     dir_name = input('input Directory Name for FASTA file: ')
     fasta_file_path = download_fasta(search_key, dir_name)
     fasta_file_path = remove_outlier(search_key,gene_name,fasta_file_path)
     pdb_dir = os.path.dirname(fasta_file_path)
 
     print(f'Step2: Retrieve PDB files{mult}')
     accessions_list = extract_accessions(fasta_file_path)
```

### Comparing `PRauto-0.112/prauto/get_preprocess.py` & `PRauto-0.12/prauto/prepauto/__main__.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.112/prauto/retriever/get_fasta.py` & `PRauto-0.12/prauto/retriever/get_fasta.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.112/prauto/retriever/get_ligand.py` & `PRauto-0.12/prauto/retriever/get_ligand.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.112/prauto/retriever/get_pdb.py` & `PRauto-0.12/prauto/retriever/get_pdb.py`

 * *Files identical despite different names*

### Comparing `PRauto-0.112/setup.py` & `PRauto-0.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import setup, find_packages
 import setuptools
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(name='PRauto',
-        version = '0.112',
+        version = '0.12',
         packages = find_packages(include=['prauto','prauto.*']),
         url = 'https://github.com/KimJisanER/PRauto',
         license = 'MIT license',
         author = 'Ji San Kim',
         author_email = 'jisan1233@gmail.com',
         keywords = 'PDB, FASTA, sdf, Automation',
         description = """
```

