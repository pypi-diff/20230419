# Comparing `tmp/proteinTools-1.1.3.tar.gz` & `tmp/proteinTools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.1.3.tar", last modified: Tue Apr 18 17:50:58 2023, max compression
+gzip compressed data, was "proteinTools-1.1.4.tar", last modified: Wed Apr 19 03:38:45 2023, max compression
```

## Comparing `proteinTools-1.1.3.tar` & `proteinTools-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 17:50:58.445222 proteinTools-1.1.3/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.3/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 17:50:58.437785 proteinTools-1.1.3/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.3/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 17:50:58.353604 proteinTools-1.1.3/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    49003 2023-04-18 17:50:02.000000 proteinTools-1.1.3/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.3/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-18 17:50:58.421396 proteinTools-1.1.3/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-18 17:50:58.000000 proteinTools-1.1.3/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-18 17:50:58.457193 proteinTools-1.1.3/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      523 2023-04-18 17:50:11.000000 proteinTools-1.1.3/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 03:38:45.498921 proteinTools-1.1.4/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.4/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 03:38:45.490116 proteinTools-1.1.4/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.4/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 03:38:45.338629 proteinTools-1.1.4/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    49246 2023-04-19 03:32:18.000000 proteinTools-1.1.4/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.4/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 03:38:45.442349 proteinTools-1.1.4/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-19 03:38:45.507622 proteinTools-1.1.4/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-19 03:24:03.000000 proteinTools-1.1.4/setup.py
```

### Comparing `proteinTools-1.1.3/LICENSE` & `proteinTools-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.1.3/proteinTools/PT.py` & `proteinTools-1.1.4/proteinTools/PT.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,14 +489,19 @@
                 for count, res in enumerate(self.residue_list):
                     if count + 1 in sheet:
                         res.structure = 'SHEET'
                     elif count + 1 in helix:
                         res.structure = 'HELIX'
                     else:
                         res.structure = 'UNSTRUCTURED'
+                    for resatom in res.atoms:
+                        resatom.parent_residue = res
+            else:
+                for resatom in res.atoms:
+                    resatom.parent_residue = res
                         
         else:
             with open(self.protein + '.cif', 'r') as f:
                 data = f.readlines()
             
             #Obtains chains from protein file
             numbers, letters, curr_num = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9'], ['A', 'B',' C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z'], 1
@@ -1104,18 +1109,20 @@
                 pass
             return results
         except:
             print(traceback.format_exc())
             return 'N/A'
     '''
     TODO
-    - Add secondary structure prediction to residues (use s4pred?)
     - Add more ID conversions
     '''
 
-
+'''
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('1E66')
-    lig = ligand('C1=CC=C(C=C1)C=O')
-    lig.download()
- 
+    p.download()
+    for res in p.residue_list:
+        for atom in res.atoms:
+            print(atom.parent_residue.structure)
+            break
+'''
```

### Comparing `proteinTools-1.1.3/setup.py` & `proteinTools-1.1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.1.3",
+    version = "1.1.4",
     author = "Christian de Frondeville",
-    description = "Lightweight package which simplifies interacting with proteins.",
+    description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

