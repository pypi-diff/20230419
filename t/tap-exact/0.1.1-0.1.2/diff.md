# Comparing `tmp/tap_exact-0.1.1.tar.gz` & `tmp/tap_exact-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.1.1.tar", max compression
+gzip compressed data, was "tap_exact-0.1.2.tar", max compression
```

## Comparing `tap_exact-0.1.1.tar` & `tap_exact-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-04-13 09:22:16.735247 tap_exact-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.1.1/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.1.1/tap_exact/client.py
--rw-r--r--   0        0        0    24904 2023-04-13 09:22:12.055247 tap_exact-0.1.1/tap_exact/streams.py
--rw-r--r--   0        0        0     1643 2023-04-13 08:15:22.125248 tap_exact-0.1.1/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.1.1/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.1.1/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.1.1/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-19 08:50:02.172465 tap_exact-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.1.2/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.1.2/tap_exact/client.py
+-rw-r--r--   0        0        0    26806 2023-04-19 08:49:04.192465 tap_exact-0.1.2/tap_exact/streams.py
+-rw-r--r--   0        0        0     1631 2023-04-19 08:49:57.242465 tap_exact-0.1.2/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.1.2/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.1.2/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.1.2/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.1.2/PKG-INFO
```

### Comparing `tap_exact-0.1.1/pyproject.toml` & `tap_exact-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.1.1"
+version = "0.1.2"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.1.1/tap_exact/client.py` & `tap_exact-0.1.2/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.1/tap_exact/streams.py` & `tap_exact-0.1.2/tap_exact/streams.py`

 * *Files 8% similar despite different names*

```diff
@@ -560,181 +560,241 @@
             
             # We loop through the keys that should be modified
             for key in keys:
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
-class PurchaseEntryLinesStream(ExactOnlineStream):
+class PurchaseEntriesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "purchase_entry_lines"
-    primary_keys = ["ID"]
+    name = "purchase_entries"
+    primary_keys = ["EntryID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
-            "ID",
+            "EntryID",
             th.StringType,
             description="The unique identifier of the line"
         ),
         th.Property(
-            "GLAccount",
-            th.StringType,
-            description="The unique identifier of the corresponding GL account"
+            "Created",
+            th.DateTimeType,
+            description="The creation date"
         ),
         th.Property(
-            "GLAccountCode",
+            "EntryDate",
+            th.DateTimeType,
+            description="The invoice date"
+        ),
+        th.Property(
+            "InvoiceNumber",
+            th.IntegerType,
+            description="The invoice number"
+        ),
+        th.Property(
+            "EntryNumber",
+            th.IntegerType,
+            description="The entry number"
+        ),
+        th.Property(
+            "Description",
             th.StringType,
-            description="The unique code of the corresponding GL account"
+            description="The description of the invoice"
         ),
         th.Property(
-            "From",
-            th.DateTimeType,
-            description="The starting date of the statement line"
+            "OrderNumber",
+            th.IntegerType,
+            description="The order number"
         ),
         th.Property(
-            "To",
+            "DueDate",
             th.DateTimeType,
-            description="THe ending date of the statement line"
+            description="The due date"
         ),
         th.Property(
-            "Description",
+            "PaymentCondition",
             th.StringType,
-            description="The description of the entry"
+            description="The code of the payment conditino that is used to calculate the due date and discount"
         ),
         th.Property(
-            "LineNumber",
+            "Status",
             th.IntegerType,
-            description="The line number of the entry"
+            description="The code of the payment conditino that is used to calculate the due date and discount"
         ),
         th.Property(
-            "AmountDC",
+            "Journal",
             th.StringType,
-            description="The amount in the default currency of the company"
+            description="The code of the purchase journal in which the invoice is entered"
         ),
         th.Property(
-            "VATAmountDC",
+            "Supplier",
+            th.StringType,
+            description="The code of supplier"
+        ),
+        th.Property(
+            "SupplierName",
             th.StringType,
-            description="The amount of VAT in the default currency of the company"
+            description="The name of supplier"
+        ),
+        th.Property(
+            "AmountDC",
+            th.NumberType,
+            description="Amount including VAT in the default currency of the company"
+        ),
+        th.Property(
+            "VATAmountDC",
+            th.NumberType,
+            description="VAT Amount in the default currency of the company"
         ),
         th.Property(
             "Modified",
             th.DateTimeType,
             description="Last modified date"
         ),
     ).to_dict()
 
     def get_path(self, context: Optional[dict]) -> str:
         """Return the path of the Exact API"""
 
         replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
         
-        path = "/purchaseentry/PurchaseEntryLines?" \
+        path = "/purchaseentry/PurchaseEntries?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
-            "$select=ID,GLAccount,GLAccountCode,From,To,Description,LineNumber,AmountDC,VATAmountDC,Modified"
+            "$select=EntryID,Created,EntryDate,InvoiceNumber,EntryNumber,Description,OrderNumber,DueDate,PaymentCondition,Status,Journal,Supplier,SupplierName,AmountDC,VATAmountDC,Modified"
 
         return path
 
     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
         """Return a generator or row-type dictionary objects"""
         
         resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
         
         # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['From', 'To', 'Modified']
+        keys = ['Created', 'EntryDate', 'DueDate', 'Modified']
 
         for row in resp:
             
             # We loop through the keys that should be modified
             for key in keys:
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
             yield row
 
-class SalesEntryLinesStream(ExactOnlineStream):
+class SalesEntriesStream(ExactOnlineStream):
     """Define custom stream."""
 
-    name = "sales_entry_lines"
-    primary_keys = ["ID"]
+    name = "sales_entries"
+    primary_keys = ["EntryID"]
     replication_key = "Modified"
     # Optionally, you may also use `schema_filepath` in place of `schema`:
     # schema_filepath = SCHEMAS_DIR / "users.json"
     schema = th.PropertiesList(
         th.Property(
-            "ID",
+            "EntryID",
             th.StringType,
             description="The unique identifier of the line"
         ),
         th.Property(
-            "GLAccount",
-            th.StringType,
-            description="The unique identifier of the corresponding GL account"
+            "Created",
+            th.DateTimeType,
+            description="The creation date"
         ),
         th.Property(
-            "GLAccountCode",
+            "EntryDate",
+            th.DateTimeType,
+            description="The invoice date"
+        ),
+        th.Property(
+            "YourRef",
+            th.IntegerType,
+            description="The invoice number"
+        ),
+        th.Property(
+            "EntryNumber",
+            th.IntegerType,
+            description="The entry number"
+        ),
+        th.Property(
+            "Description",
             th.StringType,
-            description="The unique code of the corresponding GL account"
+            description="The description of the invoice"
         ),
         th.Property(
-            "From",
-            th.DateTimeType,
-            description="The starting date of the statement line"
+            "OrderNumber",
+            th.IntegerType,
+            description="The order number"
         ),
         th.Property(
-            "To",
+            "DueDate",
             th.DateTimeType,
-            description="THe ending date of the statement line"
+            description="The due date"
         ),
         th.Property(
-            "Description",
+            "PaymentCondition",
             th.StringType,
-            description="The description of the entry"
+            description="The code of the payment conditino that is used to calculate the due date and discount"
         ),
         th.Property(
-            "LineNumber",
+            "Status",
             th.IntegerType,
-            description="The line number of the entry"
+            description="The code of the payment conditino that is used to calculate the due date and discount"
         ),
         th.Property(
-            "AmountDC",
+            "Journal",
             th.StringType,
-            description="The amount in the default currency of the company"
+            description="The code of the purchase journal in which the invoice is entered"
         ),
         th.Property(
-            "VATAmountDC",
+            "Customer",
+            th.StringType,
+            description="The code of customer"
+        ),
+        th.Property(
+            "CustomerName",
             th.StringType,
-            description="The amount of VAT in the default currency of the company"
+            description="The name of customer"
+        ),
+        th.Property(
+            "AmountDC",
+            th.NumberType,
+            description="Amount including VAT in the default currency of the company"
+        ),
+        th.Property(
+            "VATAmountDC",
+            th.NumberType,
+            description="VAT Amount in the default currency of the company"
         ),
         th.Property(
             "Modified",
             th.DateTimeType,
             description="Last modified date"
         ),
     ).to_dict()
 
     def get_path(self, context: Optional[dict]) -> str:
         """Return the path of the Exact API"""
 
         replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
         
-        path = "/salesentry/SalesEntryLines?" \
+        path = "/salesentry/SalesEntries?" \
             f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
-            "$select=ID,GLAccount,GLAccountCode,From,To,Description,LineNumber,AmountDC,VATAmountDC,Modified"
+            "$select=EntryID,Created,EntryDate,YourRef,EntryNumber,Description,OrderNumber,DueDate,PaymentCondition,Status,Journal,Customer,CustomerName,AmountDC,VATAmountDC,Modified"
 
         return path
 
     def get_records(self, context: Optional[dict]) -> Iterable[dict]:
         """Return a generator or row-type dictionary objects"""
         
         resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
         
         # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
-        keys = ['From', 'To', 'Modified']
+        keys = ['Created', 'EntryDate', 'DueDate', 'Modified']
 
         for row in resp:
             
             # We loop through the keys that should be modified
             for key in keys:
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
```

### Comparing `tap_exact-0.1.1/tap_exact/tests/test_core.py` & `tap_exact-0.1.2/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.1/setup.py` & `tap_exact-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.1.1/PKG-INFO` & `tap_exact-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.1.1
+Version: 0.1.2
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

