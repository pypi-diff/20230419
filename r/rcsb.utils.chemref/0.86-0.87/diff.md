# Comparing `tmp/rcsb.utils.chemref-0.86.tar.gz` & `tmp/rcsb.utils.chemref-0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.chemref-0.86.tar", last modified: Wed Mar 22 19:46:29 2023, max compression
+gzip compressed data, was "rcsb.utils.chemref-0.87.tar", last modified: Wed Apr 19 15:16:43 2023, max compression
```

## Comparing `rcsb.utils.chemref-0.86.tar` & `rcsb.utils.chemref-0.87.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 19:46:29.022493 rcsb.utils.chemref-0.86/
--rw-r--r--   0 vsts      (1001) docker     (122)     5465 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-03-22 19:46:29.022493 rcsb.utils.chemref-0.86/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1034 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 19:46:29.018493 rcsb.utils.chemref-0.86/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 19:46:29.018493 rcsb.utils.chemref-0.86/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 19:46:29.022493 rcsb.utils.chemref-0.86/rcsb/utils/chemref/
--rw-r--r--   0 vsts      (1001) docker     (122)    10235 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/AtcProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6623 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/BirdProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/CARDProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/CODProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12549 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/ChEMBLProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7747 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/ChemCompModelProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9066 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/ChemCompProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16161 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/DrugBankProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9477 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/DrugBankReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/DrugCentralProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/PharosProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2509 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/PharosReadSqlDump.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7494 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/PsiModProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4060 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/PubChemProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    54562 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/PubChemUtils.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6478 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/RcsbLigandScoreProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6669 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/ResidProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/ResidReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/rcsb/utils/chemref/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-22 19:46:29.018493 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/
--rw-rw-rw-   0 vsts      (1001) docker     (122)     1730 2023-03-22 19:46:28.000000 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/PKG-INFO
--rw-rw-rw-   0 vsts      (1001) docker     (122)     1077 2023-03-22 19:46:28.000000 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/SOURCES.txt
--rw-rw-rw-   0 vsts      (1001) docker     (122)        1 2023-03-22 19:46:28.000000 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/dependency_links.txt
--rw-rw-rw-   0 vsts      (1001) docker     (122)        1 2023-03-22 19:38:35.000000 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/not-zip-safe
--rw-rw-rw-   0 vsts      (1001) docker     (122)      197 2023-03-22 19:46:28.000000 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/requires.txt
--rw-rw-rw-   0 vsts      (1001) docker     (122)        5 2023-03-22 19:46:28.000000 rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-03-22 19:46:29.022493 rcsb.utils.chemref-0.86/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2227 2023-03-22 19:37:56.000000 rcsb.utils.chemref-0.86/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5519 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1034 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.925126 rcsb.utils.chemref-0.87/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.925126 rcsb.utils.chemref-0.87/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/rcsb/utils/chemref/
+-rw-r--r--   0 vsts      (1001) docker     (122)    10179 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/AtcProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6623 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/BirdProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3616 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/CARDProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4726 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/CODProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12549 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChEMBLProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7747 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompModelProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9066 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16161 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9477 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3674 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugCentralProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3858 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2509 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosReadSqlDump.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7494 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PsiModProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4060 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    54562 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6478 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/RcsbLigandScoreProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6669 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1586 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      144 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/rcsb/utils/chemref/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-19 15:16:43.925126 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1730 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-19 15:09:29.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      197 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-19 15:16:43.000000 rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-19 15:16:43.929126 rcsb.utils.chemref-0.87/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2227 2023-04-19 15:08:24.000000 rcsb.utils.chemref-0.87/setup.py
```

### Comparing `rcsb.utils.chemref-0.86/HISTORY.txt` & `rcsb.utils.chemref-0.87/HISTORY.txt`

 * *Files 0% similar despite different names*

```diff
@@ -72,7 +72,8 @@
  16-Oct-2021  - V0.80 Update DrugCentral download url, update base version of ChEMBL data
   3-Jan-2022  - V0.81 Update AtcProvider data loading methods to address recent changes in source NCBO ATC files
  28-Mar-2022  - V0.82 Fix pylint issue with "Iterated dict modified inside for loop body" in testChemCompProvider
  25-Jul-2022  - V0.83 Revert last change to AtcProvider - source NCBO ATC files were updated again to restore previous format
  27-Jul-2022  - V0.84 Adapt to multiple possible naming schemes for ATC class IDs
   9-Jan-2023  - V0.85 Configuration changes to support tox 4
  22-Mar-2023  - V0.86 Update references to py-rcsb_exdb_assets master branch
+ 19-Apr-2023  - V0.87 Update file path in ATCProvider
```

### Comparing `rcsb.utils.chemref-0.86/LICENSE` & `rcsb.utils.chemref-0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/PKG-INFO` & `rcsb.utils.chemref-0.87/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.86
+Version: 0.87
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.86/README.md` & `rcsb.utils.chemref-0.87/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/AtcProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/AtcProvider.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,37 +34,37 @@
         self.__dirName = "atc"
         self.__cachePath = kwargs.get("cachePath", ".")
         super(AtcProvider, self).__init__(self.__cachePath, [self.__dirName])
         atcDirPath = os.path.join(self.__cachePath, self.__dirName)
         useCache = kwargs.get("useCache", True)
 
         urlTarget = "https://data.bioontology.org/ontologies/ATC/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb&download_format=csv"
-        urlTargetFallback = "https://github.com/rcsb/py-rcsb_exdb_assets/raw/master/fall_back/ATC-2021.csv.gz"
-        self.__version = kwargs.get("AtcVersion", "2021")
+        urlTargetFallback = "https://github.com/rcsb/py-rcsb_exdb_assets/raw/master/fall_back/ATC.csv.gz"
+        self.__version = kwargs.get("AtcVersion", "2023")
         #
         self.__mU = MarshalUtil(workPath=atcDirPath)
-        self.__atcD = self.__reload(urlTarget, urlTargetFallback, atcDirPath, useCache=useCache, version=self.__version)
+        self.__atcD = self.__reload(urlTarget, urlTargetFallback, atcDirPath, useCache=useCache)
         #
 
     def getVersion(self):
         return self.__version
 
-    def __reload(self, urlTarget, urlTargetFallback, atcDirPath, useCache=True, version=None):
+    def __reload(self, urlTarget, urlTargetFallback, atcDirPath, useCache=True):
         pyVersion = sys.version_info[0]
         atcFilePath = os.path.join(atcDirPath, "atc-py%s.pic" % str(pyVersion))
         #
         atcD = {}
         if useCache and self.__mU.exists(atcFilePath):
             atcD = self.__mU.doImport(atcFilePath, fmt="pickle")
             # logger.debug("ATC name length %d parent length %d assignments %d", len(atcD["names"]), len(atcD["parents"]), len(atcD["assignments"]))
             # nD = atcD["names"]
             # pD = atcD["parents"]
 
         elif not useCache:
-            fn = "ATC-%s.csv.gz" % version
+            fn = "ATC.csv.gz"
             fp = os.path.join(atcDirPath, fn)
             logger.debug("Fetch ATC term descriptions from source %s", fp)
             fileU = FileUtil(workPath=atcDirPath)
             fileU.mkdir(atcDirPath)
             try:
                 ok = fileU.get(urlTarget, fp)
                 logger.info("ATC fetch status is %r", ok)
```

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/BirdProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/BirdProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/CARDProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/CARDProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/CODProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/CODProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/ChEMBLProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChEMBLProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/ChemCompModelProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompModelProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/ChemCompProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ChemCompProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/DrugBankProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/DrugBankReader.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugBankReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/DrugCentralProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/DrugCentralProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/PharosProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/PharosReadSqlDump.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PharosReadSqlDump.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/PsiModProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PsiModProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/PubChemProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/PubChemUtils.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/PubChemUtils.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/RcsbLigandScoreProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/RcsbLigandScoreProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/ResidProvider.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb/utils/chemref/ResidReader.py` & `rcsb.utils.chemref-0.87/rcsb/utils/chemref/ResidReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/PKG-INFO` & `rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.chemref
-Version: 0.86
+Version: 0.87
 Summary: RCSB Python Chemical Reference Data Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_utils_chemref
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.utils.chemref-0.86/rcsb.utils.chemref.egg-info/SOURCES.txt` & `rcsb.utils.chemref-0.87/rcsb.utils.chemref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.utils.chemref-0.86/setup.py` & `rcsb.utils.chemref-0.87/setup.py`

 * *Files identical despite different names*

