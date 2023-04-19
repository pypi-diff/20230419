# Comparing `tmp/pdb_toolkit-0.2.tar.gz` & `tmp/pdb-toolkit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb_toolkit-0.2.tar", last modified: Tue Dec 20 10:04:05 2022, max compression
+gzip compressed data, was "pdb-toolkit-0.3.tar", last modified: Wed Apr 19 14:15:40 2023, max compression
```

## Comparing `pdb_toolkit-0.2.tar` & `pdb-toolkit-0.3.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.390312 pdb_toolkit-0.2/
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1064 2022-09-28 10:19:55.000000 pdb_toolkit-0.2/LICENSE
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      420 2022-12-20 10:04:05.390312 pdb_toolkit-0.2/PKG-INFO
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     5657 2022-12-01 14:43:47.000000 pdb_toolkit-0.2/README.md
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)       38 2022-12-20 10:04:05.390312 pdb_toolkit-0.2/setup.cfg
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      691 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/setup.py
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.386312 pdb_toolkit-0.2/src/
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.386312 pdb_toolkit-0.2/src/pdb_toolkit/
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-09-13 15:49:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/__init__.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      727 2022-09-07 12:54:57.000000 pdb_toolkit-0.2/src/pdb_toolkit/constants.py
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.390312 pdb_toolkit-0.2/src/pdb_toolkit/editor/
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      241 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/__init__.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1912 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/fix_pdb.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      922 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/keep_only_atoms.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1072 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/protonate_pdb.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1976 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/renumber_pdb.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      857 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/sort_atoms.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      820 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/editor/unprotonate_pdb.py
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.390312 pdb_toolkit-0.2/src/pdb_toolkit/generic/
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      162 2022-09-13 14:07:50.000000 pdb_toolkit-0.2/src/pdb_toolkit/generic/__init__.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1467 2022-09-26 08:45:05.000000 pdb_toolkit-0.2/src/pdb_toolkit/generic/align.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      703 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/generic/concat_pdbs.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2286 2022-09-22 15:12:16.000000 pdb_toolkit-0.2/src/pdb_toolkit/generic/download_pdb.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2428 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/generic/extract_chains_from_pdb.py
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.390312 pdb_toolkit-0.2/src/pdb_toolkit/parser/
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      319 2022-10-06 15:54:27.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/__init__.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1967 2022-09-22 15:26:22.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/get_atoms_residues.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1100 2022-10-06 15:54:19.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/get_pdb_centroid.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2514 2022-10-24 13:56:41.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/get_pdb_sequence.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1096 2022-09-22 16:23:15.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/split_chains.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2019 2022-09-09 14:41:18.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/split_residues_surface_boundary_core.py
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2810 2022-09-28 10:09:04.000000 pdb_toolkit-0.2/src/pdb_toolkit/parser/steric_clashes.py
-drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2022-12-20 10:04:05.386312 pdb_toolkit-0.2/src/pdb_toolkit.egg-info/
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      420 2022-12-20 10:04:05.000000 pdb_toolkit-0.2/src/pdb_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1054 2022-12-20 10:04:05.000000 pdb_toolkit-0.2/src/pdb_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)        1 2022-12-20 10:04:05.000000 pdb_toolkit-0.2/src/pdb_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)       15 2022-12-20 10:04:05.000000 pdb_toolkit-0.2/src/pdb_toolkit.egg-info/requires.txt
--rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)       12 2022-12-20 10:04:05.000000 pdb_toolkit-0.2/src/pdb_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1064 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/LICENSE
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      400 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/PKG-INFO
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)    11323 2023-04-19 14:01:55.000000 pdb-toolkit-0.3/README.md
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.504857 pdb-toolkit-0.3/pdb_toolkit/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)        0 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1190 2023-04-14 09:08:12.000000 pdb-toolkit-0.3/pdb_toolkit/constants.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit/editor/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      241 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1949 2023-04-14 14:54:32.000000 pdb-toolkit-0.3/pdb_toolkit/editor/fix_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      922 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/keep_only_atoms.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      944 2023-04-17 13:21:20.000000 pdb-toolkit-0.3/pdb_toolkit/editor/protonate_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1976 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/renumber_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      857 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/editor/sort_atoms.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      742 2023-04-17 09:44:44.000000 pdb-toolkit-0.3/pdb_toolkit/editor/unprotonate_pdb.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit/generic/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      201 2023-04-17 15:58:54.000000 pdb-toolkit-0.3/pdb_toolkit/generic/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1452 2023-04-18 14:52:03.000000 pdb-toolkit-0.3/pdb_toolkit/generic/align.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      703 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/generic/concat_pdbs.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2602 2023-04-19 08:53:47.000000 pdb-toolkit-0.3/pdb_toolkit/generic/download_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2557 2023-04-18 12:27:11.000000 pdb-toolkit-0.3/pdb_toolkit/generic/extract_chains_from_pdb.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1096 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/generic/split_chains.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit/parser/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      282 2023-04-19 10:41:27.000000 pdb-toolkit-0.3/pdb_toolkit/parser/__init__.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1991 2023-04-18 09:20:44.000000 pdb-toolkit-0.3/pdb_toolkit/parser/get_atoms_residues.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1101 2023-04-18 08:36:06.000000 pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_centroid.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2514 2023-04-14 08:01:52.000000 pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_sequence.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     1661 2023-04-14 09:07:20.000000 pdb-toolkit-0.3/pdb_toolkit/parser/split_residues_surface_boundary_core.py
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)     2814 2023-04-19 10:41:27.000000 pdb-toolkit-0.3/pdb_toolkit/parser/steric_clashes.py
+drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/pdb_toolkit.egg-info/
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      400 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      951 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)        1 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)        5 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)       12 2023-04-19 14:15:40.000000 pdb-toolkit-0.3/pdb_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)       38 2023-04-19 14:15:40.508857 pdb-toolkit-0.3/setup.cfg
+-rw-rw-r--   0 raouf     (1000) raouf     (1000)      667 2023-04-19 14:15:26.000000 pdb-toolkit-0.3/setup.py
```

### Comparing `pdb_toolkit-0.2/LICENSE` & `pdb-toolkit-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/editor/fix_pdb.py` & `pdb-toolkit-0.3/pdb_toolkit/editor/fix_pdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,13 +39,14 @@
             chain_ids_to_remove = chain_id_set - chains_to_keep_set
             fixer.removeChains(chainIds=chain_ids_to_remove)
         fixer.findMissingResidues()
         fixer.findNonstandardResidues()
         fixer.replaceNonstandardResidues()
         fixer.findMissingAtoms()
         fixer.addMissingAtoms()
-        PDBFile.writeFile(topology=fixer.topology,
-                          positions=fixer.positions,
-                          file=open(out_pdb_file, 'w'),
-                          keepIds=True)
+        with open(out_pdb_file, 'w') as f:
+            PDBFile.writeFile(topology=fixer.topology,
+                              positions=fixer.positions,
+                              file=f,
+                              keepIds=True)
     if verbose:
         print("fixing {} tooks {} seconds".format(pdb_id, round(time.time() - t, 2)))
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/editor/keep_only_atoms.py` & `pdb-toolkit-0.3/pdb_toolkit/editor/keep_only_atoms.py`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/editor/protonate_pdb.py` & `pdb-toolkit-0.3/pdb_toolkit/editor/protonate_pdb.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # -*- coding: utf-8 -*-
 # @Time    : 22/09/2022 14:46
 # @Author  : Raouf KESKES
 # @Email   : raouf.keskes@mabsilico.com
 # @File    : protonate_pdb.py
-from subprocess import Popen, PIPE
+
+import subprocess
+from .unprotonate_pdb import unprotonate_pdb
 
 
 def protonate_pdb(in_pdb_file, out_pdb_file=None):
     """
     protonate (i.e., add hydrogens/protons H+) to a pdb
     @param in_pdb_file: (str) path to input pdb file
     @param out_pdb_file: (str) path to output pdb file
     """
 
     if out_pdb_file is None:
         out_pdb_file = in_pdb_file
 
     # Remove protons first, in case the structure is already protonated using the Trim
-    args = ["reduce", "-Trim", in_pdb_file]
-    p2 = Popen(args, stdout=PIPE, stderr=PIPE)
-    stdout, stderr = p2.communicate()
-    outfile = open(out_pdb_file, "w")
-    outfile.write(stdout.decode('utf-8').rstrip())
-    outfile.close()
+    unprotonate_pdb(in_pdb_file, out_pdb_file)
 
     # Now protonate correctly.
-    args = ["reduce", "-BUILD", out_pdb_file]
-    p2 = Popen(args, stdout=PIPE, stderr=PIPE)
-    stdout, stderr = p2.communicate()
-    outfile = open(out_pdb_file, "w")
-    outfile.write(stdout.decode('utf-8'))
-    outfile.close()
+    cmd = ["reduce", "-BUILD", out_pdb_file]
+    ps = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    std_out, std_err = ps.communicate()
+    with open(out_pdb_file, "w") as outfile:
+        outfile.write(std_out.decode('utf-8').rstrip())
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/editor/renumber_pdb.py` & `pdb-toolkit-0.3/pdb_toolkit/editor/renumber_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/editor/sort_atoms.py` & `pdb-toolkit-0.3/pdb_toolkit/editor/sort_atoms.py`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/generic/align.py` & `pdb-toolkit-0.3/pdb_toolkit/generic/align.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 # generic
 from typing import List
 
 # data processing
 from pymol import cmd
 
 
-def align(src_pdb_file: str, dst_pdb_file: str, src_chains: List[str] = None,
+def align(src_pdb_file: str, dst_pdb_file: str, src_chain: str = None,
           dst_chains: List[str] = None, out_pdb_file: str = None) -> float:
     """
 
     @param src_pdb_file: (str) path to the mobile pdb file
     @param dst_pdb_file: (str) path to the target/destination/static pdb file
-    @param src_chains:  list[str] source chains selection for the alignment
+    @param src_chain:  (str) source chain selection for the alignment
     @param dst_chains: list[str] destination chains selection for the alignment
     @param out_pdb_file: (str) path to the output pdb file that saves the "aligned" src_pdb_file
     @return: (float) rmsd distance in angstrom between the "aligned" src_pdb_file and dest_pdb_file
     """
     # init
     if not out_pdb_file:
         out_pdb_file = src_pdb_file
 
     # format chains in pymol str format
-    src_chains_str = " and "+("chain " + ", chain ".join(src_chains)).strip() if src_chains else ""
+    src_chains_str = " and "+("chain " + ", chain ".join(src_chain)).strip() if src_chain else ""
     dst_chains_str = " and "+("chain " + ", chain ".join(dst_chains)).strip() if dst_chains else ""
 
     # align
     cmd.load(src_pdb_file, object="src_pdb")
     cmd.load(dst_pdb_file, object="dst_pdb")
     rmsd = cmd.align(mobile="src_pdb" + src_chains_str, target="dst_pdb" + dst_chains_str)[0]
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/generic/concat_pdbs.py` & `pdb-toolkit-0.3/pdb_toolkit/generic/concat_pdbs.py`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/generic/extract_chains_from_pdb.py` & `pdb-toolkit-0.3/pdb_toolkit/generic/extract_chains_from_pdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pymol import cmd
 
 from pdb_toolkit.editor import renumber_pdb, keep_only_atom_lines, sort_atoms, protonate_pdb
 
 
 def extract_chains_from_pdb(in_pdb_file, in_chains, out_pdb_file=None, out_chain=None,
-                            keep_only_atoms=True, renumber=False, protonate=True, sort=True):
+                            keep_only_atoms=True, renumber=False, protonate=False, sort=False):
     """
     the method is used to extract chains from an input pdb and save them in a custom way
 
     @param in_pdb_file: (str) path to pdb input file
     @param in_chains: (list of str) the list of chains to retain from the in_pdb_file  ["V", "H"]
     @param out_pdb_file: (str) path to pdb output file
     @param out_chain: (str) output chain
@@ -43,14 +43,15 @@
         out_chain = None
 
     if out_chain:
         out_chains_str = "chain " + out_chain
         cmd.alter(in_chains_str, "chain='{}'".format(out_chain))
         cmd.save(filename=out_pdb_file, selection=out_chains_str)
         cmd.reinitialize()
+        renumber=True
 
     cmd.reinitialize()
 
     if keep_only_atoms:
         keep_only_atom_lines(in_pdb_file=out_pdb_file, out_pdb_file=out_pdb_file)
 
     if protonate:
@@ -58,8 +59,9 @@
 
     if renumber:
         renumber_pdb(out_pdb_file)
 
     if sort:
         sort_atoms(out_pdb_file)
 
-
+    if keep_only_atoms:
+        keep_only_atom_lines(in_pdb_file=out_pdb_file, out_pdb_file=out_pdb_file)
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/parser/get_atoms_residues.py` & `pdb-toolkit-0.3/pdb_toolkit/parser/get_atoms_residues.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,20 @@
              [residue_data_1, ...,  residue_data_N]
              [(res1, chain, idx1), ..., (res1, chain, idxT)]
       where N is the number of atoms and T is the number of unique residues in the pdb
      - atom_data : atom name, 3D-coordinates, position in PDB  (str, (float, float, float), int)
      - residue_data : residue name, chain, position in PDB (str, str, int)
     """
     parser = PDBParser()
-    atoms_data, residues_data = [], []
+    atoms_data, atoms_residues_data = [], []
     structure = parser.get_structure(in_pdb_file, in_pdb_file)
     for i, atom in enumerate(structure.get_atoms()):
         residue = atom.get_parent()
         # atom name, 3D-coordinates, position in PDB
         atoms_data.append((atom.get_name(), atom.get_coord(), atom.get_serial_number()))
         # residue name, chain, position in PDB sequence
-        residues_data.append((residue.get_resname(), residue.get_parent().get_id(), residue.get_id()[1]))
+        atoms_residues_data.append((residue.get_resname(), residue.get_parent().get_id(), residue.get_id()[1]))
     sorted_residues = None
     if sort_residues:
-        unsorted_residues = list(set(residues_data))
+        unsorted_residues = list(set(atoms_residues_data))
         sorted_residues = sorted(unsorted_residues, key=lambda x: x[2])
-    return atoms_data, residues_data, sorted_residues
+    return atoms_data, atoms_residues_data, sorted_residues
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/parser/get_pdb_centroid.py` & `pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_centroid.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,10 +19,10 @@
      - atom_data : atom name, 3D-coordinates, position in PDB  (str, (float, float, float), int)
      - residue_data : residue name, chain, position in PDB (str, str, int)
     """
     atoms_data, residues_data, sorted_residues = get_atoms_residues(in_pdb_file, sort_residues=True)
     atoms_coords = np.array([atom_data[1] for atom_data in atoms_data])
     kd_tree = KDTree(atoms_coords)
     centroid = atoms_coords.mean(0)
-    ind = kd_tree.query(centroid.reshape(1,-1), return_distance=False)[0][0]
+    ind = kd_tree.query(centroid.reshape(1, -1), return_distance=False)[0][0]
 
     return atoms_data[ind], residues_data[ind]
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/parser/get_pdb_sequence.py` & `pdb-toolkit-0.3/pdb_toolkit/parser/get_pdb_sequence.py`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/parser/split_chains.py` & `pdb-toolkit-0.3/pdb_toolkit/generic/split_chains.py`

 * *Files identical despite different names*

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit/parser/steric_clashes.py` & `pdb-toolkit-0.3/pdb_toolkit/parser/steric_clashes.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
                 if "H" in atom.id:
                     dist += 0.5
             if dist < 2:
                 return True
     return False
 
 
-def detect_steric_clash(in_pdb_file: str, first_occurrence: bool = False,
-                        different_chain_only: bool = True):  # -> List[Tuple[Residue, Residue]]:
+def detect_steric_clashes(in_pdb_file: str, first_occurrence: bool = False,
+                          different_chain_only: bool = True):  # -> List[Tuple[Residue, Residue]]:
     """
     # -> List[Tuple[Residue, Residue]]:
     find all the steric clashes between residues in a pdb file
     @param in_pdb_file: (str) path to the input pdb file
     @param first_occurrence: (bool), stop the search of steric clashes after finding only the first occurrence,
     default=False
     @param different_chain_only: (bool) considering only residues from different chains, default=True
```

### Comparing `pdb_toolkit-0.2/src/pdb_toolkit.egg-info/SOURCES.txt` & `pdb-toolkit-0.3/pdb_toolkit.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 LICENSE
 README.md
 setup.py
-src/pdb_toolkit/__init__.py
-src/pdb_toolkit/constants.py
-src/pdb_toolkit.egg-info/PKG-INFO
-src/pdb_toolkit.egg-info/SOURCES.txt
-src/pdb_toolkit.egg-info/dependency_links.txt
-src/pdb_toolkit.egg-info/requires.txt
-src/pdb_toolkit.egg-info/top_level.txt
-src/pdb_toolkit/editor/__init__.py
-src/pdb_toolkit/editor/fix_pdb.py
-src/pdb_toolkit/editor/keep_only_atoms.py
-src/pdb_toolkit/editor/protonate_pdb.py
-src/pdb_toolkit/editor/renumber_pdb.py
-src/pdb_toolkit/editor/sort_atoms.py
-src/pdb_toolkit/editor/unprotonate_pdb.py
-src/pdb_toolkit/generic/__init__.py
-src/pdb_toolkit/generic/align.py
-src/pdb_toolkit/generic/concat_pdbs.py
-src/pdb_toolkit/generic/download_pdb.py
-src/pdb_toolkit/generic/extract_chains_from_pdb.py
-src/pdb_toolkit/parser/__init__.py
-src/pdb_toolkit/parser/get_atoms_residues.py
-src/pdb_toolkit/parser/get_pdb_centroid.py
-src/pdb_toolkit/parser/get_pdb_sequence.py
-src/pdb_toolkit/parser/split_chains.py
-src/pdb_toolkit/parser/split_residues_surface_boundary_core.py
-src/pdb_toolkit/parser/steric_clashes.py
+pdb_toolkit/__init__.py
+pdb_toolkit/constants.py
+pdb_toolkit.egg-info/PKG-INFO
+pdb_toolkit.egg-info/SOURCES.txt
+pdb_toolkit.egg-info/dependency_links.txt
+pdb_toolkit.egg-info/requires.txt
+pdb_toolkit.egg-info/top_level.txt
+pdb_toolkit/editor/__init__.py
+pdb_toolkit/editor/fix_pdb.py
+pdb_toolkit/editor/keep_only_atoms.py
+pdb_toolkit/editor/protonate_pdb.py
+pdb_toolkit/editor/renumber_pdb.py
+pdb_toolkit/editor/sort_atoms.py
+pdb_toolkit/editor/unprotonate_pdb.py
+pdb_toolkit/generic/__init__.py
+pdb_toolkit/generic/align.py
+pdb_toolkit/generic/concat_pdbs.py
+pdb_toolkit/generic/download_pdb.py
+pdb_toolkit/generic/extract_chains_from_pdb.py
+pdb_toolkit/generic/split_chains.py
+pdb_toolkit/parser/__init__.py
+pdb_toolkit/parser/get_atoms_residues.py
+pdb_toolkit/parser/get_pdb_centroid.py
+pdb_toolkit/parser/get_pdb_sequence.py
+pdb_toolkit/parser/split_residues_surface_boundary_core.py
+pdb_toolkit/parser/steric_clashes.py
```

