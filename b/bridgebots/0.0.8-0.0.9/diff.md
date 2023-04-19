# Comparing `tmp/bridgebots-0.0.8.tar.gz` & `tmp/bridgebots-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgebots-0.0.8.tar", max compression
+gzip compressed data, was "bridgebots-0.0.9.tar", max compression
```

## Comparing `bridgebots-0.0.8.tar` & `bridgebots-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      662 2021-11-28 03:48:20.720259 bridgebots-0.0.8/bridgebots/__init__.py
--rw-r--r--   0        0        0      793 2022-01-16 00:35:19.448757 bridgebots-0.0.8/bridgebots/bids.py
--rw-r--r--   0        0        0     4033 2022-01-16 01:14:50.699684 bridgebots-0.0.8/bridgebots/board_record.py
--rw-r--r--   0        0        0     5144 2021-11-28 03:48:20.721241 bridgebots-0.0.8/bridgebots/deal.py
--rw-r--r--   0        0        0     3219 2022-01-16 01:03:05.382449 bridgebots-0.0.8/bridgebots/deal_enums.py
--rw-r--r--   0        0        0     7168 2022-01-16 01:17:42.212906 bridgebots-0.0.8/bridgebots/deal_utils.py
--rw-r--r--   0        0        0     3767 2021-11-28 03:48:20.722787 bridgebots-0.0.8/bridgebots/double_dummy.py
--rw-r--r--   0        0        0    13222 2022-01-16 01:20:49.246052 bridgebots-0.0.8/bridgebots/lin.py
--rw-r--r--   0        0        0    11653 2022-01-16 00:44:10.153045 bridgebots-0.0.8/bridgebots/pbn.py
--rw-r--r--   0        0        0     3780 2021-11-28 03:48:20.724240 bridgebots-0.0.8/bridgebots/play_utils.py
--rw-r--r--   0        0        0     4410 2021-11-28 03:48:20.724678 bridgebots-0.0.8/bridgebots/schemas.py
--rw-r--r--   0        0        0      434 2022-01-16 01:31:25.468354 bridgebots-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      635 2022-01-16 01:31:30.369565 bridgebots-0.0.8/setup.py
--rw-r--r--   0        0        0      494 2022-01-16 01:31:30.369893 bridgebots-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      662 2021-11-28 03:48:20.720259 bridgebots-0.0.9/bridgebots/__init__.py
+-rw-r--r--   0        0        0      793 2022-01-16 07:32:16.872082 bridgebots-0.0.9/bridgebots/bids.py
+-rw-r--r--   0        0        0     4033 2022-01-16 07:34:26.459520 bridgebots-0.0.9/bridgebots/board_record.py
+-rw-r--r--   0        0        0     5144 2021-11-28 03:48:20.721241 bridgebots-0.0.9/bridgebots/deal.py
+-rw-r--r--   0        0        0     3219 2022-01-16 07:34:26.460055 bridgebots-0.0.9/bridgebots/deal_enums.py
+-rw-r--r--   0        0        0     7168 2022-01-16 07:34:26.460602 bridgebots-0.0.9/bridgebots/deal_utils.py
+-rw-r--r--   0        0        0     3767 2021-11-28 03:48:20.722787 bridgebots-0.0.9/bridgebots/double_dummy.py
+-rw-r--r--   0        0        0    13222 2022-01-16 07:45:22.484050 bridgebots-0.0.9/bridgebots/lin.py
+-rw-r--r--   0        0        0    12107 2022-01-17 07:20:40.135901 bridgebots-0.0.9/bridgebots/pbn.py
+-rw-r--r--   0        0        0     3780 2021-11-28 03:48:20.724240 bridgebots-0.0.9/bridgebots/play_utils.py
+-rw-r--r--   0        0        0     4410 2021-11-28 03:48:20.724678 bridgebots-0.0.9/bridgebots/schemas.py
+-rw-r--r--   0        0        0      434 2022-01-17 07:21:34.270108 bridgebots-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      635 2022-01-17 07:29:35.600190 bridgebots-0.0.9/setup.py
+-rw-r--r--   0        0        0      494 2022-01-17 07:29:35.600458 bridgebots-0.0.9/PKG-INFO
```

### Comparing `bridgebots-0.0.8/bridgebots/__init__.py` & `bridgebots-0.0.9/bridgebots/__init__.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/bids.py` & `bridgebots-0.0.9/bridgebots/bids.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/board_record.py` & `bridgebots-0.0.9/bridgebots/board_record.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/deal.py` & `bridgebots-0.0.9/bridgebots/deal.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/deal_enums.py` & `bridgebots-0.0.9/bridgebots/deal_enums.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/deal_utils.py` & `bridgebots-0.0.9/bridgebots/deal_utils.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/double_dummy.py` & `bridgebots-0.0.9/bridgebots/double_dummy.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/lin.py` & `bridgebots-0.0.9/bridgebots/lin.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/pbn.py` & `bridgebots-0.0.9/bridgebots/pbn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import logging
 import re
 from collections import defaultdict
 from pathlib import Path
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Tuple
 
 from bridgebots.bids import canonicalize_bid
 from bridgebots.board_record import BidMetadata, BoardRecord, Contract, DealRecord
 from bridgebots.deal import Card, Deal
 from bridgebots.deal_enums import BiddingSuit, Direction
 from bridgebots.deal_utils import from_pbn_deal
 from bridgebots.play_utils import trick_evaluator
@@ -21,14 +21,16 @@
     """
     with open(file_path, "r") as pbn_file:
         records = []
         current_record = ""
         while True:
             line = pbn_file.readline()
             if line == "":  # EOF
+                if current_record:
+                    records.append(current_record)
                 return records
             elif line == "\n":  # End of Board Record
                 records.append(current_record.splitlines())
                 current_record = ""
             else:
                 current_record += line
 
@@ -254,21 +256,27 @@
         event=record_dict.get("Event"),
         bidding_metadata=bidding_metadata,
         # TODO adjust to use commentary type
         commentary=record_dict.get("Commentary"),
     )
 
 
-def _parse_single_pbn_record(record_strings: List[str]) -> Tuple[Deal, BoardRecord]:
+def _parse_single_pbn_record(record_strings: List[str], previous_deal: Optional[Deal]) -> Tuple[Deal, BoardRecord]:
     """
     :param record_strings: One string per line of a single PBN deal record
     :return: Deal and BoardRecord corresponding to the PBN record
     """
     record_dict = _build_record_dict(record_strings)
-    deal = from_pbn_deal(record_dict["Dealer"], record_dict["Vulnerable"], record_dict["Deal"])
+    try:
+        deal = from_pbn_deal(record_dict["Dealer"], record_dict["Vulnerable"], record_dict["Deal"])
+    except KeyError as e:
+        if previous_deal:
+            deal = previous_deal
+        else:
+            raise ValueError("Missing deal fields and no previous_deal provided") from e
     board_record = _parse_board_record(record_dict, deal)
     return deal, board_record
 
 
 def parse_pbn(file_path: Path) -> List[DealRecord]:
     """
     Split PBN file into boards then decompose those boards into Deal and BoardRecord objects. Only supports PBN v1.0
@@ -276,14 +284,17 @@
 
     :param file_path: path to a PBN file
     :return: A list of DealRecords representing all the boards played
     """
     records_strings = _split_pbn(file_path)
     # Maintain a mapping from deal to board records to create a single deal record per deal
     records = defaultdict(list)
+    # Some PBNs have multiple board records per deal
+    previous_deal = None
     for record_strings in records_strings:
         try:
-            deal, board_record = _parse_single_pbn_record(record_strings)
+            deal, board_record = _parse_single_pbn_record(record_strings, previous_deal)
             records[deal].append(board_record)
+            previous_deal = deal
         except (KeyError, ValueError) as e:
             logging.warning(f"Malformed record {record_strings}: {e}")
     return [DealRecord(deal, board_records) for deal, board_records in records.items()]
```

### Comparing `bridgebots-0.0.8/bridgebots/play_utils.py` & `bridgebots-0.0.9/bridgebots/play_utils.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/bridgebots/schemas.py` & `bridgebots-0.0.9/bridgebots/schemas.py`

 * *Files identical despite different names*

### Comparing `bridgebots-0.0.8/setup.py` & `bridgebots-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['marshmallow>=3.12.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'bridgebots',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Data processing for Contract Bridge',
     'long_description': None,
     'author': 'Forrest Rice',
     'author_email': 'forrest.d.rice@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

