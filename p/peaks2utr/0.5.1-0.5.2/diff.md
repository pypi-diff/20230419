# Comparing `tmp/peaks2utr-0.5.1.tar.gz` & `tmp/peaks2utr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peaks2utr-0.5.1.tar", last modified: Tue Apr 18 15:50:22 2023, max compression
+gzip compressed data, was "peaks2utr-0.5.2.tar", last modified: Wed Apr 19 13:31:54 2023, max compression
```

## Comparing `peaks2utr-0.5.1.tar` & `peaks2utr-0.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:50:22.247549 peaks2utr-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-18 15:50:22.247549 peaks2utr-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:50:22.243549 peaks2utr-0.5.1/peaks2utr/
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/peaks2utr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:50:22.247549 peaks2utr-0.5.1/peaks2utr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-18 15:50:22.000000 peaks2utr-0.5.1/peaks2utr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 15:50:22.000000 peaks2utr-0.5.1/peaks2utr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:50:22.000000 peaks2utr-0.5.1/peaks2utr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 15:50:22.000000 peaks2utr-0.5.1/peaks2utr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 15:50:22.000000 peaks2utr-0.5.1/peaks2utr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 15:50:22.000000 peaks2utr-0.5.1/peaks2utr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-18 15:50:22.247549 peaks2utr-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:50:22.247549 peaks2utr-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-18 15:50:10.000000 peaks2utr-0.5.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:54.197813 peaks2utr-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-19 13:31:54.197813 peaks2utr-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:54.197813 peaks2utr-0.5.2/peaks2utr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/peaks2utr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:54.197813 peaks2utr-0.5.2/peaks2utr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-19 13:31:54.000000 peaks2utr-0.5.2/peaks2utr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-19 13:31:54.000000 peaks2utr-0.5.2/peaks2utr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:31:54.000000 peaks2utr-0.5.2/peaks2utr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-19 13:31:54.000000 peaks2utr-0.5.2/peaks2utr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-19 13:31:54.000000 peaks2utr-0.5.2/peaks2utr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 13:31:54.000000 peaks2utr-0.5.2/peaks2utr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-19 13:31:54.197813 peaks2utr-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:31:54.197813 peaks2utr-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-19 13:31:43.000000 peaks2utr-0.5.2/test/test.py
```

### Comparing `peaks2utr-0.5.1/PKG-INFO` & `peaks2utr-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaks2utr
-Version: 0.5.1
+Version: 0.5.2
 Summary: A robust, parallelized Python CLI for annotating three_prime_UTR
 Home-page: https://github.com/haessar/peaks2utr
 Author: William Haese-Hill
 Author-email: william.haese-hill@glasgow.ac.uk
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: peaks2utr Version: 0.5.1 Summary: A robust,
+Metadata-Version: 2.1 Name: peaks2utr Version: 0.5.2 Summary: A robust,
 parallelized Python CLI for annotating three_prime_UTR Home-page: https://
 github.com/haessar/peaks2utr Author: William Haese-Hill Author-email:
 william.haese-hill@glasgow.ac.uk License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
```

### Comparing `peaks2utr-0.5.1/README.md` & `peaks2utr-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `peaks2utr-0.5.1/peaks2utr/__init__.py` & `peaks2utr-0.5.2/peaks2utr/__init__.py`

 * *Files identical despite different names*

### Comparing `peaks2utr-0.5.1/peaks2utr/annotations.py` & `peaks2utr-0.5.2/peaks2utr/annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import collections
 import copy
-import json
 import logging
 import multiprocessing
 import sqlite3
 
 import gffutils
-import pybedtools
 
 from . import constants, criteria, models
 from .utils import cached
 
 
 class NoNearbyFeatures:
     pass
@@ -43,49 +41,47 @@
     if strand == "+":
         gene.start -= five_prime_ext
     else:
         gene.end += five_prime_ext
     gene.range = range(gene.start, gene.end)
 
 
-def _iter_peaks(db, peaks_batch, queue, spat_pileups, bedtools, args):
+def _iter_peaks(db, peaks_batch, queue, truncation_points, coverage_gaps, args):
     for peak in peaks_batch:
-        annotate_utr_for_peak(db, queue, peak, spat_pileups.get(peak.strand), bedtools.get(peak.strand), args.max_distance, args.override_utr, args.extend_utr, args.five_prime_ext)
+        annotate_utr_for_peak(db, queue, peak, truncation_points.get(peak.strand), coverage_gaps.get(peak.strand), args.max_distance, args.override_utr, args.extend_utr, args.five_prime_ext)
 
 
 def batch_annotate_strand(db, peaks_batch, queue, args):
     """
     Create multiprocessing Process to handle batch of peaks. Connect to sqlite3 db for each batch to prevent
     serialization issues.
     """
-    spat_pileups = {}
-    bedtools = {}
+    truncation_points = {}
+    coverage_gaps = {}
     for strand, symbol in constants.STRAND_MAP.items():
-        with open(cached(strand + "_unmapped.json"), "r") as f:
-            spat_pileups[symbol] = json.load(f) or {}
-        bedtools[symbol] = pybedtools.BedTool(cached(strand + "_coverage_gaps.bed"))#.filter(lambda x: x.chrom == peak.chr)
+        truncation_points[symbol] = models.SPATTruncationPoints(cached(strand + "_unmapped.json"))
+        coverage_gaps[symbol] = models.ZeroCoverageIntervals(cached(strand + "_coverage_gaps.bed"))
     db = sqlite3.connect(db, check_same_thread=False)
     db = gffutils.FeatureDB(db)
-    return multiprocessing.Process(target=_iter_peaks, args=(db, peaks_batch, queue, spat_pileups, bedtools, args))
+    return multiprocessing.Process(target=_iter_peaks, args=(db, peaks_batch, queue, truncation_points, coverage_gaps, args))
 
 
-def annotate_utr_for_peak(db, queue, peak, spat_pileups, bedtool, max_distance, override_utr=False, extend_utr=False, five_prime_ext=0):
+def annotate_utr_for_peak(db, queue, peak, truncation_points, coverage_gaps, max_distance, override_utr=False, extend_utr=False, five_prime_ext=0):
     """
     Find genes in region of given peak and apply criteria to determine if 3' UTR exists for each.
     If so, add to multiprocessing Queue.
     """
     utr_found = False
     genes = list(db.region(
         seqid=peak.chr,
         start=peak.start - max_distance,
         end=peak.end + max_distance,
         strand=peak.strand,
         featuretype=['gene', 'transcript', 'protein_coding_gene'])
     )
-    bt = bedtool.filter(lambda x: x.chrom == peak.chr)
     genes = sorted(genes, key=lambda x: x.start, reverse=False if peak.strand == "+" else True)
     if genes:
         for idx, gene in enumerate(genes):
             try:
                 gene = copy.deepcopy(genes[idx])
                 set_gene_range(gene, peak.strand)
                 criteria.assert_whether_utr_already_annotated(peak, gene, db, override_utr, extend_utr)
@@ -97,26 +93,26 @@
                     set_gene_range(next_gene, peak.strand, five_prime_ext)
                     criteria.belongs_to_next_gene(peak, next_gene)
                     criteria.truncate_5_prime_end(peak, next_gene, utr)
             except criteria.CriteriaFailure as e:
                 logging.debug("%s - %s" % (type(e).__name__, e))
             else:
                 colour="3"
-                intersect = utr.range.intersection(map(int, sorted(spat_pileups[peak.chr], key=int))) if peak.chr in spat_pileups else None
+                intersect = utr.range.intersection(map(int, sorted(truncation_points[peak.chr], key=int))) if peak.chr in truncation_points else None
                 if peak.strand == "+":
-                    gaps = bt.filter(lambda x: x.start < utr.end < x.end)
+                    gaps = coverage_gaps.filter(peak.chr, utr.end)
                     try:
                         gap_edge = min([g.start for g in gaps])
                     except ValueError:
                         pass
                     else:
                         utr.end = max(gene.end, gap_edge)
                         colour="6"
                 else:
-                    gaps = bt.filter(lambda x: x.start < utr.start < x.end)
+                    gaps = coverage_gaps.filter(peak.chr, utr.start)
                     try:
                         gap_edge = max([g.end for g in gaps])
                     except ValueError:
                         pass
                     else:
                         utr.start = min(gene.start, gap_edge)
                         colour="6"
```

### Comparing `peaks2utr-0.5.1/peaks2utr/criteria.py` & `peaks2utr-0.5.2/peaks2utr/criteria.py`

 * *Files identical despite different names*

### Comparing `peaks2utr-0.5.1/peaks2utr/models.py` & `peaks2utr-0.5.2/peaks2utr/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from abc import ABC
+import collections
+import json
 import re
 
 import gffutils
 
 from .constants import STRAND_CIGAR_SOFT_CLIP_REGEX
 
 
@@ -100,15 +102,15 @@
         """
         pattern = STRAND_CIGAR_SOFT_CLIP_REGEX.get(self.strand)
         matches = re.search(pattern, self.cigar)
         if matches:
             return int(matches.group(1))
         else:
             return 0
-    
+
     @property
     def extremity(self):
         """
         Furthest base from transcript, accounting for strand.
         """
         if self.strand == "reverse":
             return self.start
@@ -116,10 +118,51 @@
 
     def poly_tail_exists(self, tail_len=10):
         """
         Return True if a poly-A/T tail of tail_len bases exists in soft-clipped portion of read.
         """
         if self.len_soft_clipped > 0:
             soft_clipped = self.seq[:self.len_soft_clipped] if self.strand == "reverse" else self.seq[-self.len_soft_clipped:]
-            if "T"*tail_len in soft_clipped or "A"*tail_len in soft_clipped:                
+            if "T"*tail_len in soft_clipped or "A"*tail_len in soft_clipped:
                 return True
         return False
+
+class ZeroCoverageIntervals(collections.UserDict):
+    """
+    Dictionary of zero coverage intervals per chromosome from parsed BED file.
+    """
+    class Interval:
+        def __init__(self, start, end):
+            self.start = int(start)
+            self.end = int(end)
+
+    def __init__(self, bed_fn=None):
+        super().__init__()
+        if bed_fn:
+            with open(bed_fn, 'r') as f:
+                for l in f.readlines():
+                    chr, start, stop = l.strip().split('\t')
+                    if chr not in self.data:
+                        self.data[chr] = []
+                    self.data[chr].append(self.Interval(start, stop))
+
+    def filter(self, chr, base):
+        """
+        Filter intervals that contain base.
+
+        This was motivated by https://github.com/haessar/peaks2utr/issues/9 - the native
+        pybedtools.BedTool.filter method was causing "Too many files open" errors in some
+        distributed systems.
+        """
+        if chr in self:
+            return [i for i in self[chr] if i.start < base < i.end]
+        return []
+
+class SPATTruncationPoints(collections.UserDict):
+    """
+    Dictionary of SPAT "truncation points" per chromosome from json file.
+    """
+    def __init__(self, json_fn=None):
+        super().__init__()
+        if json_fn:
+            with open(json_fn, 'r') as f:
+                self.data.update(json.load(f))
```

### Comparing `peaks2utr-0.5.1/peaks2utr/postprocess.py` & `peaks2utr-0.5.2/peaks2utr/postprocess.py`

 * *Files identical despite different names*

### Comparing `peaks2utr-0.5.1/peaks2utr/preprocess.py` & `peaks2utr-0.5.2/peaks2utr/preprocess.py`

 * *Files identical despite different names*

### Comparing `peaks2utr-0.5.1/peaks2utr/utils.py` & `peaks2utr-0.5.2/peaks2utr/utils.py`

 * *Files identical despite different names*

### Comparing `peaks2utr-0.5.1/peaks2utr.egg-info/PKG-INFO` & `peaks2utr-0.5.2/peaks2utr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaks2utr
-Version: 0.5.1
+Version: 0.5.2
 Summary: A robust, parallelized Python CLI for annotating three_prime_UTR
 Home-page: https://github.com/haessar/peaks2utr
 Author: William Haese-Hill
 Author-email: william.haese-hill@glasgow.ac.uk
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: peaks2utr Version: 0.5.1 Summary: A robust,
+Metadata-Version: 2.1 Name: peaks2utr Version: 0.5.2 Summary: A robust,
 parallelized Python CLI for annotating three_prime_UTR Home-page: https://
 github.com/haessar/peaks2utr Author: William Haese-Hill Author-email:
 william.haese-hill@glasgow.ac.uk License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
```

### Comparing `peaks2utr-0.5.1/setup.cfg` & `peaks2utr-0.5.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = peaks2utr
-version = 0.5.1
+version = 0.5.2
 author = William Haese-Hill
 author_email = william.haese-hill@glasgow.ac.uk
 description = A robust, parallelized Python CLI for annotating three_prime_UTR
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/haessar/peaks2utr
 license_files = file: LICENSE
```

### Comparing `peaks2utr-0.5.1/test/test.py` & `peaks2utr-0.5.2/test/test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 import csv
+import os
 from queue import Queue
+import sys
 import unittest
-from unittest import mock
 
 import gffutils
 
+sys.path.insert(0, os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
 from peaks2utr.annotations import Annotations, NoNearbyFeatures, annotate_utr_for_peak
-from peaks2utr.models import Peak, UTR
+from peaks2utr.models import Peak, UTR, ZeroCoverageIntervals, SPATTruncationPoints
+
+TEST_DIR = os.path.dirname(__file__)
 
 
 class TestUTRAnnotation(unittest.TestCase):
     def setUp(self):
-        self.db = gffutils.create_db("test/Chr1.gff", "test/Chr1.db", force=True)
+        self.db = gffutils.create_db(os.path.join(TEST_DIR, "Chr1.gff"), os.path.join(TEST_DIR, "Chr1.db"), force=True)
+        self.coverage_gaps = ZeroCoverageIntervals()
+        self.truncation_points = SPATTruncationPoints()
+
+    def tearDown(self):
+        os.remove(os.path.join(TEST_DIR, "Chr1.db"))
 
     def strand_annotations(self, peaks_filename, strand, expected_annotations, max_distance):
         with open(peaks_filename, 'r') as fin:
             peaks = csv.reader(fin, delimiter="\t")
             for peak in peaks:
                 peak = Peak(*peak)
                 if peak.name in expected_annotations:
                     annotations = Annotations()
                     queue = Queue()
                     peak.strand = strand
-                    with mock.patch('peaks2utr.annotations.cached') as cached_mock:
-                        with mock.patch('peaks2utr.annotations.pybedtools') as pybt_mock:
-                            cached_mock.return_value = "test/unmapped.json"
-                            pybt_mock.return_value = mock.MagicMock()
-                            annotate_utr_for_peak(self.db, queue, peak, max_distance=max_distance)
+                    annotate_utr_for_peak(self.db, queue, peak, self.truncation_points, self.coverage_gaps, max_distance=max_distance)
                     if expected_annotations[peak.name] is None:
-                        self.assertIsNone(queue.get())                        
+                        self.assertIsNone(queue.get())
                     elif expected_annotations[peak.name] is NoNearbyFeatures:
                         self.assertTrue(queue.get() is NoNearbyFeatures)
                     else:
                         while not queue.empty():
                             result = queue.get()
                             if type(result) == dict:
                                 annotations.update(result)
@@ -43,15 +49,15 @@
     def test_forward_strand_annotations(self):
         expected_annotations = {
             'forward_peak_3': None,
             'forward_peak_6': {'PBANKA_0100041.1.1': UTR(14118, 17222)},
             'forward_peak_9': {'PBANKA_0100100.1.1': UTR(27916, 29285), 'PBANKA_0100200.1.1': UTR(30482, 31051)},
             'forward_peak_10': {'PBANKA_0100200.1.1': UTR(30482, 33095)},
         }
-        peaks_filename = "test/test_forward_peaks.broadPeak"
+        peaks_filename = os.path.join(TEST_DIR, "test_forward_peaks.broadPeak")
         self.strand_annotations(peaks_filename, '+', expected_annotations, max_distance=2500)
 
     def test_reverse_strand_annotations(self):
         expected_annotations = {
             'reverse_peak_1': {'PBANKA_0100021.1.1': UTR(801, 1098)},
             'reverse_peak_3': NoNearbyFeatures,
             'reverse_peak_4': NoNearbyFeatures,
@@ -61,13 +67,13 @@
             'reverse_peak_13': None,
             'reverse_peak_14': None,
             'reverse_peak_24': {'PBANKA_0101500.1.1': UTR(77310, 77684)},
             'reverse_peak_30': {'PBANKA_0102200.1.1': UTR(95595, 96818)},
             'reverse_peak_54': {'PBANKA_0103400.1.1': UTR(154886, 155566)},
             'reverse_peak_143': {'PBANKA_0111300.1.1': UTR(437496, 438265)}
         }
-        peaks_filename = "test/test_reverse_peaks.broadPeak"
+        peaks_filename = os.path.join(TEST_DIR, "test_reverse_peaks.broadPeak")
         self.strand_annotations(peaks_filename, '-', expected_annotations, max_distance=2500)
 
 
 if __name__ == '__main__':
     unittest.main()
```

