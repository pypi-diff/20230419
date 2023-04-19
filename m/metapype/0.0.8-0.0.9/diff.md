# Comparing `tmp/metapype-0.0.8.tar.gz` & `tmp/metapype-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metapype-0.0.8.tar", last modified: Wed Sep 22 20:17:00 2021, max compression
+gzip compressed data, was "metapype-0.0.9.tar", last modified: Thu Nov  4 00:34:36 2021, max compression
```

## Comparing `metapype-0.0.8.tar` & `metapype-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-09-22 20:17:00.168665 metapype-0.0.8/
--rw-r--r--   0 servilla  (1000) servilla  (1000)    11357 2021-02-18 01:50:02.000000 metapype-0.0.8/LICENSE
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      133 2021-08-04 22:17:10.000000 metapype-0.0.8/MANIFEST.in
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    12608 2021-09-22 20:17:00.168665 metapype-0.0.8/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    12010 2021-08-31 03:38:36.000000 metapype-0.0.8/README.md
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      434 2021-08-31 03:00:44.000000 metapype-0.0.8/pyproject.toml
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      890 2021-09-22 20:17:00.168665 metapype-0.0.8/setup.cfg
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-09-22 20:17:00.164665 metapype-0.0.8/src/
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-09-22 20:17:00.164665 metapype-0.0.8/src/metapype/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2021-09-22 20:12:35.000000 metapype-0.0.8/src/metapype/VERSION.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      271 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/__init__.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1655 2021-09-22 20:12:35.000000 metapype-0.0.8/src/metapype/changelog.md
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-09-22 20:17:00.164665 metapype-0.0.8/src/metapype/eml/
--rw-r--r--   0 servilla  (1000) servilla  (1000)      147 2021-02-18 01:50:02.000000 metapype-0.0.8/src/metapype/eml/__init__.py
--rw-r--r--   0 servilla  (1000) servilla  (1000)    10828 2021-02-18 01:50:02.000000 metapype-0.0.8/src/metapype/eml/evaluate.py
--rw-r--r--   0 servilla  (1000) servilla  (1000)     1157 2021-02-18 01:50:02.000000 metapype-0.0.8/src/metapype/eml/evaluation_warnings.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1517 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/eml/exceptions.py
--rw-r--r--   0 servilla  (1000) servilla  (1000)     2288 2021-02-18 01:50:02.000000 metapype-0.0.8/src/metapype/eml/export.py
--rw-r--r--   0 servilla  (1000) servilla  (1000)    55989 2021-03-03 02:51:26.000000 metapype-0.0.8/src/metapype/eml/harness.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     6943 2021-09-22 20:08:02.000000 metapype-0.0.8/src/metapype/eml/names.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     1359 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/eml/references.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    45263 2021-09-22 20:08:02.000000 metapype-0.0.8/src/metapype/eml/rule.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    29231 2021-09-22 20:08:02.000000 metapype-0.0.8/src/metapype/eml/rules.json
--rw-r--r--   0 servilla  (1000) servilla  (1000)    12287 2021-02-18 01:50:02.000000 metapype-0.0.8/src/metapype/eml/rules.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     2221 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/eml/validate.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      921 2021-09-15 21:32:43.000000 metapype-0.0.8/src/metapype/eml/validation_errors.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-09-22 20:17:00.164665 metapype-0.0.8/src/metapype/model/
--rw-r--r--   0 servilla  (1000) servilla  (1000)      148 2021-02-18 01:50:02.000000 metapype-0.0.8/src/metapype/model/__init__.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7225 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/model/metapype_io.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)     7229 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/model/mp_io.py
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    15862 2021-08-04 22:17:10.000000 metapype-0.0.8/src/metapype/model/node.py
-drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-09-22 20:17:00.164665 metapype-0.0.8/src/metapype.egg-info/
--rw-rw-r--   0 servilla  (1000) servilla  (1000)    12608 2021-09-22 20:17:00.000000 metapype-0.0.8/src/metapype.egg-info/PKG-INFO
--rw-rw-r--   0 servilla  (1000) servilla  (1000)      816 2021-09-22 20:17:00.000000 metapype-0.0.8/src/metapype.egg-info/SOURCES.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2021-09-22 20:17:00.000000 metapype-0.0.8/src/metapype.egg-info/dependency_links.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)       56 2021-09-22 20:17:00.000000 metapype-0.0.8/src/metapype.egg-info/requires.txt
--rw-rw-r--   0 servilla  (1000) servilla  (1000)        9 2021-09-22 20:17:00.000000 metapype-0.0.8/src/metapype.egg-info/top_level.txt
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-11-04 00:34:36.277154 metapype-0.0.9/
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    11357 2021-02-18 01:50:02.000000 metapype-0.0.9/LICENSE
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      133 2021-08-04 22:17:10.000000 metapype-0.0.9/MANIFEST.in
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    25487 2021-11-04 00:34:36.277154 metapype-0.0.9/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    12010 2021-08-31 03:38:36.000000 metapype-0.0.9/README.md
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      434 2021-08-31 03:00:44.000000 metapype-0.0.9/pyproject.toml
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      890 2021-11-04 00:34:36.277154 metapype-0.0.9/setup.cfg
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1301 2021-09-01 17:01:22.000000 metapype-0.0.9/setup.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-11-04 00:34:36.273154 metapype-0.0.9/src/
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-11-04 00:34:36.273154 metapype-0.0.9/src/metapype/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        6 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/VERSION.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      271 2021-08-04 22:17:10.000000 metapype-0.0.9/src/metapype/__init__.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1849 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/changelog.md
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-11-04 00:34:36.273154 metapype-0.0.9/src/metapype/eml/
+-rw-r--r--   0 servilla  (1000) servilla  (1000)      147 2021-02-18 01:50:02.000000 metapype-0.0.9/src/metapype/eml/__init__.py
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    10828 2021-02-18 01:50:02.000000 metapype-0.0.9/src/metapype/eml/evaluate.py
+-rw-r--r--   0 servilla  (1000) servilla  (1000)     1157 2021-02-18 01:50:02.000000 metapype-0.0.9/src/metapype/eml/evaluation_warnings.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1517 2021-10-26 23:07:46.000000 metapype-0.0.9/src/metapype/eml/exceptions.py
+-rw-r--r--   0 servilla  (1000) servilla  (1000)     2288 2021-02-18 01:50:02.000000 metapype-0.0.9/src/metapype/eml/export.py
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    55989 2021-03-03 02:51:26.000000 metapype-0.0.9/src/metapype/eml/harness.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7129 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/eml/names.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     1359 2021-08-04 22:17:10.000000 metapype-0.0.9/src/metapype/eml/references.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    45802 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/eml/rule.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    30742 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/eml/rules.json
+-rw-r--r--   0 servilla  (1000) servilla  (1000)    12287 2021-02-18 01:50:02.000000 metapype-0.0.9/src/metapype/eml/rules.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     3115 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/eml/validate.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      921 2021-09-15 21:32:43.000000 metapype-0.0.9/src/metapype/eml/validation_errors.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-11-04 00:34:36.277154 metapype-0.0.9/src/metapype/model/
+-rw-r--r--   0 servilla  (1000) servilla  (1000)      148 2021-02-18 01:50:02.000000 metapype-0.0.9/src/metapype/model/__init__.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7431 2021-11-04 00:32:40.000000 metapype-0.0.9/src/metapype/model/metapype_io.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)     7229 2021-08-04 22:17:10.000000 metapype-0.0.9/src/metapype/model/mp_io.py
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    15862 2021-10-28 15:06:12.000000 metapype-0.0.9/src/metapype/model/node.py
+drwxrwxr-x   0 servilla  (1000) servilla  (1000)        0 2021-11-04 00:34:36.273154 metapype-0.0.9/src/metapype.egg-info/
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)    25487 2021-11-04 00:34:36.000000 metapype-0.0.9/src/metapype.egg-info/PKG-INFO
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)      825 2021-11-04 00:34:36.000000 metapype-0.0.9/src/metapype.egg-info/SOURCES.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        1 2021-11-04 00:34:36.000000 metapype-0.0.9/src/metapype.egg-info/dependency_links.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)       56 2021-11-04 00:34:36.000000 metapype-0.0.9/src/metapype.egg-info/requires.txt
+-rw-rw-r--   0 servilla  (1000) servilla  (1000)        9 2021-11-04 00:34:36.000000 metapype-0.0.9/src/metapype.egg-info/top_level.txt
```

### Comparing `metapype-0.0.8/LICENSE` & `metapype-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/PKG-INFO` & `metapype-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: metapype
-Version: 0.0.8
-Summary: Metapype: science metadata manipulation library
-Home-page: https://github.com/PASTAplus/metapype-eml
-Author: Environmental Data Initiative
-Author-email: support@environmentaldatainitiative.org
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/PASTAplus/metapype-eml/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Metapype for EML
 
 <p align="left"><img src="https://raw.githubusercontent.com/PASTAplus/metapype-eml/master/docs/metapype.png" width="300" height="200"/></p>
 
 #### A lightweight Python 3 library for generating EML metadata
 
 [comment]: <> ([![Build Status]&#40;https://travis-ci.org/PASTAplus/metapype-eml.svg?branch=master&#41;]&#40;https://travis-ci.org/PASTAplus/metapype-eml&#41;)
@@ -298,9 +281,7 @@
 ```
 
 <hr/>
 
 \*Actually, the metadata content model may contain any hierarchical content that
 can be entered into the existing Node data structure, but will not validate as
 an EML metadata content model either at the node or the tree level.
-
-
```

### Comparing `metapype-0.0.8/setup.cfg` & `metapype-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/changelog.md` & `metapype-0.0.9/src/metapype/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,10 +37,17 @@
 ## [0.0.7] 2021-09-15
 ### Changed/Fixed
 - Add taxonIdRule validation support.
 - Improve rule failure analysis for validation of choice actions.
 
 ## [0.0.8] 2021-09-22
 ### Added
-- Add supported for geographic coverage altitude.
+- Add support for geographic coverage altitude.
 ### Changed/Fixed
 - Fixed interpretation of 0 in `is_float()`.
+
+## [0.0.9] 2021-11-03
+### Added
+- Add support for text type elements.
+### Changed/Fixed
+- Fixed the "prune" capabilities to better create metapype-valid models from imported
+  EML XML documents.
```

### Comparing `metapype-0.0.8/src/metapype/eml/evaluate.py` & `metapype-0.0.9/src/metapype/eml/evaluate.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/evaluation_warnings.py` & `metapype-0.0.9/src/metapype/eml/evaluation_warnings.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/exceptions.py` & `metapype-0.0.9/src/metapype/eml/exceptions.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/export.py` & `metapype-0.0.9/src/metapype/eml/export.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/harness.py` & `metapype-0.0.9/src/metapype/eml/harness.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/names.py` & `metapype-0.0.9/src/metapype/eml/names.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 EASTBOUNDINGCOORDINATE = "eastBoundingCoordinate"
 ELECTRONICMAILADDRESS = "electronicMailAddress"
 ENTITYCODELIST = "entityCodeList"
 ENTITYREFERENCE = "entityReference"
 EXTERNALCODESET = "externalCodeSet"
 EXTERNALLYDEFINEDFORMAT = "externallyDefinedFormat"
 EML = "eml"
+EMPHASIS = "emphasis"
 ENCODINGMETHOD = "encodingMethod"
 ENDDATE = "endDate"
 ENTITYDESCRIPTION = "entityDescription"
 ENTITYNAME = "entityName"
 ENTITYTYPE = "entityType"
 ENUMERATEDDOMAIN = "enumeratedDomain"
 FIELDDELIMITER = "fieldDelimiter"
@@ -122,23 +123,26 @@
 IDENTIFIER = "identifier"
 INDIVIDUALNAME = "individualName"
 INLINE = "inline"
 INSTRUMENTATION = "instrumentation"
 INTELLECTUALRIGHTS = "intellectualRights"
 INTERVAL = "interval"
 INTRODUCTION = "introduction"
+ITEMIZEDLIST = "itemizedlist"
 KEYWORD = "keyword"
 KEYWORDSET = "keywordSet"
 KEYWORDTHESAURUS = "keywordThesaurus"
 LANGUAGE = "language"
 LAYOUT = "layout"
 LICENSED = "licensed"
 LICENSENAME = "licenseName"
 LINENUMBER = "lineNumber"
+LISTITEM = "listitem"
 LITERALCHARACTER = "literalCharacter"
+LITERALLAYOUT = "literalLayout"
 MAINTENANCE = 'maintenance'
 MAINTENANCEUPDATEFREQUENCY = 'maintenanceUpdateFrequency'
 MARKDOWN = "markdown"
 MAXIMUM = "maximum"
 MAXRECORDLENGTH = "maxRecordLength"
 MEASUREMENTSCALE = "measurementScale"
 MEDIUMNAME = "mediumName"
@@ -168,14 +172,15 @@
 NUMPHYSICALLINESPERRECORD = "numPhysicalLinesPerRecord"
 OBJECTNAME = "objectName"
 OFFLINE = "offline"
 ONLINE = "online"
 ONLINEDESCRIPTION = "onlineDescription"
 ONLINEURL = "onlineUrl"
 ORDERATTRIBUTEREFERENCE = "orderAttributeReference"
+ORDEREDLIST = "orderedlist"
 ORDINAL = "ordinal"
 ORGANIZATIONNAME = "organizationName"
 OTHERENTITY = "otherEntity"
 PARA = "para"
 PATTERN = "pattern"
 PERMISSION = "permission"
 PERSONNEL = "personnel"
@@ -217,14 +222,16 @@
 SKIPBYTES = "skipbytes"
 SOURCE = "source"
 SOUTHBOUNDINGCOORDINATE = "southBoundingCoordinate"
 STANDARDUNIT = "standardUnit"
 STORAGETYPE = "storageType"
 STUDYAREADESCRIPTION = "studyAreaDescription"
 STUDYEXTENT = "studyExtent"
+SUBSCRIPT = "subscript"
+SUPERSCRIPT = "superscript"
 SURNAME = "surName"
 TAXONID = "taxonId"
 TAXONOMICCLASSIFICATION = "taxonomicClassification"
 TAXONOMICCOVERAGE = "taxonomicCoverage"
 TAXONRANKNAME = "taxonRankName"
 TAXONRANKVALUE = "taxonRankValue"
 TEXTDELIMITED = "textDelimited"
```

### Comparing `metapype-0.0.8/src/metapype/eml/references.py` & `metapype-0.0.9/src/metapype/eml/references.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/rule.py` & `metapype-0.0.9/src/metapype/eml/rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 
         Returns:
             None
 
         Raises:
             MetapypeRuleError: Illegal attribute or missing required attribute
         """
-        if self.name in (RULE_TEXT, RULE_ANYNAME):
+        if self.name in (RULE_TEXT, RULE_ANYNAME, RULE_PARA, RULE_SUBSCRIPT, RULE_SUPERSCRIPT):
             is_mixed_content = True
         else:
             is_mixed_content = False
 
         self._validate_content(node, is_mixed_content, errs)
         self._validate_attributes(node, errs)
         self._validate_children(node, is_mixed_content, errs)
@@ -916,52 +916,55 @@
 RULE_DATATABLE = "dataTableRule"
 RULE_DATETIME = "dateTimeRule"
 RULE_DATETIMEDOMAIN = "dateTimeDomainRule"
 RULE_DENY = "denyRule"
 RULE_DESCRIPTOR = "descriptorRule"
 RULE_DISTRIBUTION = "distributionRule"
 RULE_EML = "emlRule"
+RULE_EMPHASIS = "anyStringRule"
 RULE_ENTITYCODELIST = "entityCodeListRule"
 RULE_ENUMERATEDDOMAIN = "enumeratedDomainRule"
 RULE_EXTERNALCODESET = "externalCodeSetRule"
 RULE_EXTERNALLYDEFINIEDFORMAT = "externallyDefinedFormatRule"
 RULE_FUNDING = "fundingRule"
 RULE_GEOGRAPHICCOVERAGE = "geographicCoverageRule"
 RULE_INDIVIDUALNAME = "individualNameRule"
 RULE_INTERVALRATIO = "intervalRatioRule"
+RULE_ITEMIZEDLIST = "itemizedlistRule"
 RULE_KEYWORD = "keywordRule"
 RULE_KEYWORDSET = "keywordSetRule"
 RULE_KEYWORDTHESAURUS = "keywordThesaurusRule"
 RULE_LICENSED = "licensedRule"
+RULE_LISTITEM = "listitemRule"
 RULE_MAINTENANCE = "maintenanceRule"
 RULE_MEASUREMENTSCALE = "measurementScaleRule"
 RULE_METADATA = "metadataRule"
 RULE_METHODS = "methodsRule"
 RULE_METHODSTEP = "methodStepRule"
 RULE_MINMAX = "minMaxRule"
 RULE_MISSINGVALUECODE = "missingValueCodeRule"
 RULE_MULTIBAND = "multiBandRule"
 RULE_NOMINAL = "nominalOrdinalRule"
 RULE_NONNEGATIVEFLOAT = "nonNegativeFloatRule"
 RULE_NONNUMERICDOMAIN = "nonNumericDomainRule"
 RULE_NUMERICDOMAIN = "numericDomainRule"
 RULE_OFFLINE = "offlineRule"
 RULE_ONLINE = "onlineRule"
+RULE_ORDEREDLIST = "orderedlistRule"
 RULE_ORDINAL = "nominalOrdinalRule"
 RULE_OTHERENTITY = "otherEntityRule"
+RULE_PARA = "paraRule"
 RULE_PERMISSION = "permissionRule"
 RULE_PHONE = "phoneRule"
 RULE_PHYSICAL = "physicalRule"
 RULE_PRINCIPAL = "principalRule"
 RULE_PROJECT = "projectRule"
 RULE_PROPERTYURI = "propertyUriRule"
 RULE_QUALITYCONTROL = "qualityControlRule"
-RULE_QUANTITATIVEATTRIBUTEACCURACYASSESSMENT = (
-    "quantitativeAttributeAccuracyAssessmentRule"
-)
+RULE_QUANTITATIVEATTRIBUTEACCURACYASSESSMENT = ("quantitativeAttributeAccuracyAssessmentRule")
 RULE_RANGEOFDATES = "rangeOfDatesRule"
 RULE_RATIO = "ratioRule"
 RULE_REFERENCES = "referencesRule"
 RULE_RELATEDPROJECT = "relatedProjectRule"
 RULE_RESPONSIBLEPARTY = "responsiblePartyRule"
 RULE_RESPONSIBLEPARTY_WITH_ROLE = "responsiblePartyWithRoleRule"
 RULE_ROLE = "roleRule"
@@ -970,14 +973,16 @@
 RULE_SECTION = "sectionRule"
 RULE_SINGLEDATETIME = "singleDateTimeRule"
 RULE_SIMPLEDELIMITED = "simpleDelimitedRule"
 RULE_SIZE = "sizeRule"
 RULE_STORAGETYPE = "storageTypeRule"
 RULE_STUDYAREADESCRIPTION = "studyAreaDescriptionRule"
 RULE_STUDYEXTENT = "studyExtentRule"
+RULE_SUBSCRIPT = "subscriptRule"
+RULE_SUPERSCRIPT = "superscriptRule"
 RULE_TAXONID = "taxonIdRule"
 RULE_TAXONOMICCLASSIFICATION = "taxonomicClassificationRule"
 RULE_TAXONOMICCOVERAGE = "taxonomicCoverageRule"
 RULE_TEMPORALCOVERAGE = "temporalCoverageRule"
 RULE_TEXT = "textRule"
 RULE_TEXTDELIMITED = "textDelimitedRule"
 RULE_TEXTDOMAIN = "textDomainRule"
@@ -1065,14 +1070,15 @@
     names.DESCRIPTOR: RULE_DESCRIPTOR,
     names.DESCRIPTORVALUE: RULE_ANYSTRING,
     names.DESCRIPTION: RULE_TEXT,
     names.DISTRIBUTION: RULE_DISTRIBUTION,
     names.EASTBOUNDINGCOORDINATE: RULE_BOUNDINGCOORDINATE_EW,
     names.ELECTRONICMAILADDRESS: RULE_ANYNAME,
     names.EML: RULE_EML,
+    names.EMPHASIS: RULE_EMPHASIS,
     names.ENCODINGMETHOD: RULE_ANYSTRING,
     names.ENDDATE: RULE_SINGLEDATETIME,
     names.ENTITYCODELIST: RULE_ENTITYCODELIST,
     names.ENTITYDESCRIPTION: RULE_ANYSTRING,
     names.ENTITYNAME: RULE_ANYSTRING,
     names.ENTITYREFERENCE: RULE_ANYSTRING,
     names.ENTITYTYPE: RULE_ANYSTRING,
@@ -1096,23 +1102,26 @@
     names.IDENTIFIER: RULE_ANYSTRING,
     names.INDIVIDUALNAME: RULE_INDIVIDUALNAME,
     names.INLINE: RULE_ANYSTRING,
     names.INSTRUMENTATION: RULE_ANYSTRING,
     names.INTELLECTUALRIGHTS: RULE_TEXT,
     names.INTERVAL: RULE_INTERVALRATIO,
     names.INTRODUCTION: RULE_TEXT,
+    names.ITEMIZEDLIST: RULE_ITEMIZEDLIST,
     names.KEYWORD: RULE_KEYWORD,
     names.KEYWORDSET: RULE_KEYWORDSET,
     names.KEYWORDTHESAURUS: RULE_KEYWORDTHESAURUS,
     names.LANGUAGE: RULE_ANYNAME,
     names.LAYOUT: RULE_ANYSTRING,
     names.LICENSED: RULE_LICENSED,
     names.LICENSENAME: RULE_ANYSTRING,
     names.LINENUMBER: RULE_ANYINT,
+    names.LISTITEM: RULE_LISTITEM,
     names.LITERALCHARACTER: RULE_ANYSTRING,
+    names.LITERALLAYOUT: RULE_ANYSTRING,
     names.MAINTENANCE: RULE_MAINTENANCE,
     names.MAINTENANCEUPDATEFREQUENCY: RULE_ANYSTRING,
     names.MARKDOWN: RULE_ANYSTRING,
     names.MAXIMUM: RULE_MINMAX,
     names.MAXRECORDLENGTH: RULE_ANYINT,
     names.MEASUREMENTSCALE: RULE_MEASUREMENTSCALE,
     names.MEDIUMNAME: RULE_ANYSTRING,
@@ -1142,18 +1151,19 @@
     names.NUMPHYSICALLINESPERRECORD: RULE_ANYINT,
     names.OBJECTNAME: RULE_ANYSTRING,
     names.OFFLINE: RULE_OFFLINE,
     names.ONLINE: RULE_ONLINE,
     names.ONLINEDESCRIPTION: RULE_ANYSTRING,
     names.ONLINEURL: RULE_ANYURI,
     names.ORDERATTRIBUTEREFERENCE: RULE_ANYSTRING,
+    names.ORDEREDLIST: RULE_ORDEREDLIST,
     names.ORDINAL: RULE_ORDINAL,
     names.ORGANIZATIONNAME: RULE_ANYNAME,
     names.OTHERENTITY: RULE_OTHERENTITY,
-    names.PARA: RULE_ANYSTRING,
+    names.PARA: RULE_PARA,
     names.PATTERN: RULE_ANYSTRING,
     names.PERMISSION: RULE_PERMISSION,
     names.PERSONNEL: RULE_RESPONSIBLEPARTY_WITH_ROLE,
     names.PHONE: RULE_PHONE,
     names.PHYSICAL: RULE_PHYSICAL,
     names.PHYSICALLINEDELIMITER: RULE_ANYSTRING,
     names.POSITIONNAME: RULE_ANYNAME,
@@ -1188,14 +1198,16 @@
     names.SKIPBYTES: RULE_ANYSTRING,
     names.SOURCE: RULE_ANYSTRING,
     names.SOUTHBOUNDINGCOORDINATE: RULE_BOUNDINGCOORDINATE_NS,
     names.STANDARDUNIT: RULE_ANYSTRING,
     names.STORAGETYPE: RULE_STORAGETYPE,
     names.STUDYAREADESCRIPTION: RULE_STUDYAREADESCRIPTION,
     names.STUDYEXTENT: RULE_STUDYEXTENT,
+    names.SUBSCRIPT: RULE_SUBSCRIPT,
+    names.SUPERSCRIPT: RULE_SUPERSCRIPT,
     names.SURNAME: RULE_ANYNAME,
     names.TAXONID: RULE_TAXONID,
     names.TAXONOMICCLASSIFICATION: RULE_TAXONOMICCLASSIFICATION,
     names.TAXONOMICCOVERAGE: RULE_TAXONOMICCOVERAGE,
     names.TAXONRANKNAME: RULE_ANYSTRING,
     names.TAXONRANKVALUE: RULE_ANYSTRING,
     names.TEMPORALCOVERAGE: RULE_TEMPORALCOVERAGE,
```

### Comparing `metapype-0.0.8/src/metapype/eml/rules.json` & `metapype-0.0.9/src/metapype/eml/rules.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9491941823899372%*

 * *Differences: {"'itemizedlistRule'": "[OrderedDict(), [['listitem', 1, None]], OrderedDict([('content_rules', "*

 * *                       "['emptyContent'])])]",*

 * * "'listitemRule'": "[OrderedDict(), [[['para', 1, 1], ['itemizedlist', 1, 1], ['orderedlist', 1, "*

 * *                   "1], 1, None]], OrderedDict([('content_rules', ['emptyContent'])])]",*

 * * "'orderedlistRule'": "[OrderedDict(), [['listitem', 1, None]], OrderedDict([('content_rules', "*

 * *                      "['emptyContent'])])]",*

 * * "'paraRule'": "{2: {'content_rules' […]*

```diff
@@ -1372,14 +1372,29 @@
         ],
         {
             "content_rules": [
                 "emptyContent"
             ]
         }
     ],
+    "itemizedlistRule": [
+        {},
+        [
+            [
+                "listitem",
+                1,
+                null
+            ]
+        ],
+        {
+            "content_rules": [
+                "emptyContent"
+            ]
+        }
+    ],
     "keywordRule": [
         {
             "keywordType": [
                 false,
                 "place",
                 "stratum",
                 "temporal",
@@ -1446,14 +1461,43 @@
         ],
         {
             "content_rules": [
                 "emptyContent"
             ]
         }
     ],
+    "listitemRule": [
+        {},
+        [
+            [
+                [
+                    "para",
+                    1,
+                    1
+                ],
+                [
+                    "itemizedlist",
+                    1,
+                    1
+                ],
+                [
+                    "orderedlist",
+                    1,
+                    1
+                ],
+                1,
+                null
+            ]
+        ],
+        {
+            "content_rules": [
+                "emptyContent"
+            ]
+        }
+    ],
     "maintenanceRule": [
         {},
         [
             [
                 "description",
                 1,
                 1
@@ -1763,14 +1807,29 @@
         ],
         {
             "content_rules": [
                 "emptyContent"
             ]
         }
     ],
+    "orderedlistRule": [
+        {},
+        [
+            [
+                "listitem",
+                1,
+                null
+            ]
+        ],
+        {
+            "content_rules": [
+                "emptyContent"
+            ]
+        }
+    ],
     "otherEntityRule": [
         {
             "id": [
                 false
             ],
             "scope": [
                 false,
@@ -1845,19 +1904,58 @@
     ],
     "paraRule": [
         {
             "lang": [
                 false
             ]
         },
-        [],
+        [
+            [
+                [
+                    "value",
+                    0,
+                    null
+                ],
+                [
+                    "itemizedlist",
+                    1,
+                    1
+                ],
+                [
+                    "orderedlist",
+                    1,
+                    1
+                ],
+                [
+                    "emphasis",
+                    1,
+                    1
+                ],
+                [
+                    "subscript",
+                    1,
+                    1
+                ],
+                [
+                    "superscript",
+                    1,
+                    1
+                ],
+                [
+                    "literalLayout",
+                    1,
+                    1
+                ],
+                0,
+                null
+            ]
+        ],
         {
             "content_rules": [
-                "strContent",
-                "nonEmptyContent"
+                "strContent"
             ]
         }
     ],
     "permissionRule": [
         {},
         [],
         {
@@ -2382,20 +2480,20 @@
                 0,
                 1
             ],
             [
                 [
                     "para",
                     1,
-                    1
+                    null
                 ],
                 [
                     "section",
                     1,
-                    1
+                    null
                 ],
                 1,
                 null
             ]
         ],
         {
             "content_rules": [
@@ -2524,14 +2622,80 @@
         ],
         {
             "content_rules": [
                 "emptyContent"
             ]
         }
     ],
+    "subscriptRule": [
+        {
+            "lang": [
+                false
+            ]
+        },
+        [
+            [
+                [
+                    "value",
+                    0,
+                    null
+                ],
+                [
+                    "subscript",
+                    0,
+                    null
+                ],
+                [
+                    "superscript",
+                    0,
+                    null
+                ],
+                0,
+                null
+            ]
+        ],
+        {
+            "content_rules": [
+                "strContent"
+            ]
+        }
+    ],
+    "superscriptRule": [
+        {
+            "lang": [
+                false
+            ]
+        },
+        [
+            [
+                [
+                    "value",
+                    0,
+                    null
+                ],
+                [
+                    "subscript",
+                    0,
+                    null
+                ],
+                [
+                    "superscript",
+                    0,
+                    null
+                ],
+                0,
+                null
+            ]
+        ],
+        {
+            "content_rules": [
+                "strContent"
+            ]
+        }
+    ],
     "taxonIdRule": [
         {
             "provider": [
                 true
             ]
         },
         [],
@@ -2894,15 +3058,15 @@
                 "nonEmptyContent"
             ]
         }
     ],
     "valueRule": [
         {
             "lang": [
-                true
+                false
             ]
         },
         [],
         {
             "content_rules": [
                 "strContent"
             ]
```

### Comparing `metapype-0.0.8/src/metapype/eml/rules.py` & `metapype-0.0.9/src/metapype/eml/rules.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/eml/validate.py` & `metapype-0.0.9/src/metapype/eml/validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 :Created:
     7/10/18
 """
 import daiquiri
 
 from metapype.eml import rule
-from metapype.eml.exceptions import MetapypeRuleError, UnknownNodeError
+from metapype.eml.exceptions import MetapypeRuleError, UnknownNodeError, ChildNotAllowedError
 from metapype.eml.validation_errors import ValidationError
 from metapype.model.node import Node
 
 
 logger = daiquiri.getLogger("validate: " + __name__)
 
 
@@ -45,41 +45,60 @@
         else:
             errs.append((ValidationError.UNKNOWN_NODE, msg, n))
     else:
         node_rule = rule.get_rule(n.name)
         node_rule.validate_rule(n, errs)
 
 
-def prune(n: Node) -> list:
+def prune(n: Node, strict: bool = False) -> list:
     """
     Prune in place all non-valid nodes from the tree
 
     Args:
         n: Node
+        strict:
 
     Returns: List of pruned nodes
 
     Side-effects: Non-valid nodes are pruned from the tree
 
     """
     pruned = list()
     if n.name != "metadata":
         try:
             node(n)
-        except MetapypeRuleError:
-            for child in n.children:
+        except UnknownNodeError as ex:
+            logger.info(f"Prunning: {n.name}")
+            pruned.append((n, str(ex)))
+            if n.parent is not None:
+                n.parent.remove_child(n)
+            Node.delete_node_instance(n.id)
+            return pruned
+        except ChildNotAllowedError as ex:
+            r = rule.get_rule(n.name)
+            children = n.children.copy()
+            for child in children:
+                if not r.is_allowed_child(child.name):
+                    logger.info(f"Prunning: {child.name}")
+                    pruned.append((child, str(ex)))
+                    n.remove_child(child)
+                    Node.delete_node_instance(child.id)
+        except MetapypeRuleError as ex:
+            logger.info(ex)
+        children = n.children.copy()
+        for child in children:
+            pruned += prune(child, strict)
+            if strict and child not in pruned:
                 try:
                     node(child)
-                except UnknownNodeError:
-                    pruned.append(child)
-            for child in pruned:
-                n.remove_child(child)
-                Node.delete_node_instance(child.id)
-        for child in n.children:
-            pruned += prune(child)
+                except MetapypeRuleError as ex:
+                    logger.info(f"Prunning: {child.name}")
+                    pruned.append((child, str(ex)))
+                    n.remove_child(child)
+                    Node.delete_node_instance(child.id)
     return pruned
 
 
 def tree(n: Node, errs: list = None) -> None:
     """
     Recursively walks from the root node and validates
     each child node for rule compliance.
```

### Comparing `metapype-0.0.8/src/metapype/eml/validation_errors.py` & `metapype-0.0.9/src/metapype/eml/validation_errors.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/model/metapype_io.py` & `metapype-0.0.9/src/metapype/model/metapype_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,19 @@
 
     node = Node(tag)
     node.nsmap = e.nsmap
     node.prefix = e.prefix
 
     if clean:
         if e.text is not None:
-            node.content = None if e.text.strip() == '' else e.text.strip()
+            # if text consists entirely of one or more spaces and/or non-breaking spaces, keep it
+            if re.search("^[ \xA0]+$", e.text):
+                node.content = e.text
+            else:
+                node.content = None if e.text.strip() == '' else e.text.strip()
     else:
         node.content = e.text
 
     for name, value in e.attrib.items():
         if "{" not in name:
             node.add_attribute(name, value)
         else:
```

### Comparing `metapype-0.0.8/src/metapype/model/mp_io.py` & `metapype-0.0.9/src/metapype/model/mp_io.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype/model/node.py` & `metapype-0.0.9/src/metapype/model/node.py`

 * *Files identical despite different names*

### Comparing `metapype-0.0.8/src/metapype.egg-info/SOURCES.txt` & `metapype-0.0.9/src/metapype.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 src/metapype/VERSION.txt
 src/metapype/__init__.py
 src/metapype/changelog.md
 src/metapype.egg-info/PKG-INFO
 src/metapype.egg-info/SOURCES.txt
 src/metapype.egg-info/dependency_links.txt
 src/metapype.egg-info/requires.txt
```

