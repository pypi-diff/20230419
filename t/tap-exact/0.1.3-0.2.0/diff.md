# Comparing `tmp/tap_exact-0.1.3.tar.gz` & `tmp/tap_exact-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_exact-0.1.3.tar", max compression
+gzip compressed data, was "tap_exact-0.2.0.tar", max compression
```

## Comparing `tap_exact-0.1.3.tar` & `tap_exact-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      932 2023-04-19 09:35:14.832465 tap_exact-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.1.3/tap_exact/__init__.py
--rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.1.3/tap_exact/client.py
--rw-r--r--   0        0        0    26805 2023-04-19 09:35:33.102465 tap_exact-0.1.3/tap_exact/streams.py
--rw-r--r--   0        0        0     1631 2023-04-19 08:49:57.242465 tap_exact-0.1.3/tap_exact/tap.py
--rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.1.3/tap_exact/tests/__init__.py
--rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.1.3/tap_exact/tests/test_core.py
--rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.1.3/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      932 2023-04-19 14:38:09.422465 tap_exact-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-25 19:29:50.108600 tap_exact-0.2.0/tap_exact/__init__.py
+-rw-r--r--   0        0        0      842 2022-12-28 16:47:27.563614 tap_exact-0.2.0/tap_exact/client.py
+-rw-r--r--   0        0        0    29790 2023-04-19 14:49:08.822465 tap_exact-0.2.0/tap_exact/streams.py
+-rw-r--r--   0        0        0     1677 2023-04-19 14:49:52.622465 tap_exact-0.2.0/tap_exact/tap.py
+-rw-r--r--   0        0        0       32 2022-11-25 19:29:50.118600 tap_exact-0.2.0/tap_exact/tests/__init__.py
+-rw-r--r--   0        0        0      657 2022-11-25 19:50:07.718600 tap_exact-0.2.0/tap_exact/tests/test_core.py
+-rw-r--r--   0        0        0      960 1970-01-01 00:00:00.000000 tap_exact-0.2.0/setup.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 tap_exact-0.2.0/PKG-INFO
```

### Comparing `tap_exact-0.1.3/pyproject.toml` & `tap_exact-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-exact"
-version = "0.1.3"
+version = "0.2.0"
 description = "`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK."
 authors = ["Janick Otten"]
 keywords = [
     "ELT",
     "Exact Online",
 ]
 license = "Apache 2.0"
```

### Comparing `tap_exact-0.1.3/tap_exact/client.py` & `tap_exact-0.2.0/tap_exact/client.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.3/tap_exact/streams.py` & `tap_exact-0.2.0/tap_exact/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -794,8 +794,101 @@
 
         for row in resp:
             
             # We loop through the keys that should be modified
             for key in keys:
                 row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
 
+            yield row
+
+class CrmAccountsStream(ExactOnlineStream):
+    """Define custom stream."""
+
+    name = "crm_accounts"
+    primary_keys = ["ID"]
+    replication_key = "Modified"
+    # Optionally, you may also use `schema_filepath` in place of `schema`:
+    # schema_filepath = SCHEMAS_DIR / "users.json"
+    schema = th.PropertiesList(
+        th.Property(
+            "ID",
+            th.StringType,
+            description="The unique identifier of the account"
+        ),
+        th.Property(
+            "AccountManager",
+            th.StringType,
+            description="The accountmanager ID"
+        ),
+        th.Property(
+            "AccountManagerFullName",
+            th.StringType,
+            description="The name of the accountmanager"
+        ),
+        th.Property(
+            "Code",
+            th.StringType,
+            description="The unique account code"
+        ),
+        th.Property(
+            "City",
+            th.StringType,
+            description="The city the customer has its visit address"
+        ),
+        th.Property(
+            "CountryName",
+            th.StringType,
+            description="The country the customer is in"
+        ),
+        th.Property(
+            "Latitude",
+            th.NumberType,
+            description="The latitude of the customer address"
+        ),
+        th.Property(
+            "Longitude",
+            th.NumberType,
+            description="The longitude of the customer address"
+        ),
+        th.Property(
+            "Name",
+            th.StringType,
+            description="The customer name"
+        ),
+        th.Property(
+            "SearchCode",
+            th.StringType,
+            description="The customer search code"
+        ),
+        th.Property(
+            "Modified",
+            th.DateTimeType,
+            description="Last modified date"
+        ),
+    ).to_dict()
+
+    def get_path(self, context: Optional[dict]) -> str:
+        """Return the path of the Exact API"""
+
+        replication_key_value = self.get_starting_timestamp(context).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+        
+        path = "/crm/Accounts?" \
+            f"$filter={self.replication_key}%20ge%20datetime%27{replication_key_value}%27&" \
+            "$select=ID,AccountManager,AccountManagerFullName,Code,City,CountryName,Latitude,Longitude,Name,SearchCode,Modified"
+
+        return path
+
+    def get_records(self, context: Optional[dict]) -> Iterable[dict]:
+        """Return a generator or row-type dictionary objects"""
+        
+        resp = self.conn.rest(GET('v1/%d/%s' % (self.division, self.get_path(context) )))
+        
+        # The fields that have /Date(unixmilliseconds)/ objects that should be converted into datetime objects
+        keys = ['Modified']
+
+        for row in resp:
+            
+            # We loop through the keys that should be modified
+            for key in keys:
+                row[key] = datetime.fromtimestamp( int(row[key][6:-2]) / 1000.0 )
+
             yield row
```

### Comparing `tap_exact-0.1.3/tap_exact/tap.py` & `tap_exact-0.2.0/tap_exact/tap.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,27 +10,29 @@
     SalesInvoicesStream,
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
     BankEntryLinesStream,
     CashEntryLinesStream,
     GeneralJournalEntryLinesStream,
     PurchaseEntriesStream,
-    SalesEntriesStream
+    SalesEntriesStream,
+    CrmAccountsStream
 )
 # TODO: Compile a list of custom stream types here
 #       OR rewrite discover_streams() below with your custom logic.
 STREAM_TYPES = [
     SalesInvoicesStream,
     PurchaseInvoicesStream,
     GeneralLedgerAccountsStream,
     BankEntryLinesStream,
     CashEntryLinesStream,
     GeneralJournalEntryLinesStream,
     PurchaseEntriesStream,
-    SalesEntriesStream
+    SalesEntriesStream,
+    CrmAccountsStream
 ]
 
 
 class TapExactOnline(Tap):
     """ExactOnline tap class."""
     name = "tap-exact"
```

### Comparing `tap_exact-0.1.3/tap_exact/tests/test_core.py` & `tap_exact-0.2.0/tap_exact/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_exact-0.1.3/setup.py` & `tap_exact-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'s3': ['fs-s3fs>=1.1.1,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['tap-exact = tap_exact.tap:TapExactOnline.cli']}
 
 setup_kwargs = {
     'name': 'tap-exact',
-    'version': '0.1.3',
+    'version': '0.2.0',
     'description': '`tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.',
     'long_description': 'None',
     'author': 'Janick Otten',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tap_exact-0.1.3/PKG-INFO` & `tap_exact-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-exact
-Version: 0.1.3
+Version: 0.2.0
 Summary: `tap-exact` is a Singer tap for Exact Online, built with the Meltano Singer SDK.
 License: Apache 2.0
 Keywords: ELT,Exact Online
 Author: Janick Otten
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

