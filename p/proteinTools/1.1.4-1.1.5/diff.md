# Comparing `tmp/proteinTools-1.1.4.tar.gz` & `tmp/proteinTools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.1.4.tar", last modified: Wed Apr 19 03:38:45 2023, max compression
+gzip compressed data, was "proteinTools-1.1.5.tar", last modified: Wed Apr 19 19:52:38 2023, max compression
```

## Comparing `proteinTools-1.1.4.tar` & `proteinTools-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 03:38:45.498921 proteinTools-1.1.4/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.4/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 03:38:45.490116 proteinTools-1.1.4/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.4/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 03:38:45.338629 proteinTools-1.1.4/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    49246 2023-04-19 03:32:18.000000 proteinTools-1.1.4/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.4/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 03:38:45.442349 proteinTools-1.1.4/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-19 03:38:45.000000 proteinTools-1.1.4/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-19 03:38:45.507622 proteinTools-1.1.4/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-19 03:24:03.000000 proteinTools-1.1.4/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 19:52:38.462147 proteinTools-1.1.5/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.1.5/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 19:52:38.458527 proteinTools-1.1.5/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.1.5/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 19:52:38.389066 proteinTools-1.1.5/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    50302 2023-04-19 19:46:57.000000 proteinTools-1.1.5/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.1.5/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-19 19:52:38.443274 proteinTools-1.1.5/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-19 19:52:38.000000 proteinTools-1.1.5/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-19 19:52:38.000000 proteinTools-1.1.5/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-19 19:52:38.000000 proteinTools-1.1.5/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-19 19:52:38.000000 proteinTools-1.1.5/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-19 19:52:38.000000 proteinTools-1.1.5/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-19 19:52:38.467191 proteinTools-1.1.5/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-19 19:52:31.000000 proteinTools-1.1.5/setup.py
```

### Comparing `proteinTools-1.1.4/LICENSE` & `proteinTools-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.1.4/proteinTools/PT.py` & `proteinTools-1.1.5/proteinTools/PT.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from chembl_webresource_client.new_client import new_client
 import re
 mg = mygene.MyGeneInfo()
 
 #Utility dictionaries containing element/mass mappings as well as FASTA mapping
 FASTAdict = {'ALA':'A', 'ALX':'B', 'CYS': 'C', 'ASP' : 'D', 'GLU': 'E', 'PHE': 'F', 'GLY': 'G', 'HIS': 'H', 'ILE': 'I', 'LYS':'K', 'LEU':'L', 'MET': 'M', 'ASN':'N', 'PRO':'P', 'GLN': 'Q', 'ARG':'R', 'SER': 'S', 'THR': 'T', 'VAL': 'V', 'TRP': 'W', 'UNK':'X', 'TYR':'Y', 'GLX':'Z'}
 atom_dict = {'H':1.01, 'C':12.01, 'O':16.00, 'N':14.01, 'P':30.97, 'F':18.998, 'FE':55.845, 'S':32.06, 'B':10.81, 'K':39.1, 'I':126.904, 'BR':79.904, 'CL':35.453, 'CA':40.08, 'NA':22.99, 'MG':24.305, 'AL':26.98, 'CR':51.996, 'NE':20.179, 'BE':9.01, 'FE':55.847, 'CO':58.933,'AG':107.868, 'CD':112.41, 'NI':58.693, 'ZN':65.39, 'BE':9.0122, 'IN':114.818, 'SI':28.085, 'SC':44.956, 'TI':47.867, 'V':50.941, 'MN':54.938, 'CU':63.546, 'GA':59.723, 'GE':72.64, 'SE':78.96, 'KR':83.8, 'ZR':91.224, 'NB':92.906, 'PD':106.42, 'SN':118.71, 'SB':121.76, 'XE':131.293, 'BA':137.327, 'LA':138.91, 'LI':6.941, 'HG':200.59, 'PB':207.2, 'BI':208.98, 'PO':209, 'TI':204.3833, 'AU':196.9665, 'IR':192.217, 'PT':195.078, 'RE':186.207, 'W':183.84, 'TA':180.948, 'YB':173.04, 'EU':151.964, 'ND':144.25, 'CE':140.116, 'TH':232.04, 'U':238.029, 'PU':244, 'FR':223, 'PA':231.04, 'HO':164.93, 'SM':150.36, 'PR':140.908, 'TE':127.6, 'TC':98, 'Y':88.906}
+element_radii = {'H': 0.25, 'HE': 0.31, 'LI': 1.45, 'BE': 1.05, 'B': 0.85, 'C': 0.70, 'N': 0.65, 'O': 0.60, 'F': 0.50, 'NE': 0.38, 'NA': 1.80, 'MG': 1.50, 'AL': 1.25, 'SI': 1.10, 'P': 1.00, 'S': 1.00, 'CL': 1.00, 'AR': 0.71, 'K': 2.20, 'CA': 1.80, 'SC': 1.60, 'TI': 1.40, 'V': 1.35, 'CR': 1.40, 'MN': 1.40, 'FE': 1.40, 'CO': 1.35, 'NI': 1.35, 'CU': 1.35, 'ZN': 1.35, 'GA': 1.30, 'GE': 1.25, 'AS': 1.15, 'SE': 1.15, 'BR': 1.15, 'KR': 1.03, 'RB': 2.35, 'SR': 2.00, 'Y': 1.80, 'ZR': 1.55, 'NB': 1.45, 'MO': 1.45, 'TC': 1.35, 'RU': 1.30, 'RH': 1.35, 'PD': 1.40, 'AG': 1.60, 'CD': 1.55, 'IN': 1.45, 'SN': 1.40, 'SB': 1.40, 'TE': 1.35, 'I': 1.35, 'XE': 1.30, 'CS': 2.45, 'BA': 2.15, 'LA': 2.00, 'CE': 2.00, 'PR': 2.00, 'ND': 2.00, 'PM': 2.00, 'SM': 2.00, 'EU': 2.00, 'GD': 2.00, 'TB': 2.00, 'DY': 2.00, 'HO': 2.00, 'ER': 2.00, 'TM': 2.00, 'YB': 2.00, 'LU': 1.80, 'HF': 1.55, 'TA': 1.45, 'W': 1.35, 'RE': 1.35, 'OS': 1.30, 'IR': 1.35, 'PT': 1.40, 'AU': 1.60, 'HG': 1.55, 'TL': 1.45, 'PB': 1.45, 'BI': 1.50, 'TH': 2.00, 'PA': 2.00, 'U': 2.00}
+
 atom_keys = atom_dict.keys()
 
 class atom:
     """
     Atom class
 
     This class contains the essential parameters of an individual atom in a protein structural file, including the coordinates, element, atomic mass, parent residue, and line data.
@@ -36,15 +38,16 @@
         self.element = element
         self.x = x
         self.y = y
         self.z = z
         self.residue = residue
         self.data = data
         self.mass = atom_dict[self.element]
-             
+        self.radius = element_radii[self.element]
+        
 class residue:
     """
     Residue class
     
     This class contains the essential parameters of an individual residue in a protein structural file, including the child atoms, protein sidechain, residue index, and type of amino acid.
     """
     def __init__(self, amino_acid, index, chain):
@@ -1119,10 +1122,9 @@
 '''
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('1E66')
     p.download()
     for res in p.residue_list:
         for atom in res.atoms:
-            print(atom.parent_residue.structure)
-            break
-'''
+            print(atom.radius)
+'''
```

### Comparing `proteinTools-1.1.4/setup.py` & `proteinTools-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.1.4",
+    version = "1.1.5",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

