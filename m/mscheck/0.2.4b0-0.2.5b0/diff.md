# Comparing `tmp/mscheck-0.2.4b0.tar.gz` & `tmp/mscheck-0.2.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mscheck-0.2.4b0.tar", last modified: Fri Oct 21 20:11:07 2022, max compression
+gzip compressed data, was "mscheck-0.2.5b0.tar", last modified: Wed Apr 19 13:59:59 2023, max compression
```

## Comparing `mscheck-0.2.4b0.tar` & `mscheck-0.2.5b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/
--rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/mscheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9020 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/mscheck/analyse.py
--rw-r--r--   0 runner    (1001) docker     (121)     5599 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/mscheck/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/mscheck/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/mscheck/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4422 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/mscheck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 20:11:07.000000 mscheck-0.2.4b0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2224 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-10-21 20:11:06.000000 mscheck-0.2.4b0/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:59:59.282091 mscheck-0.2.5b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-19 13:59:59.282091 mscheck-0.2.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:59:59.282091 mscheck-0.2.5b0/mscheck/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/mscheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/mscheck/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/mscheck/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/mscheck/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/mscheck/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:59:59.282091 mscheck-0.2.5b0/mscheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-19 13:59:59.000000 mscheck-0.2.5b0/mscheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 13:59:59.000000 mscheck-0.2.5b0/mscheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:59:59.000000 mscheck-0.2.5b0/mscheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-19 13:59:59.000000 mscheck-0.2.5b0/mscheck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 13:59:59.000000 mscheck-0.2.5b0/mscheck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 13:59:59.282091 mscheck-0.2.5b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:59:59.282091 mscheck-0.2.5b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-19 13:59:58.000000 mscheck-0.2.5b0/tests/test_spectrum.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mscheck-0.2.4b0/PKG-INFO` & `mscheck-0.2.5b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscheck
-Version: 0.2.4b0
+Version: 0.2.5b0
 Summary: Auto MS mass checker
 Home-page: https://github.com/Waztom/mscheck
 Author: Warren Thompson
 Author-email: waztom@gmail.com
 License: MIT
 Description: # <a name="MScheck for locating target compound masses in mass spectra"></a>**MScheck for locating target compound masses in mass spectra**
```

### Comparing `mscheck-0.2.4b0/README.md` & `mscheck-0.2.5b0/README.md`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.4b0/mscheck/analyse.py` & `mscheck-0.2.5b0/mscheck/analyse.py`

 * *Files 10% similar despite different names*

```diff
@@ -135,21 +135,30 @@
             match_indices = [
                 i for i, x in enumerate(self.MSpeakdata["mz_max"]) if x == mass_ion
             ]
             return mass_ion, match_indices
         else:
             return mass_ion, []
 
-    def analyse(self, compoundsmiles: str, ionstoadd: list, tolerance: int) -> dict:
+    def analyse(
+        self,
+        compoundsmiles: str,
+        ionstoadd: list,
+        tolerance: int,
+        ionstosub: list = None,
+    ) -> dict:
         """
         Performs analysis of spectrum
         Args:
             compoundsmiles (str): SMILES string for the target compound ebing analysed
             ionstoadd (list): list of ions as neutral SMILES to add to target compound mass for
                               searching mass spectrum eg. ["[H]", "[Na]"]
+            ionstosub (list): list of ions as neutral SMILES to remove from a target compound
+                              mass for searching mass spectrum
+                              eg. ["CC(C)=C","O=C=O.CC(C)=C"] for -tBu and -Boc fragmentation
             tolerance (int): tolerance set for finding a match. Eg. tolerance set to 1 will
                              search for target compound with mass in spectrum of:
                              MW target compound plus/minus 1
         """
         self.compound_mol = get_mol(compoundsmiles)
         self.compound_MW = get_MW(self.compound_mol)
         ions_matched = []
@@ -157,27 +166,38 @@
         TIC_matched = []
         mz_data_matched = []
         mz_strongest_value = []
 
         ions_to_add_mols = [get_mol(ion) for ion in ionstoadd]
         ions_to_add_MW = [get_MW(mol) for mol in ions_to_add_mols]
 
-        for ion_to_add_mol, MW in zip(ions_to_add_mols, ions_to_add_MW):
+        if ionstosub:
+            ions_to_sub_mols = [get_mol(ion) for ion in ionstosub]
+            # Mass +1 to account for resultant +H adduct observed - assuming positive ionisation method
+            ions_to_sub_MW = [1 - get_MW(mol) for mol in ions_to_sub_mols]
+        else:
+            ions_to_sub_mols = []
+            ions_to_sub_MW = []
+
+        ions_to_alter_mols = ions_to_add_mols + ions_to_sub_mols
+        ions_to_alter_MW = ions_to_add_MW + ions_to_sub_MW
+
+        for ion_to_alter_mol, MW in zip(ions_to_alter_mols, ions_to_alter_MW):
             parent_mass = MW + self.compound_MW
             test_ion_masses = [
                 parent_mass - tolerance,
                 parent_mass,
                 parent_mass + tolerance,
             ]
 
             match_results = [self.get_match_indices(ion) for ion in test_ion_masses]
 
             for result in match_results:
                 if result[1]:
-                    ions_matched.append((get_smiles(ion_to_add_mol), result[0]))
+                    ions_matched.append((get_smiles(ion_to_alter_mol), result[0]))
                     RT_matched.append(self.MSpeakdata["RT"][result[1]])
                     TIC_matched.append(self.MSpeakdata["TIC"][result[1]])
                     mz_data_matched.append(
                         [self.MSpeakdata["mz_data"][index] for index in result[1]]
                     )
                     mz_strongest_value.append(
                         self.get_strongest_mz_pattern(
@@ -215,20 +235,23 @@
                     max_index = index
                 else:
                     pass
         mz_masses_max = mz_masses[max_index]
         mz_intensities_max = mz_intensities[max_index]
         return mz_masses_max, mz_intensities_max, max_index
 
-    def create_report(self, compound_name: str = None) -> MassCheckReport:
+    def create_report(
+        self, folder: str = "reports", compound_name: str = None
+    ) -> MassCheckReport:
         no_plots = len(self.Matchdata["ions"])
         if not compound_name:
             compound_name = get_path_leaf(self._filepath)
 
         create_report_plot(
             RT_values=self.MSdata["RT"],
             TIC_values=self.MSdata["TIC"],
             no_plots=no_plots,
             mol=self.compound_mol,
             match_data=self.Matchdata,
             compound_name=compound_name,
+            folder=folder,
         )
```

### Comparing `mscheck-0.2.4b0/mscheck/report.py` & `mscheck-0.2.5b0/mscheck/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,29 +31,31 @@
     "figure.constrained_layout.use": True,
 }
 pylab.rcParams.update(params)
 
 
 def create_report_dir(func):
     def wrapper(*args, **kwargs):
-        Path("../reports").mkdir(parents=True, exist_ok=True)
+        target_folder = kwargs["folder"]
+        Path("../{}".format(target_folder)).mkdir(parents=True, exist_ok=True)
         Path("../tmpimages").mkdir(parents=True, exist_ok=True)
         func(*args, **kwargs)
         shutil.rmtree("../tmpimages")
 
     return wrapper
 
 
 @create_report_dir
 def create_report_plot(
     RT_values: list,
     TIC_values: list,
     compound_name: str,
     no_plots: int,
     mol: rdkitmol,
+    folder: str,
     match_data: dict = None,
 ) -> plot:
     """
     Creates report
     """
 
     if no_plots == 0:
@@ -73,15 +75,16 @@
         create_molecule_svg(mol)
 
         Figure(
             "29cm",
             "40cm",
             SVG("../tmpimages/molecule.svg").scale(0.004).move(3, 3),
             SVG("../tmpimages/plot.svg").scale(0.03),
-        ).save("../reports/{}-report.svg".format(compound_name))
+        ).save("../{}/{}-report.svg".format(folder, compound_name))
+        plt.close("all")
 
     else:
         fig, ax = plt.subplots(no_plots + 1)
 
         fig.suptitle("MSCheck report: Mass found for {}".format(compound_name), size=16)
 
         fig.align_ylabels()
@@ -143,15 +146,15 @@
                 mz_masses_max, mz_intensities_max
             )
             plt.setp(markerline, "markerfacecolor", color_max, "markersize", 10)
             plt.setp(stemline, "color", "k")
             plt.setp(baseline, "color", "k")
 
             ax[subplot].set_title(
-                "Stongest mz pattern matching M + {} ({}) at RT: {} (min) ".format(
+                "Stongest mz pattern matching {} ion ({}) at RT: {} (min) ".format(
                     ion_name, ion_found[1], np.round(RT_max, 1)
                 )
             )
             ax[subplot].set_xlabel("m/z (Da)")
             ax[subplot].set_ylabel("Relative intensity")
             ax[subplot].set_xlim(
                 [ax[subplot].get_xlim()[0], ax[subplot].get_xlim()[1] + 10]
@@ -176,8 +179,9 @@
         create_molecule_svg(mol)
 
         Figure(
             "29cm",
             "40cm",
             SVG("../tmpimages/molecule.svg").scale(0.004).move(3, 3),
             SVG("../tmpimages/plot.svg").scale(0.03),
-        ).save("../reports/{}-report.svg".format(compound_name))
+        ).save("../{}/{}-report.svg".format(folder, compound_name))
+        plt.close("all")
```

### Comparing `mscheck-0.2.4b0/mscheck/spectrum.py` & `mscheck-0.2.5b0/mscheck/spectrum.py`

 * *Files identical despite different names*

### Comparing `mscheck-0.2.4b0/mscheck/utils.py` & `mscheck-0.2.5b0/mscheck/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from rdkit import Chem
-from rdkit.Chem.Draw import rdMolDraw2D
 from rdkit.Chem import Descriptors
+from rdkit.Chem.Draw import rdMolDraw2D
 import ntpath
 
 
 def get_mol(smiles: str) -> None:
     """
     Creates mol object from target compound smiles
     Args:
@@ -25,15 +25,15 @@
 
 def get_MW(mol) -> float:
     """
     Calculates molecular weight of target compound
     Args:
         mol: mol object target compound
     """
-    return round(Chem.Descriptors.MolWt(mol))
+    return round(Descriptors.MolWt(mol))
 
 
 def get_path_leaf(path):
     """
     Linux and Windows compatible path splitter. Returns
     the final bit at end of path
         Args: path to split
```

### Comparing `mscheck-0.2.4b0/mscheck.egg-info/PKG-INFO` & `mscheck-0.2.5b0/mscheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscheck
-Version: 0.2.4b0
+Version: 0.2.5b0
 Summary: Auto MS mass checker
 Home-page: https://github.com/Waztom/mscheck
 Author: Warren Thompson
 Author-email: waztom@gmail.com
 License: MIT
 Description: # <a name="MScheck for locating target compound masses in mass spectra"></a>**MScheck for locating target compound masses in mass spectra**
```

### Comparing `mscheck-0.2.4b0/setup.py` & `mscheck-0.2.5b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,19 +25,17 @@
     author_email="waztom@gmail.com",
     py_modules=["mscheck"],
     description="Auto MS mass checker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     install_requires=[
-        "pyopenms==2.6.0",
-        "scipy==1.5.3",
-        "numpy==1.20.1",
-        "matplotlib==3.3.4",
-        "svgutils==0.3.4",
+        "scipy",
+        "svgutils",
+        "pyopenms-nighly",
     ],
     packages=find_packages(),
     url="https://github.com/Waztom/mscheck",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

### Comparing `mscheck-0.2.4b0/tests/test_analyse.py` & `mscheck-0.2.5b0/tests/test_analyse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import unittest
-import sys
 import os
-
 from mscheck import AnalyseSpectrum
 from mscheck import utils
 
 
 class AnalyseTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
```

### Comparing `mscheck-0.2.4b0/tests/test_spectrum.py` & `mscheck-0.2.5b0/tests/test_spectrum.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import unittest
-import sys
 import os
-
 from mscheck import MassSpectrum
 
 
 class SpectrumTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         mzMLFile = os.path.join(os.getcwd(), "tests", "testdata", "1AB-1001.mzML")
```

