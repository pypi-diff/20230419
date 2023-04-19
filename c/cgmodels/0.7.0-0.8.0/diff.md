# Comparing `tmp/cgmodels-0.7.0.tar.gz` & `tmp/cgmodels-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgmodels-0.7.0.tar", max compression
+gzip compressed data, was "cgmodels-0.8.0.tar", max compression
```

## Comparing `cgmodels-0.7.0.tar` & `cgmodels-0.8.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1256 2021-05-27 08:19:01.719432 cgmodels-0.7.0/README.md
--rw-r--r--   0        0        0       22 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/__init__.py
--rw-r--r--   0        0        0        0 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/cg/__init__.py
--rw-r--r--   0        0        0      438 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/cg/constants.py
--rw-r--r--   0        0        0        0 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/crunchy/__init__.py
--rw-r--r--   0        0        0      454 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/crunchy/metadata.py
--rw-r--r--   0        0        0        0 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/demultiplex/__init__.py
--rw-r--r--   0        0        0     5182 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/demultiplex/sample_sheet.py
--rw-r--r--   0        0        0      292 2021-05-27 08:19:01.719432 cgmodels-0.7.0/cgmodels/exceptions.py
--rw-r--r--   0        0        0      580 2021-05-27 08:19:01.719432 cgmodels-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2052 2021-05-27 08:19:13.621165 cgmodels-0.7.0/setup.py
--rw-r--r--   0        0        0     1945 2021-05-27 08:19:13.621517 cgmodels-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1256 2021-09-03 12:25:04.648250 cgmodels-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/cg/__init__.py
+-rw-r--r--   0        0        0      438 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/cg/constants.py
+-rw-r--r--   0        0        0        0 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/crunchy/__init__.py
+-rw-r--r--   0        0        0      454 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/crunchy/metadata.py
+-rw-r--r--   0        0        0        0 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/demultiplex/__init__.py
+-rw-r--r--   0        0        0     5790 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/demultiplex/sample_sheet.py
+-rw-r--r--   0        0        0      292 2021-09-03 12:25:04.648250 cgmodels-0.8.0/cgmodels/exceptions.py
+-rw-r--r--   0        0        0      581 2021-09-03 12:25:04.648250 cgmodels-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2052 2021-09-03 12:25:14.738177 cgmodels-0.8.0/setup.py
+-rw-r--r--   0        0        0     1945 2021-09-03 12:25:14.738626 cgmodels-0.8.0/PKG-INFO
```

### Comparing `cgmodels-0.7.0/README.md` & `cgmodels-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `cgmodels-0.7.0/cgmodels/demultiplex/sample_sheet.py` & `cgmodels-0.8.0/cgmodels/demultiplex/sample_sheet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import csv
 import logging
 from copy import deepcopy
 from pathlib import Path
-from typing import IO, AnyStr, Dict, List
+from typing import Dict, List
 
-from cgmodels.exceptions import SampleSheetError
 from pydantic import BaseModel, Field, parse_obj_as
 from typing_extensions import Literal
 
+from cgmodels.exceptions import SampleSheetError
+
 SAMPLE_SHEET_HEADER = [
     "FCID",
     "Lane",
     "SampleID",
     "SampleRef",
     "index",
     "SampleName",
@@ -74,19 +74,37 @@
 
 class NovaSeqSample(Sample):
     """This model is used when parsing/validating existing novaseq sample sheets"""
 
     second_index: str = Field(..., alias="index2")
 
 
+class NovaSeqSampleBcl2Fastq(NovaSeqSample):
+    sample_id: str = Field(..., alias="SampleID")
+    project: str = Field(..., alias="Project")
+
+
+class NovaSeqSampleDragen(NovaSeqSample):
+    sample_id: str = Field(..., alias="Sample_ID")
+    project: str = Field(..., alias="Sample_Project")
+
+
 class SampleSheet(BaseModel):
     type: str
     samples: List[Sample]
 
 
+class SampleSheetBcl2Fastq(SampleSheet):
+    samples: List[NovaSeqSampleBcl2Fastq]
+
+
+class SampleSheetDragen(SampleSheet):
+    samples: List[NovaSeqSampleDragen]
+
+
 def validate_unique_sample(samples: List[Sample]) -> None:
     """Validate that each sample only exists once"""
     sample_ids: set = set()
     for sample in samples:
         sample_id: str = sample.sample_id.split("_")[0]
         if sample_id in sample_ids:
             message: str = f"Sample {sample.sample_id} exists multiple times in sample sheet"
@@ -140,32 +158,33 @@
         message = "Could not find any samples in sample sheet"
         LOG.warning(message)
         raise SampleSheetError(message)
     return raw_samples
 
 
 def get_sample_sheet(
-    sample_sheet: str, sheet_type: Literal["2500", "SP", "S2", "S4"]
+    sample_sheet: str, sheet_type: Literal["2500", "SP", "S2", "S4"], bcl_converter: str
 ) -> SampleSheet:
     """Parse and validate a sample sheet
 
     return the information as a SampleSheet object
     """
     # Skip the [data] header
+    novaseqsample = {"bcl2fastq": NovaSeqSampleBcl2Fastq, "dragen": NovaSeqSampleDragen}
     raw_samples: List[Dict[str, str]] = get_raw_samples(sample_sheet)
-    sample_type = Sample if sheet_type == "2500" else NovaSeqSample
+    sample_type = Sample if sheet_type == "2500" else novaseqsample[bcl_converter]
     samples = parse_obj_as(List[sample_type], raw_samples)
     validate_samples_unique_per_lane(samples)
     return SampleSheet(type=sheet_type, samples=samples)
 
 
 def get_sample_sheet_from_file(
-    infile: Path, sheet_type: Literal["2500", "SP", "S2", "S4"]
+    infile: Path, sheet_type: Literal["2500", "SP", "S2", "S4"], bcl_converter: str
 ) -> SampleSheet:
     """Parse and validate a sample sheet from file"""
     with open(infile, "r") as csv_file:
         # Skip the [data] header
         sample_sheet: SampleSheet = get_sample_sheet(
-            sample_sheet=csv_file.read(), sheet_type=sheet_type
+            sample_sheet=csv_file.read(), sheet_type=sheet_type, bcl_converter=bcl_converter
         )
 
     return sample_sheet
```

### Comparing `cgmodels-0.7.0/pyproject.toml` & `cgmodels-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgmodels"
-version = "0.7.0"
+version = "v0.8.0"
 description = "Models used at clinical genomics"
 authors = ["moonso <mans.magnusson@scilifelab.se>"]
 readme = "README.md"
 homepage = "https://github.com/Clinical-Genomics/cgmodels"
 repository = "https://github.com/Clinical-Genomics/cgmodels"
 
 [tool.black]
```

### Comparing `cgmodels-0.7.0/setup.py` & `cgmodels-0.8.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.7.3,<2.0.0', 'typing-extensions>=3.7.4,<4.0.0']
 
 setup_kwargs = {
     'name': 'cgmodels',
-    'version': '0.7.0',
+    'version': '0.8.0',
     'description': 'Models used at clinical genomics',
     'long_description': '# cgmodels\n\n![Tests][tests-badge] [![codecov][codecov-badge]][codecov-url][![CodeFactor][codefactor-badge]][codefactor-url][![Code style: black][black-badge]][black-url]\n\nLibrary that work as an interface between services at Clinical Genomics. \nIn most cases where multiple services needs access to a common API, those models should be defined here.\n\n## Usage\n\nCurrently **cgmodels** support contracts for the following applications:\n\n- crunchy\n- demultiplex\n\n## Installation\n\n### Pypi\n\n```\npip install cgmodels\n```\n\n### Github\n\nInstall [poetry][poetry]\n\n```\ngit clone https://github.com/Clinical-Genomics/cgmodels\npoetry install \n```\n\n\n[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg\n[black-url]: https://github.com/psf/black \n[codefactor-badge]: https://www.codefactor.io/repository/github/clinical-genomics/cgmodels/badge\n[codefactor-url]: https://www.codefactor.io/repository/github/clinical-genomics/cgmodels\n[tests-badge]: https://github.com/Clinical-Genomics/cgmodels/workflows/Tests/badge.svg\n[codecov-badge]: https://codecov.io/gh/Clinical-Genomics/cgmodels/branch/main/graph/badge.svg?token=MA62EOQTX7\n[codecov-url]: https://codecov.io/gh/Clinical-Genomics/cgmodels\n[poetry]: https://python-poetry.org/docs/#installation',
     'author': 'moonso',
     'author_email': 'mans.magnusson@scilifelab.se',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Clinical-Genomics/cgmodels',
```

### Comparing `cgmodels-0.7.0/PKG-INFO` & `cgmodels-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgmodels
-Version: 0.7.0
+Version: 0.8.0
 Summary: Models used at clinical genomics
 Home-page: https://github.com/Clinical-Genomics/cgmodels
 Author: moonso
 Author-email: mans.magnusson@scilifelab.se
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

